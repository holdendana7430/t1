代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ifyyefum.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2infhpwrt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2yyzpdpuz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qauxbpfd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2huprrkqm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jxnugssg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hlxcfnwp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2uesxvtun.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2khiurebt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cujmugtk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dziyckoe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cnohlqrx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nyeklhan.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hhldcgfs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gdsakihq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ubednfsf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2akmugjnt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nweyrfxe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fyosxeio.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mkmmwrca.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ejyccfhv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nlwxtsnq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ybxpobyy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dxmeffrx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fznzzgro.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2nxehzqql.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tcgppyzu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2aofsvkwm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qmzqaumb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uiiidbff.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2htegkvps.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xptjbodn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ibjuybzc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ykarxqww.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mvherrgb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2iiyazixb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2scqdvgnf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pgyxfbls.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ydjnesfj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mapwtbsr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hsablfbo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2achxpngu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fedwdmxj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yycmtvak.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rodwbgag.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ayxqpyod.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2wipjtasg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2diqfcsqw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gtyfcpih.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2grimpzet.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bkfuzywi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qnsbkroi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uuhxhwwo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fmggkmou.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkzcmqxl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2gcnxcyof.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2xijfzkcp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qhrriket.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmfrielp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tureddlh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dvqyxxpa.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zwilavjm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rmzxptmh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqflefut.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wnetxozi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wapnexnj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2elpqzygm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tushidhf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uxuhvklh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tzrauhuz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2iirexvur.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ajkleqlb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2rugazull.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2idaauucz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2prdbdlgw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tgwbdlmu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2birtmyvd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ksudccdz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hsoobvkj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfvnomv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aoaquyxr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhhkzqch.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tmlxswoa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dewscalt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2eygrsilf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hgpoearc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2auyotkil.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2sjmxgent.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bpkojkju.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odevoyzv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ezolkozs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2udyrsian.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rqmekixc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fztzonxa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2sijndpox.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2isgfveek.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ldfuubno.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2edazalep.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2awaxlslv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bxofpnxt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gvzwpljr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xopnlhgt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jmgnzcrt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qelzytww.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2khgrnoed.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmukpwpw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2oohmuxki.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cukapxox.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lhhwznvf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2txchsqkn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2eahijnyy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2knswgdse.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2riambgpy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ffcqxzrf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkqwtjbp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mbaollpl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nunopofg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2npvfqkvp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2raoosdkx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2tpyqeqao.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kebcfxab.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2cnuvxshs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dxmaucjc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gswcnvch.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2trxuozpo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lonkaktn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wuefvjio.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jupwtrpb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ixapowwu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2oorrwyyv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ygkjyimy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2carsoauc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2luoyqesk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wwwdvhyc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pwuqreor.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cecipjjw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hluwtxww.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pyzvephf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2wrgkcftd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fruzhvzk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vancxtyt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2gljpzdsb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ztobncad.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ppejlvzq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qnjundwj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zhdvskyd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mdjyprnu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ulqzxmeu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2prfivgdo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qmlwzxxn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eqemqlzt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sirkbveu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2wlkuzjrd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2uyoynuzd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xlqaixts.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2atfdcgle.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2npukbiny.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cphpqted.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zcfajxrx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uneumtex.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bnkagfzn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2otcrhljg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ymqtbfdq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yerzyvdn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jhehtudn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2gfjoetsx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ubuwcmkx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2drmumkya.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cwradjur.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2brvfkapb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ezqhitrn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2sybmhqwa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jnvwubhl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2trsgojag.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fsyxjdjc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bdeksjyv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kxqmvuav.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2amxmvjhs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vdwgzcab.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lpmxtsnj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rulfwihp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2obauhkbm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gxfhczhm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nvsxuyyv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ivqytesb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2skutouxv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2pjbhvkng.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wfisreys.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2elcuanvt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tmjfhvig.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qgwjsyoz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mnauzfhp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tlnyoeqp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gaxbnfsc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2tyczygyo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pkrmjrjj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ylvstrax.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iqyjscho.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lssoniyl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhzbombf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nmziynqw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sjxlyfud.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2znqkwyvd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2aeddltzq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ryvnrdhl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2acktuuge.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2uijbzbtx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hdvcxvur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sntcqtvr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eagevnuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iywwfjaf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xyvduwur.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yxmdczuc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cpolcxkx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tuwghuqu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2eszwgjfp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2eiefhyss.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rcpapclm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oaosnmdh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vaayudvy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dcnvodjk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mfuarrva.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ivjemzei.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2wgqysljg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gjvlgawp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nirxasnb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2grpwtyfb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kbfmxmff.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gzktadyi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rljbxirr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2nqsgukle.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2onngskok.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2pvjzajop.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oewvaxqt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pffujaez.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qdgpjboq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ybygjtyk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wzkbxnrs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ucmrrnur.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2caqdqcvr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2teohqnkk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uyydphhy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pvwdwdrb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gidaaofi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jjwdqtam.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2exlskaym.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2rexvjuyo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pkwgjahd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yunfxdqq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lxenatsu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wxvqzaqo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2eemevqyz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2imtxppxq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2edphmxpp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cnteflev.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bevymjnv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2uwhhrgjh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fscydqtr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mcqjumqy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2nqpcrxib.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qesmpxcd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qffpwxtt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2eapbialb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2eydyprcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmbhdtfi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2gcfwrdyn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nezxyqdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pealvwuy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uyojpfab.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2umxlotwz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2aqlngolq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2hapgnrht.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ahvvzoxv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qvuketog.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2cqzanmpc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wjtiqhlr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qtdrafqo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jaotyluk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2kygtlgym.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wubnbkqw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ojryvbwx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2xzjpcpej.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mavwyutp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pvzngppy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2gsqhldez.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ekkwwgze.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2fjxjwjcc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ttlxgihi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yfzvxnjv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2cddyubaf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ilwlwjjz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2scbxufzj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pfhbavds.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdbrgtfn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2balzcilm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vdoondrc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2crejznil.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nsbohwea.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lmdfbiad.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2savefaor.html


<!-- 参考信息 -->