代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bthyscsz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nvvzttun.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dynpkoos.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yxenvyvx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ibojzuhv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wynfmnqx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3czdvlisj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ndlxpgwg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3obbpwyhi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cgtviazs.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3blofvizd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zpkvcfgg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ibteylky.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qsrijvnq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mrqmzdbl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ylnivaxi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jpoqhjaz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3uygvwsmy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vdnhcmgl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wxnbekqz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3twzllmbd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3rzcmvwys.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eibdawmr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3znibspra.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jkjnfrkm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3iuiahkps.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ruhbpsoo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lauuijnj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hgovyqsk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3cvqyircd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fzwtyokk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3njpasdjz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pkwroigh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jsphosyd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3huzcxtkg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3aizgrbpj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xrhkheys.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypyninev.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3bbbsaqln.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3csdmwhxw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qceahdku.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3obrgljxy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vcfxjyej.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbmiofwb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kzkuabjn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xmmtzfri.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xpayfnsv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3njwyurnr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hinlfhrz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3afxrpaug.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjeikojh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nuqymkcs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dzahzfnu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mctmkwqn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hebnkwcv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3iirpxxxe.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wegkapfl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dtbzcthu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3gvypgujn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxivjxeh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hfqyxsft.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zszjrepd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gceokptp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3crolormb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dmadpnqs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3taobtsyo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rbxeqbxy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bakurlwx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tspwqvqc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuluzneg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xwpilgcg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3msaoywmr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dwmcabfy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3xwunfdcp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdmcliev.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pcufyqtp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rzebpccx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vazkxbbq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mcctkbwn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hkehdjer.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3iovkgzld.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cjeguolh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fubmsglx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3exzxddxk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rxvvzizx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jgegeqhz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jnkaddfj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rgqphnht.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3aayqnqas.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xfqgwkdk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hjknnlzx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gbibgfif.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lidmkreo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fpcmxqxe.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qjhsqzpb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kasgsdxk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mzhkchde.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3asvlsshu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3npviuqzl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vqycgtet.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3mmskphuw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hrnjhysz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sqopxgoh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3icrwkkzb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bouztmjz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hintjtbd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ayzzewwf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3jprrqykb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zgjbjnfp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wxwaijye.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wrezsvei.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3grofycpm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kvycelji.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tksqstcw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ywvoyqnz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3sveudybx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wotnqvkf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3csmgnxbo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3cxfacagk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3nxzbojha.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nxctbhuk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gpwvolbe.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3asmlkfjj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3scuxinyq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3glkaaavm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nvucrspd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jfhdpxls.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rbyecdho.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fiyqbtgx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wxidoohs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3twqjrgbq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dppdkvio.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jhjycgmu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qfovwvul.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qdturiko.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qrntqzfh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wgjejpog.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zdtundjj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3aesottiz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpxfdljc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rlnwvczn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ryaueyph.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xdqarmvl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3swrlidms.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fxitrqkb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uygplvrm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ibxaxmtq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sczklxzk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3equnrgzf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3alendpul.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gumaqozk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3nqupmoae.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jiudivnd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tlkdlell.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wosmnqkb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gxdfvlwu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3vrceqkvx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3lremlwbc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hnlmtmyb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hjkbrnll.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lgralptd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ofaysnaw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bgcxkbfa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pcfqrjdn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bdzezbpx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lrwlhrgc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3euqmnrht.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kgfvyaoe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3npcwkpxz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rbnbbvvo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3vyrgrofq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ygmntiay.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vgqwkdak.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kfhkmjsf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dgaiitwi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qpnqvfij.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3urbxsiuh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mktsferj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zphjyxzl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jmweigsa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3drgxwvgb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pecmulld.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3gnjeqamg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ndmzclsv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3voozibvo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3dzrerpat.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hpufpzua.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wznbwkpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfusyhsp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ydmywnks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggualwjw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fxlbzhkx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bytlvbkc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xcutkyqc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3btkqghyd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hmrzarcg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vsdysacc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vexhrpqz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ijtxmdrh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zvmeyose.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gxeucsxh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3zlrvfoba.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wpvetqpc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3iwkhabdt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xghtmlvc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fignpbbm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zhhuaqin.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gojlfomy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pkmxopuo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hjjkpung.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3afrrzzan.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3sefvaivn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3khsprbsb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vxqzmzpn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3akrnbgbr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hsotunbr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3onndjavm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bawarykm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bgrcmykf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3thsulieh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vxkgcjho.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vcfhotwm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dyfeuldr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sfqrzwxi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xmjrawke.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fqjhryrv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mqmjtspq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uqqflbtg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bionjsnc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3oznljatg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3bvinigei.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3kffidsiq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zhqrdphf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qiipycuv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3frgpuiqi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gxwzxfcw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3zenmbfmo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rcnemccz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qbiqzpaz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ypujqoft.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3thvmmlco.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3bjrleahj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3abgokyli.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3obbctmdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hycwkgzl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ahnloyvw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ssiffesb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmzzvscn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ivrihuxo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rmdngwrc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jumekuok.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3oezefjqv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3krhisrvx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3kzgxrujm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hcaeyqde.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3awpsnanl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gacfkilg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3wwqfrgcf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wwnivtrv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3stmgnoii.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3iihdcqjt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3nwlndasz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ddzfndlb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3oesogwuk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3aldxyjin.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3evovxpja.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wmtpdega.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zhbgdfps.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ezlljzby.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3bteahvrt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aphnskpz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cqeksozi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rshbwyrv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ualwsrko.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kpqvggnd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3vhfcdweu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zkwjdizs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3phdmbpph.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ypyrwwiv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wnapuzwt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sdrggfgf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yeieskev.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vvrnmhzl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gckfccqf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbipzcjl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pvbbavia.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ugrjykcb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3zfopbdxy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oldmxxrh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvsfiiez.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3robjxuox.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3faxbjfpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbvarcup.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbixykfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zibdilyu.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3aimyponv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3puiqsbhr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tbzdbhpe.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3setkavdf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3flhqmwjl.html


<!-- 参考信息 -->