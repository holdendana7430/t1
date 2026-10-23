代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bejynvnq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jnqbqfdz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qmlcckbh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kagyafbe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ckinutbh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pzjclgos.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ymnzvtes.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kutxdzur.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3knhvpsel.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3vfzqonwe.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zriywvea.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3loxabblv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lcevozpt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuddoeo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lzmnxwfo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cwntuvgw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dumvruhd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwpdcxoe.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zizkbnsa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jelzhuma.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3beolgnwd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rmifspkm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dypcivyy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fqibsetw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgmfytam.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qntqwfxc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qfsxdyde.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zwnikzyl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pnflmgdk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsmysif.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jutfrukx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hfkqwpnw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fghqbtcn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3srssnngb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ssziywdu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dlbkanaz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kmbliyqg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ahizgnyj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3chjlqvsa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mwjrzzxj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yhkxddzp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yctbwhku.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cdwjllde.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kdkusnba.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3uaeklmqn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fwxcatja.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ewxlosuw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3rahgoerf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fyfchixt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vekimoxo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3evrahlff.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vjkciato.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nstpmpxq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3haqcqivf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ahmkxjpy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zlvjbwvm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3hywjgdjs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3opthxdon.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fczzbxvx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ugwtddsc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hwgimhxh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qiwmqyvs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3edyhfoxi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lhgetmub.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3oitjteob.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3fscqinjv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vndaoidi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3eetzyhss.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yzvqekgt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qfdfkglr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcaghbka.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3esibnvut.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pzmvyrff.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3swezmrqw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wrymamyi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3loutxlhm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hdfjfdlt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qxnyptyq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fhwqtedb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wewqxhor.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3axezunob.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hoyqgdtx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yrfytreu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xfgpthju.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qgnszfen.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bjsfyrop.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ybeytkyn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3owywetvk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nnzjcayq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3otdjupgq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yaewqeid.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dragbljj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fboedhgo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ilakkfvi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vvsxbjrf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xcrvwjxg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3sybaxmku.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bvrpform.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qvdrhyxp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qiqmfeuk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xetyagfv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifeiqqlr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3nofigfmj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nifsheyt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fytgadkj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3luyswzyz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ciswbbei.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mzhhfnfg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zvbvzwqv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ovhtpixz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jcqiectb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3khmclyhr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fpduwajz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mgsscmrl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mazupsqm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3oqxdwhqj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ftjflvil.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ykmkxakg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ljsvoktm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ubdzwpvr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dmmlvker.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3akxkxwfy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3azaxgycj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3achlhiqf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bvrtlvpx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rpptkqmk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppimcfqp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3brqrvndn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3sthmtbij.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dkuluwkp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mrxzkuxy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ioupajal.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kdtooyhf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wimlpngh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ugxedgwg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ezplzjvy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lzvrqtxq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dihfjngp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fbxnbzca.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hwpxfvna.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3revrhwoo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ofcnfqpi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3fnwafnfv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jvqotjqc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kzwernku.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lgoymhdt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jaozvlny.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3krkpcyro.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3cornkeng.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xonqvnzk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yjpgiwgk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3uukfkrvt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3txutjgdb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hekgrhhw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3irgywftl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3skthjwrs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3geirgxtq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oulliagl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ciewxknj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vshmpbwr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vufwzhvy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3oybwciay.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xpckkusf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vnzqywvy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3botukrmu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3xuihdbuw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmasftcy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3srjrmllg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dxjokbqz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ecrccqxu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hpyglspx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3moiodkik.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3kqbcqxfx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fclrdbvn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mnqqhmna.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mcweoqgt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3udkgouzm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hjndeuto.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3houpffgf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dtktodkk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dsjyrfwo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ssozcdhj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qdqrnofh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mjdesxry.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dbngvxgn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dzkhhwff.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mpmxfjem.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ufhvdfyl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ticrzcng.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qevhfamq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ippaiori.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pzltbljy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uaapnxjy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fflpnvsk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gydpcqbz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zigpchhm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3srxbbcvc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ooutuqqc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xfhmsucm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ciuontmf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vomyrnes.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bnedalcr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ptjmmypg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xrqqrezt.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vohmanig.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmtkopwz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xedikrvi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dxojtqoa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uzpadmnv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ddtnheud.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3rjakizqa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ysvyvopq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dfhnpawn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dognfsey.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3yuymgqnq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ybjajpcl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3qqdxalvp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3mlddysrv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bnbyanil.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3hxwswavw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqxsnxur.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ntlqxfwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3timwgmwh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hgqsrgry.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ogpjqosh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3djpddqvm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xmevxvgb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3spvhhotr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ldbzxsdo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wwojmkmv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dorbfuir.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gkdmmmif.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3vrnbrclg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fidqxaqs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ajzhnzzz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3xglwftbs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3eurkkfyk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xrpriqny.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ipekatnf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ihllozai.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hqsffksx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ywgbdhrz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3olhacecy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3imbqxmfi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nqufodnt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uiyozpqr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iciyorch.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jqwzfuaz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3fimxmtfs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vknukmdo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hnqrnsfl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pswqemuh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nblfuviv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bomnqkcw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rnahafqm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3camthlvk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dprbalvu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gwobyyjm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3pjntezsn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nqabnbus.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3gjlseruj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3griceaeq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ybatmpkc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xfmmmawi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3aqsyeiko.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xumxqlgm.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3esyccinv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eekcnflq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uqwmvqrf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vvlvturv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ndbftenw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rwnalkdp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kenevkjm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ipejfqsd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3mgasmwnr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3lpxrcewh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsgxtqtu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3bzzaqpek.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ldimliau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmnevnbz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3alaaepmn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3dmvnpvrw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vccvxszp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3isckwiai.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3guipwqch.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wbjyinrg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3adhzbepi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3owmdaroy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3yuhrvqiw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ukexlxce.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vmojvljk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3pqkamdem.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3merharag.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kjxiewjq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3orqusmau.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qspimjmc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3knwyiuwh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nnvmrqjt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3otdheluo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3qfwdgxgd.html


<!-- 参考信息 -->