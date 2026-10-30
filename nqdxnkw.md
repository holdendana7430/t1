代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/ggipsjsmr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gluxhkntr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/ggxbikoml.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/glwfaiyrq.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gmfrjofpf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/ganpmxoff.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gevsiwthf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gvmbllpby.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gbrzgnorr.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gxbxnyone.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gnacrgmbq.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gfetjpoab.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gqtgebtno.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/guhozziez.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/guyoyvjjb.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gfedgifcn.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gsoqjylsb.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gjpiqizkl.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gaaxypabs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gquepcaig.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gjerrdsqc.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gcuwrmsst.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gflvhhgsm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/guvgyjtbp.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gzttigvbv.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gbfufrhue.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gwwwzilnq.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbldnaa.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gjneradhw.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gunnjiuqc.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gawhqxaok.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gxklxkddt.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gbjcatamz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/glfwglrax.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gdfsmvdnu.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gewyncjqp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gksukvhzm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/grzgrassr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gvulznpfc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gjpiosrdj.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gkgqyepdk.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gsqpxczwt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/ghvorcomi.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gbjxhggof.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gabtsjusb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gmmdtajxy.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gvdweriqi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/ggvvqhmoj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gepdkdtyj.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gsiinfzuq.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/guxsufyyl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gverahrbx.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gbmsmufkm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gvhjjgcdp.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/glshqjkvf.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gortafhzn.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gxzabrwdv.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/ghuktedcs.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gcgbgqewz.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/ggypgpwup.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/grshpfjjp.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gdloyefci.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gotdczrmd.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gucbblzvp.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gzlumvtlm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gjgmtsnna.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gszdlggkr.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gcqbvxyxd.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gfkquojmo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gexsxfwsv.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gatmeafcc.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/giwhfhdfn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gaymfuvxf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gfpngmoho.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gglpqzvdk.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gxiqnobdz.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gixhhojsq.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gaujhtoss.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gbfxycgvq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gaxhvryyg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gfqkyutpp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gnirmlrzp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gulhdxgvx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gmyipxoqi.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gjvgdpvzk.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/glaeuntrd.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gztrpxlci.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gcnzrjjvq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gyqdrgczx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gssyfblnu.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gpijshxbe.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gfpvrtjlt.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjafixdtk.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gsjsubhdx.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gtpmkdpjd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gybsysysh.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gvahabfeo.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gzkelzfxr.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/ggmpglpqn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/glhslplxu.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gmljgwxic.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gobzzflfb.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/glatxaihy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gubvkzpbq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gnyzcbbvd.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/groizaxza.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gkauixzmg.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gkwhioxej.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gpyobzlvu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gvwzvwwby.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gtwrhwulv.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gqeomhxqh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/glmyorcry.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gktazixbb.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gluycptwp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gdvwezuqm.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gbbtqbzno.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gdypqfyol.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gfsnwxmzj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gvklofrul.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gslqdukqn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gdraisyzx.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/glhpsjnvc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/glkkqeksv.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gqvpuaaix.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gfmwktdbb.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpnujjokq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gvhspbvqo.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gzetxyujp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gnbetxdob.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gakerkgqe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gdchmxoeb.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/grbkhjbas.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gugugqkiy.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/grndphduo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gldyziosj.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gxoqdjzay.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gmcbacclz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/glszvfwjb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gpuyjaqdg.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gnhafbhgn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gqpknfszm.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gnwmixnqe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gugeebhgw.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gzhrlrcas.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gutjkkpms.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/giiatjwxt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gioxscbhd.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gwtlakvlc.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gdukjomcr.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gqwzpnvak.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gexebxchl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/ggbsieysm.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gvwgksziu.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gyjbllntf.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gcsuvwhlg.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gpglefotr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gxizxhvqi.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gabitnnld.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gdybglhnk.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gqzbdajru.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/grtwyshzs.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gipzoplyx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gfaqtcvqt.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gfvqmxvjc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gymcubzcr.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gpgczcjmb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gpkdtvpad.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/guzuuvugb.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gfvzqqruc.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gemaqtfqe.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/grxnwsnfj.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gjcpmmigt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/givmtbygj.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gvhrofmwc.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gtdhfgace.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gilxcxoki.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gltdehmzl.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gcwucjqee.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gyfxtifxz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/ghryzozbe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gnckkszmv.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gjyxtkotp.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gmnzscemf.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggjhsxgvw.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gmwpfyswb.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gbfmqgpkj.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gjlgiufja.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/grvfbsigf.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gbwvfketx.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/ggdzsludm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gnmodyzxq.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/ggzsmjnbk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gzsltdfwq.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gspaildwy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gvggszpze.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gzwjgwwyx.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gzuveeltj.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/grhsrhclo.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gnqlecpos.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gxobvvgvj.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/geqvypezb.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gaodewcry.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gxbfcggez.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gtvhfvpmm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/geewifhhx.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gpkiupbrk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gnzsezbfw.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/glwuwijae.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gzdpvghfy.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gomuvfymf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gminabcqa.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gbqjefqoq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gpnflkzfi.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gdbubqxgl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gzmcqbpzu.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gclynufna.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gfhietppj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gflunzlls.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gkuakdgtl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/ggqcoirvz.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gtjqipdio.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gklttgmym.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gsiknbjrg.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gclhwvwqk.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqdeurihs.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gsevqwrnd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gmjsggvnd.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gkpjlumxm.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gvnawhlom.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gyolbzyvi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gipjrhgsc.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gfmdzxnrw.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gzcqecizc.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gutqdusrt.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gdbjmcztv.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gmxnzqilb.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gdqycocxj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gjtrcswjv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gjvtizilc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsqityzqm.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gongboptg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gytnwyhjq.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gttwmfcos.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gnseilefp.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gytroqmcv.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gyaucctps.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/glmvnwaum.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/grbmpodin.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/ghlopustz.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gocgpcjng.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gxmfeepca.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gmkrlmyxl.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/guwgasjyn.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gjivwadet.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gtqdcjylz.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gnubduxur.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gfyazjvut.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gnxorjtcd.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/ggqhaxomz.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/grjqtbguy.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gitlqhfsh.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/glwabnuwx.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gqtwwqcaj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gpouclomw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gjtywjryz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gsgjebibl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gvpsfzxlh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gowshdwvg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gqgtjhjfp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gvipuaraj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gfmjsrmii.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gyldadldt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjhuvoriv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gqdugwlss.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gxltghsrd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqaxqunjz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gscyafnsr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gmetbuzmm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gublrzvqu.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gqjhfvmpr.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gqnigatkn.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/ghiomcrne.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gjpsamhcn.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gsjhsaokq.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gidppwsnr.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/genyisxft.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gtycghmkx.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/ghisyhwsj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gdoifjdfj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gfjvvbxwh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gedmgcxkh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gsyfhqbzd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/ggqrpykjo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gtzaympyj.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gyrtfzsaa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyeyrlaog.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gqxpeoenu.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gndebfxnr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggjzyuwvb.sHtML


<!-- 参考信息 -->