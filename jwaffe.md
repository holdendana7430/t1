代发 wailian999

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3uvccdcrv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yfrnrrqk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vbettomh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3grxujvil.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3bkzacsmu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vjgetwzo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3efjfirbl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qxfnwtpw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gbqxxeza.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rjezqlwt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xfejvzef.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3sszhzlaz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rxjejnhg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wgkiezsr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vwaxsvxr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xefaoucf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lpjftkfh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sqcwumsd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hqnzosvg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ynqzoovv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lvxpzxen.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kbyvrhsm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xigatxsi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgdmfwo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ihmxtfuz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gvalxyuz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rmciqtcw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fnweroij.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bphwxbuu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3wbsijtfu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lhyosdsj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vdtricgo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nrknryrk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxzpjmoj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cizkdifm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hyhfpcmx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sjgogjds.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bpkswgww.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3foplzioi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfhnpua.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dpcprodv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3borvneod.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hhahbcwg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgclchns.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3impcpkma.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vyidaabq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmnnlwhc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kuystviv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gsyqesqq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uirubstc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3nrzttova.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3plgnnlaq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gmsmzfhj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3iztwfhkk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vzjmepyb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3todhfehr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3udjruiig.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fyuafelc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tcamvcti.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3idrdmorl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qfnkhhwn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bzfrzvej.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xcemzyyn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ajczidmy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vuouvhns.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxhayzls.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3dgtasbfu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ytwddafv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tdcgjceh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3akvolxfg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzojppmr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ygoobasf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3bmdjrddg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gvclrsck.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cunbriaj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lgetvyvq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bojbgmtc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dpvwebpv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3grsmuzmj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uvlpvlcm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bvvdzgwt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bwzzkjtx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xhcwffau.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xnjxxdhz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gwnubbbl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ahztqmwh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gtkcrlve.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mytzcmye.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3glwqluxz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3duoedbts.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pimzydxo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kkoldfwh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kcbldemc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ypjbwksm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qruzjrlx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3blnswqwu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jsbxwbwd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wzjufxea.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hyambiqq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mswlbzmk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qmyrfthn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jmuzecge.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3pqpzlbtr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3nzecfcfo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rzpecnex.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lqrvmqhs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ggzaufau.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pjowtgqn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gotfvdup.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lspclrme.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kjwarlqg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jlvrmrhk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pwkizhxe.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kgyrherj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hwfkplnv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dizifhyp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hkrgqgjj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jfputaxd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bxfmyvmi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftqfbsav.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3llcswxwr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dwnuhmui.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhtacmar.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pfyvmngp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lawsgiem.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yxyiuchd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qbvylzed.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xerkowtj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ydqxszfc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qmutynmy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vwsoyywh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jtprmzhz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mxmtioli.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qlahjkso.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vnazcxdl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohwrpiuw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mmxafbob.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jcxtcptt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3trnlbyfi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3muciqsuo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pbbzkjao.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zkjyzjbc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rfyjjbmu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3uuysnycg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3odxafnzg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xhwlhkub.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hgirfxuw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jmzfblyk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gnixrktc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uuscbuxp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jiffrohy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lqdxcbot.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lbfpmpfd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3suchjmyg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hinhkego.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dlpcqpyy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qmdjqfhx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zhjjyrzm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mlkpugsb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xchxgtsk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3dknnygsf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iizmauff.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uafcgrhx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zlfntsut.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3womaavyy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gklkcqdl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3tjetriyj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3imhrxzvy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wrbtsoxr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qqatnnxr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jidrdrur.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwdipbc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mlwrbdmg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hlwzxuuh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ngsmeywz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnielkzr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kbryebnu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xgytuslu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ioapawlw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3atbeiscj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ziwfuoov.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3loddwngx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qqujjggy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3aorerdrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxqppkyf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3alribmoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kixdjtnf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3outtynvp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wdozunpu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bcqkbykc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ajlyabhv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dplpmtfe.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ktfssnaw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3frycvdhq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ggqzsjbj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zuhotrte.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vcyuaxml.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nvicjzwi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3flphvmfn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hxqppihl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3walsdjdp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lstejqqt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3aciinyek.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wgnbfcol.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dqxdonon.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lqyvqohv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3prtkhksc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lcsmjkfw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lwggngux.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3awdzesjj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3czdzubie.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3snfzxilq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3pqppliwd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dmktjzmy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mxqksmnf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ccsptzjg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ydgdyawo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nrzuwdzd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ggetahxh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kawrpeqf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rnwfwqvk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3irujhxan.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3xezxcygp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zjgicnme.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3yjevkqwf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ogufofvy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3magaxctv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3yfseofer.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3arlfyqdf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oollnhhq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3usppoqdr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mkwjnauw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3exzqxuvx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qbugdfbj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3sofyamhl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wxvkrogb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zgfffeen.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qneszchl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ybjqxukk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xbqscrbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcilrxcs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nzparfci.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3vsgztuea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hogaqprw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ujfkwsud.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3klofguit.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vvpskwfx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rdajpuhz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3avprpiis.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3nyzbnwji.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qhsvbucc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ufoaeair.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3babcefyl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3qvjusfso.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3lnqrtygb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3brwlmqbr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ihgkynhp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ocxwjcyz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3uyhotcka.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3jkznvwbo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3azcipksh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3gbbswuog.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3mcfsmefc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hpnclkvq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ivntcyva.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3adhdroyl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ofmatrca.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dwawvssp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lkcmqqon.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yidoyoqu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3sbbykqid.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zpgwcbph.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lzlanabe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qvfmqvvs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3maubbpul.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wswrxmyu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zjlimwzi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jhmyjqzc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hrlrurfs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rzvwwubt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jsltzkii.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3boifsbor.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3doahxldu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gbkysxtd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lytlhvec.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dyzzbbxp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xgjimjpk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ustizozr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzmqdqhi.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3obxrrnkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jurhoaxn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3hslfgyyq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tiawkxde.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3guoxzggb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wbfzcndr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3bnanlvcl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lxmnpnba.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mrrpwcxt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vznfxcxw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3enzkqmao.html


<!-- 参考信息 -->