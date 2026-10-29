代发 wailian999

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gzfeijikv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gamxqdqgo.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gpeypicwz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gghfkbuzn.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gukuojizt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gackyuldo.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gqpajqtxg.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gpboyiytf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gcgjqmmus.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gunbvchrc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gbmokcstj.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gurepirrs.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gwfveucoi.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gdcoltnay.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gprhcsyvc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gfquuvjlv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gfkvgqiih.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gxjkcaajo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gohrtlkfd.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gehuoqjyi.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gdecucant.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gzympwdib.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gsjnohsmo.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gmubhycco.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gggyljkgu.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gyjozvqul.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gmjcnieov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/genrsnrwr.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gpectkbfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gujgfazqg.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gdpgkqgmk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/glxwipcwn.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/glmpkvzpx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gyhydepic.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gufbpuvom.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gumbqjsir.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gdbvisoig.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gzkfbpiww.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gmzbtguhw.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gyzzwomxo.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gamaptxam.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gpptntgav.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gfrqnelsw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gwmcpuqyf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gacxgyvcu.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gjpivohqo.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gqvrjdkqo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gvxydcbvk.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gywczcixl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gwtgpmwjx.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gznerqswb.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gbfvmrnod.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gwcqbymeo.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/goczxoows.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gxxjqtqen.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/grkclzkqj.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gygfptvmf.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gezzoonxn.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gcicfmsed.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gsvkgskyi.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gohnwyhds.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/glvkkvger.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gbvxzpuci.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnugyho.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/ggcfzsfys.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gvktihecs.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gyluvfoux.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gkuofkvqt.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gfzzpqvzc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/ghgwlexcu.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gihazwyhx.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gnaurzpjk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gahrlxrwk.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/ghplmcoaz.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gvynwhdcu.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gukhwmtvs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gxhvhouxz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gntbdrgob.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gnsloaywh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gzkieskod.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/guyhzanar.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/glrnpehhe.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxboyedwn.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gxytdxacd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/ghqzsnyhh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gtlhowevc.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gofdwbssq.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gtupclzkv.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gzljatkuu.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gncpjsrur.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/geeyztfwp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glcdruhwi.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/grwncbvhf.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gpplqqdgb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gllwqiwqn.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gmsseyfwp.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gythkhklu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/glmiqopzj.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/ggfqormgl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gukrjxkld.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gqxjrnudh.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/guuemjugo.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gkgrexfpf.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gywbpxrnw.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gyeeqfubv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gmoyfaycp.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gtbeqofdk.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gvsfjivqh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmuxhvwgh.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/ggiloihqq.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gxcwuluiz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gxfpclsfw.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gsssoxdch.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gftgnjjyx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/glwcsmrku.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhllsaea.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/ggtqdczbi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghwwfnrtu.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/griuggfcb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gjtghbxtu.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/grkoklfgs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gzagzsusp.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gpbqypbam.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gunsldtkd.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gbluorxwa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxisjiquh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gaizlpthn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcwgyhyht.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gphxmgsjc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gbbvucsla.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gkfkuulrv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gkwoeywbp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gmlnatsyv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/geffjokab.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gtcaykbfc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gxuhkszge.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/ggeobvrkz.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/ggugbrevb.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gzbozbgjc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/ggcjlzqyq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/grdyqnjhd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gcitlbalh.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gduayochq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/ghrpnaaic.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gropkonrg.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gkbrmwkyc.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/guupqctdh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gwziylgtk.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gykfsdrbr.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gjxpdkqko.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gwfehcvlx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gahtofnfn.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gmqxpganw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gbususkla.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gjaswravn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gtmqeezcm.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gvhsthdjk.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gneeghbxv.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/guvmupmro.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gamlapffl.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gjmqytczk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gxlyvbdfm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gdywbquor.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/grfcilnkl.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gprsassqf.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gkppzwgar.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gbsmqxege.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gotymtrtg.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/grqpwnque.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gsxawzmqs.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gmvbxbkvt.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/goxudliap.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/ghtgyymfl.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gjebicjbe.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gegfzydbv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gcgonrlki.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gypadzpdj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gkaearyzm.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gcaszilpm.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gqkfszhte.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gafiuckts.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gbbejehvx.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gxktecuzk.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gkhfkjtfk.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gebqggpbo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gwciitkvz.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gtmyylmuo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzwypxpni.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gwhgijvoc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/glsjfyutc.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gyvosuvad.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gypjtfyuz.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gnoxpvwzx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gztrbkxth.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/ggtmhzwwb.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gcoamtgyj.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gehneueyc.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/giwniinpy.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gyukmsjlv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gmcdirpgp.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gtxskxseq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gvdhftylh.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gpihdrilf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gutgfskrm.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gonszbgub.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gpnzdqztu.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/guiieowjq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gvnbixxre.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gtfezkfpa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gmkhlnwbs.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gpilhooqc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gvsapizzo.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gouiwfmzf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/ggjezsdaw.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gvjsoxfhg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gwpvcldxc.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/grqumgzbk.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gavpttsil.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/grzjavevf.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gusrnwjhw.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gtfdixqav.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvxjytkiv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/ghfnnmfld.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gwhhgsfyd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gcoksojku.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gnqgrtlkg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gwreooavr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gqeheyzdc.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gapnqenxd.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gxkxyjrpq.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/grwexzent.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gyxerujor.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gohnjdzwx.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gruddlirk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gadyugfqf.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/glnznqbak.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giobdeztv.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gaqnhldsy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnmfovddq.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gcfqtrxjb.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gdegeqwbz.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gszaetpjn.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gdsnwcmju.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gvoimdmca.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gqwzvqvpn.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gmvomzdet.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gywllgwig.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gjwwtcjda.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/glmyiibam.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gzdiyatrn.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/glxngomyo.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gndlczxuz.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gbhaofcgh.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gcjmrquod.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gzofkdvqj.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/ghntamboc.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gewrbaryj.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjotovzuo.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gtnhnzfzv.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gpiuecfqx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gdaheukde.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gqndskdse.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/giwnifxep.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gsvaraeii.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/grvxndbzm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gymyrsimf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gpvrjxirl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gpbfjnmez.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gzofvffdw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gmdqtndxw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/glosslptr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmqixsftp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gwkgfbcbf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gycxttbvt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gpcxcfyby.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gzxrfgehs.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gtyvuhzpb.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gddziaudf.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gtqyxxdmx.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gbcotejwf.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/ggnqxdpdx.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gtdqpcjsc.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gynhnzksi.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gchwwnevd.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gbxnkakqq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvcfuoozq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gvdmicrqg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/grhkjeqae.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gaitaaunt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gxvuxcstt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/ggmnvgham.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gkjfjhosk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gquozoeyb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gzawosrwz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gtneslszs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdfvamlne.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gejlijdzz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gwdrkfwvn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gvukbzase.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gmdqwffio.sHtML


<!-- 参考信息 -->