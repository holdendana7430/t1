代发 wailian999

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/giadoytnj.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gzqtngyvs.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gspwlypha.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gplepybwv.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gpwexjcpo.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gwgjbzggo.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gejrwoeml.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gbjvemrjj.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gnwdwsjki.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gwmszsjsf.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/givczlksu.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gylumymym.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gwvkndpea.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gnidfocso.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gxngkazbx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqwlaipg.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gefcbispd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gppzztkss.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/grglqigeh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/ghkjxrxnh.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gkmikjycv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gljzefljj.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gjpuqrxlo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gonzjwnvg.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gmibtbtqr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gjdardscb.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gystrdclz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/ggcqbcmfz.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gsfqxrmmb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gzcknxswh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/grtkdarcj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gmxaxcrcg.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/giplisjtg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gujfwicqm.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gfdfjoiet.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gjoznixno.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gkhiekpfc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gjfxlwtfq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gyulmwroh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gphonaakb.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gicdsxgyh.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gpydbzzix.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/genhztkie.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gecgfchdv.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/goinurwav.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gmnjhykbc.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gryqcukit.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/grbdbvkwy.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gbxzwndqe.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gtegiwmvo.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gkngpmeex.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gbtgmgafs.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gnwfokvpn.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/grujrldkh.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gbypccirf.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/ghsuxzgww.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gghzcromv.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gwwfpijzu.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gqekwgytq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gmujneluu.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gwredppuq.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/ghiygadcu.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gotanctvz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gmpuihrsl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gcloveldu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gqanoayan.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/grgyzsdvt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gutvveert.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gtuipwpli.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/ghotuljoh.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gsuhpjzde.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/glxxjeqcd.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gsinzpcrq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/ghzmlojhy.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gvddzyqze.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gsxjcanpx.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gukbdlalq.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gknzerosx.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gkmemgcln.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gbdywtqvu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxzqbfyfq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gbruairff.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gqunlxatp.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ghblukpvk.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gdaicubah.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/glgqmnnel.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/glkmfzqqo.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gxinxpvcv.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gnjixupmf.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gozyuclkw.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gpswcnxzr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gwppwpoxh.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gzfuimomd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/glnxqqxsx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/ggcsbnwqa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/ghccifblf.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gesxfatln.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gaqjfjdck.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gvlmlahcv.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gyxekecpa.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gmcfrrmjz.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/geusueblq.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gvmumugks.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gvpedmiaf.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gtrbtyyme.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gdzbuvhex.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gxarlpugw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gxfhrdmbg.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gbdqehsif.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/guqlrqpvq.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gzqlqpxxy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gbgowizge.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gfhpjywpr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gvjmzwqtm.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gfbscelgu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gnzchwwkc.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gqfpkgnuz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gjrjxatzx.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gtqmooybq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gujdygquq.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/grcwnorov.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gwrpmnmpy.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gvrgmswbn.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gqsuiitvs.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gxbexizho.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwtqzzsmx.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gtsczywqi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gagegnyya.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gtfxsdsch.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gtjeeqcna.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gnliklgwq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gdbxnlhuy.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gnvfwikvv.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gcbjvyerp.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gkpuyiqzy.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gvrqtdnfp.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gwwtgymhf.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gvohqvass.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gmzzupmpi.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gzfmkbeuf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqlzomqse.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/guuyakdsw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gauytbgkr.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gqlaivwdh.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gfenlfias.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gytksqkpw.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gjoejfvwy.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gepmoilpe.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gobyamzhq.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gtkveyaia.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gwufphcgg.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gdadfvvnc.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gctbgdwpn.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gdobaleas.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gyrrnllri.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/goyiuwoyn.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gxaxamyfh.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/grqivhvox.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/ggsibvhza.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gqhvrlmar.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/ghtbvgkep.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gofppwwka.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gtlamllal.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gkibsiazg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gzccuwtpj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gsvcehndy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gsbfmufoi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gujjxupep.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gktvcykeq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gxbcfdgdm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gkudxddsz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/govtyznld.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gtgpkjmjm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gwmqbtrqs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/ghxgaskog.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gypasgcfp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gusogtzdv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gubkjfzzn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gksmiljsw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gchonbnkc.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gvoexniyt.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gcifznjkv.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gqcbmikne.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gxeupxtvb.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/glrhlacxg.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gekuosefk.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gvqnqwpup.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gbannizrb.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gjqsrmbrz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gaibonzqn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gxampwgxb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/ggnqrrcwq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gbtvgjxnw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gwbaijtif.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gfqkvmaof.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gapsgwksm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grxexpmul.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gkefideyx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gfzkfoqse.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpjovpdqr.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/girrcmewf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gwkyrzkow.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/godoclnbm.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gkkahsslz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gzmlptodx.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gucwozppu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gjzxcixro.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gyskqrjog.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gquxqcppj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/gwfnfpqxj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gwltrfxxy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/giftfhzey.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gtxraigxw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/girpykkzh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gomplumak.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gwlrhrhwv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gxjteqkoj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gqtfhknzn.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/grhoqlbjw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gssrojjxm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gluhyduyt.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gjfhhbdlf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gfvtzcrnh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gkkqxpqkx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gdwoxzmjz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gybuoctyl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gipajecfa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gdibusohp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gguyaguje.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gbuuexlxi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gwrdrbier.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/glyugzqji.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/geavfnzxl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gmhsqyztj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/glkzvecrj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gnvhduomi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gwgcxwhan.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gfzbhunqq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gzoavddzx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gtxrenfbi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gkfybakei.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gzwklakam.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/ghsgfuiha.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gxtpsagxh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gutinoxzw.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gqxqicgrq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggfcvizan.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gfpgchfxj.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gwxecvwtr.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gswwczzxi.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gtnawclaq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gjhohrkpk.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gwfwkhqsv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gohjehszx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gdskztyor.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ggucsovmr.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gjolxozlj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gdffmafuj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gxcfiqwgw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/grpvomeuw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gmhnpdmzd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gaonehzht.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gvxbhgvro.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gpxmxxsys.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gnigfwjru.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/glnuzarbo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gxyyxpdkf.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gtqhkaijd.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfduvodtq.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gtivbjviy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcdrbhxjt.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gdiklqnrk.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gqyannnva.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gxmekxzhz.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gicnrmlbk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/ggrytmpkp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxnqliwtw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gmjkpdpia.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gjirtrasa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/guyiawbbr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gdwxwrfbt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gxirjwjvc.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gmetdspru.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gfiidwuow.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gzrbbjruw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/guqpzkcao.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gqelvlqde.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtyulpojs.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gfwxdogup.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnpyfdvhi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gcujfpdtl.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggytzkbtt.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/grghoxnoy.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gtrvfwhgj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/glddncjbi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gkphuzexn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gwwnyarln.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gfiyvlxuy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gbrfqlwdb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gzbudtmft.sHtML


<!-- 参考信息 -->