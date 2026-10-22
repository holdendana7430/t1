代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jiypgyom.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ttyvdtae.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fqbueqar.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bublsymv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mjarzvyt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mdtplyel.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2plmhosmg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lwcgmynm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hrioshml.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkvhvapi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vxkdjtpa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2midmfpxm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2adaympmv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2osjubauh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2whvfepbj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fragxnyf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zroobljn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tvcbfxau.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bigpmpyy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2wjmwienw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xmujsvzx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xzdipwcl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2afzhtsns.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mocdvnsa.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tblirvpj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gjwozbcu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pujoxepr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2fuclsgik.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wuavkfmg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gplmbyvj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sibwiyao.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fbxyxpzm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aoemhpkf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wwfbiuum.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hpkhsgno.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ujwuigjj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fltnaxxb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gxgebjcn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dyisembv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vgbqougw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2aobtmmbp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2juekincw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2envvruev.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pxhandrj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ymixqgpz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fplmzvay.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sxljkhhk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ubcofpqi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xpsgwncz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ayldyhyd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2upxbcjfs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uwfpfdzl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2isavdsjr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dhavvmmp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2attnmfaf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lgkcoopl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2qxwcomla.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sxuxkjds.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rolldfql.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2duamlgga.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2poudyixn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kkmxjkjq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vbfywsrp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lsecuxmr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ywrklicr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ipldzhdz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2npfoevvg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbvgmsu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lzkluaoj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uvlcnxbx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2srltfwpy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrwvrng.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ayofuluu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pvpmuwoq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fatlhsux.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qvfxxtlj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gdzwuaqt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wuuqoskq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2cxbeaszm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rtemjulx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lnpqyfcl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ntgiudtd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2edrqxemk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2brtjrxkp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lgelhpps.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2aogdsdxz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2snecfisv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2coqcfwea.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nqnahvaq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2vijpvyad.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jxeewlmc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2fpolrbqb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2uzuenrdj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oxmgjdho.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2etplqskp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ubrcochp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2jgkkrlhq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mqtdobdu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dssivgkk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2waqblist.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tbwonzgp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dsvkpmhq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hyqmhdyq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gbbzlgtd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2rbdowchh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bmygwhco.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2uamuqvyd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cccrxirs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zvhadvai.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mcjossnm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2wgtymxco.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tzqpmbwl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jatrviyb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hemnmqad.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rhcdfqsa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vapcvsmf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ywlapzxz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ffclkacr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lvhlqqrl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cssejiah.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lowynnxw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xdclehtj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wuotokgi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ugmwpihp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2nftsjnpz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2haqoqrsm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ddjehefa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2dnrljylj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwieqkog.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2embdbfbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xttjrive.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2crjylytv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pbamfbvo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2laypzrtc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ylwnbcoj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2wzywnyvj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fllqcmls.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xsxjjmwj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fkyetbiy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2symplrmg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qflnvpzf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2idkpdgcv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mimesqae.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2cszdxkws.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2spdmwqyb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yghrfnvt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2orabrvwo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2slmstcbb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2cwonjwrf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rdvjliuq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jymivewg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qgttpmfa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qfrnrlek.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2biirilqq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mrvngnpx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2iheceofx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xicbzlct.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vtjbjowu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ndskjmpt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cmjjagok.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qvlylgtz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ozqwbzwn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hzzloguo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gyzmnypq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iabhfcqd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2adsqyppj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gxjrxyef.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mnpejfds.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2qctwhwxt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vowbghen.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kdlrquji.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vjhiyheb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2lrtvmvcb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2auhsxjbc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rtbacvhs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rkenprly.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ngedmjcr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pkqpnddx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lbvhxchp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2buutddhh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lqjzbevt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2eqrlvzmm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2stvpssfi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2frtknynq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfdmzkhj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2yrflgulg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2eghqxzzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2punncrmm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2devkdlbm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2yoskesyc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bfrwuwco.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2hkdvdsbp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2dtwoqten.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cslajxni.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ywnmqxmt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2knexztpz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ljgervqh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zknnvdcd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2iuibsdrp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wbwynazb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2mhstvxdv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ztlnsktk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2bjgggcba.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2avpmbevz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2fvlrqpgh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2cmdzswuq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2huhyuxpd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2fnvatlbs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2azeyzepa.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ybdiptta.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tbsmuvtz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lbjgkxzm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2flmvnjeb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xplxzexw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qcelksvn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2itkizstf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajqhjzbq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bvuhwtom.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bfgvxwld.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtcybqnu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mvxzzpbt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trgrlfcj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lgmumfky.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xxdbzggv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qlizmpdy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2orvhuknu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihnxqioi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2nxqicvqz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mhjbdzpj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2chlrsrjt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hqdmccap.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyiwuguj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lusizlgz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2bmfewlsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktqfflku.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxgivuhl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2iuawogmd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2kichywdq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fkgjxmlu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2fkaftshr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jqivjlva.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pkzzdzal.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bojatcjg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2caxkbjus.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2psuqtxhb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jipetykd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qburrnom.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nsckikoi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tgqurior.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2axlarsdy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2puqcedxv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2oeglfdjk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iucwmtqu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ilxujlir.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2sxmnqbcj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ctaabvfd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2csudrplc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mxxpgyld.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lcqyokhh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2klzkzrtw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lgoekopp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2colnkzap.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mukalgfn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2gnklzjgr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gwkrryml.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sigojfby.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vgssoatm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fitwivrr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2tserefrr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2raxxywig.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2gwfnzzkn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tmubfhhe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2tphddmbg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dpcsjwsg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zzscmzmj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ntkaxgno.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqotjeot.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kruccyzt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwwottiz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bqodhvtm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tdoxniwc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2twznxocj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2pxlvczoz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2luwpgckl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2srsczcrc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sjuxcxhc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hnasxint.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jbowhead.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yhwulqpf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bdltvxss.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tkhsscuo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2joxmnyjt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mdxfgacy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2txnweaik.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfwekrj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqbkfci.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2cmusxjoq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fygqgeug.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2gultupjj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fbcekiob.html


<!-- 参考信息 -->