<script>
    import icon from '../icons/icon.png';
    import demo from '../images/demo.png';
    import heart from '../icons/heart.svg';
    import downloadIcon from '../icons/download-icon.svg';
    import windows from '../icons/windows.png';
    import apple from '../icons/apple.png';
    import linux from '../icons/linux.svg';
    import contact from '../icons/contact.svg';

    import features from '../data/features.json';

</script>

<div class="main"></div>
<!--Hero Section-->
<section class="pt-5">
    <div class="container">
        <div class="row">
            <div class="col-12 d-flex flex-row align-items-center justify-content-between">
                <div class="heading-brand">
                    <img src={icon} alt="" class="head-icon">
                    CP-IDE
                </div>
                <a href="#download" class="btn btn-dark">
                    Download
                </a>
            </div>
        </div>
        <div class="row mt-6">
            <div class="col-md-8 mx-auto text-center">
                <h2>A lightweight, cross-platform code editor for <br> competitive programmers.</h2>
                <p>
                    <img class="head-icon" src="https://gblobscdn.gitbook.com/spaces%2F-LBKK1y7h_XWAtuRJG9X%2Favatar.png?alt=media" alt="" > + 
                    <img class="head-icon" src="https://cdn-icons-png.flaticon.com/512/833/833472.png" alt=""> =
                    <img src={icon} alt="" class="head-icon">
                </p>
                <p class="lead mb-5">CP-IDE is a cross-platform code editor built on electron and ace, with an easy workflow for faster and easier testing of solutions.</p>
                <a href="https://bitbucket.org/aritra1999/cpide/src/master/" class="btn btn-light svg-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" class="mr-2" width="28" height="28" viewBox="0 0 32 32"><defs><linearGradient id="vscodeIconsFileTypeBitbucketpipeline0" x1="-792.28" x2="-793.365" y1="633.265" y2="632.418" gradientTransform="matrix(12.821 0 0 -12.821 10188.143 8132.963)" gradientUnits="userSpaceOnUse"><stop offset=".18" stop-color="#0052cc"/><stop offset="1" stop-color="#2684ff"/></linearGradient></defs><path fill="#2684ff" d="M2.909 3.41A.9.9 0 0 0 2 4.3a.8.8 0 0 0 .012.155L5.82 27.568a1.22 1.22 0 0 0 1.193 1.018h18.269a.9.9 0 0 0 .9-.754l3.805-23.378a.9.9 0 0 0-.737-1.033a.911.911 0 0 0-.147-.012Zm16.035 16.709h-5.831l-1.579-8.244h8.823Z"/><path fill="url(#vscodeIconsFileTypeBitbucketpipeline0)" d="M28.776 11.874h-8.419l-1.413 8.244h-5.831L6.228 28.3a1.21 1.21 0 0 0 .785.3h18.274a.9.9 0 0 0 .9-.754Z"/></svg>                    View Source
                </a>
            </div>
        </div>
        <div class="row mt-5">
            <img src={demo} alt="" class="demo-img mx-auto">
        </div>
    </div>

