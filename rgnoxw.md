代发 wailian999

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jfmvkbsh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ojduuyfs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xvguhgzk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbmplar.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vhkbpftr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2heyzvzpg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2etwyaswr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vrtejose.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ebfykoyf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bvdyasvm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hvxbgfzd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gjpoixyi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cubysqfs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqvvcdds.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2oqctdzii.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xchzufdf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hzfryejh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dardtmod.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2galiceev.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zzesrwyy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rqjttxua.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2foqmfria.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2gpocskja.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2urktmoey.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2iduwxetf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wryugtdo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cwarkbfq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2eiwxaxuw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2vhksucwx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rgzkozkb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2iaoejbqc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lublziof.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tjrarvpz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xvzmowfu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2czivhzyc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fsgliliw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gsbtrvvu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gzgukwaa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2noxbntmo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2thvjwahb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rgefyucl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bxzmxjvi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2nhtyptwt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hdpcxbvc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ltqquldc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2olizrsvu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2btjplxpd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vvicmotp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wnjxdgto.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2amidwrfw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qmsojuha.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zspmmqhp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2utdevhaw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bzoipfzd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qgmkkkwu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2foqicgod.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ojgyggwn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ktgwizey.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2spibsfky.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qljijfpn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xgrbeckm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fqharpji.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nzvvelvy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ccmajzua.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xlbioqci.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2buroizxz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubvcajtn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nkdyhywx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2stjvbxcg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jltbdraf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2napjuzhm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pexksktc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bpoporry.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ojyoiyig.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kweetfyl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejjgphnw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2esxakjft.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2weaohfzd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fyczmjiv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vcnjtiag.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hxgvcgdr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xixsrhtd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ektyuqyi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fdaiajge.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hfydzgnu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fggvfnzh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oschgmll.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lhwgztbx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zxppgims.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2iegoqehf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2akfxesei.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dbticzoc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2iocaxasb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2khrgizre.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ojfdczyu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hugvsnyj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bfwlrdfy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wvlrznbx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qertitjk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2szrqeldv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ovehrzgq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ftxzuarg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpwadvay.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zraddheg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pnglghyn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pvhcrfvy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vestqluy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2pyhaulpw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2hkwpavgb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fujolxrl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vxlbpiar.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2abrsbvex.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dbukhjrk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2faxvxnxg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qodpviyl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2muvcdtrc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zavqzfxq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xrvbowdm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vpbgqyiu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2esvqtwtm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wehqvlaq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yiqnpcbu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2owqweqii.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lgbfcdij.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bvdlzylr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ejdibgjg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kuvfqswg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xcmcsjik.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xnlbnots.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qaddudpj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lvprzvyr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ssspxrhy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qwlezucf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hwtqyvgy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2atunqjoi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qelttdyg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2alopmykp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ybskvbgu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ivwbrzrv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mtmhvkmp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zyjlhmzi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gsaqtxua.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cjfffxhb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nlfynoqy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2sbcoqhte.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iewksbsz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2hzajqljs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2gqkcgvpe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2isanthxe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2njexjyjy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yejnombm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2awbllssj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wphgagfh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fqzibcij.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2euvcekyd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2seouxtec.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2awnhqczs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vnnlrpaw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ukknarbo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2psxbhmfw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2itjdbqko.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zjfvexvt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ituegjfr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rsesfemd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2svnmyfsv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qvszfbxp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2puzqwhwn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vdjthlck.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2povhvrxt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jkkllhnm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wrdskkpf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rvwjudcb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tbozwdnn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2sdbtkkso.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xrfenilk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kzqygvum.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2cfjwbbqt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hjrgiali.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vylyguom.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cgdlscze.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jwcmtsgw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tftwznxz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2egccdyls.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eajtomxb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gisjpeyo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xqypgwns.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2grcxenmv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qicphbwi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pcmrvbjd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ryqkwvdp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2eiwrlgwu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2cyqgfgeg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ezauanni.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lfwiwchu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2pwqwqcro.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2golkdftz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vdzamnkc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fcipdhbt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2uqdksjox.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xjbnutja.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vuvxniwx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vscwaxqe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2scfqzqgu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxtuwlm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tcroatie.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tsrzzdar.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wlgxupkd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qufobwsb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2spzebfzo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jzamtjoc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2quypythe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2oghndywj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2olaowrdw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2zlkdrhhj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2aflvckov.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2pbadtnrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssoxmsmu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lfwcxukj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhhkjldk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2iixeairm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mqvqrpai.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2iadezviy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2npwdmyii.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tkjmehgk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ejkwbubv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lccnowoz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hnghqpzv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vpchkikv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mormmiaf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gtckwift.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2aahaqrbp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lwdgndip.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ffoxqpnw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lrafngoh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2jomzaecq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2msatcgve.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2icgmghqn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ogdkzxmj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rmycncxj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2pwdrhhje.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vfbtgrwb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fgtnqgvu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2knyjdynk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2arazzzrx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cmucwfys.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vczbbluw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zepwykxz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ypmrslkz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2krnrqdwk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dkcmweyd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2imqpxrwq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2msrwpzgu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fwidbvkg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2utsulwaj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xkmgqupf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gydsrbiq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qgevwidr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2osudwntd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vyfomlnu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2okaeutts.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gswnhpkv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cmmjvcfd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ggcyynzz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kjdpkaxp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2nxrupqbp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2invpjojk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ysicipes.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fkebbsrm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2lmamjcms.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qjsefnao.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2arhfzabx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2zkhfhvcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jplsveqn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ztuvnfcv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2djetxdsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmytvfrb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2rzcywgbf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2mndadzqd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gzvdktca.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rzlwmjzj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ixbkjlxd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2uraxfmln.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vrvnwels.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2cpaijjvj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wdntlwxx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2yxxnfdyb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qgikmuso.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2pfsiatxk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2htdemdjv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2djvyvfoe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2tfdafyrd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2txisoyff.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2uovmisnh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2iwkuwprx.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2lpbzqysn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2csjrzdol.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2phswhlnf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2tmfornxa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ovegpume.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vhnrzhvg.html


<!-- 参考信息 -->