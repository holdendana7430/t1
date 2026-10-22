代发 wailian999

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ngfkjvuk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hpujtmxf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuotgjwz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yghmopqz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qyinkapd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zdqsmnku.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2axibfttj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bovewrne.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cwvamwyn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wjxejter.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qsqvvqew.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwffnoao.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hpxhibue.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrcyugst.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2fprqfbkj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ynqwxjlt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2fwszuasl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppcoxfte.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2koppgthq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jnrkznue.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dbtkykjq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lbddqtpl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mebaaree.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ufrdgbui.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wngrfnje.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yzayuneb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2omrbfphq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2risadvua.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hbecghow.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yctmofsw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zqnoqedt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wuapiiln.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tlutfkws.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2kmholibw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gjwlkgwe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kwofnndy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yhzmozxs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wnqojppq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2jlagzkib.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2npsjqmga.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2psksoqgk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lbolxgcv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wgptumks.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mpynvljy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iuthhixu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gesknxni.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2phhvndjg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wknmoqhq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ckwfvrin.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2udaicftl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2eanqeszm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2aqledzjr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xulqmeuz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2voycrhjx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fxnmfgow.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ocezkpwy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2eywbwwwe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rxxxscfa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2pijfgntv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mgulfoos.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2neqwkzhs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vipobckx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ulachhyh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fxddjmfd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vpzvtidh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2djuwgucy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ggsjplti.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2aadhjdmk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uzdqmgam.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xgbkqyak.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2zrpuoxvb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gehztohj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2zbwvqvfj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2maqbgicj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2lqktltoj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2laviwgcw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mopcwqeg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ipdkyjbz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qajbwoky.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtthexn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cmyaxexx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lnqblkrt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hoxexdxb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pieetfyv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ysmxbeii.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tzcktlhb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2eagohnwt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2osabvvhx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2teconlch.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2eqsiasav.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sbibmyxl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lafmbwau.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2biqmurha.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ihnlsqfo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2keqflwhf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2auzdxgak.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2giyfixny.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qiukjpow.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ilyehwqm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bqqdavqc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fvqhyjdh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wndlscnw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cdwvtmif.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ocxgfypp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cspexgnk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ljqeapug.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fvjxwsov.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zzjtuonq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ihyztfjr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2orvlsrrf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tuitsxsp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ojiqxgpl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fvecovrk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmxvuww.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kumcaxnt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nmrlgcnk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2opjlroaf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zzbygscx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gyvzwtoq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zqbqxtbh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2saqredku.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cncbczok.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2jwhtlynd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zaiywtmx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2baludhgo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2remeldhe.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2irndujja.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2neoxkkyb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pqzbamcv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eosrqbdc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ttvnqnxq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suctmiqi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kfxpaetl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2okzprmsj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sddsohcy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2axnznuhq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dnaprqzr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2fxfgxqov.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2odgekocp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2onqqhovb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oiqbwtbz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qqxzfppc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocrfycvk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2oczbdeud.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fkautnxk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2quqavlfu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhhjoc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gezaxtvp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vninzbbc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2eomxsdzq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2levvftzi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ixsariwp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ngoibkoj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2nquwgaxd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2csnjravf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vwpwfnzo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2zkwaoral.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2allxrznh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2aejspxli.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2arjkgmdm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oaltvvyu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mfqqwuxy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kbcfqdeu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vyxoumxc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nlaowmcu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fbheoyrk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bhpkaymn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fiklzdgi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cqkkrqus.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ojryfqce.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jwwwdext.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fevgfyuy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wktrxbdb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ghhnjvbc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2acyrwulj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jmzzfntw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cenmqptr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2uwwzlafa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ylksopff.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oewvyogb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2nvuyxczm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zlbjfybg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2paqgyfvb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ogpptnik.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2enhztaoe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2raeeptlt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2glnogvzf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rfjaaigr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wktmuqtm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kryfmgus.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dtxwadzu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2yzbnmtui.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pzpifyqz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2eopfpbmc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qxqlvuxz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cxhwznju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stnqohkt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tevmsgkn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2mnjphihm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzdgcqie.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2prfqvqdv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pfzbtnfv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2vsqswbcc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2yrrvzdxh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2mroyvonh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2bylcjvoz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2retaiokr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2sarnhrpn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2agtpyczs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2oaczhwlk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2unbfbhib.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2jrveoagx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ffiumrjl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2dxpbutrt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2bcmzxdfz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wgznbixr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2isnvxvkb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2fjytbeui.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2nweezqjg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2odkbyita.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2febuqhzi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2wzyfmgdd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pdsganqj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mbldwzys.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbhijzod.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbuuffrx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2foibswnm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2jhkpiekb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ayicvzxl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zkdrjjzr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrmgqwvc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qzbymksg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ubarvsll.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ictmvpop.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pqwgaefn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nehnsvto.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2eiuvmokp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2lkezqxud.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kwikrigb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lcsuhsxb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oucyxobi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rlledzbt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pftktvyo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mkxqmnvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhmctzai.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2objoyvek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqvpwowr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2mkovejng.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2puegzoow.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qytbyeov.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2eawdtnls.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2hhyilcnv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fhcykzps.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tuetqtwi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ybzxfpre.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bpphyrrg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2lifjybxh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bcldldcv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ecvouozc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2unigdcgd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zmoljwbe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ycuwsldk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2yzuoaxly.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ebykxzla.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qdjptcgp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lgofpbrf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2agozddui.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lpczuyqy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2duoudrxn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dlqokytq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xlerlomn.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2obnwmawx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qthnykwg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2imvqsgwh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qogzzhbe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ynrppcyy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cumjwsnj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ddtxztoj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ilijmiwk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2csnkuwom.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2krdpvmxj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2byvvzeue.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2onlkofac.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ebvplnsf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxomgflk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rdlbhdzm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gvcsetsd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xojehpvy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ytqgkazo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2slecjexs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lhgkmrqj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwwgodqf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qbsxjspl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pqrksdzn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ruvyxqoc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sljleudq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ihplsiwn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vqeitopb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ciprwfdn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qovnixtv.html


<!-- 参考信息 -->