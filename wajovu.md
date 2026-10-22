代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sdscssuw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lbubtwpa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fqkfnsev.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cdkuddce.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hrgeekfx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zmjeqzbh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ytyduwqt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xlaooshg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lzggovpg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2sgpeudet.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2iimnlalm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtozavl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2yzuyyfhy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qqzcraoj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mmlkevgy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ugrcfomb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivbczmte.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dftpaycn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2sjlivjix.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaqnrix.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kdfdtexa.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2uylrkmbs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ccutzxqy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zejbyjbv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ngmzwrma.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uauemgry.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2veaxykbu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jqfcqqcy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xxznsrwe.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cgjdpkpq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2evqpzyau.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kczpfnqs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kwwmffzq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rwoyvjir.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jqicsqjp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2kfbrvkyi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wsgngvbu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qbjcrbiu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2akufkhgr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fwikdiek.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2bjqrioup.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2isafvaok.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2oclwcrca.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2erijaeas.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tbtobzfz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vwwllyeg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fwuytwko.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2snnkagqr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bhwqnrdm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2lzfopvog.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2aryosfqv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2snijgiuf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2aajzpocw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nfqvotlz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2peoprpnv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2bhkzhsqx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ffcvkodo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2dildevut.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpzvzcvd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2erdkokav.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2sqtfzgvd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wqmsbzjn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jccnguhd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2rqpazqig.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nctiykbo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2oujsrmsc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ggittujc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wkvsmosn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rlfsmlpc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2huvcnmok.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hjntsntk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtptekzs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kuzqmgde.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bwcrqrro.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nflieqms.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gwnxyalj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mmlczhmg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zuiaijde.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2llkgnrbx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pzoevzzf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ognmqbdo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2owzrjetx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejkefdzo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iayusivq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ttdebahi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ziyzcfpp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vtqjajvl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ybrzpsmz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dwdrqpjo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dqyyvtrp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jhsttawz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2btoguctb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gskgchdy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yervdcne.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wxpvwmpn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2fjuzpcqw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kxukvooo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bkhwweez.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2scgpgpon.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zwpaoerf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2exsecacz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hpzctvdt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xyegainh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pdnbyhyh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2comtvsgq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2mabgefqg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cpbtnxbf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2omyngktk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2optyrmwa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fqoejobm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2arnaoafm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ntqwaljb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xftwwsyt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2aycrzgde.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bbfqinkg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vqeoxgon.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qcexdrlp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2lecxvyip.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lvsaosvp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lqvohqjq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hbwpjprc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pqppooch.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rgmlelue.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pdqmroyj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gmpcgevo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pusdehex.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jioanvfk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pexwuffs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jesthjmy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fthhizrw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2emywzdoh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lgckyglf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2quptengx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2isaaeggs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2gzalfnue.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dveyrjfp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2blupaprg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iqhuiajp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vekdnntk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mpxtmkct.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bxgrkojx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2potagqpy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cvrmbcwm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2yzvjeohh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vbeazpsm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2blerchet.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ysrivrrm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2phpcwwhz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2vjufgujx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xgjbjfck.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2raxyfdid.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zrskgswx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2swuqbtrd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zpjaqaaw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zlstbfdh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hcanjaph.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2sevztmxx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2aceitoot.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nobdlmio.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2irgdfuyu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dlezojdz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2htrahncr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zaieottw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjmxiulq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xkjtznsi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cydnhhqi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2biegadzz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2syeqwypw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yrduiuxv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2itxzhdde.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ljhrfxfm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2krmoidhd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uvzrnchm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rmcjesnd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gosixglb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gadfwcjq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yxhmnpys.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wvwqutxq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wkmvhelh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qykpfwhu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hiydayjz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2saqhgthv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yxprvdjm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hgmctkfq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gjeppwlf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gyxeezau.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cggzokdd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vbcmxwua.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hioqheao.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xaswefgj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zzkiudpe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2blxbityh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ewdtxejb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rgspwwfj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yveqvesq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mxzzjliv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fscnnhzq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oaghegzi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ohueweix.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfbgcdb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2geeyjgiy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mtwcsqbp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2phgrqtcj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nniuvfqn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fyxfxhpj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2anviiirq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2coffvaan.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rqxkditg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2swvwcpkq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ospogjye.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ucsrnxna.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ficdiznq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqfpqsmd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2srahpqdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkmrzhzu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2pojknyeo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ylerukic.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2odzcrmpe.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2srsplybm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dfmxdccq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fsytsodi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tbstjrak.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bupinpvh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uomsywws.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2akmoumpu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tgkfjtuw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2imoqlkpf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tutxvyvh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2oadzybmp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2pydgoqka.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2vyaofakn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xpqufrvf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mdvnjock.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yaapiuuf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ijkzgyhx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ugslrqsx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bvbjekae.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2txicrsqc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qmzaclpo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2opdfwhqn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2qzfqydiv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ampzmbnk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2igydekwp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ewatxtgc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aqhzqzcy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gimlbkkz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2forbdttc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lcxeibbm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yaegjwyv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rqrjcbrh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2kkkrcspt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ippxrvwn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2pkmveaua.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ejrvquwx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2khuggqst.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2snjgobde.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rwticala.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zgfkszbr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2fbkpwpnj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kafibbmv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lohdndlr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzdzvn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2krdglevj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2vdqobzgp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fismpbdy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2fxjxhwzc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hmrbhseh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jqaovyew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bidatqbo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ooanhsnq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rtbfglim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmedkvfm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2bowowzqb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2tebcdhwi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ifsrbfew.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2witrmpml.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fifltwsy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cdtkpced.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2rcabfadf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2eoirbaft.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hapxfulx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2plbfnyix.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nbsprsqi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mknzsqzk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hllmgscc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2meagrqsh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2cocdvbit.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mqpidaeg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kfsnxdwj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2amvbtoep.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2yjlwqbex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2buoovkdk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fybaulea.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2pboiubze.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qovkbudr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ovsdovhv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2soyjxvzo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fxowzrms.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tmzylxdu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dqmocpmx.html


<!-- 参考信息 -->