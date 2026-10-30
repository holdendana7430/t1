代发 wailian999

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gpwjhfwoh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gofnydqef.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gausealjg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gfiqzbqcj.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gmshnppkc.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsoakalng.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/grlfcbhah.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gpbnzdzir.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gvqexroiv.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gtvbdaxzg.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gbwntbayc.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gplsjknfm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gaypkcvqe.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gainclqhl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/ghykbsewy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gltrkzowl.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gydhpzgzt.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gtifyfzvo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gpwnkyzho.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gtwqkgqob.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/ggtqnhfaz.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/gdeiolres.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/ghrlnaqbo.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/golbjoyfc.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/glyaibvri.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gomkedwcz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/gwcptbzkt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gqoyxmxib.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/ghcwxpmbs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gprcukzfg.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/glwkzakax.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gvxbhtchu.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/geiomxxdu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/giksstexu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gfgatrywc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gwhpkwicn.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/guxlezhxf.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gxumqvjte.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gtsbogvsn.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/grpfgyflt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gcjrnrflk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/ggafcbrko.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/ghaymwtoq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gokecqbpk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gcsfjrdyo.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gcmverahe.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gcxpevozq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/griirubjx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/genspalta.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gnlwvigky.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gkmnysjll.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gnghbrbqz.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gdgemhodt.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gkrqiogxy.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/grynohkhw.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gcdydhsqg.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gkxtsvfqz.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gffldxsta.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gzheqenuu.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gbmwlazun.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/grgevwvhp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gbtcmgael.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gbbusvtpd.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gwvafcpcl.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/glyitcmbi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gnujqtsus.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gqfpmvait.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gyckilwal.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/glckwpgti.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gsobmqbnw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gkramcgaa.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/genzpbbgp.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gunznjxcu.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gjmgkxkmz.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/glbddfuia.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gxjgnfekn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gvmslohhx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gomhkkgkh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/ghzmbcsvj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gewizttxl.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/giivdwfqm.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gezliwykj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gmjwmbyzz.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/googaokvh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/grgzribvh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnqvovjwz.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gtnorxxsf.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/ggqdnwbdt.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gzhyxytaw.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/godstkpcq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gtnjhpnwm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/grxqviyjl.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gmxypkotg.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gfwvhlbje.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/glubcnjpl.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gioqsxzyi.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gwygwkspm.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gdpwzbjme.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzswmyygp.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gsorlaqne.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gkbbdfvar.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gkmpuihgb.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gjyoyhwlb.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/giaylmcnr.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gokwuhvaq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gczpruthk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gpauqcpkc.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gghbjvjdl.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gsnsadnxf.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gftklgqrz.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gbpdldrzy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gmxjyozkc.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gehtugifm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gawyhvoep.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gaklioojm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gtuwdsjyy.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/grkfiftxv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gokygxtos.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gwzqppsiw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gqavecmvq.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gynqlsvjm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gsvrdpctu.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gqkukmxrz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gmlljycun.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gctmtolny.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/guouhlqvh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gwzazdesg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gdkrcdbkn.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gzwzyxnbz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/givygruua.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gxzsxqhpv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/giedojgfo.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gkfgmkowp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gefyoajfe.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gcelokdpy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/glspqaudv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gfotuwrgt.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gqfaxamtn.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gzxacgtmj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gacvmcsyi.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gbwtaklgg.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gsrlnqgxm.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gfdxdxfuc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/ggqjievxr.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/ggpslwygp.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdoghrm.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gblcwsqpd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gnnxcjbwy.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gjfojbswj.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/girgpdiro.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gsvqklisq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gdbimphhc.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gsymcbpib.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gtkxahumv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gbbmbkgoq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gtwsokwyl.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gueecniva.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gpaqgstpo.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gxujwvjnj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gvzgvjthb.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gzgekgfbd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gbybrftik.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/grhxkxeve.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gggxiykpn.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/grkwccjrr.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gjelbycjg.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gpzduubqf.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/glsxmtfxp.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gfejvtooo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gcrfnledl.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gxdefhrrp.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gdatmcoki.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gwkbkvcvz.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gabzrhoxd.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gbimvegxn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gnafidgez.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gtrvwuyty.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gumheyxnx.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gennjmsdb.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gffsxyzuj.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gzgalswjm.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gxyhohfkn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gbbocrrad.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gcpttallk.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gpbcpfyqa.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gogfkjotz.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gdmmtlunl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gshnpejef.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/guzdrizhv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gydvzcswo.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gdcrrqakq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gaqxityeb.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gcqyywbwa.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gxfdgrkhi.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gjbmoyggw.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gzmrmseqj.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gesgznuvt.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gxvqlcoex.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gulbthrey.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gzdczjrqz.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gpponvptj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gelrllpqv.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/ggnkizhtp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/glpxvmajh.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gzeipiwhp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gywqacqch.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/gweadcmzw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/ggpfmhepr.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gbglwuhsu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gqvhutaid.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gwwecznzq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/ghhoxoysn.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gjnnehbnr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gefeosfzj.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gcahgdoqh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/giaronvsp.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gdaxjardy.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/golnelqvf.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/ghcmzdfrh.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ggcsnwwzk.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gwhpddgnk.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkwqlzxlk.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gxborilwj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gtfiuqzgl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gprudgomy.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gailjallz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gfuakmjlr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gxdnkrxit.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gvrrhxbam.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gwhjgmolc.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gkyhvjexe.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gspkrxxsv.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gnfttbjms.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/grquezfwr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gnakjcdyk.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gmpdjwudk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grhzfuzed.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gnkehdbek.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcqejlauy.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gtogttotx.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gkyxbxmgx.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gxvrmfhlq.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gsqgskvin.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gkuplhrny.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gvdgswkni.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gsqpjacuu.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gksghpzef.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gxlfehwyn.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gvrtpumjt.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gdgfflvom.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gzmgdxigx.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gzxnxsoxp.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gpdgjfdrk.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gkswtrqjx.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gdgzyzvvp.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gjbqxublq.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gdrdbmekl.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzyhdzmoa.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gpadlnvbw.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gcrpldatz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gxssnqbpk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gmjmleshb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gsuqtdtlf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gvybgzjgt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gccwgpvif.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gfujjetwl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gwjwonrlj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gfsdiovno.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/godxtqncu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gmkpqgymv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gqbmyklwr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gczbhtioz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwiavofyp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gljpnkrnc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/glgvsitxk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gyndgkvmd.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gqzccsgzk.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gbaharqzi.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/grthazerc.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gewytldqj.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gtvrrkolt.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gkhzrcijz.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/goskwqhrh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gotodjgoc.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/giuwpnynk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gnjhiknwj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/giwnthjqu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gdqmsykjt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/ghuvustys.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gwuxcvzfl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/glknywjng.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gneqbrary.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdjtlpyec.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/geumjrmqp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gqvkvohmd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gntxfjghz.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gqcphgkfl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gymnzapsd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gnhrpowma.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gtfibbfov.sHtML


<!-- 参考信息 -->