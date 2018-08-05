---
layout: page
title: Contact
subtitle: 
---
Have a question, an exciting new idea or need to discuss matters? I'm always looking forward to friendly communication. You can find all the necessary details in order to make contact below.

##### Office:

- F-09 Telecommunication and Networking ([TeleCoN](https://www.giki.edu.pk/telecon)) Lab
  Faculty of Electrical Engineering
  [Ghulam Ishaq Khan (GIK) Institute of Engineering Sciences and Technology](http://giki.edu.pk) 
  Topi-23640, Swabi, KPK, Pakistan

##### Phone:

- Office: +92(938)281032 --Ext: 2684
- Cell:

<button type="button" class="btn btn-email"><i class="fa fa-envelope pr-1"></i> Email</button>
<button type="button" class="btn btn-ins"><i class="fa fa-instagram pr-1"></i> Instagram</button>
<button type="button" class="btn btn-fb"><i class="fa fa-facebook pr-1"></i> Facebook</button>
<button type="button" class="btn btn-tw"><i class="fa fa-twitter pr-1"></i> Twitter</button>
<button type="button" class="btn btn-git"><i class="fa fa-github pr-1"></i> Github</button>
<button type="button" class="btn btn-li"><i class="fa fa-linkedin pr-1"></i> Linkedin</button>

You can also send me a quick message using the form below:
 <div class="well">
            <h3>Create a Message</h3>
            <hr />
            @using (Html.BeginForm())
            {
                <fieldset>
                    @Html.AntiForgeryToken()\
                    @Html.ValidationSummary(true, "", new { @class = "text-danger" })
                    @Html.HiddenFor(model => model.Id)
                    <div class="form-group">
                        @Html.LabelFor(model => model.Receiver, htmlAttributes: new { @class = "control-label col-md-2" })
                        @Html.EditorFor(model => model.Receiver, new { htmlAttributes = new { @class = "form-control" } })
                        @Html.ValidationMessageFor(model => model.Receiver, "", new { @class = "text-danger" })
                    </div>
                    <div class="form-group">
                        @Html.LabelFor(model => model.Body, htmlAttributes: new { @class = "control-label col-md-2" })
                        @Html.TextAreaFor(model => model.Body, 5, 55, new { htmlAttributes = new { @class = "form-control" } })
                        @Html.ValidationMessageFor(model => model.Body, "", new { @class = "text-danger" })
                    </div>
                    <div class="form-group">
                        <input type="submit" value="Send" class="btn btn-default" />
                    </div>
                </fieldset>
            }
        </div
