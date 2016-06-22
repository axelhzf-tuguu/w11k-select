# w11k-select Changelog

<a name="0.6.6"></a>
## 0.6.6 (2016-06-22)


### Bug Fixes

* **tabIndex:** make w11k-select accessible via keyboard with the tab key


<a name="0.6.2"></a>
## 0.6.2 (2015-07-06)


### Bug Fixes

* **infinite-scroll:** rename directive to w11k-select-infinite-scroll to avoid name-conflicts ([4044bef0](https://github.com/w11k/w11k-select/commit/4044bef053bcd43ad58515b5bd334ac17c3c4916), closes [#20](https://github.com/w11k/w11k-select/issues/20))


<a name="0.6.1"></a>
## 0.6.1 (2015-01-26)


### Bug Fixes

* **track-by:** improve hash function used to calculate ng-repeat track-by value ([03cd453e](https://github.com/w11k/w11k-select/commit/03cd453ee873ab7ee3c4c99109d53c2f6d1bf4a7), closes [#17](https://github.com/w11k/w11k-select/issues/17))


<a name="0.6.0"></a>
## 0.6.0 (2014-11-11)


### Bug Fixes

* **bower:** update dependency to w11k-dropdownToggle ([ef1aeb4c](https://github.com/w11k/w11k-select/commit/ef1aeb4c9b7677106ab8622970fba8311be26632), closes [#14](https://github.com/w11k/w11k-select/issues/14))
* **filter:** select only one item in single selection mode ([8c928b97](https://github.com/w11k/w11k-select/commit/8c928b976f8a77b51d0b964ea069798cfa51075a), closes [#15](https://github.com/w11k/w11k-select/issues/15))


### Features

* **styling:** add LESS support ([4523b512](https://github.com/w11k/w11k-select/commit/4523b512cbff0a79e001ad02cd4b4e4f924d628a))


<a name="0.5.0"></a>
## 0.5.0 (2014-09-29)


### Features

* **bower:**
  * add support for ignoring files via 'ignore' ([200933b8](https://github.com/w11k/w11k-select/commit/200933b80920c42f40bab1c6ab1714bc272ad654))
  * add support for 'main' files ([e70f4f17](https://github.com/w11k/w11k-select/commit/e70f4f17d14cc24edd21468a56fb49475289a4ad))


<a name="0.4.7"></a>
## 0.4.7 (2014-07-21)


### Bug Fixes

* **select:** do not override ng-model with empty selection during initialisation ([585f8a40](https://github.com/w11k/w11k-select/commit/585f8a401f445d799e949f616da17d7635e41fcd), closes [#9](https://github.com/w11k/w11k-select/issues/9))


<a name="0.4.6"></a>
## 0.4.6 (2014-07-21)


### Bug Fixes

* **select:** do not override ng-model with empty selection on config change ([43d1b5a6](https://github.com/w11k/w11k-select/commit/43d1b5a6ea3b20e3d2ecd4cd7579e2ebde2b4f85), closes [#9](https://github.com/w11k/w11k-select/issues/9))


### Performance

* **options:** improve performance for updating options and change ng-model from outside 
  * use hash maps instead of lists and indexOf
  * use while loop instead of angular.forEach

<a name="0.4.5"></a>
## 0.4.5 (2014-07-07)


### Bug Fixes

* **options:** make checkbox click same like label click ([566f2b15](https://github.com/w11k/w11k-select/commit/566f2b1525ca6f6b52bf42bcaa0ef041c065e6cb))


<a name="0.4.4"></a>
## 0.4.4 (2014-06-10)


### Bug Fixes

* **options:**
  * mark options as selected on change of options even if options are objects ([609c0b4d](https://github.com/w11k/w11k-select/commit/609c0b4d4ca3f359e232032d690d3f4202e4ff2d), closes [#7](https://github.com/w11k/w11k-select/issues/7))
  * use watchCollection instead of simple watch to watch options ([02c2b97c](https://github.com/w11k/w11k-select/commit/02c2b97c031d51e45be5964a5a56f85657293239), closes [#6](https://github.com/w11k/w11k-select/issues/6))


<a name="0.4.3"></a>
## 0.4.3 (2014-06-04)


### Features

* **select:** improve styling of 'select all' and 'select none' buttons ([6c2a714e](https://github.com/w11k/w11k-select/commit/6c2a714e36f78d9189752b1a0d155e9df61bb1c2))
* **template:** include dependency to template module ([356cd817](https://github.com/w11k/w11k-select/commit/356cd817bcbe2334d8d52db5dd9e69d9b3cda786))


<a name="0.4.2"></a>
## 0.4.2 (2014-06-02)


### Bug Fixes

* **select:** fix updating header text with custom text ([c85102d3](https://github.com/w11k/w11k-select/commit/c85102d3d434e471f89e9a85884870f2354c68da))


<a name="0.4.1"></a>
## 0.4.1 (2014-06-02)


### Bug Fixes

* **adjust-height:** fix getting parent without 'w11k-select-adjust-height-to' container ([994c81e6](https://github.com/w11k/w11k-select/commit/994c81e6ee5c0edb50b584782557470bffcb2766))


<a name="0.4.0"></a>
## 0.4.0 (2014-06-02)


### Features

* **adjust-height:** improve adjust-height to support custom margin bottom and specifying container ([ef1bedc0](https://github.com/w11k/w11k-select/commit/ef1bedc07f5972ddd8b75a70e7c7961940ae05dc))
* **config:** make everything configurable via constant w11kSelectConfig and w11k-select-confi ([9f1dd673](https://github.com/w11k/w11k-select/commit/9f1dd673cc5b3af6d76446e846d600ded2cf894c))


### Breaking Changes

* Following attributes are no longer available:
  * w11k-select-multiple
  * w11k-select-selectedMassege
  * w11k-select-filter-placeholder
  * w11k-select-placeholder
  * w11k-select-disabled
  * w11k-select-required
  * w11k-select-style

  Use constant w11kSelectConfig and the new w11k-select-config attribute to configure the directive (see readme).

<a name="0.3.4"></a>
## 0.3.5 (2014-05-27)


### Bug Fixes

* **select:** prefix attributes with 'w11k-select' to make IE happy again ([cdb21df9](https://github.com/w11k/w11k-select/commit/cdb21df9559fbf003a312d90c341d6da6cd512b5))


### Breaking Changes

* All attributes used by 'w11k-select' directive has to be prefixed with 'w11k-select-' now.

Use

```
<div w11k-select
     w11k-select-multiple="true"
     w11k-select-disabled="disabled"
     w11k-select-options="option.value as option.label for option in options.data"
     w11k-select-placeholder="'All'"
     w11k-select-filter-placeholder="'Filter'"
     w11k-select-required="false"
     ng-model="selected.data"
     name="demoField"
     >
</div>
```

instead of

```
<div w11k-select
     multiple="true"
     disabled="disabled"
     options="option.value as option.label for option in options.data"
     placeholder="'All'"
     filter-placeholder="'Filter'"
     required="false"
     ng-model="selected.data"
     name="demoField"
     >
</div>
```


<a name="0.3.4"></a>
## 0.3.4 (2014-04-09)


### Bug Fixes

* **options:** do not identify options by index, otherwise changing options won't work ([0cb34def](https://github.com/w11k/w11k-select/commit/0cb34def4f357fe9b967b2f69a96dd2dd883ba64))


### Features

* **performance:** improve performance by not watching options deeply ([45428c6c](https://github.com/w11k/w11k-select/commit/45428c6c770c0ddee6b8e50a0b08f8ff613c471e))


<a name="0.3.3"></a>
## 0.3.3 (2014-04-08)


### Bug Fixes

* **IE8:** fix adjust height in IE8 ([60f9aedc](https://github.com/w11k/w11k-select/commit/60f9aedc4389ba40b6b4c09918e2a6782e0e78d7))
* **options:** set model value on change of options without making the form field dirty ([b2471961](https://github.com/w11k/w11k-select/commit/b247196189ce702fcc3b5c520325d87489b16efb))


<a name="0.3.2"></a>
## 0.3.2 (2014-03-30)

### Features

* **performance:** optimise amount of options added due to infinite scrolling, for smoother scrolling


<a name="0.3.1"></a>
## 0.3.1 (2014-03-30)


### Bug Fixes

* **filter:** call selectFiltered instead of selectAll on enter in filter input ([e48fc290](https://github.com/w11k/w11k-select/commit/e48fc2901fae4f984bbfa53b18e41f0470a6cb34))


<a name="0.3.0"></a>
## 0.3.0 (2014-03-30)


### Bug Fixes

* **directive:** fix memory leak on scope destroy ([ccb0affe](https://github.com/w11k/w11k-select/commit/ccb0affeaefdb8b9ec6413350c65751b0e616f80))


### Features

* **performance:** use infinite scrolling for more than 100 options
* **select:** close select box with 'esc' key ([e579af2d](https://github.com/w11k/w11k-select/commit/e579af2da8456022dcc9ba742727534680b27310))
* **styling:** make font-awesome optional via own css classes and make button texts customisabl ([772f4802](https://github.com/w11k/w11k-select/commit/772f48026cd027a0f4d42eb19f1ba81b3fd826f2))


<a name="0.2.0"></a>
## 0.2.0 (2014-03-28)


### Bug Fixes

* **buttons:** fix clear button, separate code for deselectAll and deselectFiltered ([46cd098e](https://github.com/w11k/w11k-select/commit/46cd098ee2d978df1d3b1ab0da190837d7c2e046))
* **styling:** change css base class from ww-select to w11k-select ([f95d746d](https://github.com/w11k/w11k-select/commit/f95d746d4246423103fd58f002bc4c5ac2c09de6))


### Features

* **dependencies:** eliminate dependency to jQuery ([759ce975](https://github.com/w11k/w11k-select/commit/759ce97594fd1b21be959224020d64929757767b))
* **performance:** render option list lazy (on first open of dropdown)([6283848](https://github.com/w11k/w11k-select/commit/628384802720c9bcde01dc087ae1524b3cf29b70))



<a name="0.1.1"></a>
## 0.1.1 (2014-03-05)


### Features

* **build:** include sass styling in dist ([292e6047](https://github.com/w11k/w11k-select/commit/292e604727ab11cd568766f0e6a3f350471a6928))


<a name="0.1.0"></a>
## 0.1.0 (2014-03-05)

### Features

* **options:** parse options given via attribute as ```"value" [as "label"] for "item" in "collection"```
* **ng-model:** use ngModelController to expose selected options and support validation
* **multiple:** support single- and multiple-select mode
* **disabled:** support disabled attribute to prevent change of selected options
* **placeholder:** support placeholder texts for dropdown header and filter box
* **template:** make template url configurable via config constant
* **selected-message:** support customisable text for toggle-area
