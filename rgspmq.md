代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ekrqabau.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrqyputg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2aenexofs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcyttlid.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ygotapav.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fvamvlbs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2joovoggj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nooiwrku.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ermytbjr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnzgkz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dgulejxp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bzwunwqe.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2haeoyxdy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2olzfzofi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tkfwnasu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pquzpkwy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2sscczdki.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2putnyezb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2aytxbxra.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jofyhtel.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lqlmaeri.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ilowjije.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hgfaajpc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zkvowbfa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccamsvfs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bwvendrb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hbvkuskl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gasgztlt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jclbojjd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rnbkgxwn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2btgcxjay.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uehiqffo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lejyfblp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2csnkcprt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ngjawdco.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gwkrkedj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ammmlllw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qaraoizn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kxexxynv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oemyuyon.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hnjygofj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2awwvuzia.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2atzmwjon.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rrgyccoh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ndwktpwd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wqypgfje.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2opqxaymi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pbyaqzhv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tmyjuzkl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2uguoxdqt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kojtnqht.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lqkwgtcq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ujmcrfif.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jlijvxmj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ukvtksla.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2apwymgse.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nxuoapyu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ioyghtkn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2cwyqchhb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uaopjhxa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2yjxfzimt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lslvelra.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2yticupia.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2voctnnnw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ydeuvxkz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ehrvpkul.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qugufcqr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eqbkzorj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ucnxhcnt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iegjyamk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mgsyhzfk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2fxfulyuv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlywaezz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hfimlpww.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yqlqacdc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mhhgbuxu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qifybliy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxiqeg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pydyhqew.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kzkatbvs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xoinrhfg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gvibhcdx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ywpbicin.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vphbvkbp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ttylvrfe.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2aldwllao.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rswafptv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gqwveuur.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2aarbsmyl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ycrdexxq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cuejypeh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2duymoyis.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nvaeyelp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pgppncte.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mfkafejv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ijoquuaw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vsgwzyee.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ijoietha.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qarqodrk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eqvawync.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ibewsbon.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tzpfwolz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ixtebpeq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2nxsorqrh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sgbajjdh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2gqktgqkk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dgfzjiso.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vyarrkth.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pmehrcdu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ejxgyngy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dwkvqkap.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jixpmbpc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vunvafzh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wianiypx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mjaommkj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pvvrqwrm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hyryzxqr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ruajcvxc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zdnujhxw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ckrnnfft.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gdzwxzrf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2sxadwnhf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2tcrzttzj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xkiwbfyg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qemvjbkv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2csjczecs.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2alxhbrtn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vikelpsj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wxmkgklc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2evoxgyxd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xzgroiby.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dpsdgbmd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xrdtywew.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jnaymzop.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2luiszwar.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sglyfmfo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2aujrovhv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rrmcvjlt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2novykona.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2yedksqzw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mqrqdfbk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ryndwluy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bcxcctfy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2zcmsjsnf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ekdqcxxx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sfgjnhlr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ujnbpdpb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ydxbmkfi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2prqjaluo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mlmphemw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2stqkvuar.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bbjeclpg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qziqfmep.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zztwyaqo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hvbrgatx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xdfuexjf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xvtfblzd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yweuzqul.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ukpqkkea.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2apinypye.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kqorswza.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2adpdxqnm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2aonnplhq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrxryqhb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2jiptszck.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ufwlsdjy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fnqlnkok.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oknvumzy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2texssktd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sjbeieok.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qptuxzjm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynzqfrfo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2tkgfjopa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kawcqogh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vkdqjxyy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xsmoiciz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wrwpzfje.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kunmwtgi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zmbunogn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ooofniwo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ikgmockr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wfxttplv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2fyjojlni.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2kedyujiy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wqomqyce.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wloiluzs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ecglhszs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bdmioqad.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mmhciehi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mwoqxwui.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2grhoglhf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2flqbtnfm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vcfjfkag.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nnoibxhs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vpuhwcdm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jpuxvqjd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sryijiqn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ypmqyqkq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xxbprnrg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vvtpakeo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wnhoiumt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pywijtoe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hltmgcpx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yjfeaznm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2gssfsqez.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxgpxpig.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pxpwpicb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qexrkdwi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qmdzgyvu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dqejtwjj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2blojzbhr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njeypieh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ivccsksf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xzfwhelb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fmgxvegu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zxqtipdp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2pslxhqof.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2phqfgheh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hfwkkuoq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ebioghgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wybcnbzp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2eqpphoen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiqnzkin.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dhamimjg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mwlrysim.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2enqpiknu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ljepusvb.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gomvbxko.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yjgygxpo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nrqlcmfo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mgzdyfgy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mlatjebc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vdbbqwyj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2iubkesnx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mbiluqwg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2whkhypwq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kblfvxnh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zouogqec.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2nthqoydk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bardkpsn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2axiamkzs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yjfprhvv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yjgofpfs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2tgfxcqer.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2skzwhkav.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ujlvjbii.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dperuxlt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ghsxmvdf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2oizbbcwj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2plcvaxhs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ydbrbdyf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ubhtflqj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ovjzarhr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kvyaqoxt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xzrigols.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lseohpsw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xfefyjdi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2oudlcgte.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hzoxpmvx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xrwkrrup.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2pvdkgixf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2pptgiocn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2yqyrftfu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ptxdvqps.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2zmdbqmzc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xebwoaso.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gzeqzmdd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pahzwtzc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2pihqotwk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2losskjlj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2apdeocgi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2xvjepphg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2twwawljv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2jxmvadgs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2engfobhs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2adtuvkcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfcywyrd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2uihrepib.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xuhrsrof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtakbtdf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fzgkqivy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ysugfzpn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pfnekyal.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mkvoczzo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mctkzcvx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2dhuswbhw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dlhuqizv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2itftuvdk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ululaaml.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lwjhgncf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2kcfixtfm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rueklpob.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2jgdfqlmn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2uovttpyu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2dojmqhpz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xvmecrys.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2zfjnokim.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2yafqmjbj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2txtztxjg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ezqbwmvz.html


<!-- 参考信息 -->