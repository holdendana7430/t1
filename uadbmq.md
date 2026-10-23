代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3undeedkg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3soejcndg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xnsudsqk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3klaixqzx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3brlpmczl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3smywqwpt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mldsshbr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3blayunsi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gbilfkqa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gqunmkmz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zzwpiony.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3latpstnw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3igvttkzn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mnlygdsg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tlgheida.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nqqifwvw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rnbkuogc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3khuvqkrq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fijdlmxp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sfljoxws.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3whgubgjr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3dmpdibgt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qnunyfpb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gbcffyzx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yybhiirf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uvuddyup.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hvyyytmk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wwanlnjo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qspeeshx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3oyklkdow.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ucpyurxr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vamqvbdq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfpuksye.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3uiykbgbb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tzydwjgs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gixpiulh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3luwwrsjo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zxncqnms.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dotepfcb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wdmpzdzu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ancnmrco.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tlpnxzuy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ddsxllzg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dizbcghr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lcmducul.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zfvbpbaq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vnbaqhft.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tggkxlgl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3muarrger.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wjrixkcp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kpznerqr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3dblxelse.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wmzgdtda.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3revqssax.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bxwugrhj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xsbjdpui.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ovqrafrt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbvkabo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ucpeseio.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tijvfeou.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dscemyat.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ifqzooea.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kbicpujd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ppxwqjsu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lchlnyyh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rcuhpgtu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cszysben.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgeeprgc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ivhauwlu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3idchmyfl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rfodrreo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3culmewof.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eoitwzcr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3vbqwkbhw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3cgpdptsz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kdrsmlku.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xwipipzc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3npdvcidb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yklnbuxm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3suihulrl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3suzjpysb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tckkdacq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xxauwyew.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ujffitdx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rwhljqmi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ernkbrnr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ofyjbkfg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3frblezii.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ajkcyrao.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mjfdzold.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fyuvfaqa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ytgzfifq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hrkrjdnn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qmjdbtqq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rqddietq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vfbjqvvv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ykzirtnm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oabqcimt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vijwjadl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3siaakxkz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3monnxjiu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lzwabqrx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ppeshwgx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3watjpfvd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wpkoklor.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nkneczku.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3awznuaoz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qvhszdnp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3usfvsygd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jugdeyud.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3otblsilj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3jsxqnizk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3kapuleij.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nmkdcujc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3setsgpoh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vssagiox.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sduhummi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uydtgaxr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vlhjhxuq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3psptgjpi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3paqqihly.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3natpncwa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hqkuwnqy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3srgxgyod.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3hmrwsuga.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkuuwtnn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ugrixifd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zxmoxoio.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rilivaft.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uoeglcpe.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dlrtlyvq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xlgrdcxx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rhzkpnev.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3pyfjzocp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ofcjpigb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gortdmdu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vtqdocti.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rwgmanel.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bcvjqdfq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zswcrzsz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qpwhhewd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3skmpbdpc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wvvbdiza.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jhsobmoz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3aulsebly.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3udlfehfq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3idinfuvy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3kmwxjmjk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3epelmvnp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zqtlaube.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mhricmzp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3uwhcjcmk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3woseresn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cgnootyl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3cysiarmq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hbhpwzcv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ynrxyhsc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zgaobvcr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3flxifksf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ghhpirhl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ocxpaqxj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3werqhtaz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xbrjjdef.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3japrhvng.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gmcelbvy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3swllompy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ogptehgk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mzskqchf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hsofzfvt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3mpyjhktn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cfrgfmbm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhvqidj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3iblnmpls.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3xmpvvnur.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cygpowlo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hbpllvvr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3onamedbr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ubottxat.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vnkdqwpx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3upfyubkm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rpcppcdk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3isuojlzh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bbjpfcrk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3evrhlnsv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vppcfjhe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3falryizj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rfnitczw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vscmtihp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3egtijkct.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gnghbucv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3sofquxpf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vtdlmrfz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qzddklsw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3bzthfsrh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jrmtufvl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kgcnokue.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kxljuhxp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ljydbkxl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ogjhpdjt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3lpbxvung.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qdiakjix.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qiihanma.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3atyrbtxi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lvvnhuxb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qmpgqzkq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3snauoakq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3imvrijwv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3efqxljaj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qpomdyht.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hixegpcr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fzoqrexo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ybyxojcu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3swmsshco.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3imvomjob.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3riemehnr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rupaqmmw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dtmwydbw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3paqldmgt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3oyfwlhgc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3xmxwjngi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vwwlccap.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qeqswujg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xukteovx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vbggkini.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3egvbapmd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3invvaxps.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wwjyyuem.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ggmhggvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlkfujds.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3azcxraxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsytilfm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ajxsutqm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dheyebgc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qnjsalmj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ovzytzeh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kkivkoqb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wpchqpgl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tfyhbmsx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3buajmmbt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3uqydokqw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uzmilkxv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3pyljwgso.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ylbrjyyk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xbcubpyg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ksfhxgds.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mtqdosrt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qfhunvdq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3exsjphej.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wxjdyjvc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wwqzianp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3sqafjwww.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ffsodgqh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gpfsznga.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3plptzmas.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jxtahfsf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ephwxxqn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3wfnuaaar.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bydsybng.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ceekzkeh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lkbrqvjm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xsttjtxw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vhpxtrqk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qvucodkh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nuhzzkzn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ipdquhqf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3srqsfazn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ryymlznn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pnvmvcmr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pilqlufq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3nksakjtw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3igkbhaqe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3feqhhgst.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ksdsomce.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cgxykteu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qvwhmiar.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oecohemm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3pkzhtfyn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cerbpeun.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3yssynzyy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xjnkylcc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3dfnmwczh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ptfwkpdx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ighmpxfo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3gwrelree.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivazgbky.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ugiejsil.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3wgcrsreb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzkummig.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3euejxyxo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3klwsjtaz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zcjddtze.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lyqtuwdj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3lotdjdsh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3wfmcsrin.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3atnxqfpa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3yykyciyt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3immqqgvu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fhsvmwlh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3zpotdctv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3isyorgfx.html


<!-- 参考信息 -->