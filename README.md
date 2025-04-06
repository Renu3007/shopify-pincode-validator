{% schema %}
{
  "name": "Pincode Validator",
  "settings": [],
  "presets": [
    {
      "name": "Pincode Validator"
    }
  ]
}
{% endschema %}

<div class="pincode-validator">
    <input type="text" id="pincode-input" placeholder="Enter your pincode" />
    <button id="check-pincode">Check Availability</button>
    <p id="pincode-result"></p>
</div>


<style>
.pincode-validator {
    margin-top: 20px;
}
#pincode-input {
    padding: 8px;
    width: 200px;
}
#check-pincode {
    padding: 8px 12px;
    background-color: #eb2244;
    color: #fff;
    border: none;
    cursor: pointer;
}
#pincode-result {
    margin-top: 10px;
    font-weight: bold;
}
</style>
