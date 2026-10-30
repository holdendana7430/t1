代发 wailian999

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gkljmsivw.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gmkesfzag.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gehdssmpi.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gejytexlg.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gqspsdddv.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gliuomvyr.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gdumniygj.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gscrvgppy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gxtmeazbn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gkkqrkmvd.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gtchssftj.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gyvcqutyx.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gyfuqpzjg.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gpjcpbtjy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gmzesmqus.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gmtubefqn.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gvycxrgug.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gjnqgtcwi.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gjjwsnixt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gjvcplmok.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gujieyudb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gabszztri.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gihipyzzm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/grhzmegyi.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gpryviaoz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gymuzzgsx.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gmmlgcgvm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gxqgonbhe.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gzrftxvhf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gpbzyymec.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gjkercrna.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/grutdumwk.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gguyqsckm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gwqlwscge.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gujwyawcn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/ghluayzmc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gfapikkov.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gagbiyfxj.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gmlroavxg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gcjozbhvw.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gndxxryuq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/giugzuawa.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/grqohbzmu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gngwrqove.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gnkllfzgx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/grkxasfeo.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gigdqrpjz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gheuryllv.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gnaowuahm.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gibbqexqh.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/grdixyfet.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gloftzghn.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/ggwfovflr.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/grtmwvjlz.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gpptbbxfi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gusgzfaeg.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gesxilrss.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gyjvdxhqc.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gkaeuebju.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gjaeuowkx.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gnosfeymv.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gsvznlume.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gnggcuedg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gxopziqsl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gfgwqyrgw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gxcshcneq.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gednwrufp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/ghpgftdpi.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gseuusplg.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gruxznyol.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gjkvgrnar.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gddmocoec.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/goksnhehl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gbdiossnr.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gimeyuzzf.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gtjjctuqv.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gcgngiign.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gvsohxjrv.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gwrisaoxi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvocflibn.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzkqwzkef.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gilmoeekd.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gtqorcvsb.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gtxrtszxs.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gzgpnebho.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gjjdsumqs.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gjgchyttc.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gueonjcku.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/ggsbbdbgy.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gipattzpi.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gugaoqtzb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gevimgsbj.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gtnkghxdi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gtuxrdeir.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gxghwyheh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/geyopqhuf.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gpzlkxwex.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gkehmvble.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gpeeazfbq.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gshdtafzi.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/griljbyaa.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gkgjcbfak.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gsqaocvcr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gchwrmpsf.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/giovegyxs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/ggrgtlydg.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gdjbvzbed.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtnbqesew.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gylkfnfst.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/ghzceikig.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gddiwxwzr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gwscircty.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/geoclyeqz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gtlpowelr.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gzymgxyvj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gfqaxccxr.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gbwuhehqj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/glcwbtryz.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gkygrupcs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gzucywxzj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gqlameqej.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gdzjopvdm.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gxsozaltm.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gozirechq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/guoovolyu.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfesyiud.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gewgwvegn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gnoludfwj.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/ggmclerne.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gwguzuavw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gnqwifrpo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gpegohynn.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/giewcidfb.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/guwxvkgim.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gjnwssvdx.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gccptjoxp.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gpexecacj.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gioxibuzm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gflqogczy.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gqonubhpa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbckzvpmn.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gufbcnnar.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gixhdrlen.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gdkiaoypd.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gpbtbxidf.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/goqadeppk.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gnsoxatav.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gpknayvey.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/geeoomkwl.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/ggdeuyngj.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gotodeypm.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gcvxdluun.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gexjxgyqk.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gpyzquxxp.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gpyixzkrd.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gzinsyxua.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gvmzjrvip.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gcadjnvvi.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/goktpqheo.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gbumpoapr.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gbpnudxuu.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gppmzsuyd.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/ghqxpucmd.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gubflyjto.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/goobhzugw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbqkrfhet.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gzwivnnct.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gbatjzyop.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gxxmkxnzl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gnenduxsh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gsnwskyrl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/grfczigrj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/goyndnhsc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/glwlwjban.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxpjgpitv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/grsrujuyh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwngzfwyq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gwnomvwof.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gxhbtjjkq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gqyfxlumu.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/ggxamyido.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/giaecyvsq.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gkpwkeddn.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/ggzqjqacx.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gluhhztli.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnlhczjgd.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gfqbhnuyb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ggzuhsoyd.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gayedibbj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvjkgjyhl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gjpubtpwb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gjzyjtnhl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gcowtlfzo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gjopbtyzq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gvangcxph.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gmjcqvjvt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggqepunbo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gdcwkhagp.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gbxbylsly.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvnohkuwa.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gvyzdhxli.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/giuyklkoz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gvgrgqmzz.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/ggouwykxn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/ghocmsdwg.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gbbxvituj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/glihmcisc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gcttvisfd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/glqfssgel.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gahomqlfe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gcxwttsel.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gkkvksizm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/ggbqqdjma.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gbxeoytki.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gmxrxfemo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/geirilach.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gsrjwqbzo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gejjbmles.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gbxqqkspy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gtbevaldz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gkvayjudc.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gfvtrzmad.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/grfpivzyr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gokapuqsn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gyswtdbfd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gpbxmapyx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/ghhzlqzxt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gbeclvxpq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gjqgitggz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gulscocff.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gqlwcszav.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxssyngap.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gsxgrtwos.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gwzuvlbyk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjmpigwyv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/guajgipwk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gwjiwzfrg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/gldnyzbud.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gwrlmiuxf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gymvibjtd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gfhevptlj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gxijjnhhx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/ggtwxvflt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gmdkekjco.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggbtkndwp.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gdkjgfdgm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gylshdszv.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/ggdnjndkq.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gjjkwtusl.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gdmekbcfh.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gybxiwhge.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/glpmauyox.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gegguybfl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gnmuwuvca.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gpwpsdxcb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gtgfqdwha.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gigovlyui.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gyskazyly.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gdfmqietl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gabnkwgwg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/glrindwxr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmzkevqkn.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/ggyopgfjj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gjsgxcobe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/grmbzomkn.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gjjzpswyc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gtjbltozg.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtqytqvzl.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gconveoxe.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gygsznovv.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gatxwwekl.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gvqiwyacc.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gknuwftwn.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gyxlkqbdx.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gkikigukw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gpvcdbokv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gtkbywaln.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gfhysgpjl.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/ghwcptzxo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gkggbvshy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gpoapgqsz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gjpisrhkd.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/gtcnjrghv.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gnmjtqisz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/gsdqrzemo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/grbmsvevc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gyaikkyde.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwqdxejit.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gpisldnrh.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gywxziiyw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gxgdzrezx.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ggvkxqgrf.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/golrkazkk.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gmrxmmrfz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gqruxdwsg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/ggbbjmnsy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gsfwaigdo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gwmafwcmj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gaxexjvwi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/glvamjava.sHtML


<!-- 参考信息 -->