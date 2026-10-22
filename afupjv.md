代发 wailian999

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ptlryarn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wrguoask.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ypzudcav.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2komqxcvk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rrfrsrvg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ozfmdzem.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2rpdkezte.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vlmrvdwz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wrgospot.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ejiynjpd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qgldtlkl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2clpyoshw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ngpbfrgv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ygnirkol.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2esyyreng.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hozbqnwo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gzuwvtyn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rfcvcbxm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xaotpxpt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2elijncui.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2eptrtemn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ezvqzdtc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2swwcfebv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mhirbgqx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tysyenxn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ueqahmin.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2njtbktco.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2knlenbbt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2siwdjkqv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2sjifueae.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vzhgjznr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2amdfmgmx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lgbbxgpd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2huujcqnz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gzmabkma.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2opzhakne.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bethxbsz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2djjstyeh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vdgqtkyx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2byqwvckg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2svqvfbsc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2mouqtkml.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nheyksqg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2khqmwdsy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nhwbafcn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qysfcfhx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ghknddqb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjhzptk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2rbsvepyq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zrlmripb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mqgesexr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ziqumcda.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2byizfgxx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rqbwlimy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ewmdhxbe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2apzricev.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2soywrpps.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2owyujirx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dovtgecu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ktucafoy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2abzsqcuc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ruklgsdc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywcmrmpz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jsozeidi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bljykxup.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoptoaeq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2subsukep.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2teopzvne.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2uusosnjm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2lqqcqcwq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2chbtovls.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bcnjyzvc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hbgeyddr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2islnyrdq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zvvgmszc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2eybdvkxp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vqmefogu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wvxzjihn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2orxixuhb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2suooryga.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ogyktakj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fxtcvosz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gluncjyy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zeunudcc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ypphqeha.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2otrcrhig.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2czayzkyw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exvruuef.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uwscylkl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ndylriff.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ejmlnont.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cucghypi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2esnngebx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pzcibtjh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2tnyqqulz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rcdejvzx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kneqjhef.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2iunprmfi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2drkvrlcs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2nrtffvis.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2grtrxfma.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vxzaceww.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2eszrixas.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ouwutyoz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hrvgnezr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcryvhow.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vxqcnwpu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rthptqha.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lkjxuutk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nradfczb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2theoetgq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kuvsbjvq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qttaonxx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rnvjxxiw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2iglbsedr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jccqlrta.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wktpxtjl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oefsbpld.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2psmtxwzm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vxktjbkz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ixbzmkfe.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uzsrmlrc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bpzwpmkc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ywcmakrc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rzywuovq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pnipayyx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gnurgfji.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2uausjkvb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2cgrcuyej.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pdkvqwki.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pxeybnbk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qfssqcsg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jwabpkst.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2igpnrtde.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vtupcima.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ptxaghao.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ddcbsxsg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2grrigkzd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jvslmdee.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ybvqamqu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2jdvprbvo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pzjrmcsa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rvbkrlcr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2oxzofuwi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fahotfox.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rmemarzj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2flapfjnd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wmpbnwsu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fycsuymc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ejyypqca.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ttazzipn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bftrfhnq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2farjrmma.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vfinpbeo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qcbekfrq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gxvgdqhx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cpeieyum.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ursnbvdi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2uybytwmt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2twgkfked.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xlgkswkz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2khzkylwh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fbwrcyui.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pdouippz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kfvmlgot.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dfzhtvby.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2wwwzitcp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjfjxoof.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xskdccyk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2agsssgtl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2isxahpbz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rfefwesm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qeqtmuuv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2iiuzhpqw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dyboeyah.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2iqvkyuoo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2emmyxdud.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2iwbvsegc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2svpsnbdz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xlpiecgs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2aujzbcow.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2cstbtmlw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nykojnvj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xlmkwihq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gptdqpvt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xfkajpff.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oldjjezd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vruycklx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2obtvvgiu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cwlympmg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2emlepzdv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2scfkcbgc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wudqtdyc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uqlavdkm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vctsemwg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2axusmptv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fnhgatwo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2trmnvvdr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yrnvkgjj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mykadlph.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kkvxkdwq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gasfxzcm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mscupjpo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eqxizdxr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pbbnspnr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zhhbgmqw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fpalhujd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2browoqhk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2elnpcutz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tqxyzvdc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qkdfgiwl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hacmefor.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dmaavdcb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ofpoigty.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ypancbbr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nlojuvze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olmivoqw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dcinyqxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cirdwftb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2udqxhthj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sjbsanjp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2usbescvy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dspeeadz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nqgqtszy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xnudkmya.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bevpiugl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2puufjnpr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2esrppyvh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jguzdpen.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qtxazngf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zlbmubah.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2eczphdrc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bvtglwhl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kxrklzdt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xedjipsg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jazertsg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vakkkxhm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jppoyjou.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tqkjukpd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zgdokyrc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tdrsphgn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2apgddnyb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fldinjmm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xnflsjod.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2klhclefi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bzajgbsl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ppwxykkg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ijqmwspj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2meruztud.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vqbewjar.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nnvkspyc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2whoxuhnj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yciutyli.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fxtbjeeq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2woghjaxl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2usszxkho.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vhzbcrcd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fojvkbky.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2udfcnmwi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2empkojen.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2zxckfstk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qyzeqlqw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cghyqlok.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bbmmqngq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2gqijoygh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hwtxwpyh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cpmuxphd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2cnbkdual.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pzzlptqd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ifvffusp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vgpdnfum.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fqmixdry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlhvhexj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2atrpckrj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gyenpnim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adzdvwny.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gkegcexj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gmmslqur.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ikeaabvg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mfcyavvy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hpolkgtb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2dtqabjlh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ntqqrhyx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2kctqguyz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2amegesua.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lyxquqha.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ruwmnnwp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2znjisziw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ksvetmek.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bifjpfvc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ctocchkh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2japvmget.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qdcpolpa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yyfskopr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2gcfrydop.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ttpfoqxz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wwbngrig.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kxvidmwm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kakbehms.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jhlqtgnh.html


<!-- 参考信息 -->