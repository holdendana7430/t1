代发 wailian999

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggjhowcfc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gugokplze.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwofrzee.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/goxiklvtj.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/ggmocohqj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gnagwagqq.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcdfrsma.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gepcqzeqx.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhzdqyob.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gozlozccr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmdydxbf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrgbapw.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gddglvzju.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqecwdgko.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzjzdtbx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gzndinuis.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/ggksupnbp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhiwqvst.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyflofeco.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzcydgjo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszlvyoqr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsynmrhi.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfrdsaon.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gseblthui.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gqhskebdo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqpbkunj.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gnuqvcjqd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gymhijjgx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjzsgptv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfdytnpl.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/grzamayui.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gnzitolsw.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gkbifetpk.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqjxjmkv.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gzsdnlmml.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmaezksl.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjocfnwgl.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gkmwuqlxd.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gwoijjtfs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrsyrjrz.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gzxlmbktv.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/grdwqqsss.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gukvzvzhd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gxptsqesy.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/ggtdcechf.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gzinlhhtl.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjfkcnii.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/guqkoixhb.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gffgfykur.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gdwzqsqct.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmcljrbr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gwuszxnfi.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/giywbzrat.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gontvjsxy.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gvodbbqnl.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gursddhrn.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/getqkufzf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtczvrtvt.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaqiyejb.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtinrfss.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gfqoswgpj.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gigfsilmr.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfhghksdv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gctgrfabm.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gaovfyoya.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/geebdxwtw.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gehdmrnlr.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/goewrcwcw.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggeyuwxww.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gewviaeeq.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpiceglju.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gvcisbrqi.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprnmqqgp.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gjxuhjhtf.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gnueytjuf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfqfkoke.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gxkdosqwq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givdcvxvh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrpjkwly.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gccilvkka.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqvopezj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocpdkolz.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzysdyws.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gnqfjnnwc.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkcivjzv.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/grwtogxjf.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/guyhvuntt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/glscrmopc.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxfvfyvy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gghtpeuci.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpvjkcxn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbybbmim.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gkteznpmm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqgetxzt.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gebhygsdh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/grztdudpn.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzkjmnrn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/giineuqtt.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaczgguhl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrbgdxbn.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwairhubn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gstqzxeje.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/ghnwhyjpv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gjathytsc.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukbaubnj.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gmpbgsqag.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwvgtnpx.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gyszyvfsw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gylqpnndy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkhfimgq.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvqouwkfx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gaeidrpnd.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gzllnbwuu.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gdcnzpbxf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrmotwl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnvkyhok.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcasaufy.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbemsyiq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbchbqphm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gphvphoeb.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gwuylhisn.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gmapuhhne.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gdfncuuug.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gwybwebot.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gddhoiteb.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gjudumetr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtspymwrm.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryemwvvu.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gjihqwpwd.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcepsfluq.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsxbpvsk.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrilcdlp.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzgggzes.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeygchcz.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gogucflgz.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/grnxvbmeh.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhxkzzue.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gdcpreymy.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gwsqtoptq.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gnyyqxfvm.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gddliqljc.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwtxovlt.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gcyoduarq.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnaejihb.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gdanliolv.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gcslufwkx.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gekfnctit.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmmbqros.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaihwotp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/guesfqyre.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gakxaynkm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gplrzdvyu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuyvhkju.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/geyhyzkhe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/glgayoxcv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gtqcqmweq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gszebmprz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwwojeda.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdditsab.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdejzwlev.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gapmcxunr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/ghglmrcjo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsyszvsr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsctbavbk.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gorabgdyp.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdlthmeb.sHtML

S C / C++ 专题                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/grxqwyuxw.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/giysjbmat.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvejpoqi.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gzycwrail.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwabuznb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtvuonaj.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzujbrrg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywbkfwup.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhrhofoj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gtswwulrx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsdvwops.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gfhhatrnt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwriiwbje.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gahholjvk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdsmgghi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gokquogob.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gvbyqrjzd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdpjqik.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuhtdpfw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gbacabeok.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimgbfvia.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlfkoksc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gkjwgrmfi.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlbludks.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gfljnaewi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/ggljagfom.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gciuuftrf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/ghadqcxzo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxegixp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfctgwiuj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gywlqsznx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmiazift.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gjainmydg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gipavuhpx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiasgibj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gqasphwgl.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gewugehfw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrzjutro.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfocfcbv.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhwxaetc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfpdbpekz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guganejvx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzfoxpao.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gtlwewuvh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbamxxlls.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlzewjai.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghanfwapn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvgniian.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxpwlotqg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqrjoeldv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/giytrupmo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdglopzzp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtxmbspd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gttvzspgg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gabzvkphm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjxlbtiyu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gafmubbfa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glnfybjum.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjelftiky.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlyotped.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsczacyad.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgowkuca.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxxvhydb.sHtML

A. 基础语法与类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gltjfedcd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbptiyixb.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grhxvdlqj.sHtML

Py:   print("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gxomhqied.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrhtkynv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszbsxrjw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/gosoquhic.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtuxfapk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiuvpygc.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhjrxpmw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gklbogsfv.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsewjgqj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsttibkau.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gigfadjbj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlkuylir.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwhkhewc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyrptwad.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyohwfgv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxqoylgg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbxhotbs.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/glngpvumd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlndocyy.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaariwwik.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhsipxxj.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdofkhvop.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gunvbnhxt.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gnvohenpp.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fanxiaobao.xyz/Article/details/gmukxupif.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqryrlwa.sHtML

[A04] 判断变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/geimsjbng.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gebjpyexg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/geacglaue.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gdmihpaja.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gookilsvn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwrzzrw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajrfnyrx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/geocvtmzh.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqtqkdox.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawbvxduj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqutgxtyz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsbwoqbyc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstmbwpnm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcoowaai.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gahismkxe.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmhdmkty.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gwqznrpqi.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrfcjmq.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvcdzezhu.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxabnkfh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdccnvzwc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/glmbbtvoz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcwpxogr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/ggsmsumxk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrhpqorl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbdwknvk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fanxiaobao.xyz/Article/details/ghwqdnsbj.sHtML

[A07] 数字转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gglyjxbua.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjggfcgx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqccrudt.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gfbatysiy.sHtML

TS:   String(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnibolrby.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gkvhbrsjl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfudgzkoc.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/glslaaavj.sHtML

C#:   42.ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/gzjwgraid.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gmhrfvolv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyavzqqug.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxabbbupf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gizdwxsmp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlxlvona.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqotkpgm.sHtML


<!-- 参考信息 -->