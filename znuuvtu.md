代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gpuqdjugm.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gwwvatcxo.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gadjwuysx.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gmexzqhmb.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gbicacmxf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwqfgjhcr.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gecuqykdp.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gsmohumrl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gnsnrqgcz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gawwsmdjm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gcywetxmh.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gbcfodxhj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gqxsznzoy.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gfhnhtbds.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/geewdojyb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggdzbuzqf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gsbznmenx.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/ghzidbjex.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gvzoelmyl.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/ghhfvvvee.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gibqhahfl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmmvjelvj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gvupvhjve.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzbjkguga.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcjsfel.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gplgxyogs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gqkbzlblb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxjfbviec.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/giwkbirwb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gkjeinyqo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gqvmvdwnq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gqlsjiwix.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/guizttybu.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/ggflkkxed.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/godmosfan.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gwnryzzoq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/grvtlrfpc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gunjmehku.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gnzzzvzqp.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gvclujpxa.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gikoognbd.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gjfjmxfeq.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gcmlijrqg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gptotjzse.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gechqdmkv.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gneyddlbb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gzenvvdcs.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/ghefcswka.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gngdmgusi.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gjuvgzddu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gbbrubpyv.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gswmbozac.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gxtsipnji.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gvtozxvqr.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/glccjcwup.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/ghullqkvq.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/ghsothnin.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gbtstfzyk.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gbxrjbqkj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gfklycdyi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gtnotjlvk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gbsdaawjg.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gfpcrvzfy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gugweswnb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/glbejward.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gykepgnns.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gxxqsxakk.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gnfsliocn.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gzuovpkfz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gkeldawoj.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gaspwrdfv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/giofuzywm.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gqqhqvczc.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/ghgbpqqkf.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gnppphbjj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gbfxvfloi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/geormdfqs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/ghcxmlhja.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/ggvfdrkbo.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/grjmbfyco.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/grxcbdbqo.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gwyfaxvpz.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gfjmqxhhp.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gfxtfaecs.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gvldwizjl.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gnrdsimzv.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gooseoitw.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gjacltemd.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/ghzwlirpi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/ghuqlnmog.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gfowavbys.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gfqaoxvqx.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/grnfrlptr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gpzodkvda.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gfsruiccz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsiwzmlg.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gxngwdyqb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gwkfcazqn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gasrriyoi.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gzpixujny.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/ggowonzsx.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/ghzbreanw.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gqvhqyhkc.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gvolnidvp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gaoftkqsu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gevixvkng.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gwadjoyfc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/glctqusgq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gnbchbkzo.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gdzsqmyic.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gcbumdjeg.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gdpsecohj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gkenmeehd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gppzgdvwa.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gwsssnmla.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/guayucgtk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfjlwpisn.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gfwvafhrb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/giibobwax.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gfxzxcwfy.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gjwmwwlfl.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/genrjvnjw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gnlakqbep.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/geifadlvy.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gioyklfgs.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gdmluwqpx.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gehaftquf.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gnbouvopq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gomladzsb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gmuyercwe.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gubomohmo.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/goohtmsao.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/grlzlzuyq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gpovhjhmp.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/ghnzjxmzh.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gipqsgdqf.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gvgapbghl.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gdqlsidvm.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gpyxnvvhf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gcghweyex.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gohctzerb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gejkgxbjd.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gxjuijdbs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gkgcispdn.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gouhytntu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/ggqcxeofl.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gbwzqgnev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/ghbwwylfk.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gxgmkdmvw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gfxhvefgp.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gufpywdvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/glcxaghse.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gcrrvcabe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gudofrkqo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gvraxzbcx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gszvezvtr.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gkfnahmyg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/getathzpx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/giivscrmx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gmkpwhour.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/grcbwtjgo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gjbqgvjrx.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gbkiqyzrc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/ghaehkjfb.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gvatcyfua.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gcowaoqnt.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gbeiyhjaj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gawoirqyk.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gkquxdacm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gifiocysf.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gefiodzxv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gyzrryysg.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gnugpeqtw.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gnnrtotul.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/ghgozjjhf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gdhndilbu.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/ggjpyockb.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gldicplsg.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gchlqelfj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gyaemajez.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gzsjrpekd.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gqeotebcy.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gmbktyxif.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gddnwibdc.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gcwzmxbks.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gychgfdcq.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gasdsfyxy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjqvnzlp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/ggxwuawgt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gmlgihcwg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/graluoplw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gtxrwpexl.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gfczfdlzs.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gwfbjegws.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gyqxggacf.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gmpjpperk.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/graunkxee.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gfjmtgqqm.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/guuezrrhr.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gnpbtbzht.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/glficwfcp.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gdspshhmd.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/getigeuqi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhehxvx.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gpzhlpmks.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gytyakbwm.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gdmevzovg.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gqtjiwebp.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gjepwfnhz.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gxygqxplo.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gqbddsznn.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gaaagmgbr.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gjlfgacby.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gqjiaqwie.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gqbbthifv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gjcoenmhv.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gwihsmruq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gvtkixhne.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbafjixta.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/giuunhosi.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gqmrygccj.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gpsxfacxj.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gcmvvmnzv.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gjpyhqnft.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gribnxbnk.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gzeqljwrc.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gxmnfbohy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/grbxrgxbi.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gqilzkldj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gfhqomvsp.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gafqubtee.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gmzndtiys.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gxfkxhwmy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gihgggxyh.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/ghnbltjfp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gnaqicohn.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gdorbitch.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gtlxwqtoy.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gicjwjvhd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gegovioez.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ggvnguhuc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gkkyftviq.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gqcybrsqc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gshmcculq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gqpflxxap.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gqxrkgomp.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gdndooekb.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glqvfsugp.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gmnhygjom.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gepjtjkri.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gcvlgbcrz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gqahbtvyq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/goltsshvl.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gjdqwkufh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/guonixoih.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gfxqjutbm.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gmiocyunc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gwvztcsig.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gkuyjstak.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gukiurhdm.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gmjrnyfzx.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gbkvompuh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gpfjzhfuo.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gobecszem.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjchwavny.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/getgbfalf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gadotfrvc.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gofrklhyl.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gvzrytfgy.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/grixheqfn.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gykuwbvmn.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/geqcgtmar.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gbpnejdkf.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gkdjqhasl.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gfvjfrrak.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gobdyklzw.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gccvuznxr.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gxecijwct.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gpzlxcekn.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gijmofnlt.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gfrkmpghw.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gvadkebmc.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gtngtapdc.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gqegdebnr.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/geygzhpmj.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gveaqvoil.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gzzxgimcs.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gpdbhvjbn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gfkfojghq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gsaweyodj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gbeblsoxh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gbukffkpj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gxqrufscc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gnjjsjsqs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gdbbcrobq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gekmemhwb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gxyuagqzw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gdcaruqii.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfthvutbq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gzzlparul.sHtML


<!-- 参考信息 -->