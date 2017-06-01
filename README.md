

import gulp from 'gulp';
import gulpif from 'gulp-if';  // 语句中做if判断的
import concat from 'gulp-concat';  // 处理文件拼接
import webpack from 'webpack';  // 打包
import gulpWebpack from 'webpack-stream';  // gulp处理的都是文件流结合webpack处理的工具
import named from 'vinyl-named';  // 文件重命名
import livereload from 'gulp-livereload';  // 热更新
import plumber from 'gulp-plumber';  // 处理文件信息流
import rename from 'gulp-rename';  // 对文件重命名
import uglify from 'gulp-uglify'; // JS，CSS压缩
import {log, colors} from 'gulp-util';  // 命令行工具输出的，log.color输出
import args from './util/args';  // 命令行参数进行解析
