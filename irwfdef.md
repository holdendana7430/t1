代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gndjcgqmf.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gjgxdsezx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/geswnburw.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gkelrzsbk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gpyahdqfz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpekiyiyr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/guxmobdnh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkjtejqoc.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/ghdnrmnlv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/grogjdbwl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gzljgsfle.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gurblmyoq.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gvxakffrv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gzipaiecj.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/glwzwdhit.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gbfbtdjpg.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gcivpxvsb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gtluomfcn.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gurqqceqd.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gbgsprjpq.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gdjqexbjh.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gxiojksuy.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gfnfbaipt.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gplyztncd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gxhrjjtbk.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gjuiekujb.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gxsidwsgk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/ggfxlzprt.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/giiarccwg.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gcpcrjkak.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/guxkrtwxr.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gkffduhnd.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gxoxvlwlw.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gpdipocyv.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gsplrtbkw.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gfgjocond.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gikvxoeie.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gwbudhabv.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gvlwoyebx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/ghhjxisjx.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gpvqujkej.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gcsdulgsn.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gpjukyfbp.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gfgrxnadb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/ghfyvhauv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/ghfwuqdbz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gfmixydnb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gwzumkooh.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gwssyisoe.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gqejpfzes.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gsufsammp.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gyqmkcdcz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/glvmkxrpe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gruvwkpum.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gxixhbnmk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/golohlfjh.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gflmbxsgw.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gxvhynlwm.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gadyclmom.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gntjkvomb.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gbzzwguhs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gttborusl.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/govrcspcb.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gyrfidmpx.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gxcmcnzyr.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/goplkvxpu.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdwtuypdi.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gnvbbfdib.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gewioyyhm.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gkehaxqfl.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gwifttswd.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gkfdhigtb.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gkjopvbsg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gmvkznatm.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gutldackn.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gjcgckwhh.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gxlhrqftu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gubrelmvt.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gktiwuevc.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gsgilthev.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gxqfzyedr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gzklpbkds.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gsqlpdlyq.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gcejbidbd.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gyivgawvj.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gikqrqijh.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/ghorrqmyo.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gbjnnfhnj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gildnjduf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gwgketrrc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/glmrbddmt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gpcbvbkyw.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gwfkdhcrx.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/grsbeiwmm.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gmqsoqfbo.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/getighbew.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gsqqjxjou.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gjbeedjtx.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gysbsyifu.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gbqcnvfwz.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gypkgjdvp.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gxlobygfy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gpbblfzon.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gjqstrwak.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gsnsggxtw.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gcdjypkyo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gvvvvjmsp.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/ggnsvlqcj.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gdijqnrlr.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gsywkytll.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gsrbavoco.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gwohlxbwo.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gyspiqolw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gxuwkymnh.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gdopaqljw.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/giqztlbry.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/ggdilvetb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gwnmlntwn.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gjfydjdrt.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/giemduhnp.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gbzchlrxt.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gzietnnmc.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gkpborwcn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gsudcwqzy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gcffusgur.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gfyvrgicy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/grtydofff.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gqxvhpxll.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gqpgphlwk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/ggxbypyzf.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/groaspcnm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gkuyprird.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gnpauaahj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gfosnujhg.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gybhsbdcn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gdgdbiaga.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gtjajygne.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gmhxzhuym.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gxmayeise.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gecimccxb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gqwsadtjp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gnexgpioh.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gnuocdcvg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gujbgbbcv.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/geswutoct.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/ggncgckvl.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gbtgvzjhs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/giwuujmhy.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/glvdnlkcv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gufmmgfdx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gohndovto.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/grshfesqc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gujtexsnu.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gnjenrqkg.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/goyffdbkm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/grshrcfec.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gumxmnvjk.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gjfdblwad.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gkwttnkxi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/guyahiffl.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gnmvkgubm.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gycydwrti.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gnkdqzrku.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/grnklytxg.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gfleuygni.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gvbydubkg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/ggvjfhoje.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gqvericmr.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gxbxhjuqz.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/ghcfygced.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gtiqtyhma.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gfrcbozir.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gzhbdotyi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/geuekgpar.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gqqbibmss.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gkuepyonc.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/govzakbmg.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gbnivnspd.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gemounpab.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gnpavckdu.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gmrnzvwni.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gcqjkmwqv.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gawnwdcbe.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/getevfvzi.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gxoczuqoq.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/glienqdmw.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gzwfivtar.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gncnhhshw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gxhrmmfbt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/ghgbegoqq.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gwqfmptgv.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gzqndeabk.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gxshhgiqy.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gilpkyrrg.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/ggclithso.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gsbccmxxn.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gxgkfgvde.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gpjrtrewl.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gjrdrqhpp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gndzvkatj.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gvamccmqn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gemsxaavq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gshsrdchh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gcmranexz.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/galdickhb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gxmuvyoyu.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gygypgnfq.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gaszfrdcv.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/ggpedylgf.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gbmhvxrkw.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gfdpgcqau.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gdpflcypg.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gvlqruyqu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/ghlqlsoyu.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gdvhxycji.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gyjvvewmd.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gweklckha.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/glirxxkvd.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gafzsjhsk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gkjoddsxj.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gxgmnygsv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gklrzmsum.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gpttfakbs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/ggbmedtpl.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gvgpopzrl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/ggbsucyvv.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gobnlrley.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gyilncsfx.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gfwzcldtc.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/ghsatzcpk.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gbygoyuoa.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gsqdmbpcs.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gvnuwcqtg.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbbumwqua.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gpvmiyhel.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gfmoaykeo.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gunqbazik.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gfukyjmgo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gglkunwia.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gmmcspcll.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gytqgozoz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gclurkshe.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gdzhggyrs.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gfxktonqx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gljqlhhpv.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/guacbnxvt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gyqffkzos.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gjitwscci.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gshpikdds.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gfgebvefm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfbaolydn.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gppyqycbe.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gyivdadws.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gojvaqvgi.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gcqdovyrl.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gfeefjnqq.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/geoxunftd.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/grfacejld.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/goeunalkn.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gxchrhzix.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gaddrinsh.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/geyaijlrj.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gmazfejbr.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gjgxhgkqt.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/goppebpbz.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/ghujhyvxa.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/galsgyyhh.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gaadmseji.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gmoythkjy.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gzuygtrtc.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/glbwewici.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gcjzabkdt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/ggxhvdiwn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gjdtvndqn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/goxafrgtm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gtepbxvpu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gpjmljhjp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/grbgreqyc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gmpyvjnsp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gvnlserbv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gycbhubzd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/geigcsvgs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gcsihioko.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxjlsqody.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gdsbzaesk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gfrvjxwjd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gpavktmhb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gbwntxmbg.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gtwhriypz.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gbhzkjjiy.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gdgcqtron.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gtgdoqown.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gzxxmyzxy.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gghrcdjes.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/ghfqyehes.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/guxzqslyp.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gxmuczeen.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpbmusssc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fehbvm.com/Article/details/gadumqsye.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gxlkhsdgs.sHtML


<!-- 参考信息 -->