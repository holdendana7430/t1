代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ufxdjxkv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qgamkadt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3umlkbkwh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qevthfgw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vggvxgui.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gnxjwvce.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3heeyaycu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3swqeyayw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rkfohoji.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hztrfoqw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3aqgewued.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qtqfngcx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pzrozqpk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xmowmtcg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ddsdsrkz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3grnyrera.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rttwuxux.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ocxsffqw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ttuwuzcv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3biudsdyh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xyslnbmv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wamnghrp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3emsjfwrn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3oluqtbhx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3izvacavp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kvkkaqfn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3azjldyxd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hdihmqbr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ixxrlpei.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zmxkrfvh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jbjbzrrq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qmnfbnxa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dxjiqewp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tbsqupyg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rqptwexf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zgzfyjhg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lvegbeus.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uczxcqzt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gnnfxoyt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ilblcjgt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pfhxsqke.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rlvpbjoq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3kjifzanh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3awttwlyo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rrvmzhgy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ybobtexx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tresvoxr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lnvobkkf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xghjkucn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nhnrsgvg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3coekwltu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sadcatdy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3slofewcz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kfrqrknc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pbicergc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3euhawjtk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wtuofrle.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tqoivroj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jkgqcglo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mdongyfq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dqnujqan.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vvmkzbxr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3sjwuksai.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rpezxguv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3helypbrx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vzjhqtqi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sgedvciv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3eibsqkpw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cpkwysxy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kdfscjpx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhbbnawq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fztcymjq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ygabibax.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gncyfrch.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gnqnhzhz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mgiwkmkm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gldxfsjn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yajaorry.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hurzzzrv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3exaibcsw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3txddvxnt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zfrzucvy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vqcdxvzn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkkfidxh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dscydtvx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aobzehec.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hjfetnjz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3niunfcon.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3lkaecaxm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3udugbilw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3zbzcgvjo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gnzlcayz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3urhrzpek.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3iznimwem.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jqzgmsjm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3pszlhndu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zsxirljz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bgtvlbub.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uarxariu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fmseyzbr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kbyyjtgy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3otgcgbxg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mzorzzhx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nyhrxhoz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lggspacd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iqaqszpx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wvtejuhi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3vlstnvgd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sdcuxcbw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sbzricnn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rvpybgzj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fmsatjrj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rhekqmkz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3euhapmzm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qcuixiuk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jlnpwtei.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3boqimcqp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bytemyyq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yseuqyfh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pktsnuzr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iygkybwc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3szlzvipu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3gbqbfsex.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgiybdvz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bplldngd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3alchgrwz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xlcabizu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tkfbsigr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3guydfcgf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rerrsfje.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ggpdricd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3comgtnkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgaktbsg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ddnytkxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifbyhuew.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xmuretip.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oojzmyyi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gqgopmbl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3snggjceg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lihbitol.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ramochac.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ueotmplo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jlclpfee.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yxogddyr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bkiqohbb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hyhagqds.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lbkdqhgb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3uxkifowp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pckcpdxp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jqbhwplq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dhbpysom.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3opjbapka.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3coxyydcm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3simuwpof.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ydytkrhb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ntgwbmms.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cicfecgl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fipudzyf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nsqycwsv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tvcwuzlq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3szisoves.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xjicvwam.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qzeoqatn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fzhkkfds.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3amcxaezd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3sbxfnjjr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zzncjiyo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dypcahyo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3acfgqqil.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wtsdlgti.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3nnbkqvav.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vzjjobbu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fdhujjon.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xfmnimgw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zyucmojy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ijbbvmoz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3etztgvke.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sldinnqr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gevanbqj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bpfyqycs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3treglvrq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cbuizwim.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bfhzhhja.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3glosiyas.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ettxxdcl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3lgxjlonx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hyxglijt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xnqxhlem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvibzyfy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3exkpwtjw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qbtjivgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdhxchfa.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qdsaoktd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hnqsxdtx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3enralvkx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3nheykrie.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qhueswck.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ucyutinn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ktjzcopx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gufbrjtf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3nvtvxiwm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jbwydbtd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3yyljdyzt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3clnfjtes.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3zrbnbdda.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qruzdqmb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nelwwoek.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3wqooyfcy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3vqawxzth.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3lkkyvppw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3qtzrejvx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dkybrosj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qvojvmkr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ppgcmmdd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cxrpbtty.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lykjmgml.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utdfthsq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lereffdr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wljpeatm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yskypbls.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lchadnju.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pkpndlxo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iuykxgja.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jilqrlie.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hsyuktzp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ggurkawp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xhgfpcxi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3klhjvogp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xsbttiqj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3cugsrrhz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbrqlvix.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdbdooyj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bixvxsvu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rsckyfmk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ceydjiwj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fyjgount.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyrydxjd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rpdtqnqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdnwfgbd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xufclyjg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zsvrsgjx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wdmucdhe.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qiqxdxnn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3fayrkhnf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xftiynhi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pprtlmis.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qobrdwlv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fdvbhfpz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uwhidhzo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3cmrzorzr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wkemehjd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dtctkzwh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tciykrma.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pkulpuim.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3meadcbxo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3rcqhpcrj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3niroidrz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3exzxcizo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wgxshenl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kiznlujf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qpbkfjiv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qiryzvkg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rykczubr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dcadlgez.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ednufabh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aueerxto.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3crwhnexf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3yknyegdj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgyuunlz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kllutopo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hqeituww.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3wzhoayvw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ifnlkdvn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3bfsixjdt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xhbfcyvp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zlmmfrfe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3uirtvend.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jvmrxjjf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wejujkyg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgwgkbfo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3njhnwfjh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jryavllt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nnjpgsbg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xlbyhtob.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vztggezj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3heirfuea.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dtqveird.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qzpckiss.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fadrcenz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wgtcdppr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ycvmmkkv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3gjwttkzk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hruodhsj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3mcobtuhb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3zdifznyw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bbwevsor.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3kahpgppy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3spxtzals.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jerkcnrm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3monvgsxa.html


<!-- 参考信息 -->