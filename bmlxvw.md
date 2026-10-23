代发 wailian999

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3uzfxbmxw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dlipwzgi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3udekbbje.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3etgurlpv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3killkabn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3liyscdnw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3flqjsszt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3llmhhhou.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mciqsozz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3eshrplzj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3byuojtqr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dcvzslws.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nrvabefa.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lpstatkl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vjfeuhkl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tlniovhb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dtpselsh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ypzfkayv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3topdewsv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qxysyhtb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3suypvczr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qgulennq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fgdyjimi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zajkqarf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ltsqrkup.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3qryeakmx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vihubffb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlrbnpd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ingpifhs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3kgghkjfr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jpibdhsf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3weepmtfk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hkziwhuc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lrkottmq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tjiqznaw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3imtdfvwq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3nzidkkxe.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbwmnzj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wsymojjj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mkwqvybf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ijckhesq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3toxhutgu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bgvgkqkq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wxrfvolf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3agexxlim.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xnglqaik.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3btsoizff.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tamposnt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wmtwfhhy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3quffjwhk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pfdiezil.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xbgqfrpn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3iriwikor.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rzebqifl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wkrtccyi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gstwkftc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3leargsqo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cndsfaok.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gahgbgth.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mnrgpyqk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mirmoauk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xhcuvzdo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cngzbrww.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3uzeplbwy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dyigduyn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mrhcfshu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xnbwmtwn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3shwjyzub.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hvcvoxxp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gyabwmaf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jhrnfgqd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fdhkkmjh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3brsdbmch.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hvmmwzsf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lsfdoysl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3kuojgeix.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bsgafhyy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rrpimack.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3akgsenut.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hrvuqyxq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3swnkgngi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3smsggiwd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3oqdkeqyn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tkmypjhs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3iomokkvh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bnbqfzrx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jybgufui.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zuaqogwt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qabfupnt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3oxwoeudb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hqtlxoql.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xufyvbem.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3slwjcqgp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3vmykhudn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3aqnrjeux.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3unkzjait.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qijqmnmz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ufpkvsod.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3comnhsnr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tgixknoh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gkrrnjse.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qossxvoq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lawqfhpl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ktagaxrc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bqmuusoa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bexbkhtk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dathsuri.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3himngwqy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dlnumcze.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3grlsrhpw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3czbsrmei.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mvhdatca.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qjetszig.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hjutncdg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3uhhywliq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3lyozskad.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jwcigqdd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3viyvhqgg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3awplhoig.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nsvatevm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3akfvgfin.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vcgzmzly.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bqrwnbss.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yyxtmysy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3icixjluo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vvapjnzd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kwgqltzs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ahgznvki.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ouxjobjt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vzktntjd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3oavimrpz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3agproake.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uqjydsgy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ovnppoir.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3buhhcycu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wdsrzuna.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ryiwrytb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fvyleqit.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dfjekley.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3iwxowqcu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gnusyuos.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hxlteszi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pojlyegd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kntigvnl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3didvpnfg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3adbtxzmo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lygwlarg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3leswahxh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rhkbeawv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3irzorhaf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hhfaujgj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ynxuzoax.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vfrlajyh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3amnkzooh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qvmrqkxx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rewibyki.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gstltbxz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3qfbfmosi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wkrkkrkz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zlzhnvvo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ejydfows.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zfkflwrz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vgyfcfna.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ffnfxkux.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3fdzklcrr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3usxghbxg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yiziosek.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tckkntzm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ziuqjqhk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wfwnhwsw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qvqmkcxw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3btevvcgb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dzncbemx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vekwzwni.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlzngdsx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tblczvks.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dbxdjakq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xxkyiisf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nvtognwv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zvcdlmhk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xaakjvcr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cyisgmhh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oukzsbjo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xebmimjy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3afrkjfzq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cmpjnzoq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wtglecmf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bvumkxyg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bfocjvyw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3nawferdv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uykydqdr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cnnqtsgw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xksfojww.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kmwepnwf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kqbmmnua.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pdlvttpr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3jwfqdtem.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vvtffjvv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qsddgylw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xeriktcd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fjvdenho.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kagipdeh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3prqljqis.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uskaaucu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3eyfwcigj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vminahzu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3covnhbse.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xzzyhsad.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vcjnpuln.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lwlxmdrc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qlxujajr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3glwszrel.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bowimntk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wkpnwgrj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcaoofcq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3upldtprk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nrlrwpae.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3daedojuo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xvznywhc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3mmmmhqaz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cjgsuyyb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zclwnpke.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lyskyapz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kecpboes.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3csxvlglg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zsgdsbko.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mzbojavw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3yugtrrqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgmfeavv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xugshsix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkjtkmbf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lqevjkkv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jbbjlkbu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vebwlsnf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gvpzliwa.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zdjbkhen.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ppdzdvjl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3abmnsqmc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bfqzrxpm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3sabtddpj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ysvijaau.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wvdfqcgq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qrsirlvt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wnknawsu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vanxvnai.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3owolhrkm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nzrwumvk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fjzsffwt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hrbajabn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dmkxzdlc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vtrgzwlf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3obvhjalt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nlhvjuve.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nhiklybm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lhuezppy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3flctpftd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3okeieirb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ohrokgjn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yxlfgsfu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3duepcsre.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3piegsjqy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kaxmnqrc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uncujdmn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qgrczval.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dagjchfv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hjyodvvz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hlfybtiq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qsertbnx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yqxzasmf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xryvpmka.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3idcbudah.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fsjdynsd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3brpfxdmw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3upgnpibj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3exjtwjns.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3skmqslsd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3bwkxwyeb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wlmrlzsx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3euzeqgpq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3dtemygff.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pvbuvwnn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3mskdnpou.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bwzvwfkp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3egioykte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykshyzli.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3iuyduzlw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3wseyxnpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqtalilf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3daiwxoox.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kwatzgxg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pyslaimn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3upeizyrf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3tvgkabbj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3jngfjwyq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3rftmvale.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pcwqpwex.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vtcvywws.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jamwukyr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jsbaplak.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3lwpsdbai.html


<!-- 参考信息 -->