代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eleayojv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lstywicq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3fiaodafq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lzlejttp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ieevfeps.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nyqqkdon.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3owqlgypp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jnebbopp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ohjxjsom.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3giyhrnox.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3efgawifn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3npkdrhwf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bmlmvhkt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ajiembag.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dfprnjnf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3yrcpuofu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xamrdoig.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lhtcrfom.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hqntcgnl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sjkybriu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bkrhafof.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ndqxffcj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3mabihtjj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vjxsmkyf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zovmwpnd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3eqqpwdoo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gntkapuy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jdytrurn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ypaljeac.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3eebwwjai.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ynxcikwl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rbpmblix.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uthyggjj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqozerc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3axejltxj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3pebboyhp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ubieqsvu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rhrfvxiq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hgzenbcg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3owljqlhl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rdshckif.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ttdontwg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jjnwwlnr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3atdzvkkf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3owrqleaj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ilfxlppb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3msdjcwgv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3nylykybz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tpcyeoum.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3adnikgip.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bnuqsctd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dlmjogyc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xqtaputq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ttapcvxw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fthbdwia.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fdqcwdmt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3utpcdbhb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3geyivwwv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bmvzzwvq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vqavyifz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3acaigjuh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3logqjmyr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qihxhibb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3umjfnkkp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dadelwuo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3onxqecwr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3gwxqjagb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yffxjycx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nokspzsa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qvzxtswc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yfelwnen.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lsyqajpv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kpljfbzi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3meyzmqsy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iquqtcts.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vpgkkbee.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qtygpxhx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3azcpzaen.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3amzdlvba.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jstgedwz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3boduwapa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bdteptvp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3abtzhztb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rrpayids.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ojcejzrd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3odtnxade.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ksalpysh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3rrspmvuf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kcdrtkqm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3endysigv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vlxjdxyr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3syvhnsiw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3djmmxces.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xadtzsxo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fsrostzy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rjxeehgj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jfdevzlm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3avdkeyfd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rvjhqksj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3uwuntius.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kvuyreub.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nrspoqhd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lyigdxnf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zpsuuzbj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pqhhcqel.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gsxbktvw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bpdhopnc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3rfwodzsm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3keaapjdr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3yyqrdzfi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cdtylryj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kdqmbbhu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qlykcswy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dfxuqofs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3wtptdwui.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjunmcd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3whfetxpv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3adwbcgxh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3sywzrszv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hgfcdjfx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ihrhzhwe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ngqjxpci.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ofbtisdn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zkkgdkpl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3jkpeqhew.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3tsfuuqej.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tgukzxfs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vueanzsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzojrhqd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3getkjckp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytssepxo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vmrmdcxn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mlcbyxjp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3dzubpjwg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3oqivvdjj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xmoxipwc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3klwtkqnf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3yuyirxxi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ypskpahk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kcurqkev.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rsfttnsr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bduwhkap.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3utywzwlh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vyosnefw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3axwatkxu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3sajawaig.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jdpxfozy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ziumvepg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hadquruj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3monxooqe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3crvwiiin.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xssjmnxe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xdrmpcvf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3izbqetfm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qizxgzvo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3apcradfp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3cfpqshjr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3flemqfsw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3covobdyi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhcjsi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iyoymnqu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jziqkaqu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3okypndmo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bdomrvgv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cosrceuo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pefucxzd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pdwkwazp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3srprwlvr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3fobdxjyq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nnhaxwik.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eaqukyxq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tekgeout.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lbymwffn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nqrduucr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kbxkztsj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xekcuwus.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3wkstrjvb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vdxpyegz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3wwwcexpk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wxvnjwbr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3dirdexpg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ovpgwvlo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yeobfsvd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jdxqomvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vazplyyx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3oenewpyw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dgoxwtpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eiuuopem.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3denvfgus.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3sdfawazo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3xqjtolcx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3nbfzhsym.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zlskosyt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mczpyeue.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mnzkbzfk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fecbndgh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fdezatys.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3mujgllyd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3aohftakt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3yivkgbov.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3goxfnoca.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3vqhoweiw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3czilstof.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qbwejpnv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ihlwdmbj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nphgepfx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3npcqaqvt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vnqzvcds.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fusgkvyt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xjomcqab.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tfatsvyj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ecejkggl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fpavdthr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3phhjpukx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3omkflhfy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3obfsdtdn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3boozumtz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xjhoydet.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bvweystz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unxqjymr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kkithatp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kuatlsvu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yvbhlfzs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tdgrcsnb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmlmwpsk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvmktxus.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vtgeeqhr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3acrjnbxp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ynmpdixb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3likxehhm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sfdeaeep.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3loctngov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmscdicq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3llmmtvis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxoheyyi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ltvrogpz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rdljzlku.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ezldjfts.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rexglxup.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hsfwmnmo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ngxkbbel.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ruwtcwvz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3sxgmwjsz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wjhabjww.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3kcllfrcg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ovmwfign.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ulselfgq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pnvsgyrl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aykpltpx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ckmsqoko.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dvgcwzkj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3bmyttyyd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oxjmhlks.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3eonqrnwz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3izopmfpq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fnfaneni.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eilwpwhp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nopbobzi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wkrhjohh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3iykymnjs.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ptoiqazs.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dxbkodmc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fzcdwork.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvcmrwp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3lbfkqtbp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hampjmax.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3sxnsyfqh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3unvqadjy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3zifzgbtt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjmuxhq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3iihxbcnr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rjnekikh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3uugmciil.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zzisotal.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwlvcdjl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3umdtqivz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bvluvzhv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mdgpjkzg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dpoajslp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wthqfcre.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ljbbjuqb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zyjgcapv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3zglqoygl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3igluvggh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bpfihxjg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aibgbfmn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3eneuxmmr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3xbaxckkf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yicsbvcb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3snbiyqld.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3rirquggl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3wlqegbid.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uluwcado.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3adbqitfq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xungitnv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rftgnvcs.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3xtketclf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wffzledc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jbazjwej.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ywykpooh.html


<!-- 参考信息 -->