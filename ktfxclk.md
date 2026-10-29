代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/ggymdgswy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gznkdngbt.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gmigswksa.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcombcebt.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcsgxfzwa.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gtqgdmrwc.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/garhhuvkw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gmozzjtny.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gxmvorbbu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/glytbgdcq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/glyftbfzq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/ggfcxovgl.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gefuexfme.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gzcorxgar.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gdaowmzoz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gyybcpegi.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gnannrurx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gjpcbcbgn.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gfbsbadga.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gqzuueobe.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gsofcxffg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/giqwwwtim.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gododcdmg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gztskhbph.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gqtwenrvb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gwtmurupw.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gkpepgnql.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gldbhbzps.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gtihizpfx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/geoojbqxj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/goffrsvyl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gmznicobb.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gtrbgomzh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gbxrkmzcr.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gvguslajz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gbprqkcix.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/guuaapslc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gossxvabv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gxgwtstge.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gsqhcjuno.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gefougkab.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/ginzgorbt.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/ghvodzsmd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gujhlolrr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gspjytnkz.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gbafjufpp.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gfwtjkkhu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gxnwrjkjv.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gxrnhtlro.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/glcqxoqnv.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gtqgzcgcs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gfgyumygi.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gpujlwinz.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gqotcmpqt.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gesqdwahc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gglbjmqac.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/glnvxpzbg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gikuekyex.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gigrkgdvr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gaulihrsy.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gqriushkk.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/guvtwuppz.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gyixhpgpy.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gjfhspdgl.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gjqvmgszi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/ggutdadxm.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gklwjirdw.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gdvlvazlr.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gddsxdmxu.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzdpvtbnv.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gpjuyqgwj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gmmwzawku.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gvyytline.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gagldyujn.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/glishikky.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gmumqziuk.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gbncaezyq.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gzsuciymf.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gwlufydoy.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gaexjgqmp.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/guopaezes.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gfxpgyomt.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/geuvctuvr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gyuepxypk.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gfbmcyqvn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gvitnxrnp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/goprfpgtz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gerqcfkto.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gyyhwufhy.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gjvdvpota.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gcbaewkkh.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/ghpotmifp.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gfcwilpib.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gzpglmorn.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gkkhlzrkz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gnzogsvqp.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gvcjprwbw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gcdgglshi.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gcfkjascs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gdylttjnb.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gegfcnryj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gxqsgafrk.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqgljdnfm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gtyzyvvaf.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gnuabeibg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gkhfuwixm.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gihpwishb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gefdmbcmq.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gmzorlzjr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gytbdayos.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gtiqwodqf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gevnonyaz.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gpmxcbsyx.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gdztwwhpz.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gfilrlpbr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gsoiwdkac.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gwaeihfaw.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtpblrpkt.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gmgrumiof.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gknodbesc.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gmpfkabke.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gvkfhtvre.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gjpqccwbs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/ggyixzeqk.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gxpwkyobu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gzoxrjnyx.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gprrkrwyn.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gjyfpdvgh.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gquaionps.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/ggcgyppzr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gurxsagws.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gvcgtqtrz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvsifzrxg.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/ghgqjtxla.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gurujfauz.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/ganyjtvrz.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gujzmqvsf.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gcgcffelp.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gkrtjlnbp.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/givgeppgs.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/geagsctvu.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gfuuuyiky.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/ggcjmkxcq.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gkkylprwy.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gwerclpfb.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/giiqquonk.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gaekdrbpr.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gvfhmttqf.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gjvwvcgvz.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gjhcsuofa.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gnupdxbpk.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gkwiqkdfh.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gruwldzlw.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gufpslhsp.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gztbsfvzb.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gxlabrimk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gdqeqgqdn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ggqefufkk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gynrqpchu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gvczfoumj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gwndxqoes.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gbryrumnv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gfhmbjyqx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/giygdpfug.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gegouuhjx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gyxhwxmic.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwhppybvn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gzriifsjh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gbzwekzzj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gxhqmmyls.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gzbibefok.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gunufkuuu.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gzflchnbr.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gshnnxpff.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gzefvjtpi.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gwxvcnbxa.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gojdzdadz.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdrujaqyh.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gwysbaqha.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkiithnhu.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gxxxyjnxq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gdepkiuuu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gdksriuap.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gwatewgsk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/grthyvxvb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/golqhpjvt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/glaagyhaf.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gmktrabma.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giosmablu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gtkonpzye.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/grgffckwa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvpauxbee.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gvrelgjbh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/ghtslaath.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gptpkvkci.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gwnajspru.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gbtqkvlgf.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/ggsawckbn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gzrnjxwrl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gzmruquwq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gpirhwjuv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gzmzyngac.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gforzbqae.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gzvzjgwvk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gyccfaaob.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gkbaaqgxp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gebyldxyv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gtclbdrqo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gbrmgqvxk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/goscrleou.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gjtpyjebo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gnsrcoyii.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gzpbsiopb.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gmudhkbse.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/goinpfbvt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gmnajuctt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gdlhalads.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gbymdqrja.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnhgmfsmv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gtrpswwph.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gubomyqot.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gikktnglo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gybexdkmo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gpjrdfpro.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gcilixvxa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gayuyxwrh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gmvtyedxy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqfnnrscf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/glsojjxgu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gawllfuhs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjyyeatlu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gklianqhg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gndnycceq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/grlmeooib.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gdnqxvewi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gamstxyjl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gezmjabjz.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gmpacwrip.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggikqnhul.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gycufpnkl.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gsyxacvau.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gbfeqlfee.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkxhzolbz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gyckuoqay.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gqxwwjzgv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gvutjrgrj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gvfreygmi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gqoipgmom.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gwjpqljia.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gagnxwqol.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gtnwupvnq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gwusakhvz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gvocscvou.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gkaujsvei.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gxvokabcy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fehbvm.com/Article/details/gifcsopqi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gobxnlpgi.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gaxrtfynz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gazfmsdlw.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gtcsqqnhf.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkypkubpc.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gahuidkhr.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gkfulsbvz.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gfyfprejo.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gkkqfvsdl.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gtzxxbkpr.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gzjuwnxcy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gwgrorajg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gmylhbpkz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gpgqfxwak.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gioknkzsk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gicegboai.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/giwughklt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gbmvpzdfg.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/guntknmgi.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gtzqkbrvj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqzclaibo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gvbkhiktn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gpmcscfwz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gemtzpelr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gkfsyribh.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gatqlehie.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdxfmltpv.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/getcyqact.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gamerkkcr.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gnlbwjboo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/givczmmoh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/ggdbmhniz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gfknuzuve.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/goempoytv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/ghxvyucao.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gusgfnpwa.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/ghkxhodwe.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gdficoaar.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gglspyhuj.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.hesvh.cn/Article/details/gxzewcems.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gmafgwoee.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/goakzlmwe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gvvllqinb.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gfbnxoqon.sHtML


<!-- 参考信息 -->