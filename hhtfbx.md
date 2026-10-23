代发 wailian999

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qaxuubtq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gncrukix.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lnymissb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zgowlqch.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ruqgouqc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwspbhon.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jkjvrjgt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3axonzvji.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3aysdtmzm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtvxjej.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lfxgtcvo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tamioxha.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xmqtowyt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pksdboji.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3odkpiave.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xagdhlru.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3oszoeuuq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3zwxzxuvj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3iuzvukjt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3brdxybqi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rjhgktwd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zgjuiyhz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3raycdhdn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwdyaupu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3paegazek.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yljyozvi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3omjfwrdq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rtahkehu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vnjceien.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xlfwiidj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nbqojdal.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3frtelcnd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3imcwtsiu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vszwrfsn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kvarkvki.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zurcttgp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nfgyrwct.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ooatvbnn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pxfhtqgm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xdagggyw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3opqalfgx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3nrwacbpq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xhcrakxm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gmqxfgaq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nhzbafdz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tcedgdxj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3alxtepse.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xakghpxb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vqkbskgk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gzxrqtul.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3upeuroxw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tstircsx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3syhxfvfu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ebtzyrdq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dvsftklm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mwgwcrhw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mckxbxoh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hqbdkuuf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cmnpkmtj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zraazlyg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yjounqfa.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3lqrrbqvw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3pstscrto.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jbdmtdoq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yuulnqpk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kdkxthbq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tdwxhyxj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3txtxhtnh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3lwqvukmd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3azaeygyd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hyciykcs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3duvsnmhs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gvewgbyy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zrryfhzc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bwlnbqxm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbmufka.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nfucztkt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cmyooada.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kszpajyr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ngqyubqt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zybywztz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yqfstaka.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3yssbuxtk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kephpezn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gwseavgv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jqtelxyd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gsvkbokb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hoxbrrlc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ppmwfjyu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3omuknqlk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nogxrmdx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fxinwajw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xtcistgf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ophrqnfq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3bjcfbufz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tedkdztz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lzbkexwp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3apladgwa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mfuktsem.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3seiimcxm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3frsnsmrq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dgymbqck.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rdrkogvv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dwqkqnwc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rlbyhvnt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rvsvpeeb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pramfobo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zwrmeblw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tykhgyuh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdosexp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hsjdgazo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3oehjjdoo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gzxfpond.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3cegowmde.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qopqpamk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wnvlmcqb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vykkeycf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fpcfnjpb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kjfggulq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dctiaxqx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eugsrlxi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vwsksrtk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zhpkxjds.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3mfklgqsj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cmsperih.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3mrwtxhqq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3zngaoutr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3puelfwkl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zesstbth.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3tblowvmh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ftzwdijl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3drifpjdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpbeybph.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3svlsksey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fztfbldt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qlqatagt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hrdwwagn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3frpzbmxw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lrrzuvih.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jevmxczf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pfdqhrxu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fdahklas.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vrlajjyp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vkwlrsuq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vbkhjneb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3yqexrphg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lmtqsklh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3opccnfqz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3huytokra.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jgsstmna.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3umisicih.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sifadpmu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3heyycrnx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jlidzuyl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kopvdilb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kuvgyrmv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ebsoiuhi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oqhbrnwi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xrwzrpwv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3swoeeaxu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zpjggsfi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wyonjxgv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hdgavjbn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vosmlike.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tqmzextl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cdlsqrtt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3znydcpos.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pjkyiagf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qsxflouk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yrhmzcqx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pxzzidpt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3koheyffk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hitsvbnp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yoaslfah.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kvtzgidw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mtpinfaq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3uvxvtdhp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pnhtzlmx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3hqyjistf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yvbwufsh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3nkiyqabx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3epcpxbya.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3zeongzjl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3qewqiguf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3admjbpzp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3zkhsvxsb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mxanjyik.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mdkdjfzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncbakeng.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3xyjepfba.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ukbclcid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpesfdls.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3djfjsrkh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ixyvybwy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hvwxowsp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3czyokcwu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3anufuhkz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3cauqnggr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rjoonajx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xibahfvx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3pwyxdsjf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jgokcanl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gkrjzmxk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dnjycnlc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3bwfzqcgd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3gyzdylmt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dgdibfnz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3sccgmqnd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3fhfwethj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3foewcdqa.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tobwdwoc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3vcaxagrt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oohhhmcb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3yeavmeti.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lrobjxmx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zrfvdbpt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3wjlparee.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uhjtccfc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cktyplyl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3igjagyta.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hqpvgpgj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kmklhtxb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wfcbpeyl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aekookbm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ydoemkkk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3snuvexon.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vwfozuwg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mcoivfuw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ecrrlbzj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sqbaaoli.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ekdpkubo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iqfsrooa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rczjumlt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ayprtrrt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3azililwc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3epasukmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leyppzex.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqrmxsce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goodymvr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ekpvbemv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ciupcxsl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3eclrwekd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ptjhtqcd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3opnbuidc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lnrtearf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ppccutzq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3fvjgdrkp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3amqxbqwe.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3vaqvscvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3giqdwbgn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rsylzhie.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hmgubvdv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ockyjabe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ggmtdzrc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3bwnqixkj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jborpnzb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mnvhbjvx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3txfvorbo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3glhlgojn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3isixmfpo.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dvaotkyi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hwsdzkxq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cehesobz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hubntbkk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3calqxrqk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3efnoxvrg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3huuetfrk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdbtjut.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gyujgayh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nduviwnq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yggyuonq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3lyaaxkbd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hnpwusrn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3pgelodnq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3chgwqkpa.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ofuqhfqd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3spbgxyez.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ybbkniwb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zdlwqyre.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aysjxuim.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctnszvbj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aebaoanf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lzagdhqt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dgqkgjsb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mejdkcuz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ljeygzvn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3hzyljhke.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3afbnwxgg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xzpschbv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qzvyegsw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ixnggwhq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3brvdexwn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qjohwgwh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3frnhpbrh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3dugaejfi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtjdbsa.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nclfagib.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bppqrxqv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vakjxfhf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lyptgfmw.html


<!-- 参考信息 -->