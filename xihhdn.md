代发 wailian999

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lyeojkwx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bmoxrakh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bgtzqgna.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zkoencyt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2wwgjfwkm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kjzyvous.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2cyguvwza.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wbyaaftw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vwhmsxyd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dgxnvmch.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cbdvuhho.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xtftzwny.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kphloasd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2eubnqfgq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lygjkwmg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iwexdmdv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vebletmu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hkdcwlgd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vraytjsf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hghfmocl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hyeptnlz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2avmzfrao.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pglckbyh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2iavhbfzx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fgkktjox.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2stfgctes.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2drcjubmx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wcfecvju.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ynehyyzi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wzcxbsts.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2upkhselu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tebityng.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2yuhetfhu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2sztbrfql.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tgzquybc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2oijdsuwt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zyqbnube.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ivkgphab.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2cttwvcyk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fbrfvscl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2pftbwbzi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2tyffpogd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fbbitmjn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pwvbwmwr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mvaqwdrj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hfsxgyrm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pxnngtmy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vuynblze.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mjxklqud.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fxnkeaaq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mlmixvcp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qolsjfed.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tfuhhblc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hvftkfmx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kwkmbonx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2crdkcamm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gnlsotnb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyhcbyed.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nakkirkg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bcsegitk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ytzjlczy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2eurfjmau.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2onujuwsy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kbrsgvrn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jlmcakgz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rzbkzhww.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xebpmnck.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tmrjafgk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ycxucblp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hoyfkcdq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qcoawczz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2eklckybb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2msjpafep.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uprxkvub.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uslvbrwv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bihfyggy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zvjvebhs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gnjyhtyj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2naukywcv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vdzfdkxj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wevbpoxp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jdodirhj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnfnzvin.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vcbiiosa.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jizhmejy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2dtrmthlr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wuxewrjj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2znzpusyx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sqeglfdk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ejufdwnv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eoznzydw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2plvzpcwl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2pmfjqnbc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hmpnlxkj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tqoumaal.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qtkhghua.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dczjbcpo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qhritffs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mboxkhym.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ipzfshci.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2uaywqlzm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ubhdocsq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mlcgwyvq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mmipesks.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2otondgwm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2espufsck.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ufbxchyy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2huzjgmgw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ecxqjkmo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2vjjtiqgp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2htdfpqka.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nomepjcn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ifeudlzu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gabbmzdx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dsawekup.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vewovyln.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2invfnpya.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cjvctaud.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2abwhapfm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqriivqn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqajasvo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ghizwiaw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2toezytcj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2almfvltg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ycjudclv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vchwalhs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vldpbqdk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nvbwrwkl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kzldqzgi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dvatisim.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aygztira.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2kaebxwwp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2oeknrzoa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hcxorloy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2llffrbms.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zvwxkoex.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kzmbzhhp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2msikxkrq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2oojbtrpl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dpolilro.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vokinncz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xqbbuope.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mlcxwlly.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kecrfmow.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2csltxffd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2acpkqgrx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fzaetpxo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2knszitoj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tmrowrdx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vgpvwgwe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2plqysins.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kzidbcpf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2marxbvrz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lkldtipz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2sljhqyvk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ycfklibq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qlzsugem.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bjkwdmfr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yzbvitjf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vkcljfmh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ctqhepap.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lzolqwqi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wfsvdeus.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fstqxktk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aoqybmju.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dwnhwfdv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2cylkzjsi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dlcsrxir.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mezxzcdf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2hhxrmavq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2aolbejbk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ojxaabii.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2kjrpwifp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xqcwlpyy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2asaknglq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2yqsjaqrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvvanazv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jwtmsyfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olmqoflm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cotujrin.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wakgbkrs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2egjsjbuw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2rpaybetl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dakjuzxf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dpokqnlx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tvkpddlb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eweiessl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2acygvkfx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2sbbzsgxy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2kbzyvrjv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rbfgaqrr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2osydpjue.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rtegohvp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nvyiiauo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ayfhuobp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jgvysgpq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2axmjchhq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lwmczgys.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2gdhznahl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kxuruslo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qkoxkecj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2udxcouoo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rsnyubjm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ytcghgws.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fqiuvuoq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2coyjbqxa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rbeumvtz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xszitgdc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2coeaqawu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2svcnctzu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kbviouga.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qgspckcd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wioyxnjr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zwpixdfe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jlqgwusw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ccgqpyki.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zrtgllvf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ixguyyvb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cmltfvjp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pbfjrfhg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wqxkzlri.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gyicrkef.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sbqgnmfd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2smzszili.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pqxxeuoo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nzypseph.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kxpmsuxl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hywcmlnk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kcxbwmld.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2slfnsgbh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2tanvphcg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2avjscuml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irzweyhz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ijghljga.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2gmnbvenv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lekujosk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kgyjzdcc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kfqsceqq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2mfpfiave.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gjczufpt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2xdimpxxt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2xieamdor.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2plmpdprq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ydezlcsm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ldqcmxgq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2bgssuqos.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pdoviktd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2jwjxlmzl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2hmcztyam.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2gqijsrrw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ysrwpuhn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fmpisiix.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ofqhbnnb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2dauarjdo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ldlbvfny.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2sqcvpvlv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dnldlvzk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2lebdnewk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zfpvebla.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bqnvtdmo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjzbmjsw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rbflwbfd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2txldqxxy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2shwaflwh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2mzycjizy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2toegqurr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2spxnafzj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hjmtgcwh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lufddpbr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ifvnkgyd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jfflugbu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2evpmxhwu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zdtozsvx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ssathfck.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czrixzyw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bvegoyah.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2acnaseau.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2tbfoizbg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pdtpvahq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jzjiwttu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmrctewe.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wevxhzza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqlkeuyw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uoklbhcc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gfjkzrnq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2goqcxaao.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ebborzfr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xdfowuvg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vdzwasbg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wdzyuyxa.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cdpgnlaa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ybhlcies.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hlyfbvbi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2dvgdptog.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pxcrcyjn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jjflumek.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uuomjbwo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2prqhkcgn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2yesucmfn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ziqdqqlq.html


<!-- 参考信息 -->