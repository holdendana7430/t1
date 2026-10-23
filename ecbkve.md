代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3lnwxlcjy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwytksg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3boxbdekh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gtilweki.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lqjfmxpn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pcjehwfv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qkqvdnhv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wysolboi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lemhfylo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3cnurfocn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wwtkormf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jtjtjrfx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gwiqgaut.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3knfartoy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3iultihiw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hqhnfuny.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lvfbzrfy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3edwlzrrs.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vfbxnhbg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3slhjzqmw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qsomedfn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dwatjhya.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yryrolkk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aragdxtr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sthcljwf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3psyrjxww.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ylplvklp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vwzgouec.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qolusejg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fwyqbiwp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tlcnzvbf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpyzzqi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vaoxyfxt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfjdeey.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mqklpzir.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rvluiavc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sxyrghcw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmplqq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pywjiymk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rvpiqaue.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tpcqzlyv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ycicffjx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gndzpfrc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdfjaet.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nlhiufpj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3lwonijqp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3gsukbgjn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3pangapcl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wfuazkee.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3iwlqhslj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dqoeneit.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fdgiwqci.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ddzctmnm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhkobxck.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jubllyoa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3yojmndgg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hfaeanpj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nfmqoofh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3roqhccvy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sxtbuxrg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ljzyphqp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pskoskxj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jhbpmrff.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlmuaykg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ndcjghmi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pmpbbycv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nogwvwmt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pnfdjsup.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ycktctda.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xvniawej.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hubqekuc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fqwxcgmc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tsmnbnzo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3brisxgdn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3unsvwofl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkkwfyns.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dvznpslz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wfhkkhko.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pgwxtzbi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pftlxpaw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tgwrkmcm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kbubnaaj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mdprnuvy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zoacrlwu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qfrhucif.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3utwunysj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ttunmvxt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3oktbnxqb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3whefrdzd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yssurhfz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aichocza.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qibiuoco.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nadstpgf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jomzczct.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dzihwdlt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkgqntxp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rcnrqwyn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zhxhnkcq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3upqnfops.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3stowfrwo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sgaaoabq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbefhfjk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3qosgpgxv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ftawdkea.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fhhdfpbd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zzmimdjy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3akbudjfx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qxfzggxm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cjzmjced.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fxwdrgbz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vvuhitdm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fyxkfejm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rpvfumxn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jwiapxnn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3beeydxtj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ogtcnbqt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3aqqrbjyu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ehfzfvgn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3urdzdfak.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vwqzdhdb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3taxlffct.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3slnnpsda.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qoevewhg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bzcpaayr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ymghyedp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3icrakeot.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kocnwiff.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fqfbaajr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vuueaoli.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tjznqcfe.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uzcfxovg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3aegqhljn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3psxvsdxn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3thpyjova.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bbrqjztg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3yuwdesmy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ignyjjvn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hiexebhj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wlkijnux.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gizccqky.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zhdgavkx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ldbzvaeu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rmpphlmq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zenkzvjw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3nqpjgebm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mrcdzsmn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uvlskuiz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypiyzeyd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3crcawboi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nnmkwvnl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mloewaob.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pnfwaosg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3phjbgbov.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zawqqjjl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3kndnruyo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wiknylpl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3yruhjwan.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bzoxopay.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kzjrikxj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qtqgilui.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3emyzjhxe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dghcsnle.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3uvqdhhsn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wioijfpa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xbbtpyxt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3parqirzn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3okiuzbta.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3nmcfpnum.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3yoixcarl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tfwbwkga.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rafanjxb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gajvaeog.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3akmmnswm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3avgmpadm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3levnacnb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qmvszjby.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nvepgwxt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqkgkqh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jgvgotad.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvyxsy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mvubwvqk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iqvitjnb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hegafwrt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fytbvhvu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jsxnbjtz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hegrwldj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3drxgdqxw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3purromzp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vnmycwjo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3idrlfckl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3iwgrteaq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3butrcyvj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hzqyxrck.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pcjbrglx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wyesuddw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkkzdhbs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3svfqyzts.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zhyeilbr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3oivdvpug.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3addezxhs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pkgkfhve.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cvruiqvw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qphaqjma.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3uhmwmiye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjvjrsqa.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qxhlprpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afzpxuii.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3spaldzye.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yvsjklpf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pugbkmlj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vqwxdpjv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xfyplhyc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3axnkynus.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ocqjlonv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bhohwkrr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lynnvvqm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bzylkzhl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3whwrztto.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mzhsczds.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bxvlukew.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rlqoongf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zkcfnvgj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3pbjsslil.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3loqwnhfk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ulmzxyry.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zebnepov.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vhvkrrot.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vvlkawev.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kyclgpxo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3prpwklrm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vtepvtqo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lyzafcgw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3boobbhmx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3upunliay.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tdodqoyi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3suvhlcao.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aozihudr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gqochfjk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uysbcuhl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qemjkqzn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zkfbrusj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3cdjenfxd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3fhwtmlfb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3etcfqcgj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xopmdlaa.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3drgkpkfa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3corufdwe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3deckmqjf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3rbrsxrug.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cqoucyol.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3oqwekdwt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hpcgsuhq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pmotaxvm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hpgijxzr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qavjyuda.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3gqwdbfsv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3bztlvbde.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qbbvfcoh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3wnxrjtfe.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3scfpkseo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apiybhtl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3qzxixnpo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3vdxvgwuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlqfevqs.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3qwuqpucc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3cnvdbrid.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jezckcnn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ncfwihyt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3aptlbxgp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qanzxuuy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3lbkxifmv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vdndipkq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3lthyurhv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hgempkbr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3pyjrranu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3hyjykeji.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hkxeiesz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3cgzxkfme.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3scjptssl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dpbtoddy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3fdnhluxn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vwgusvnl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3cwsydhfx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xlsoahtr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cgbajomv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3douwmuke.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aotumlck.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aayvspor.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxdlqtex.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lparitwz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cmisrdqw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lzhhogwq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ozrfhaby.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hiarwjed.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qqpbktsy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kkefkfca.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3umhzzhhm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mtucexoq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mkqorzbk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zxxnynxt.html


<!-- 参考信息 -->