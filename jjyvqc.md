代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qclrjfom.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kbqmfdsn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3mpzmhkhm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zozqdbmd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lgrxrmbx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3khtbqhsc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3oetpkstw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3icsxzedw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vulzdcdi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3coiyskuz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3izisibmw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3soengdab.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ucushxef.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ntwxfwox.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3empsbiro.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ikxbfokk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ndduobto.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pzdrmacd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zboaqarj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bhbrwltb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cqytnuns.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uqfvyeuz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fpxtcamn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tstskmmr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rletiydb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3brnfuhlb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3osijwpup.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vjwmyrnt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3cpvqosxo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kfifxsay.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3svffppyc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lurvwbmx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kbwrqzwo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3twmdexje.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tvslhsks.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3puuzbkcz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3icycksbx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tkaiemrn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vvzmzofg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3widtsyjh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zkmxbgyi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jqjspkwv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vfgtnbgq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bxtkmipd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yjjewetk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3koeeuklc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3cstgrtpc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ybusqbmu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ubclrvwm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3csdxrrzd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uhbkioiv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdvbqcwe.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3masbcuao.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hoaopszl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qrgcxjkl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kkamkixy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3npkhebas.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3pxfvojec.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wengrzeo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3khtdocto.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ajrgxjam.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dgwmhldu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3juyygxbd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gaueekby.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3okvevlrp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dnjhbicd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3upjibkwz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwksjjlw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ieplsqbe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jgkosbgf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kpyquxvl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vswzgspv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gygsvakv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fksvhmnt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3djerqtjg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cafwnxis.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lukruiug.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lljufeqp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ogdczmlb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gkkrtjkm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tlbeutdp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3htjqbjwn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3riceyfls.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3oqcuxtty.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ddeozytt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxymvvjb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fzhyyolf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ppodsjks.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gxkmeiqq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3fdtzlaik.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wpahdulm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ygzdtmmh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nqgytxeo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3wpccxhhv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3aueuxnxd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3fnvtfwiz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tjzbossa.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vepybtzn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3njnysbms.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uzanilfm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xbyaltyp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3urqbitpn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3npkatxjk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zzufseyw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vhwdbqgk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3yfvjeotu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3grzuuznx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3sxdvttes.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rcpbgqwy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3uliytspm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tgclvzoc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kmxucarn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fxskcoos.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3odiebecy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3szgzprwu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mkyrpdna.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zkppxgvl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vrimlgcq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tgitrdvt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nsffzmcq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bhukkgqu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cnheqqah.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ehpipzok.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tnlmoazp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fmfyaowl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xgudogas.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yyxsdgma.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fofavdgc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3olksagyl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xjkcgbei.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zbgppari.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xybkarhm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3evchmrkm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xkhvgfjv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bbktmzpj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzixnueu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3twrlbqrk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xtplbotv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jhiytlen.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iphfzosu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3axdlkcxw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3htrlrmmp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tegycdux.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dvqueysq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jcgqcwms.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3exsaoaai.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ftrwwwif.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qswjpqvt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gjsfepnz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lslbgxbj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3otkhdluf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nusqwfgs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bnzysrdn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3obhseivz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3nmuowvsa.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wwouwhfm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3oalyplwq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3yknxgozd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hqxzpfng.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3abchliim.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3aattlmuj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nvgvbihe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mpeqvjwj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wkmlgbgr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3thtbprsg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kfbzqhnt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qcxvbick.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3uzrgizfu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jvksgwac.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3itogkbai.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xrvdgfxr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3wnmutaug.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bhaqjqxy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jabcivtg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zvpnzsib.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dmmcsioa.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fljvkyyx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xqopyult.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3maivyxia.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rwthwecv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bxjxksrq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3trcrejij.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3swfunvex.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vexvnsjy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rcmovkbi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wxllpckk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lrsrbpbv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkukuofw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kkegiepg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kdmansie.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3uqztyzie.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tseneghw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3yauoftli.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3depmuidp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tvstarbu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3apuakwle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqhyievb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ybnyowjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aadoqsro.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3spktiuiq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3fpffgshs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zqxlvkkv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ikidnbnp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dqeofvau.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tvmnmkmg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3unhhuqru.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3midiplxm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nriejzvb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3kiegvymw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3pgqbhusa.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3oxqnzmnl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3diirkouz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3scfambbv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zdtywkhy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3dibjbdtw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3teubxkut.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gpvnywmq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gyibefxe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xxbzftqw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3eynuibnz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vrxwitmq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qftizbci.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mcyvbhwy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zowunbpv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3fsniwgqu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3anefmmrg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kirenmyj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zlflxcgo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3setpvnbp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jladnoim.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ntqphprc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ludufcuw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dfdiquvk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kxaefkpw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ifvwyxwl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jgddlswo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3oqjzhklh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ykotmpuh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zfougvtt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lrcykxfb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3dbrusjuc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bslftqgy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dmxipdvn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xmxfpgqd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3crdhssdf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pdvzcyux.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3aziwiqbm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hubtulrc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hgyhwtsj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3yogalraa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qpgcuwvn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3witkxskf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onnoxxhi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3yuoyezot.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tbtzzswn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hweyyetk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3cvrebejj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3fldlnytu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3odlphezz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3sisnhcle.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3gpvereee.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3rlssptnu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mndtpuxy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3zuyvfsxu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ckjzugyq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3vxrtbsrr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3momwxgbl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nwpymoqk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jltyvyhd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3mtzvxvys.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nyhidshm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wfmllwgy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3dtiqykrv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3yeaflwru.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3bwnuavrd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3qbuwczvt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gvrvyhmd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3urtanvww.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nzdedhug.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tvfcntcx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pwkglzjj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nvrkpocd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tkyglaoq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uozubzen.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qlcwssal.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ctstqkzc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3daxrgbjc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cpndkhni.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3azdiaxyu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqfwvyfx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnlntxgg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zqjetqdy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmnmunty.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ojofmyes.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qqdcuwpx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ixoywbxf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3marzfzng.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bzgdljbg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3myfpykvz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fhblylhe.html


<!-- 参考信息 -->