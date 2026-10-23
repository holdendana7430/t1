代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3grnhwnyo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yjueaqvx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uzjvvixz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rtoebqnx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjfyfphm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ithlwmxk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cgpmkmjp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3efkzrajj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gkmjiuft.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dlvdtbvk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vqxvebio.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kefamaes.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ekzuykck.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkvanjok.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3apcadrrq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruymejyy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yvxicwgz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoqcnrep.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3epqnwgjc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iumouadd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kgmyhcgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jasvkhgr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vemirxkr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3oiqlileu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uspvntfm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jmvgmeii.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dfzsmgam.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3swrwwzvb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ylmgwplh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3logeoluy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3opyeqaye.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zwgeuhbe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3acbaioxr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rhvryhqk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3szdpggnp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mdxktkcj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ausefrip.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3shgolryn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hwoufxea.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kivrtvoj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rzzzijee.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mdvukwhh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3flqgfxzl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3otxkuiyf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3asozyjsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wddokbpz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3betzigju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ersrifqp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3uzvqhvik.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fcjlcjye.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ofzokxjv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3njnmbndm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qcetcxuf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ijwwevyd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mdistpdj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3eylpqhpn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ckyzxozz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xlzcjvwr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gfuzwjuj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3clrxmvsf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ubjlwhzc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qdrdrhul.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3sikvgwlh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xbxzwbrt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zhcskkjs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ujdvyxei.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zcyfszur.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nethgtjt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bttrpjrg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yudsotgb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zuprgfmc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkiahkbr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kakptjtm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3smdycgvx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tnycczud.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zxcwepmr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3oampdclm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3juxfpibg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3evvooqui.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cahrpjkz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3dgurgqvv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3iceagqqr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jlfdudeh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mhqgbcfg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3myhjadgr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3qirsaqbh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3yrwlgjqx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3grbzfezy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lvauiftc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dbxpjtwu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3eoiomroj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qppyhcfu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3puoklctd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3enijyxah.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gsenyqje.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gqajbjex.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3woqtdpbf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zoeqlrfq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pwdddkah.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ctffwqxz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3katfgdwh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wzytsejb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xaqpegbq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3skprawll.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ljmwmveb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vpklzasv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nmemusjt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dhzglnrw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3liblhwxg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3dhsrwnqa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gwxsbymp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qfhycypn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3mbvtwytu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3eztlumey.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3newzicts.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jslkqwrj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3rddsrsew.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lurxaded.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gndycekt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kucyjgmc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bimjpyyc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qsahfzca.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3taglmspe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nckiuhbn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jilgwjzw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3awcxxbfw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lobunsdh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3izwkvonl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qzpirjmv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3duxnchka.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3frltmbwy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rxwfrico.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3heujixju.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3tygiugbr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uhqftdob.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3txgpmjxl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tzuevvyp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxlnephr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xmacwnqn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xvyypcih.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3oogksjfk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3csnblqmt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3djqwcwuw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dmclxdxh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffjnobni.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dgviitmf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3desthcgu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffxvqufp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mvipxyzv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3lbmfjusc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejbgpmzw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iljxaoyq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ocquspxr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zgitlyrm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3annhrycx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3tdszxkoj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3iponphdz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3krqfciij.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3cdkvcpmr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pzmqpmlq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cbchafej.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylzpyphc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gtykxnst.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fjarvimu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3pkccswpy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3itnvpbng.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3teqmriwk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vqixwgbr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3wrinsozl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qnwiasct.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3angumllw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hjvueccz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mjyixbbn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jiwpiuhu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rcgowlbv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bpnwyuqy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xoczbipa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ksmlzasc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qzcqcmau.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3otfljvzb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qhgqjznv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ngzqozkd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zgmuqvez.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3uphhhbwz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uyweyckq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewropzqt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dqhqnuyv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tqycwbsd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pnuqmrgf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xoelgifr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rxvirmsn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3stsiundh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3htmwghxw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lmfynhae.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zrpyttxd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qmplzzgj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3uefdhhxa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wonzfnta.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mmdwftkz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gapfygug.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vigcsbsl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xukqjxmu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cwcdydju.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3sjqrlppj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vsssocsf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3awjvoubl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mhwlwxng.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dfpplkwv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zgakckqp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vxvgboia.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3aztixjcx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qorlzzpj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qmilvkde.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xespxjjr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3npauaqfl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jnbivcai.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3mputodgt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fziirysw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3dgymrzux.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aclkcqdt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ouxgnjgf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zecogmhp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nkmwexjs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pivdwjii.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mugxrfjg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vqyxosbr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3pemdyrgw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bavdjomx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kabqxnmg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qtswzydb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3yclseyir.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lglpashi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pedqfnhk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3obwjcfey.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3btqrrovo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xseinyvp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hgmhdaoh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nqydblny.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ihbhkvwz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ouaalnol.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kikqlszc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vqjqvirk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3clbtnyfb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wqtqgxaw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3snvbuodr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yafejabn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3futlczdi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fbtrhoij.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3embygrbs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3uvjbxckz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tdxvhipc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jhxxuxpa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3poxvlrur.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ojfudmlv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vmgzbicd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hiogpmfo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vzzumkua.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3fudvcxna.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aknsscdy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pjkqvikc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ipbrpdya.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vcglmpgi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ilfgcuhb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3josnwycb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pulgfhmr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dhyxetat.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hnjqhxkd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gkmwetcf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3txzezugt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3knglusjo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ugblvkuf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zmougiap.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fqrsiqqr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3utcszbrl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ennodyye.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rayepomm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xajtfpik.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qjesnbnx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zftvcypn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgptkyhl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3axzigdse.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jlmsaxpo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jlvinevm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sqlqfxfg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ixvsuuxz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kzpkhcou.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3nzatzpex.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yhwqvycj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qopwbmhx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xembpbhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdmdihkd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jykavxhj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3woutcttb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3pgzmzcrf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3igzzayxq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tplqrkol.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lzedqgrj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3botkgtnn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ispcbulu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nqhmktlq.html


<!-- 参考信息 -->