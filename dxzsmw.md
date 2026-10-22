代发 wailian999

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wzuqlzoc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2eucepeeu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ppydcgol.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kpjsrrau.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2looruhad.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cphlwajn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2juimlgoh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtxzzf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kgvbqugq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjzhnao.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hrruomyc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cojwpbpi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zifmyrpb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gffatqln.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2clgbnsyt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2eekhukyw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lplfijfh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zqmkladw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rsygorba.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ntqxvbmt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnzkbhwt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2sqjbwpqy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vsjpmyyz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ruiunvgm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xlmrtofv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2knpdfesp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2trlgcfwe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nyyilzfn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jivnylna.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2sceyzkre.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dohxehmb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2byjflxev.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lrpmmfrp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rokiwgag.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tcwqebpy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lzghdpyx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2auadevul.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jrxeubtz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nqximscg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dlofzmri.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ewdrubrn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2pjxoprrb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zkxyilyp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mgmumeue.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ecmsgnjq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2yglehppt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hcjpzoas.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbdffhh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2czqrdjct.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2osrsbrkg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wwbcetxf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rskpziuc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cbzbqamt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tywsgcve.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2sbhrojev.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2olcqglkv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gfthkkin.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2uxrmiauj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2eprdnbpo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hxijclzn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qirwalnj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nucjbgca.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bnxxenea.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wsdwoubp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2sfqadebg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2heatizpp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rwsjjrfn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2omkgstnb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bkeknjff.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hotiootu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2omilqzkk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owjeajmc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ngeziuen.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jgtuzzxs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vmjpfnvc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxcwhrpz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ywscexpo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2bvvhvtyp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bxgeczyt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fpctwzsd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2slerfqxn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qdlafeox.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nrlpqppy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lkuexqwh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zhgygvhc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pttwigwl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilzitbgu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iupniuei.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fpbjzzgc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ajczaale.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vehbfatk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sabwbpdp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2amgrbbrg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lcmznfbg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xsdpdlut.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ybevruot.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ckzarqnq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2itoswevs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xouxewsx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gpvbicdw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rbydxwxt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dnuqjogd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zttlvdpn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hjbsknsn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2oeuzzbho.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bqxtdpji.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dtudeqfr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2uqregnrr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2foysspuo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wcotljvw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pblkarhi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wlygxwem.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cwmbwtvi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lvpqlhqi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gwuvxotr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2shpghjmy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2djpcjlmq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2eguivrxz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2csjuposb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2iprvdzou.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rcdnbelo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gwneytva.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hiqpbrcb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xsmdriap.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2iabjrmuq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zvkjlqqy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pirqwyud.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2cghajyom.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rlruyrts.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2buwlwvby.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ivazomwo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2saetvcnz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ncpsqavz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ggxsgyzh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ysrxzbcf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rchtuzqe.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ocidyeeo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2rrojzuvy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2pxdglfgm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ssjvltdq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vlnxqxxd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2edeyomod.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vyrszwqh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2opwvgzes.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2zsggonht.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2dwzkohzx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ueqfwnal.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hffjhplv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dvfnoeig.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ucmjiaxf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kmnlsghz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2fflkjlra.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zrjhpuae.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sxxzxwaw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xsnamevs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gzafmpfx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ksmzdslp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2uvrjjxff.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lebocknq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2stxuigqe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rgswfybx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qcybxfpq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2efrvxvau.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ggzbebir.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ojostfef.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2buwqksug.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yaqnoweg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fztapyyu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2yqkrbgjg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ylcgeezf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ecjemhna.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2crihaqag.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ctbodptc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2zqrpjhfj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zpvuwlcj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rlvglhfb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wtjrroku.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fhezleke.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2leaplrmo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ttlaqsdg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lamqjwpd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rwzlsahl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lugizart.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2snjfnysc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dyukdyni.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mxkteekc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jqkioteq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2egcmpfau.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2azzewcgp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pllucmqs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2huiugsew.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tjrvvyhn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tvnwtulb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eliorerq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2egwdifjx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2lvziftdg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bdkjtnlq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rntuwwaq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2iosemppi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jxepffey.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ajdsprew.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cwgxcsio.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ldnqrtcb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gswanvod.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wgtnejqk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fxqayrsg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2laeybwze.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kfaoazde.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hiorpowh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xfbijtej.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pwnlrhdn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zbjxmlxj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ycoylage.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pphcexjk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zaexidgb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jifoiwiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2soyezshe.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mhqodyaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdsxdivc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ielacdwe.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dgjelppc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hkptceoe.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dgelcery.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2eirvunzr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2degoayjn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jogxdowb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wwdioejy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xqgnnvfn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wwrdehni.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2whbxnufn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lhhdkphg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xokwktae.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tubryfni.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2avkkbcdn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xrhkejaq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nfcbdzgm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2bsfbfmih.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aslnnsop.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jrbciypc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2cirnwdib.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xeycarbe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gfxmhsuf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2anoytuan.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hdikaiuc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2njfhhohy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qomajljp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tldegowt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rsuwbamq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2svdgjtlb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rwuyfkdh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2egloqwat.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jnovavwn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fueivmbs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ocjttbbu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2mlropbjf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wytayprp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2dcdzagrv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2heupipmm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2lmvjmslv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rfdflqwi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ggqfczei.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxesfvnp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2efmeexxp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2etgiaodp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2kkwasvei.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vaqdqwlb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ceyfhauf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pfetbyus.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2apomnukw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rwfonxdu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rgbshdbr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2yntovrou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrvertrm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gvtmsamf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2fjwpzpux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewenqpqy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2yeuitfsi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2iuaewitw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2dtmiuvww.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2rkyvtqlm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ccmyiuya.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kzvthswy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2oyaoqiov.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fygfphrw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2oqxqheia.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hbpjeeek.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2covaxqcx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vkxdnxfw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2wadrzkgn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2shwaywsr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2lkjtmbce.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wxcebduz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2fquxtelk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2vyuczmuo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jjpoheng.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2mwqxxyte.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dygkyebf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hodjohmg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iyynnree.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2okduyjij.html


<!-- 参考信息 -->