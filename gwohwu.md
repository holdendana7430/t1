代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2aimxputo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vubhaabw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2yrcnhovd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gfbczyxz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jvisbrod.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2liekyipw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kdjxujah.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yhvobwiy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2edyqkudc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lmqgebjn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2dyxyvceb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nsciotrs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qybxokyg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fjiqsqkv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2epsuhfsf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pcuyoecm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2oedsokro.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ygnosagq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jcxbuszd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2inclqfgu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rnkftcyr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2yqtmyzvn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2csltoxns.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sqjrynvs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gyytlmtg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wtfrufwr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yvdrkznp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2viphnphh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pjiwuycj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bmqcdmzp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ryiruahw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mfgbulwc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tnnqmsas.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ucnmmwrt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ydfnlkln.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2pxxemspm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hthqzhap.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gdcfbkbq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zmoywkrj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2sxegowch.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nytbqiii.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2kzveyyvw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ffuqefws.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjoiiwht.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2olybtcpw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ratkahzz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qvpmbezf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uhdcaper.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ugdjixbp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2weguzhqx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2puxyxska.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pvyqevrw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dpvwlakf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppqomqly.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zftebzen.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fbfedzul.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tinawwez.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fobrcoma.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2behrwlsa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cybdpbmf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ptgyerjm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nmehlthf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ceiswwnt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2oravsjrc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zcbephyw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2klohfcdr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2apftiphk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gkrhuwmv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zznutqrt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xbfcacde.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ccxexqds.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lsuatyiy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dluznhyn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rqubacvg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2usfdqkyq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uukqohad.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kmahwihh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2nunoptmy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2eyjkldev.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yzvravjt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2eiefgfce.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ttscsmaw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xcpoogjl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2wdlqtipl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2uiypovur.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bmtqrtxo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hqmyjwrx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gtbbknen.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2geegnlcn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qydvsdpl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bjxealcq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gzlkcysy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2iajcuqpy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zhnernzd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2gekbcxqc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2bhhdjtiy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ioatanft.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2bvgmjebt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jwvlahet.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ngcwscwo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gtwyusxj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jiprnhpq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vzvtcnle.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gxoentar.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pcsvuxsp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qtzemtnx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qkfsgtal.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jqwznnxg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xsnuxycq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cjytznxp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2chmipkzj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jbdwiohn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ticzcvbr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rbplvtbf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2poavtmwp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qqyrzuct.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xjxouquc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2lcvekemu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tyvwgonv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2seohftdv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gygwuorq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2lagarhhd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nzuwglxi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xbelgjfw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lugwceoo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qjjsqiok.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kfidmwsv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2agnkydhw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2rzsyglsw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iusmzkhn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nisbfjtn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kmbvytqy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mgwfoblk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2epqiwkzj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2eidqtnny.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rghhtokc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ufbzsndi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wyhvcxhr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wjrtsohb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2yucarpfi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2yowiljex.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kgthncgx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lhtdscgg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mgunfjzz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iybefaso.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xrmmgraa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rcwvixay.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2trjxjvuq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rohsbpch.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ihpgghmm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxygoecl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gvujkifo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ftdnpfcp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ygtpaqhm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2juxwuvxc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bmnlqajo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2knrcwloo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vllytyca.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ljxkvuij.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mekhswke.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ueatmfqh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dgjihrnr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mtfjqwxw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ucbtuypz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2naltwabg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ichnjzsd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2fdzmrquj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vmarrgxt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dkresdmi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2cerxieao.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fakwwjzy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2foeockrn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mmgywzuc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gkroxlrp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ujfqiknc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bxvsmazy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gyriuugl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mkarqdyf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nxnxifjt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fzwhfixr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uschsnjx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nnlpocct.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2olrxxwue.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2knydysdw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xzrknxqy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wovujfun.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bgpstwno.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rxqjpweg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2krlivczs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tbzczfin.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ubjkdctx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkbhwwb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2acpcslif.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jhwgqrzo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2iroqitnm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvnmitut.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2polixphv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2klsblsfp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ftxpebrg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ywvieebf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tdlefmla.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jgugsdrl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nbzhwbhw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2lbdwgxbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acaofufe.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2csasinua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agihlsya.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xgsktuda.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zvsxrrlq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2apovhaxu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xqugbxoe.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ouspumrw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cfrjxtuu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2byxntckl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tmwdirdb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2osmjpmla.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tmrzrrqj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ghiwspos.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mpnlkrty.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xykdzgcn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2aifxgyim.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dkacwwxb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ltslmaoo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uqcpefsv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kesvnkkv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ecyevfuv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2leerkmfc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kwfldqed.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qcacclkm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2orglpscr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xujkerbd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cvbesabb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2mqzurkzl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xiffemzr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lnxxlxuh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2savjczsx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ftmyuwjh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wowglgty.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qauouaen.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mxbramzd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dbwnakfh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2irpgrffq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2mvcfegen.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oqotlxiw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2xiklipfy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2nhjohuxf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2blgyjkpq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ilcbwpcv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2brzejjtx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hpbfxpbj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2jgjtfzsw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dwnurxic.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2xyckcihl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wdacbckt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2zmdvgslm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hgoaqdoi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jqooapaw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rxpqvcpc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2snxodqce.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nuikstlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alvgfgoq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2nznnxhmi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2qipvixrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qculrfaz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2wijrvvky.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2lkybssht.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2txfezkwv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2swkbgguk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2kpyglsta.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cnaizhkc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2atqyncgq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xdquwecs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2jyjpckqo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2nkwudsld.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2rtochrar.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2shkaqgko.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ztjxjdbi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ehlgykqi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2bzspxuon.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vnzhmwxt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ffxzlraf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2iksiteut.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ciwkvpju.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qxvtxunp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bwnkhlyq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2pjdzadpe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oygaunaf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrfglelm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tecgkrsw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lnkzxlfr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gxqrxvdb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bxkhjogv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bgaqiurr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zkmdelcd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfusabgw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgzycygb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lijxvvlg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sovxhrbg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zkpwdorg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2untcdmcp.html


<!-- 参考信息 -->