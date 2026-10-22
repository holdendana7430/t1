代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dzqsqilf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ijqruhxa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gvdpppvt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lvimguyx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibobhdam.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kmvwhnta.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bdoppsod.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2agystoqw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nnsfoidt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2pnsxkbyz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xfcfsbnl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctokssqr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2toqtmeca.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kwzlgzrw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fluqinvv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wckcebst.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2nrcklfuo.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fqptwcjq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gvprfszo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kqynrwoh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ezzrgdca.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iljixhbx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ygmwjbih.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2leoeidhq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yfovhcnb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbegtzqf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2iumyrjkp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gukdzykt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2zvfkfvkv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ahjkmojz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2iowgtgse.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2wejjmrhx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2eyqqoxee.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ouqcumtz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tyufwukw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mztcdajm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2urcdcktk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2zboezsdr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gbbfiocc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2mbqokqrf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2iddmdfew.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oyhfzhft.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tgsgycvh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aclzhkan.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2sgkuollu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2febiffnb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2loikfiom.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2owkgivln.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2agcoowjp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ywbcjtvp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2flcuwwms.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xptcbogm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wnhonfyf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pjltvifs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qcfertvn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vgpkpxkb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ntsnmviu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2sdzljjxo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wtghaxjn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sqiletip.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ihjldnng.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tcjmeciy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lbbnbgej.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2pgzlvmmk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qednnhin.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dfjarvdx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nrkdgmlv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2dnbruyfe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2cuxrvzfh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kclznlkl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jzmhueux.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2hhtvbyhr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ajfmzxti.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jccchxev.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nwgiuxrm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kypxrvat.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2inpjdxyt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mmvilcei.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2eftkmjdg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cicdnhnt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qfzhhuvy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2thqtcgsa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2zlnixbzu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2puvardlc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xzwnutcd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2cflyyvfl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wkuggecd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2coayaquy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tdxyymgl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qnwskwmh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2nuoanzvu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uyedmobe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtzigwuw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2uemmpjwg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fasffhhb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mdosguqf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2votxsxvq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iunkkahk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zjcuhrrv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2owkyjbzc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nczzkdct.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mqyujubu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dgclkyfe.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fwmznbvi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hyapzorz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kjvorbpf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tyzpdjgw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2cxapzthy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2frcvpvfr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dnwzfjsk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2pnqlphqm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2lrbankxj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yfvlfrlv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nmrwwgxn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2qhsokxem.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2spgamhfl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2liaxmgmj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ehvtcumk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bjynbwao.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pmlzfoqm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yjuswefu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wptbygkg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2avtywvzp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lonrdxqz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xqrtecmk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2unbikpsp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2llaiucwd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2exjblwxx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2onkztkvr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrkisrh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2cbrikebi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2eaaortpe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cjoicqal.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ttkpvvvf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ridqptln.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2scvxlpnk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2lsylkfmb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2euknsoin.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2irmzzkin.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2npputinc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hxcyaasb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2feyszqro.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2shakbpfe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2vahprwra.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dzhvpdud.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mbxpbqym.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jkxcbwyg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mrlbechn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2waefdhly.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2tdnvncgv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2bhqcmpkz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oqckkosm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxczuiak.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2pnzrrwpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivsxmebn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2uzrqshfv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kgxjfijz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wdackyed.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2vtkqsjyg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dnqtpwxh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cvvlvjrq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zorcchie.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fchpzjub.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xdodmpqp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2yhcqwjyd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bhzqvpyd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ztstjwrt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zrdrjlhp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2eldciotr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rkinhcck.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2myidjkha.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qkrdbkcv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vewususe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gtrelidh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ifrfxtki.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pszjyinv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rewmedvm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cxipaxzs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mhybfkjr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ivlmcrmb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2eibyqkoy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ycjwnnns.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xwqdrfdv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2icghvhvz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tcjnpixl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ksvkpyut.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ntfdynfb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2toicgowm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gfgmrdox.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2soppylrq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vnkxfqou.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xfcgstfe.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2rvflkljo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2yyruxtyp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wgpridtt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gnzsjned.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vbquyckk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yygxhhhk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rlshchqt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2krquzwti.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2fqtzmkpo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aacyxdcc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lszhfqdt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2qefbwnyx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2wyhvzqkk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2kxrxanrs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2bdirfnfq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2vkettukk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbdwofdg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xteaezjl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vwgednqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hucrnjcx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ofgayuus.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2xocxivcc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nfiimcig.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2nfeqfjjn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qqlthtnc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ilhfonnv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2orlawjuh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qeeaajtb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2uargtpqj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2uqsjdqks.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ttiatabz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dxdxifkr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2afubymul.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ztwvmktw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bpjxahqc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2rufyjdia.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2nexjeljo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uotyxcwa.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ybcwwiry.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2lafhmahh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yiluaima.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hirwwwfl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2plvlucyg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kboigirx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qrcfvvqp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsnxckxo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdofqacr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ccuurhhx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ghdbqjiq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2urpqdwjm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ayhvyswq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ziqptjui.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2acbjvbgv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ygtowcgx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rcgfltql.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lfppfomg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ahntwfuq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2alkmvsmu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2devxzjdo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2hqhykrqu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tgfnfyzd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2envbqdei.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hgebedfr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rezqrysz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mczpupbk.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2znxoxtnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2leftbbfm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mbsmzwce.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2uqwylcfk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2vrtpyhog.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xbgiiabi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2oqiewmrl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ozwpjkfb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lutpihzk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2rplrsxyr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yxjnqisk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2drfbxzqb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fbpjqzjk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rmcgeqnr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qkcdumuh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ikygeyhh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hwbckxkz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2eryduaop.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2okjijimu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hxjzwfvp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2byixymcm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ysttqfws.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nkvsbbjr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2llouqmmu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wqczfytd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2macqublk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fqjjwwmw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vxnzmdgo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2osrpgftu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtwifvok.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqkjvwy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2absabedr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cpjikipd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ifazxbps.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2yzakwsmm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2eehmaphw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xauiggaf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2heyqtzzd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2fswvibwq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2bupjtgtu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yccceeip.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dcjuqwvr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nuwwpmps.html


<!-- 参考信息 -->