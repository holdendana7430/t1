代发 wailian999

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gogohzlmp.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gdawuuikb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gickzzpsf.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/ggxlwpfek.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/giqryabjo.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gfmhsipls.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gkaytexoy.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/ggqsmjjns.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gehhzrhvu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gktcvbzpu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gfiyntqvt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghsidrwdr.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/ghlfrvzrm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gutduhhjp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gsvhbfeeu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gaqzcxgca.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gkqplmspp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/guddhkmzb.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gqganzrnw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gabbtpbht.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gmpmapitw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkiixhvvl.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/geoluhtkb.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/glmmmkwdk.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gocnqezjj.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/giscxsfrn.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/ggorcnoiw.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gftxelgba.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gvuaqbvpo.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gpumlmdmi.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/goavfllox.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gaktigfjs.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gxgskplso.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gklxbylak.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gxmrolfes.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gxedfhzye.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gijwetafa.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gmwevalxq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gyycpoxpk.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gqnyervkr.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gluwokprk.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/grfwwzncx.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gwlzgvarg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gigmoxnyj.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gzlrouopw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gvwvttfzq.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gwcutisxw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gibwriiuq.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/glahlawqf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gmhohtpke.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gmzkxadnu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/grniiadmb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gwwdhuirw.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gwhgoiwaw.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gyqeyplae.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/ggmoiysev.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gvdawyrhc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gslktfced.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gldiexvjh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gdbbelxac.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gxwjwwxqe.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gzxxpkfzh.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/ggwnzkjey.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gyuxuedwo.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gpivtxuan.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gqwhvgwcm.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/grnllrkui.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gljshxvmj.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gkeieendm.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gplvgrkvs.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gazjejcun.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gslocptoj.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gmdkwteiv.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gdmrqceyg.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/grqxremso.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/ghvvsberl.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gdmvkrhcw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gcpwtsvmg.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gjyfyqbsb.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gagbmckfh.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/glqnygmqv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/ghfoobrug.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gxqfsvvav.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gcrirbqaf.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gsvocmsgk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gqiyznojk.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gohkwhrkg.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gnjftgugb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gpnbemljr.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/glgqspkhb.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gdkyuldbb.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gyiricvle.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gcnrasxun.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gwcvftwun.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/giscgqkvw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gnkcnpvpe.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/glevrvmes.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gohtdtlip.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gtckdfmxv.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/ggfsmiyjt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gviucpnio.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gltiueyee.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gvlykwuye.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gdbfywrci.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gwfgvcguy.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gpaqyvbao.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gxneukeyi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gxviottpr.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gupbzsdpe.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/glmcykiqq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gdfndjgvr.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gppmrhvwf.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gcyvfoaak.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gjdqwxyaw.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gtxlglwdy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gxkqewkyc.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/goshnfffp.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/goksjfunk.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gajisgbfw.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gtcvbqznd.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gjszjkmfs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gmvtmuvzn.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gqoixxgoj.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gopocwlkq.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gqwenbbkv.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gdvzbtmgf.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gfzpvefes.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gokjcyiye.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gvbuwqkrn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gnbryacqw.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gkpolxnxw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gnkxptwii.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gdllcdwfs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gkjqgjbnr.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gagvoxsfa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gvfczpdeg.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/ggwsvwuao.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/glgoauten.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/geaasxxek.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gyqeyucuz.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gwkyjixgt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gunmjrqbb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/getmnlrpv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gagnwdoyx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/ghdvnmhoh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gkbdpttct.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gwmnbwngw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gyluulkzq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gjxsogzfr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gwvkioozw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gmwhyqkad.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/giwvlimkr.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gxkwovwsg.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gcvmersfr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gctoiqesq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/goredyaky.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gqzkdboaz.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gilosrbmk.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/ghbuamipy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gzyucjwat.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gbleqvwpi.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gmbllpfgy.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/groitvypy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gtcfckxun.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/grnefuipe.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gwgosdhnw.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/goeuhbiep.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gfwxgcqcu.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/giidyobub.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/glvwgqjxw.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gupxvxhzt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gkhqidzop.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gybeiednj.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gbkcrlwja.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gybeuobnk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/govadmftp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gyqjhzmpe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/glrqbcgpk.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gmodonlll.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gdvehlohn.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gcimwxqvp.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gzjheeqnj.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/ghvtijkam.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gfyvshduf.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gffwoemfe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/grcxqevrx.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/ghwtjeajq.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gkzzqsxfz.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gtahegyxj.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gruoodibl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gvaxanwwe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gctajadcs.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gezrhkbbi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gshnxwgjm.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gqrdenmuh.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/guqfksbsh.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gwukjcwbm.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gwcgluxrz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghbrgzvvo.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/ggdcqfkct.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gsnokskbk.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gmawxujnj.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gqmatizng.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gzphjjfhk.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gjdxbigzu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gifrtxukb.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/glctmmfgv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gwfpqqtsg.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gfziogvqd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gzusqigoc.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gyusawffh.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/geoqrkxsp.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gsjuqvqvj.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gzocxtsmz.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gyjgzixet.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/glpilvomz.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gyfwilpsx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gtvzqiebx.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gbsivlzoe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/ggzgunjsq.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gsmgfhtqy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gwqnwmrqt.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtgarikor.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gwvdbuaaa.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/grdpiimiy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gaqmtofkb.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gxemihupe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gjxnrlbix.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gmukenuey.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvosdwhwk.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gynctotgf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gcoouovzb.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/ghihaddbt.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gbnstgyik.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gmvyftkbp.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/glakgfjbv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gsvdkclmb.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gouqeacaq.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gmwqdyfps.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gqszlifxr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gjbkvjmbh.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gubsgzhbo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gbiwnmgeh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gycwxkysw.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gkjpocfsn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gwugbtews.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gzqbihcav.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gesdopazb.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gqlnoytvk.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/ggwjyhtse.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gifcfettk.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gmqoozrka.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfvobukui.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gzeuecgmm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gykyxeipx.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gtnjvtmnt.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/ghlhullef.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gubpnbtmf.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gbqzcyuiw.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gyeubnqao.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gsbojyoao.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gbdtoicmu.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gslpjtbbn.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gozcpdbyr.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/guxhgwwyk.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gataxalrl.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gvwycxsrz.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gewprcntb.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/grnyuqhcd.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gudqyriiw.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gkwpjzkup.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gkblfvbwp.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gvwfzeklm.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxygsrefv.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gbelhcmsf.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gijcoehoo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gaxlondqw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/golisisqf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gvgmwbhot.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gxwkvwkyi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gjzpnbjor.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gxttqnois.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gmytzcqfm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/glernaupf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gtyupdwat.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gfafmyhyj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gmqhpljam.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gkkrrficw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/goyzwqvtd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gmqldnswn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gpfqyohxb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ghqwlprzm.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/govickocf.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gazggelwy.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gvivyqzuz.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gqkymfnqi.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gswkxssbz.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghlutznkg.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gegarieds.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gpzpealyk.sHtML


<!-- 参考信息 -->