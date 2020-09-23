<template>
  <div>
    <!-- Content Header (Page header) -->
    <div class="content-header">
      <div class="container-fluid">
        <div class="row mb-2">
          <div class="col-sm-6">
            <h1 class="m-0 text-dark">SAJ WATER MONITORING DASHBOARD</h1>
          </div>
          <!-- /.col -->
          <div class="col-sm-6">
            <ol class="breadcrumb float-sm-right">
              <li class="breadcrumb-item">
                <a href="#">Home</a>
              </li>
              <li class="breadcrumb-item active">Dashboard</li>
            </ol>
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row -->
      </div>
      <!-- /.container-fluid -->
    </div>
    <!-- /.content-header -->

    <!-- Main content -->
    <section class="content">
      <div class="container-fluid">
        <!-- Info boxes -->
        <div class="row">
          <div class="col-12 col-sm-6 col-md-3">
            <div class="info-box">
              <span class="info-box-icon bg-info elevation-1">
                <i class="fab fa-artstation"></i>
              </span>

              <div class="info-box-content">
                <span class="info-box-text">STATION 1</span>
                <span class="info-box-number">UTM</span>
              </div>
              <!-- /.info-box-content -->
            </div>
            <!-- /.info-box -->
          </div>
          <!-- /.col -->
          <div class="col-12 col-sm-6 col-md-3">
            <div class="info-box mb-3">
              <span class="info-box-icon bg-danger elevation-1">
                <i class="fab fa-artstation"></i>
              </span>

              <div class="info-box-content">
                <span class="info-box-text">STATION 2</span>
                <span class="info-box-number">SKUDAI</span>
              </div>
              <!-- /.info-box-content -->
            </div>
            <!-- /.info-box -->
          </div>
          <!-- /.col -->

          <!-- fix for small devices only -->
          <div class="clearfix hidden-md-up"></div>

          <div class="col-12 col-sm-6 col-md-3">
            <div class="info-box mb-3">
              <span class="info-box-icon bg-success elevation-1">
                <i class="fab fa-artstation"></i>
              </span>

              <div class="info-box-content">
                <span class="info-box-text">STATION 3</span>
                <span class="info-box-number">PASIR GUDANG</span>
              </div>
              <!-- /.info-box-content -->
            </div>
            <!-- /.info-box -->
          </div>
          <!-- /.col -->
          <div class="col-12 col-sm-6 col-md-3">
            <div class="info-box mb-3">
              <span class="info-box-icon bg-warning elevation-1">
                <i class="fab fa-artstation"></i>
              </span>

              <div class="info-box-content">
                <span class="info-box-text">STATION 4</span>
                <span class="info-box-number">KULAI</span>
              </div>
              <!-- /.info-box-content -->
            </div>
            <!-- /.info-box -->
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row -->

        <div class="row">
          <div class="col-md-12">
            <div class="card">
              <div class="card-header">
                <h5 class="card-title">Graphical Report</h5>

                <div class="card-tools">
                  <button type="button" class="btn btn-tool" data-card-widget="collapse">
                    <i class="fas fa-minus"></i>
                  </button>
                  <div class="btn-group">
                    <button
                      type="button"
                      class="btn btn-tool dropdown-toggle"
                      data-toggle="dropdown"
                    >
                      <i class="fas fa-wrench"></i>
                    </button>
                    <div class="dropdown-menu dropdown-menu-right" role="menu">
                      <a href="#" class="dropdown-item">Action</a>
                      <a href="#" class="dropdown-item">Another action</a>
                      <a href="#" class="dropdown-item">Something else here</a>
                      <a class="dropdown-divider"></a>
                      <a href="#" class="dropdown-item">Separated link</a>
                    </div>
                  </div>
                  <button type="button" class="btn btn-tool" data-card-widget="remove">
                    <i class="fas fa-times"></i>
                  </button>
                </div>
              </div>
              <!-- /.card-header -->
              <div class="card-body">
                <div class="row">
                  <div class="col-md-8">
                    <p class="text-center">
                      <span class="dot-blue"></span>
                      <strong>Ammonium</strong> &nbsp;&nbsp;&nbsp;&nbsp;
                      <span class="dot-gray"></span>
                      <strong>ph</strong>
                    </p>

                    <div class="chart">
                      <!-- Sales Chart Canvas -->
                      <canvas id="salesChart" height="180" style="height: 180px;"></canvas>
                    </div>
                    <!-- /.chart-responsive -->
                  </div>
                  <!-- /.col -->
                  <div class="col-md-4">
                    <p class="text-center">
                      <strong>Realtime Reports</strong>
                    </p>

                    <div class="progress-group">
                      Ammonium Ion NH4+
                      <span class="float-right">
                        <b>0</b>/200
                      </span>
                      <div class="progress progress-sm">
                        <div class="progress-bar bg-primary" style="width: 80%"></div>
                      </div>
                    </div>
                    <!-- /.progress-group -->

                    <div class="progress-group">
                      pH
                      <span class="float-right">
                        <b>0</b>/14
                      </span>
                      <div class="progress progress-sm">
                        <div class="progress-bar bg-danger" style="width: 50%"></div>
                      </div>
                    </div>

                    <!-- /.progress-group -->
                    <div class="progress-group">
                      <span class="progress-text">temperature</span>
                      <span class="float-right">
                        <b>0</b>/50 &#176C
                      </span>
                      <div class="progress progress-sm">
                        <div class="progress-bar bg-success" style="width: 70%"></div>
                      </div>
                    </div>
                    <!-- /.progress-group -->
                    <div class="progress-group">
                      <span class="progress-text">Turbidity</span>
                      <span class="float-right">
                        <b>0</b>/40 NTU
                      </span>
                      <div class="progress progress-sm">
                        <div class="progress-bar bg-success" style="width: 70%"></div>
                      </div>
                    </div>

                    <!-- /.progress-group -->
                    <div class="progress-group">
                      O2 Level
                      <span class="float-right">
                        <b>0</b>/120
                      </span>
                      <div class="progress progress-sm">
                        <div class="progress-bar bg-warning" style="width: 50%"></div>
                      </div>
                    </div>
                    <!-- /.progress-group -->
                  </div>
                  <!-- /.col -->
                </div>
                <!-- /.row -->
              </div>
              <!-- ./card-body -->

              <!-- /.card-footer -->
            </div>
            <!-- /.card -->
          </div>
          <!-- /.col -->
        </div>
        <!-- /.row -->

        <!-- Main row -->
        <div class="row">
          <!-- Left col -->
          <div class="col-md-12">
            <!-- MAP & BOX PANE -->
            <div class="card">
              <div class="card-header">
                <h3 class="card-title">Station Map</h3>

                <div class="card-tools">
                  <button type="button" class="btn btn-tool" data-card-widget="collapse">
                    <i class="fas fa-minus"></i>
                  </button>
                  <button type="button" class="btn btn-tool" data-card-widget="remove">
                    <i class="fas fa-times"></i>
                  </button>
                </div>
              </div>
              <!-- /.card-header -->
              <div class="card-body p-0">
                <div class="d-md-flex">
                  <div class="p-1 flex-fill" style="overflow: hidden">
                    <!-- Map will be created here -->
                    <div id="world-map-markers" style="height: 325px; overflow: hidden">
                      <div class="map"></div>
                    </div>
                  </div>
                </div>
                <!-- /.d-md-flex -->
              </div>
              <!-- /.card-body -->
            </div>

            <!-- TABLE: LATEST ORDERS -->

            <!-- /.card -->
          </div>
          <!-- /.col -->
          <div class="col-md-12">
            <div class="card">
              <div class="card-header">
                <h3 class="card-title">All Stations List</h3>
              </div>
              <!-- /.card-header -->
              <div class="card-body">
                <table id="example1" class="table table-bordered table-hover">
                  <thead>
                    <tr>
                      <th>Station ID</th>
                      <th>Station Location</th>
                      <th>Ammonium</th>
                      <th>Temperature</th>
                      <th>ph</th>
                      <th>Turbidity</th>
                      <th>Station Status</th>
                      <th>Station Details</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td>001</td>
                      <td>UTM</td>
                      <td>0.00</td>
                      <td>0.00 &#176;C</td>
                      <td>0.00</td>
                      <td>-</td>
                      <td>
                        <span class="badge badge-success">Running</span>
                      </td>
                      <td>
                        <span class="badge badge-warning">View More</span>
                      </td>
                    </tr>
                    <tr>
                      <td>002</td>
                      <td>Skudai</td>
                      <td>0.00</td>
                      <td>0.00 &#176;C</td>
                      <td>0.00</td>
                      <td>-</td>
                      <td>
                        <span class="badge badge-danger">Down</span>
                      </td>
                      <td>
                        <span class="badge badge-warning">View More</span>
                      </td>
                    </tr>
                  </tbody>
                  <tfoot>
                    <tr>
                      <th>Station ID</th>
                      <th>Station Location</th>
                      <th>Ammonium</th>
                      <th>Temperature</th>
                      <th>ph</th>
                      <th>Turbidity</th>
                      <th>Station Status</th>
                      <th>Station Details</th>
                    </tr>
                  </tfoot>
                </table>
              </div>
              <!-- /.card-body -->
            </div>
          </div>

          <!-- /.card -->
        </div>
        <!-- /.col -->
      </div>
      <!-- /.container-fluid -->
    </section>
    <!-- /.content -->
  </div>
</template>

<script>
export default {
  layout: 'dashboard',
  components: {},
}
</script>

<style></style>
