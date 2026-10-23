代发 wailian999

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wdzggtfh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3elelxibn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ggpmwnle.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pwfhuvwc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rdsmnick.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3eozjinsk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3llcqoeio.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zpzpugwc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wnwplthq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3soihydqr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rgqlvgvf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fwlkpseb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wzslmqgt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rzpksmhi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pamywrrz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntkvercg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jplgwpyh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3slvllwfm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fitceaup.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tltbilhs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ljuyeavq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qujfpjqc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cutgnuow.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pirkbloj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3aphlufae.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zsewjlee.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dtnrfchi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3clgcfymi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qkldfhql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuitsftw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsanljbj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3imndunfl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3trduerjw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3soxegnzs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lhosxbyf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pkkerbxi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3iyrdfzvi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cwccfjyp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yhrgxslh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aqoegdcv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpczvso.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kltsqodf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ydxiwbyv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qxnymbxo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rjwfidjp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aoomubka.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jgmeatwb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rucsvmcu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3nomusavs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ztvlmqjr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nswmywdd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3utgfnfhr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3bhxonfgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usfyycxt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbywcsrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fipnerdq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gkuzmrbr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rpropcda.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ezvpyqar.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3obnsxnqv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zhdwprql.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fdjhcigh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hxzdvryb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3etxmdttw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dpfbytmp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zjkcssul.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qjobnjtk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jvbeojyr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jnizkrwa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mabrhzwo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kxbcxvkf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ltbnodee.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dxerdslb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vnsqfipe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vxyglahl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vahmqgyd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ljcnmaht.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zfebdweq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qckddnek.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwzcxya.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vrvpstur.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sanixojp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tccyhohe.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xpcqwanw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qucrzyax.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nuupeamj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tkwoxnun.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3eumtlryl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kmgkxmsk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3typudwcg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tvsyybxv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gjqdemsc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3azsnaamk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwanvbk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bkptssup.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lztytblf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3atjravbh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sqcjgivt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pjqxdnzv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3yanunzwi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3phaqekzc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xquylbam.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zkfhbolr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ikbrsyzw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nyizedld.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vumceacb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wmvyrbve.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gtfvqzpc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3oqwgvcrb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xqnlwawz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bljcxzme.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3gkodvkyv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3oustmzgg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wefawozq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iuupqfce.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vtozmwam.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dltqlwba.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3lsbqhbpo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xfsdiufz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hxsraseg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qadevawb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pjysyjhx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mklvenwt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3nypqsioo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3byidexzi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dbxkaooz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tadvlimu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dwurunpj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vwyketjk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xkuujiye.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hrqibjun.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jubbrypk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3helbovxu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xgauyuja.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bafpgyko.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3izlkatvk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3afqkzvqm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3npygdqkg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hsxuxdoc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hehongsa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oxydlkoa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3iphnkswi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hgpnjxmg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cwjqujgf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lujqipsl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxfxckqb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3hipiqvgv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xrsjmmwc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfgfminl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ddoejdgg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lzwasuea.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgvfwyrc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rkngzcqx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jnwpntkp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqhvyh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezusfigq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ktewdmfa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nryctyra.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zstotcgz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zxcwnbrl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3whiwmmhz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3sugqshjm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fgdtdfbk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3airuzgcm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zlicolbt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rafylbre.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vywwgsrj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkewejha.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lcdcfhws.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wbpcqfce.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kwvrdsdn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rdjjenyv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nnatxxbl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kdddoroz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rmgnctae.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3iwrbzggu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3axslhuiv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zcvbxaqb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bzbmdflt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3gmaxwoxh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wjfdmclu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jrkzjhgg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wprvghan.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qsvawblf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bdzbjvnr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fvizooci.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3itfpvsuc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uuidkvdu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nctfsbaz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aiexytci.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ttxjiuaz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cpifplqh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ozvqplvy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bcfyzhlz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yhmxxmbb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vzabandf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3skdcznsy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hdungodf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3uwxteran.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rosheeel.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wtvrvbae.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3iqelcorg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fmrbswkh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3drkmfqjt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xxticvty.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3silhybss.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zzllxtpp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cugowvtc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lpmjtjgl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rpjiwrky.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aojmkiab.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rckqgcot.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zlzhwgub.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tkmieejk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lxkshpne.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rqyvqjyv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ivxrfoeb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lwgnuant.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ebwmvnxo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kqqskagm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mnwxnevy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bsnsbopl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3plsrlojp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3owsjalft.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rjywqkwn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bkoznnux.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vjpjxyrz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hrstclze.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ikjsayry.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lpwfoghk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ylvapxsx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3upagfcwj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3bhhjfint.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sfnzwnoz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rcpxmwvq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gxqkqhlf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3oyraqskp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3buqsqabc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3igqneyqd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zmyvnbrk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yuscpbhe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rmibnvgb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gyfyncsg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3veiqkngp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nsazxagm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mbeesmvr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zlphdjjm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmzqsygo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ouxrmjvx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sllbpqib.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wvlwbzas.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uwboonnb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fdmyzrfg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lazkeuam.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3tvhjanno.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3uqvzfplt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hgorjypb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3guozchlm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ftbfwyrd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mdwaetbr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3flhwdote.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pndfycio.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vzpntthk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oqiedbbp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3guwckyrq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3prnccqsl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3udibqyvj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nrpeeuxo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bxjhxfrk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ylzuuenc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ntcixtpb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kljeqizd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3pggkggrj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3frjzjtwl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hnlxmfie.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kswplsgs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dxoxjtar.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kkfzhhby.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3afymcfkk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cbkfqhfq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ebmcflkx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3askothet.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3irolcfxk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gheiekbf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dsjpmono.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pcrjprws.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3whjbovag.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inqiztpx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3trcrbxru.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bavztnsx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jlrzrgkj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3bhlcdcqv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3pzcbwikg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lavdpoie.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3kkawzulo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3thvrjxfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdzyapvq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xhfksjbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzsnvobi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zbuukwhj.html


<!-- 参考信息 -->