</section>
<!--Features Section-->
<section class="py-6">
    <div class="container">
        <div class="row">
            <div class="col-md-12 mx-auto">
                <h2 class="text-center text-md-left">
                    <img src={heart} alt="" class="subhead-icon">
                    Reasons to love 
                    <span class="text-success">CP-IDE</span>
                </h2>
            </div>
            <div class="col-md-8 mx-auto">
                <div class="row feature-grid">
                    {#each features as feature}
                    <div class="col-sm-6">
                        <div class="media">
                            <div class="icon-box">
                                <div class="icon-box-inner">
                                    {@html feature.icon}
                                </div>
                            </div>
                            <div class="media-body">
                                {feature.feature}
                            </div>
                        </div>
                    </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>
</section>
<!--Used By Section-->
<section class="pb-3 download-bg" id="download">
    <div class="container">
        <hr>
        <br>
        <div class="row">
            <div class="col-md-12 mx-auto">
                <h2 class="text-center text-md-left">
                    <img src={downloadIcon} alt="" class="subhead-icon">
                    Download  <span class="text-success">CP-IDE</span>
                </h2>
                <h3 class="text-center">
                    Total Downloads: <span class="text-success">100+</span>
                </h3>
                <div class="download-section mt-5">
                    <div class="download-cards-container">
                        <div class="download-card item" align="center">
                            <img src={windows} alt="" class="download-icons mb-5"><br>
                            <a href="https://bitbucket.org/aritra1999/cpide/raw/f0de3d8d2e294830f7ffc6b990a0605b78692cdd/out/make/squirrel.windows/x64/cpide-1.0.0%20Setup.exe" class="btn btn-secondary mb-3 download-btn" role="button">
                                Windows <small>x64 | exe</small>
                                <img src={downloadIcon} alt="^" class="dwnload-icon">
                            </a>
                            <a href="https://bitbucket.org/aritra1999/cpide/raw/f0de3d8d2e294830f7ffc6b990a0605b78692cdd/out/make/squirrel.windows/x64/cpide-1.0.0-full.nupkg" class="btn btn-secondary mb-3 download-btn" role="button">
                                Windows <small>x64 | nupkg</small>
                                <img src={downloadIcon} alt="^" class="dwnload-icon">
                            </a>
                            <br>
                        </div>
                    </div>
                    <div class="download-cards-container">
                        <div class="download-card border-left" align="center">
                            <img src={apple} alt="" class="download-icons mt-4 mb-5"><br>
                            <a  href="/" class="btn btn-secondary mb-3 download-btn" role="button">
                                MacOS X <small>(Comming soon!)</small>
                                <img src={downloadIcon} alt="^" class="dwnload-icon">
                            </a>
                        </div>
                    </div>
                    <div class="download-cards-container">
                        <div class="download-card border-left" align="center">
                            <img src={linux} alt="" class="download-icons mb-5"><br>
                            <a  href="https://bitbucket.org/aritra1999/cpide/raw/f0de3d8d2e294830f7ffc6b990a0605b78692cdd/out/make/deb/x64/cpide_1.0.0_amd64.deb" class="btn btn-secondary mb-3 download-btn" role="button">
                                Linux <small>x64 | deb</small>
                                <img src={downloadIcon} alt="^" class="dwnload-icon">
                            </a><br>
                            <a  href="https://bitbucket.org/aritra1999/cpide/raw/f0de3d8d2e294830f7ffc6b990a0605b78692cdd/out/make/rpm/x64/cpide_1.0.0_amd64.rpm" class="btn btn-secondary mb-3 download-btn" role="button">
                                Linux <small>x64 | rpm</small>
                                <img src={downloadIcon} alt="^" class="dwnload-icon">
                            </a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-12 text-center">
                <br>
                <h3><span class="text-success">or</span></h3>
                <br>
                <h4>Just hack it and build it for your own machine.</h4>
            </div>

            <div class="text-left mx-auto">
                <p class="pl-4">Clone it.</p>
                <div class="code">~$ git clone https://aritra1999@bitbucket.org/aritra1999/cpide.git</div>

                <p class="pl-4">Install dependencies.</p>
                <div class="code">~$ npm install</div>

                <p class="pl-4">Run it.</p>
                <div class="code">~$ npm start</div>

                <p class="pl-4">Build it for your system.</p>
                <div class="code">~$ npm run make</div>
            </div>
        </div>
    </div>
</section>
<!--Contact Section-->
<section class="py-5">
    <div class="container">
        <hr>
        <br>
        <div class="row">
            <div class="col-md-12 mx-auto">
                <h2 class="text-center text-md-left">
                    <img src={contact} alt="" class="subhead-icon">
                    Get in <span class="text-success">Touch</span>
                </h2>
                <p class="text-left touch-p">
                    Any suggestions, complaints, or issues are always welcome. Whether you have a question about features, source code, or the editor we are ready to answer all your question.
                </p>
            </div>
            <div class="col-12 text-center mx-auto mt-4">
                <form action="" method="POST">
                    <div class="input-row">
                        <div>
                            <label for="name">Name *</label><br>
                            <input type="text" class="contact-input" name="name" required/>
                        </div>
                        <div></div>
                        <div>
                            <label for="email">Email *</label><br>
                            <input type="email" class="contact-input" name="email" required/>
                        </div>
                    </div>
                    <div class="row mt-2">
                        <div class="col-12">
                            <label for="messagae">Message *</label><br>
                            <textarea name="message" id="message" rows="10" class="contact-input"></textarea>
                        </div>
                    </div>
                    <div class="row ml-2 mt-1">
                        <button type="submit" class="btn-secondary submit">Submit</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</section>
<!--Footer-->
<footer class="py-5 bg-light">
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <ul class="list-inline">
                    <li class="list-inline-item"><a target="_blank" href="mailto:aritra041999@gmail.com">Contact</a></li>
                    <li class="list-inline-item"><a target="_blank" rel="noreferrer" href="https://aritra1999.github.io">My Site</a></li>
                    <li class="list-inline-item"><a href="#download">Download</a></li>
                    <li class="list-inline-item"><a target="_blank" rel="noreferrer" href="https://github.com/aritra1999">Github</a></li>
                </ul>
            </div>
        </div>
        <div class="row my-2">
            <div class="col-md-4 mx-auto text-muted text-center small-xl">
                &copy; 2023 CP-IDE - All Rights Reserved
            </div>
        </div>
    </div>
</footer>




