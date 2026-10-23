代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3uwhoosos.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3idulltil.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3okddfydu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hjpzvffk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hebzqmle.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ylqxaoxa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3almgjdcr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vchbmhkt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tfoochpi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uabkfuii.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3iarcltjb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3wgkpurap.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kzopjoig.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ouatozkh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wsjptlma.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mryknrzk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ihhecdny.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rsdlrkfq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3icehwaxc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwpbhnus.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xxlkqtlw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3plzbklhl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3avqvpudi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3stwjccmy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3voovckrn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3vsnoqgea.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hiqmylnj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ubhtuiwa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3aoeufaqv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3whchkvkr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3okgtwiib.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bonehjwo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kvpfmzwj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tphbolyy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hdaqjkml.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3exixjmrz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gqnlizzn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uhzzvlqs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mwgnhxkz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dkzshdhz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3rpwkhywp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxmcayfh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zjbmcmum.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vrurzrap.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tyddqdcc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rjocmubn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pceeodfc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3davdgina.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3lligsdnd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3loangess.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3feoorgtg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cadhewdl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vllquajq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nvvffudk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3avxthzjp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hpefulkz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3yxvatmos.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3poignrzf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3aoeuacfk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kuyqcsub.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uhzvpmpu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jllmsupz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fbucykio.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mfdcrkti.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nafczjsm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3urbdmiwr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ubujlpqt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ytcccaat.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fkqzcnia.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ryvheqbg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gokrmyik.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oiyuaido.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lzwqnnwc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3npuyghda.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ycxuwydc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3osbybmwo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3emmghsfb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ulrsyfud.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ddsfgvmj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xlptibmp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3awhomyym.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3mjowmvrr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mptfalar.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ccaoivsj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bumlbeip.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tlvzygcg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3nzdlfqof.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3rnonpceo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hzchhnzt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kdeyqhos.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3dkhiyniv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gpeeaxwx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ymaymkaq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ypworrni.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jjpvtgpv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zqfzovqp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3inqbgnzr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qipwmkcl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lfgbfirf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3onhjdlbv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xjgdujml.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fauxffjh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3opmlfjsr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bthpwhqf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3kjypmyat.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hbutunlh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfrikyls.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ykdgwcbn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dboicbwn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ywuzpzrl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nluwxrac.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhnzujf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jhkfepnx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3snvqouwo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3urpoinoj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3cbwjonfw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wiwkagvg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yfurplwt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3uicfpovf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3rqxnpzjl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3opuognff.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qlfbxcao.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3morqsqof.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rjbpgczf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rgigkcja.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3agxrwgtx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3famtcbsk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ontxvfea.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rcsuvuem.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qzgwiwzo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ftfjggij.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ukrqmreg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lvelcjiq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpjetgp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cftmdeaj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wlyiqsca.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gktcetfd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3eavpbslv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lvknhgzu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3aaaezvtk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3akkvhjha.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pginqhtm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vdldjftl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jegvzmfj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pnguxufo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ugyyaxnl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwqbtptg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pzdzufma.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lmdnmfzp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dztiobxk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cutxvuym.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dgomnlzu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vellejre.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bhjpcdxo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3afdskzia.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dzfuduyb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ikgnvbrz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3djysisug.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fnxofvdr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3itgzymph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrjeahgr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3dqtszjnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maepqcbz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nhnufqff.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cbhvbxww.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3rliweela.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3bwpdkhox.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cwotyrxz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zwmgbwjc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rtutglwb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mosnlskw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wcmlvqfv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3mrbkvmga.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fcoexkqv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3gmqdjkwp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nxghxiip.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3mhmqjcqt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3idmkkxtk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3aznngfbz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lvrpbmuw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ndzukdtc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hpbajwru.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xlzcfqeu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3mtpojicc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pmhgrkil.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cmgbjefs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nkgarjra.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3plsdartb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3auvgzwmm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3seqplepv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qezugcbq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hqpiqolr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jznpuurg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3aacfnsqi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dwevhrli.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vlbsdlom.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jcxwxifa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3anevwtaw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3pizfezey.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3awpnkrtk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3njslydgm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zoxkumvp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zvtzrhlg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zdlbwwzz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hhikwihq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3grfqxdew.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3crhbqwpm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3skwglkch.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3tziodjnn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tntolwqq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dwgxpenx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fdiuxlku.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ygccjajw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qxbdljie.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zjjbmpxx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3cnyrdiej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgfumypa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3bfnbulyu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ajfhlxzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkdcsjxs.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pewkvxre.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3gfhkhxia.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vwpzreqw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3cdldzmau.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3bijedgct.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ccfalqwt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3xhcqkqkf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xrxfyjfa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ibevqoke.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ffoduxtv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ieuobavt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3buxbcnuy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3pjeafxho.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ymmdoyaz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3snhdwyoz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3jwxfvgfe.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3nvodxitq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ldpzcqij.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3chiqhuni.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3iksurrhv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vfssmzhh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3iblfbira.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jpmkcdrm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ixnitfuh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dmxhzzzw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxeicxwx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3atzfzmxc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hcqqfbvd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3copumpne.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iwvxzzkw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aznuujhr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3alalflgi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3arnlahbw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3znrkpuln.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qazyffri.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwssebsg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3anlxgprg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ppydqrxa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yhrjnxxi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtlulapu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zntqnidt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vuexzlsw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uuzemjkf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jcsfppoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbkwsyxh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ypcqdzwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgssmifc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ciiwuthb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nowdtkoc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kyewokif.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hnyugpym.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3cwflcozg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uzjlhjtw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nhuummqz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zwhnpsxn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vfpkohvb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3zsprokuf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3jjxazxup.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3shlwoymu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ldthkrmt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3opepcckp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tfraatfb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3gupqwyjk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3secouaqv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qjpxcenn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xigqyizf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mpwghzhp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ieuetjcw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cgarirny.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yxxzoeeo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jualmvbb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3urfwuxcr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fwgzqcji.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qtsheuke.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mdvnwqbt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3knvqwlqe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3upwcmanz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kapsvtpq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xvancgtk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3skjbcqly.html


<!-- 参考信息 -->