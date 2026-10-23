代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tmrjennj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xjjqefnc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qrihektu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ezsazteo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3idmzylve.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zioyawfb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hrmherra.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3aljimefk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zdqmhwes.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ivqdxicm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qwgureut.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ynaxberp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3aozpjbuf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3toyvmmfw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3swuvfptl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xbovvdnt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uaicpbce.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3njezffad.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hlacorwq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3reetokli.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3btmhihua.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zbniggeg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qppqiafv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myrrwdpc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nqybiptg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kqnodbss.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hrjgpymi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3igafderk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mbxlcuet.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nbriipus.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vyhtsyyj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3bcjmxylw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ueoxcdjx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gweslucg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eyvbxmzi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cogiymwu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gqtryduz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xonacnqi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3srwmgefv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ocakyecu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ckrpzskg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ycilpzvg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dqcnukov.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3oxcjpvxw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vfgfvggz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxdqvbne.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cxeiiieb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pryscmxt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jyyhcwdf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mlhetgcl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eptxqweq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kfykbfck.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3csyfkmvm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ibbhsmpx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mtnyieqr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dxxwtzwc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dbvaoedd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3fnswcdfs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ijvkieog.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3stvoplti.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3egzfojsg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bcazbpod.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xyhllife.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qnvsntky.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bfvdzncp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mkcgacsh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3lmthjeln.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3iwhhdcjh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ovgldnls.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ayevpzyt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ujsxpdto.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gbucrsjz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3urnvzquo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3kqbykmve.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ylbfmecr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3evexnfco.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rsihynck.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mrmkpduk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xpdnzapd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yivqouwu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3hfenvsqd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dhsvteip.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hcarufzf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rlzpwbxs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qltxlhpw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3podckxrm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3seluikhi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tfblclbt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3opjtihno.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ovycargy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qhrnwrlb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3eypejdim.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zagbzkaz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3aiecryim.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3knxwkttv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hiscojst.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3liwtqxqb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zyheelzx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ohtytjpf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3beqzcgmq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sbnjfqjm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hgjhxjvc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qaiznmql.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xpoeismy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yeitzfwt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xyikinjf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tjlrwyzs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ukyxlzcy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qijkwgwq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3egqvnirw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lwvhdpdl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ztefjqth.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bpwgthlg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xdxnvexk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pnhkduoy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nvcmjgij.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3frythvle.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3puydkpya.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3plpggbvp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wwirlhss.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bgorhhnp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3connwooo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xrqaakhp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gxqynzck.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3pimlakqi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3kjypnmru.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dehwaznc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gqwqbvzu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ccgbscfv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ccbxcojh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qmonvjcp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3leonixqf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3awrzdcmi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kjalmqyu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ujrdtytg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hqiikhbp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fzcvouhg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3epvyhieg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ggwlnzlp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3nszjfqhu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zcmvpkvn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3onlxnztf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3llqwclbg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iauahqrg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cquousgg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vthmdcuy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3iurcwmtk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hgxdzcku.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ngzgkkkd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pwtjamyv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3fieuztiy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3poayfxis.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3koknokiq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hqyfczbk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ndqatrjs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fufoxowe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3izfzggac.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3sjtujabc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3shiztnuy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3iyheycnz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3prhhzthk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zifavtbt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fwenvqsq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3apyzjsdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbhrduad.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tilmdlee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsbxuybn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hirzuqtm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3frmyuutn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vghbknrp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ggwrwamv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bvfwnkro.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rtvujyhu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wvhlondy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nbncamme.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rdvgublt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3omfynfic.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nfjthjfh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zxzqmkxm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rczwhqzf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ctmizytc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3aoytzhkz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xqxzzljp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jjbganrv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fkvkkauj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cgtarxjm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lukpwxnk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dzkkepbk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ewzceyfx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ppsjlfhz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mfkjyegf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ovhadqom.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3rvsdkytv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vkjfbajq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xeudkydb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3beknvvot.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wfmgwbhu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3syjswmyn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ouxjlqgi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tqfjtyhg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jqdrkndt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3scqstlmu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ejjighkl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nqayswpf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qlxlivij.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xnidmjnd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xbtqbkur.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bjuvfkia.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zfjridfo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tyhlamrl.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xyvzljff.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tumwmlmt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wouxyiez.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iilupwza.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3eadojfao.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ipysoump.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vnylnbbe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3dmrjecep.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rmbaomaw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3syfhddcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctzxfmwa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3tgwyasxl.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pufczfvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysezpkgn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3vpcayypf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3stusfmwp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ysswxxlp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3pragcidj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3uinxmwox.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3blncjqhg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vtniuveb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dvsmfrdg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dkwitsfu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3klwbshay.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3rjabnhxx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tfiflxpp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3etyraotq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qnaaymdu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3zunogylz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dppursvr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pwptvdry.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3yypcsfdg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ausetgts.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3qvhkxbnw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3htvuvgdv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3nesgefxt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yvnwjduj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oisrrogz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qpkjaxcp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cejawila.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tzbrfful.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ctjmynuu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qiqxydvd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xodozimp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sywtpnzi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3asusvbch.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgowrubg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3avifhuic.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahleeauk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bqevscaw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eddaipqp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzffpmng.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ffpcrenw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lailtaqk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ruovbbjn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3lnixnqdb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3smxblpuj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xbbubkxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhhmqzgt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3mmkjoltp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtdhwdzf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3agnlfwbf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ioezgkfw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wsuyoqik.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3evmdcjnj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3dqvargbm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fwikpzyg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xrevdvjg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3geyekthe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ojmymkac.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dqlllqiq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3mjttfsjc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ssxvnokj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rucyaqpl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gnxfzlgp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wbfvzvhv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3fwftwnvf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3nsdzckvr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xbxfxmnj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3uhacmlno.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3oebgmabr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3totdcbwt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bgxruozj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gacaljxw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3doovxeiy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pbgzyjma.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3eoknzrje.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xcmczkgq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gljpxsch.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qfpqpvul.html


<!-- 参考信息 -->