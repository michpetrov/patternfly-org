---
title: Area Chart
author: lhinson
layout: page-no-design-tabs
url-js-extra: ['//cdnjs.cloudflare.com/ajax/libs/c3/0.4.10/c3.min.js', '//cdnjs.cloudflare.com/ajax/libs/d3/3.5.0/d3.min.js']
---
<div class="tab-content">
  <div role="tabpanel" class="tab-pane active" id="overview">
  <!--
    <p>TODO: Add Area chart description</p>
    -->
    <p>Jump to <a href="#example-overview-1">Area Chart</a> or <a href="#example-overview-2">Single Area Chart</a></p>
    <h2 id="example-overview-1">Area Chart</h2>
    <div class="row">
      <div class="col-md-7">
        <div class="example-pf">
          <div class="cards-pf">
            <div class="container-fluid container-cards-pf">
              <div class="row row-cards-pf">
                <div class="col-md-12">
                  <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
                  {% include widgets/charts/area-multiple.html chart1="area-chart-1" %}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-7">
        <h2 id="example-overview-2">Single Area Chart</h2>
        <div class="example-pf">
          <div class="cards-pf">
            <div class="container-fluid container-cards-pf">
              <div class="row row-cards-pf">
                <div class="col-md-12">
                  <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
                  {% include widgets/charts/area-single.html chart1="area-chart-2" %}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div role="tabpanel" class="tab-pane" id="design">
    <h2>Description</h2>
    <div class="row">
      <div class="col-md-4 col-lg-3">
      </div>
      <div class="col-md-8 col-lg-9">
      </div>
    </div>
  </div>
  <div role="tabpanel" class="tab-pane" id="code">
    {% include nav-tabs-code.html angular=false %}
    <div class="tab-content">
      <div role="tabpanel" class="tab-pane nested active" id="html-css">
        <p>Jump to <a href="#example-code-1">Area Chart</a> or <a href="#example-code-2">Single Area Chart</a></p>
        <h2 id="example-code-1">Area Chart</h2>
        <div class="row">
          <div class="col-md-8" style="padding-right: 0px;">
            <div class="example-pf">
              <div class="example-pf-demo example-pf-demo-no-padding">
                <div class="cards-pf">
                  <div class="container-fluid container-cards-pf">
                    <div class="row row-cards-pf">
                      <div class="col-md-12">
                        <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
                        {% include widgets/charts/area-multiple.html chart1="area-chart-3" %}
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <p class="reference-markup"><a class="collapse-toggle" data-toggle="collapse" aria-expanded="true" aria-controls="card-markup-1" href="#card-markup-1">Reference Markup</a></p>
        <div class="collapse in" id="card-markup-1">
          <pre class="prettyprint">{% capture markup_include %}{% include widgets/charts/area-multiple.html chart1="area-chart-3" %}{% endcapture %}{{ markup_include | xml_escape }}</pre>
        </div>
        <h2 id="example-code-2">Single Area Chart</h2>
        <div class="row">
          <div class="col-md-8">
            <div class="example-pf">
              <div class="example-pf-demo example-pf-demo-no-padding">
                <div class="cards-pf">
                  <div class="container-fluid container-cards-pf">
                    <div class="row row-cards-pf">
                      <div class="col-md-12">
                        <!-- Important:  if you need to nest additional .row within a .row.row-cards-pf, do *not* use .row-cards-pf on the nested .row  -->
                        {% include widgets/charts/area-single.html chart1="area-chart-4" %}
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <p class="reference-markup"><a class="collapse-toggle" data-toggle="collapse" aria-expanded="true" aria-controls="card-markup-2" href="#card-markup-2">Reference Markup</a></p>
        <div class="collapse in" id="card-markup-2">
          <pre class="prettyprint">{% capture markup_include %}{% include widgets/charts/area-single.html chart1="area-chart-4" %}{% endcapture %}{{ markup_include | xml_escape }}</pre>
        </div>
      </div>
      <div role="tabpanel" class="tab-pane nested" id="angular">
        <div ng-app="docsApp" ng-controller="DocsController" class="content">
          <div ng-include src="'/components/angular-patternfly/dist/docs/partials/api/patternfly.charts.directive.pfDonutPctChart.html'"></div>
        </div>
      </div>
    </div>
  </div>
</div>