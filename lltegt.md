代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2emgetthj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2adcjeupp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2femsqcis.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jbajzgcm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cugdhpfg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2heoudmtd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pyiqjukq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ikirkrvc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2uvnpvgnx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yxfofqzj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vzanngnm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rcwtxekv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lrmbyszm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vnbdarhd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kmkazhfj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xmwkijry.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2mwiqgufh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pmdltrgf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kvdookoc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2btkeffhg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cbhoyfee.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jmrteqxs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lswttmnj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xidceqjz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vnehbdoo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rnydfgfc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qhlbjpgy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2memkyrch.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdovtses.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gohhjqxx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2gsaupeig.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ykckejio.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dswsttya.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xapewiac.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2dwxllqoz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ojiyaucn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2sbsxlhbp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2swqkstkb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2cptzbiuq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2noupocqh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2raleeakn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2nmvvalyw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2piceimzp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2typsxnah.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rfxpppca.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jdgxixpm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2csesnusx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2sxshsoik.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ghdsomho.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2cpfrtlll.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pnvlxwla.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cedqutkh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ohcsfhml.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yqqlypuw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kprhloll.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wzmsjzog.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ctyrdzeo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2obhmdkan.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ryomlxlh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cfonfjwz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bolmqtwg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2iintbaka.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2sfcmodek.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fwysqxcx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2onjsrbii.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2pdyavofp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rbswmmoa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2srzyqmsv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2oohmbvth.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mcqhloiq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2txeskvsn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vvmwfjov.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ysaodegv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uewbehjk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dxvcrjhy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2iovezwlf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sflcbbtv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2loohcoek.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2swboxuhu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2brwpyelx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zduifbwh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2puifnbya.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zcqzzdse.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsxfuret.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hxirjqul.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ydtxyouk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ijyjvtpa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gmgjdxbz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nhvsncfu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lyoiwzgd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nbgdlmpd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2demrxigv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bvpoyers.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rzhlusco.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kcwqxvyv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tdkmccbb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2naijlzos.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbhvnitz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dsuughdd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2opkksfjs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mbckndun.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nheahhgn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ipwlrufb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tenfcliq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qrtyvrrh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqdnmgdc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uwjfnzej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2drrdkagn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xrjzxzwx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fxkjlgex.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tygjjvvu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lsnzlpmc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qyqhzfsm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfrbtnwd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kyertytj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rvdyrjpf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2akfstqfo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2evcvbttr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qtgxlksi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2gmpuqjaf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2enbfcdpr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2etohzsyb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tivxtwip.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gfomlilj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rivmwzeu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qnmdqgmi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qdkkkcgx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2eefydstg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dgkutznt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kqnjvpil.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rlectuky.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jqagbaak.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wevqqfzw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nfmzjhpw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2oemvkppe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zlglvgfs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rnxogalw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2lpbyzmcs.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vepttrzb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qhpbxgzp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qthhgbbp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2yqkohlui.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qpzgmcyx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2mubnoltq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2drreozrz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ygywzyub.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mrmapxvd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cefkiunt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2upiwwvbs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2iaweuyye.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mczzpcyk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dtzyimxh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2fwurfyib.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zrruikhd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ljfbftdl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ybmxejrx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gcmhvsro.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kmdaxgcu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xyxrwmli.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qectdghw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2bgcmguoa.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ynryiayu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bqmoxuit.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cfnpzyrr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ildtnllo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2tqgsdtzj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dumkiikh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mfstfozg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elpiitdk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ftiwkorz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2avotzlgr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ntyesoqq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2znvdrysn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kwkssbhf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rvpejzev.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2riwgundq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lrecuvpq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eysryrja.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qsvowuct.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2prtjoudz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pyqgylau.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2elxznruz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2euvxnxfu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ajqdwxyh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2izydsfij.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gyyypzhz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yygpqtop.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yeixkjxh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qgxazeez.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2smrcaunt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wrqqxjht.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sdjljldj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cevehjxi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rfdxflsf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hhdvamec.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ioqowwle.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rwokzisb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vlgmddyz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dczutjzk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qzfxlkzm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bmpyhefp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmsfatz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qbhhxujx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hzkihzxq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wmanfxrw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ptnrqxgb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dwszcgxt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gbvvpxpb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2imnpychq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2plpdarpb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2nfwzxsxx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lwakaorp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dnskvrbj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2scgplbxy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ewuyvulq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2adsrkepc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cjqvwyll.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2enqwomkk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wpsnusfe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vdgjsdqo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bfxmuamn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jrscjqjx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pbitavio.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cbhyulos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivjrfkdd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qtysfgvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sixqrmui.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2aazmtoop.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yeohkygq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xdshkhda.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wfshrctz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xdyzisjk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ytgnstyu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ergvdjol.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2peroaegx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vlqsrirv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2votudzep.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2iwwddrzb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nikoxvpj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mmqnribk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jcgfkpxi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ulnohqhw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cgnopiva.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nxdujxrf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2famayttv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2urfqcdge.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2przjrzwj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lldsbfpl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fxjqtuit.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uwxwvvvn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2htekmpre.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2snfpjczb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2voryfnaj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gigcoadx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2btwiogcz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ozixekrr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2npiymrmy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cdxxjhlj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fcpmijcn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xwckjlam.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dtrxbhdo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rciedkgs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2iyzfybbx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yblksakc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tzeesklb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ygzrkabx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2cphxldod.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rbhzajkv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2fihrupcs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2okkxatqv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2cbkfosyd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2godtmkbt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2uutbqxag.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xftlknrx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2fyxnwbjy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2gyuteyck.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2nhomguvv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2cowoacyp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ssjuuyee.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ftxkysmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftvkxspj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gdkaotpc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2xdaxnzec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnzthq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2enbidikk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2etrfstqt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2jluzkbqx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lxjkcgoi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bxxovldb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lghwlxlf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kwxwokvd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2dbxniuem.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2igulzbmp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dntlrydl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2uevkpduq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kxmmwjxl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2blidzisx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zkyiohdw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2eaggeucr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xytlksxp.html


<!-- 参考信息 -->