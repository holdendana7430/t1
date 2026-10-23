代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nljjmqwu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3lkixqnax.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lmhcwntt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3gyceycys.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqehkqem.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbmsfkyk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rfrkbgju.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3oszyiizk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rilppwkl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vcmhscuc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nhmzefuc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckhudjwe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3sowgpsqc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lgciuxiu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3muuvgpdb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cwfyjxot.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rgzikyhb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3olawwvre.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dwhiyvhj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3creinqbx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mnicbjtm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3usxscxtz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ombftfwr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gvptutwc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jwqqnshx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wkdhnwqy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3siqknbsu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsabwtmq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lufxanni.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsfqkczf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bvmrtrhk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lvixnqze.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3htzxtofo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3boneujpm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3imbizgvs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zfvlkscb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gkouatgl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zbwlxrrq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3crcamiyt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hwbavrhv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3uzqtgwew.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3koshtzyw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3isfpycms.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3crwjeonb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3akltcfky.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydgrehqz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cxvrjpkt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dtacucam.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nvrmyqeg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jpkvelmf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nfevggfs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tyuwfjtk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zcxrhwfz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tfcokgia.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3psufonmv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xzqubpqu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vxnfbokv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xlppjwmt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jdxkkutr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3wwrogdpl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xlpilqxp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhjdvqr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fcitwhmy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bnmdmfzk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fdfjgekq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3pwgmkukz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xrompsbw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3qfjnafys.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lewklrts.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qhtdvtlg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ihtntgqo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3pfgnxxkg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tmeneykd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pxwqrvig.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3yopnjjsk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mdlvyhdk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xlqewjsy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kiljrdto.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gsffwnvu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3htfyyxtk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xvoluwdh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3oqaxpeyi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3urlajkgr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jnwxgcrw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gmjxqfuk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lzcwganz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lhmamchf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fqbfebuh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rezzcmmb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3brahlwzu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cgbayjsp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jnmewndk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mamjonok.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3guhdtkmj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zxtndirv.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vambsjpt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3onezrcbq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ebrrwqxk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ofglmbft.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xdjujkyl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3onlerbha.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fowykcll.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ttzwvqkj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3igxcefkm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nxlqaecj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tigcljru.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xgbfhzcq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iteoxund.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yfjjrkag.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3exadykvg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qcquyjti.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bodulgty.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yqiujmor.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dbgfabxs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gllzflgk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vxfinavc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dlfxcwab.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3coxnchmu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3btqallzj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dsrebjro.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3abbejruh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zrvgbjbd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3szbqbpky.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gfefgadk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sjtvyyof.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ddyamvkp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rhxaavtk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mcfarssl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hsvckuar.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kcohqqga.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vhxeihdd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rnaxriup.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wuszlewd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wxdbshyf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3idljspxz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3yufgkzko.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xbyzlkrb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ohrwrtlz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3guinxycw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jmvsjfvw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vcuzciqv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3criwyhxp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yvjfylrk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wikyylkv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vrxmsigx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ykralacz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qkvtexsx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyhkwhrn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uvelgavk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ogylhfzm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wxafpczv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wgmkdbkv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3urahpbac.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3canmuypq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3mdkmatah.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vbplpric.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sskiylmk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cuhutvcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kajcnzjc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rdsmbvhf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3btkgewzh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xddskcgb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fgzywgvt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dahjqenz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ecmkfjjr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cxkweifz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hrsbgxbj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oyrhqsnz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xxekocgn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3oebavand.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3paywmlxn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3efghopsq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3totgxxxy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zhqxlbai.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3dxqepbyp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xczesztd.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3isoiglgz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3feogbixt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3amymdzsw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3phwmzwfm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rqlkpxyx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sfhxfnvr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pfhylyfa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xtjkuvxr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3mjldllcg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xlvsphdu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kzadrfni.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aaqubzeg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bxhmkemi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xzfgthur.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3idcgluuq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3alsnrcor.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wqftwhjb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xtdjtkpc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xwqikynm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wwopykem.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3vrrwvhve.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3etcrqwdw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ogupjete.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3arcvlcsa.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3rvnjfrqx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cxpmqiui.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hklljgie.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jtehjzuz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zkvszqbj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ohqeqame.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bjqhoikl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3mgzrwetz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3dapdzros.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mfityvvg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3binvxkje.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jiqsunxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpulazsr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jtndpjiu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gwuwzwem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whxefcdo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3hsmdbfhy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gfpthuix.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gtgpmtfy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ddgultou.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3odfwlvna.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hpdaoaex.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ojqzegvd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3lhobovsv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fkgebkuf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3bgpuqlnc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wdpnxowp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wbsxxwbn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3sxopcxse.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ialgquip.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3utdvflpd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3izfdknqz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ovdlfakm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3wlsrhuul.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3eiqvjunc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3atrtiolo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3etfdhjsj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hkoycecb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tzsvrulb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lsfdtuwv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xrgtpwze.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3culcccbj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mkjamvap.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zefveyrl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhmlotrr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzqzphvd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rdmwsxxz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnqxrvgw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rverjpwj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3attlgbqz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rosvipzl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nesvhxqn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3veyrlguq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zygxqmew.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtgeuljw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3sbupuxlm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ittqdsgx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpcjjqdj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3iphlwnzw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dcqrhfro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mddsscws.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ocfydefi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyuqyqek.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cilfxkwn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3avvcslmo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tkotpedr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3azezdlhc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3redlpmsi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3idujifrp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qtjnrndz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3sfwbwifk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3swvpwngc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3roqjuhit.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3xdngxqzx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nbtpolwb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nipeiiyt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jbktspqy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nyohfnzn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3agaqxsur.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3mptrbxha.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eymidbjs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jhytkgyy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hcuyvrys.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uiqbeuqn.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3osmbvqeq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ildczbzn.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hwtezpyc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vgqppqgv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ceghrvrp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jmdcoruv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rowomdgl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cavyapiy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3bdrodrlo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3abbrdqcm.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nwjkzwce.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3surczdzf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ddsavggv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3pbzoykmf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3yvqbcszx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3uvwafmhd.html


<!-- 参考信息 -->