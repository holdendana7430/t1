代发 wailian999

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qafuwsmm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jsikozki.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftqqbqor.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2txcnbtcr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ovpqpvgl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tgnbkvmp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xivchuit.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rdpxjeof.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gpctggqc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fsnxults.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vfvvsyrl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rkucxlgk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dmuwymze.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kroeqbub.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2elzrepod.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yzpqwtxo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ijcuxxmy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2cyjihudl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wvlnsjfb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jzlrfogg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rkaoncdb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ligpuaok.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fmzanqcd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lgqpmxtc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmhpgwos.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kcuxqjza.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2usnznarx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iwwjmtvk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gkzqrtvz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2orpmktle.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jrjzanht.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2msrovqzo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wrvaajjs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nmyybadl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kbgfuscb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cuelfnca.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rpqfpifv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yytkifya.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cebgqoda.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vdwwukdt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2miimgxmi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2iipayeof.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wrmpcytm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jokymkcl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2uotrpzjd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2akbwpvoq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2acrssztr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ictznqyf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lqeuqkgz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2mpvceija.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2puheztuu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nzyhbxow.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zcclhrkz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2awqravqo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mggcymkt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2lvfrtzjt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zudrsaek.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2doxlhlmb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vdbbypwp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2klfnjrvh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qvlbkngo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mtgjlrpt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nzurnldh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vyelryll.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xylslpcp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2evgreawu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wqkpdtfx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xeayitmu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubdadyry.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtzdqvcd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zskbeyup.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2khzvrmym.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2glifcvmh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2lvzekvmp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2bbgwpthq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vonpybts.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2bjurrgxh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pgthgxoc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2itkbhmpw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cgpsktkq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2bdalndgf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hxlquaed.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkzsgijd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2soosiuvx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2slaxvezf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2kpnjhyqy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2plghvtjb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2dwxoxgxd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ejrltjxm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mvigsdbw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfigzozy.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ygxnvuav.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pczfipjs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gkngmnci.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2iibxdcmg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fxqmrlps.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2yzirqjsa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgnqcupx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ncvqzylw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pfznokdy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2veqrkrjz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bjhsrpce.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xrblckxs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ptncvoyo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2cazrenfn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bszhtjpk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zowikfdp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2dztzgfws.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2creqfaar.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jxsxoyaa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qmubrowa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2viitdfpz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vjwwvzbc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2clyvygma.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2abrswgho.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nzfkujpc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2znllavtp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hhwbtmda.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ckykhjep.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2libfcxoa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2satsoloy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hjuxhbdo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zqwyfpsz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ccphprjb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2txcctpvh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2irstlhwc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2siyyszis.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rtflqzle.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gpmkcsxf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xaaadcqx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uqfxlref.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dzvllvol.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kjaifdsm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qgcvttfl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kpyffpwq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fwpisurm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ahigbzuy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qnypljol.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2chcqtdgj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2mktddbym.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zdqwmtfi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qhcminhk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2juloknwq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2frtoobqd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rmspzehb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dljtyjrv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2exobgnti.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nhtpljaa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2chhmrrts.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ezncmruj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2goeiajym.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nxopomgk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ensfgzkw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ymysyeps.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ccgzicbt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2niffpijd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2doiqaulb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oeebdjyc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2epcorwqf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqewynw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dwdymurq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2yeotabtd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2umbtblaa.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uzcavbaf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ggkoljja.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2igibgqty.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2icbtngck.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vvstrmyj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lkdbtbsa.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2rfrcfyxn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2cjqxhihm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2weihkxmx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2gwjwgomr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rpsimtus.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fgsfzktt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2nkwazgcr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pekcntgq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2glejqttp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uchkbcmp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rjedkngb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qbxjmitu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2sktnqxwm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2nmpmjsmd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jzfqlehy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vyzyfssj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2lvbkcwiz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ipbejroe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2euipllgi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qtrzwjtd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2usbaurmb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hurpmnwj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kueyelgf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qcryytbb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrhubvr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fneckjde.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ingnqnea.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nwukeiod.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zeapnrhw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gcqkeztu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bsbuvmco.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xjvenjbt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ynrthske.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mkuwopog.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wuvbholy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2nrhkmdjz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zfszyxye.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jwqbvrpy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2acsxlbhf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2biikweda.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2myaigobd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sspofyey.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uuoaswja.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2azoqdtcf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wymsygtm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2irlgscbq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vkytylzo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jsobysth.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hobfmszl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2duigfstk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gulrypqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opkghqrt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qmsgxtdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbeflfbk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jdkkipbf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2wxazbhww.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2upmbwhso.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ttrrnuau.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kezqglqo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wdkgiqom.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nvavhwnb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zkdfrriz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rrqqczkq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fwwefpqm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2hdyganwy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lltlkjze.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2tdxqtcks.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2zobaeuce.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kueqqalp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2aujgbzht.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ifkisciu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2zxlreasf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hianeywd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hjqusvau.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vkxicrxx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oyahzhil.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sjhtsxvv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fgmlxfsf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gevqdrnc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2npmjunsf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ylsbgnkr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rudjmpwu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uhqtatkj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qjfmzwxb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wdidysgh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2voaodrnu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bunkpfvt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ntyruuwg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2idjyfakn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ihpzpnvr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vjsnpwky.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2cwsjrztt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ayxwzqdk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2hsgbpgsk.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xikocpwe.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hulivwix.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hjbeumxc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tosohqxu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2forixckx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zksyumpy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ujjeudwy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2bhlvdnqo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kwzgdshp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2bbaddwcj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2tgnyfmak.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2npyikuqk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2cbpygtio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2logceigo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2lyoktnfz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rnzdukpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmnnmfus.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2jwnrncpk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2bszefaqt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2djhmejrr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mdmqgqzz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ecxzguzn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2egipictc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2jcdqknst.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2swnuxtvv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2tvacxawy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hmzdxscz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2onlddbyg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2puizpeqq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2kdetmjxv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dtwyhgaz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bnfqhysd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2kilqrpur.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2xavytksl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2sdzkhzzz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2xhavrggw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2zcimxuyv.html


<!-- 参考信息 -->