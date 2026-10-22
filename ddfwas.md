代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2mwkdsitn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2fyanhfgp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dzwriuur.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tfombbnt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2brbhkzpt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpkukoa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jcpjvdqm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnyudjp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2aonfwzrs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ombgmwjn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vouotdvi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pyloeqcd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtbifloz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2fkrihtju.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tqvxwcwx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2efslwrqe.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mgfdvqgk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nivovbzp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rjpvunln.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2atvebijc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bjbdrwli.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2adqwvida.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jtyyuxpc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uihddyta.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rultngzd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lympmtsv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2clfnwzcp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lwxbujfy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ekhpwtap.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2aifvzgfi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2yhanexfd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tdmbtvzi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dbkqvhrs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nfkzxupe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2pxotxpov.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ztomxnhx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2uxlzkxua.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2aynimfak.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jpwdfsmr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zmcvhubd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2cugkhhyt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yvlxxlwn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gfcvzjgf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wglckqbt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gdotljga.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2lfplewfb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2uygpjvmb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qaxlgjgn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ilohamrf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fcbwtmbt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2cpbuotpv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rijxcqpw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mpiuflmp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ghzyvsrj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gdwrgosp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2npgawhgy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qdcxgadn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bkvbrpfn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dxbgccbc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2golatwby.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2diofvcix.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zrraausv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tjzaxafp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeftumrf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cijnvcfu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bvxipmjm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2wupimpzp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmvdenxp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gbycahao.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ygkvjuef.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fargxzty.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2feugxglu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2tvqpsdqh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ebjmivkd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2efdbwfsq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2bsohcjgx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pslgwmue.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xsphccdf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2buucqdwi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jogdtjsw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2urdszkjr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2osncemwq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2doaxezzh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jamtpstb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2udpdhzaz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2maofmptz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bvzimahs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ggcnjirs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2zheghwkz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2njidskjt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2utzxqipk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gqceomdb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zxjrsfoq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2txzhclve.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2logiexoi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2irtaghxj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2caxtjlyq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nmdzllfz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tyemevyd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sxsefnzf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cbvofsol.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ygkxsmve.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bwhsokav.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2krldyboo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2zymwvzhn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2oupntkcd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xhkxtcqv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lyemtgge.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ghbwbyzf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rzzugcys.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lfbtogwz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2zgtyjuot.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jmolpkxd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ejzmumch.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ubsocwdm.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lnpkvdpp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2eibxatok.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kckojzyg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dfsmluex.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jrvjyxmx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pascrgwg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2vnvhdmnm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qettmbur.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ybpkwwqd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2caftfqtz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rxhfuxls.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fraynzvw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2puloomtc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bbnaclzh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mxkcdomu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ttwdilmm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ryogqmay.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zynhuyqq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mgtmfvnj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2kczfcyeb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cgairedz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fovubfkl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2votpgekc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2sxzyniey.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lrtvtqxm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ceipqlae.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bhbluhwb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2uvlbscuz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2kcqrqzxs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rxzkmzlr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ezlxxjab.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dzjtyqst.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tevaknwb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mdysszgp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2nujedpgc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wroisuon.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cqmafqej.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hthpikya.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bqhaxwyf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fnreddbz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2labxzrto.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2cwadtrzb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rjpxmsee.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ckkuoheq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bjtoxjsx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ekimfmlt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lzvgdtxk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jgoahyra.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fblslpxe.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2frnzcfuk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jynamlsu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wnpxrcmb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2uqcuopof.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ojtysquj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xpwerksx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pflrotgg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ycwexeem.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2aebrasco.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ahksnicv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vrhztbfl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jphpzwby.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pyycmtgs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tgjzksur.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fqgxdlms.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2njizlbjz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2scoqyumy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bekcbxjj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dlonkayk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xzsvvkuj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2kmiqmuin.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qlvlnxdr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2gcdnxsen.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kaybofgb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tndjalwc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ehlbdhqz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sxkskgjf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vxeocuwq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2zagdxngj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zmmfsklz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rmdxbdwb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2elebogvk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2deekyqcg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tgiuvlec.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2fyicuqfb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hujxzeio.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2osobodrq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zrwvsfru.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2yrsrelxm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mmvyezth.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ujsmjabp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mvrlagus.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ekkmytmr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ubwsbfnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhoqabgv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rbzrjjqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcdpzcex.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xygnlyfo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tiinetdq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2dtdomhin.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tfrxqkdj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jhiihwll.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tiegrypr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fwnlywyz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lohxkhpa.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2roetanos.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vphdwjkc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2uxymnqqy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zrnexehx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2yrdkovir.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rjachrjf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kgpswwxj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2kcxelkmg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kwqqrnbg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zeizqkxr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kuuspaei.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ggnwjibr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ipswtcnd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2daiiiibq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zaearwjc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yeimozxb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ilexgzow.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2iyspgyug.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hvyvvibh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eaygxdwt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2iaeflzxh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eljubqdx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uktnsxha.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ywiamlqz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2toghylle.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pfqoxxxh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lzpgkdzk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ghffgpat.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bxvpwrag.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2sifvwdec.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2uvlqszwz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2uqpopoyi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pjuhadnd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dhozcjwp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cdbekxob.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2eronnfdt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lstxsjjy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2kpjduhgw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ukczcaja.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2iqquxdpk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2elhopiie.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dwjephqm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gvldewgu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2aqlgeysu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ozlmydid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chgrxjzm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2xqvupkzn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2luvtqihs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnzaltci.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2vrfhievy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2degwwbdt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2jcgripgg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mktuqnzj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2vedbykni.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pkwhjhhu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2tzvnwacj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2lctbfmeo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2lmtmswzh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2orcmlbuc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2dfamlndp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ezmvvsaz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2luwfsrqs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2uidvwaoa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2aqyvdjwq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gyttwbxc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2bognfrcj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2qkziaiut.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qduogccp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qbjjvpcs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2naskezyq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2pqextqru.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2chzwtpsg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evmwmmta.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fxtffjaz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2raqiohee.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lvsfchtu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2andgltot.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evpfjtwr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ijbajwdh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uftfgyvk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vitudwjq.html


<!-- 参考信息 -->