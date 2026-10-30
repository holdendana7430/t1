代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/glrfudubu.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjxfsuob.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/guvvruydk.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gxvwgmahn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guihvucod.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbxymgmhz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjonofkwd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkvkjywih.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gghrrqmed.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhoumlew.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpwviiqp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmqgjsqhs.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gydaqxzzz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/guoxnecjb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkykcryr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gvmfzbrhx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfrvngkm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/genmgutkp.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxnnaowj.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmyxejey.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpimadkfg.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxjrgmet.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgtezjux.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/goyfzoyrf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gkdfyizun.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpcmrqlw.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfowxmkuw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiiadkuo.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqvesbnbn.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwxhhmrsc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gecgelida.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvitcyurn.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/guxwxiftj.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/guavduaif.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/grhjuncxz.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gpjzvpmto.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gakgngyve.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsttvscyb.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkeuusuy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gwriawewp.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gaarijuuk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoaywaps.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gguhpxijd.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzggrmpec.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gfkdsfuxi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxzrsstz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gvybhfbia.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwczoger.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjjurcre.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gbszoaxzt.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxtcqauf.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhzkzlnr.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gheupkbsk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gfvdphmqr.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/guezzftwk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/guhtkmhmm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gctrvjcus.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gcnjbekvk.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwythqbu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdxztjbi.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gegpbzzss.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gdatgmldb.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbkakflu.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gpxrycaqf.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedyrhmvj.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gpvvobnfi.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gkkzvgnns.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/giliavccb.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqstjab.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbvrknem.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gttwrpbxr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/glcmmrmsh.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccscsjzo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gvfnljudy.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/glmtkgdkb.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggllvzpkf.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkzuxgri.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhikabyu.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gonewzdav.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gsltuqogx.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzfxkxrc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/grjxvazcy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/glbseehbv.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gtszodngf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxxqveer.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/govqbzipt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gothtswax.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gotdvtkjb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gdgitbtdi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gopfdssfz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gldmukcak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqijdujm.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghwoemez.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gxrlfiifg.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqyodcur.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gnbktwdnw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/goserqzma.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmfgxlyq.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfeiaudof.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gqspnjxuw.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwelmcdfq.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gzfnlnwdf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gjateotjs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gucpurjwh.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhwhmbxq.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/geydurcex.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/glvevgawe.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgvhbxhl.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeqcgacf.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gekfbfreg.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwmyliil.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggenqyrzc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/ganimnmgu.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvorerprc.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gbjvaeqjk.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhhpfepq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gishzfumz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcoeahmv.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyxhshgh.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbvoktno.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbezwyus.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsrqdrog.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyakhjil.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/groziimuc.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwclwiztp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gmlmpsswt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxktnsub.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlodexqf.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqaatbu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpvizogr.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpptjqji.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnzwkgyz.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gccbssxuc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmbbjpvm.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ggfmwbttp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gexaggrzb.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/guvvzogpr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebbuwrse.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gpcfnubvt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfrocdsr.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gpehmuoaw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtdpwxzr.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/giixzwbzm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzskysyto.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvamtdcry.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gtdmuquqn.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqvlawak.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gpzubbntg.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geptyluae.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/geinugyyp.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gropnzoxx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gtahclrmh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnewfyrnc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrclqpqc.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmxaxfgwz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfepkbqz.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gbvsfwkyi.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gpjghdwqh.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gewyamnyx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gfaonrghg.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/ghuqexgbw.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gnshmvsij.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gcjrgpdcg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuakcfis.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaqodmgl.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gnrkpyzuz.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gdcxqlkff.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/giiydfshs.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gktgniqkk.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsgaouv.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/galtbbjzj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbaanxnv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gifdboetq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gyglxzeoe.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgftrhzz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fanxiaobao.xyz/Article/details/gjctcpyvl.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gqushqvxr.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlehqvsm.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gfozwzmqb.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggocsffzd.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrbvinql.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfiohfzl.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/glogqytxt.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gohvlztsc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcnqufxo.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/geldsjqct.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gykgymoco.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gprsbzlgj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gelrbcigv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gdkgdnscn.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gzouawils.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpltdprsa.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqtsiynfs.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gmolcaaqp.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/guuriwniu.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gwojtujza.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtnndeeb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlzxaaqh.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/grctwfwzy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gashpkvnk.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gpsigzcgp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjubvrsub.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ghzmupbnu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gvghxbrmf.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gxarpjsac.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmkersog.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvlaaofde.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gryujrgwa.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/ghbykhnni.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/garslaavb.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/ghvdumbca.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghndbpfqk.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gaogzsotq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwphozoa.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gtefjqmcf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtdvdpru.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsqjthui.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjdxhqujo.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjcudwtya.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gqfhccwvv.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gbflejzvx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gletiwqjf.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcujqqynr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gqreouuqe.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gzroopolx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtykxcyhb.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glavpempx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmcnbmgl.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwjvrlci.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfxkqwqj.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gyyhvvdnx.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmldyayfm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxytbcabo.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfdhdlzf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/geotgnplq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gpqovgqmy.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblunqixy.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcgewlfx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaubdspqu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gruqpyvdy.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwcadilw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gcpvrcnsz.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gjkeixuew.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gyqqnaziy.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/guiolwhhb.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgnxegtk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gcetqnfla.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gclspcmrf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbaxzltb.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcpjfdmv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gntjhhjlk.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gcdroozpg.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggggpbrln.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gdymbnems.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/giuwmwhsm.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmddveja.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gwinxkbvs.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwkffzode.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcbuovzp.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gamikpwzc.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gihdlsnsu.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/gbqtplggh.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcfghfjl.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/grzuzlqas.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gyfjliqar.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoxiltfh.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrhmnxxp.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkiabxyo.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjkqjiok.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/govuizcdm.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqoagwuw.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjewdzgsm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/grifbzxsz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gerivfkei.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmfrugbd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/genixhqdg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gjwpnmcgx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/glwhvvhli.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gcpldkvhz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwrwkxs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gcobitqgl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/giydbzysb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/giysidluv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gevekzqqm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpkyejto.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gbymuvsnv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gjmabbgsz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gjwqlvaep.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gxjxtdzoc.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/guuznoxgy.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/grzisoeez.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gemiwoukd.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdorrhtcb.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzbihpgw.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gpqexjkmc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyzkuzgk.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwfaftqh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyuqzgmd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrtxqihk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gitauvgue.sHtML


<!-- 参考信息 -->