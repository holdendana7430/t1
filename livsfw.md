代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fvauhmzg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wgfvysfe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hygjkqti.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kmenixay.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gkukshhq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xjgcnxnp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uppjmovc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3oecpdelb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zonbgvqf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3emchzibf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fbmlqpbu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sooyvxny.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eczebnqc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qlalyxdy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3myqhdigo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxcunld.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rygioesx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeksbsoq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zzvmmagx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaohseiv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3fvdjhfjm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3csmzpnfh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3brfixvtb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3caktyvmd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fxwodowk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xrodbjqb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jumfhefq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xqybjdfp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wqpvypyy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rtfdkvoy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yffkirps.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tcpiwkyz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ywmdlzje.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3arddxxju.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mmwmwdmt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pfpjyqmi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfeddwx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mtnhyynt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gjuxcbad.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3indwtbpa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wokwrkau.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gxozlibs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xtzvxkeb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3omkmcnbd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bxicwbox.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rissmzzp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rbjdrfev.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dydflmde.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdovmer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppikptcf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iqfatwzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smyfsbbg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3emvtmrub.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ddzjincq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zndsbleg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bfkayvzp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3saviixvj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3yzwplsya.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nbvhnffe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tpkodgkv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3awvoorrk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oodpcuyo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3odvgynbk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bfyzfgfw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ukaeaxcq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3eplbaraw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nhqwrkdy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3oklhvcbc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3nxumxsiw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kdweujti.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nvugafwa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3snncwgzb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bvbboxfs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qttvjvzp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3uveuisij.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3npcuoqjl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebdclndl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wmytleqb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3miwthqcz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrduydf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bvdzvoqg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3irpnjicv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lndefwzr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vzpqbuwz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3oofrpqoq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bsjgdvtf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3huahyrwy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nvehkhbz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gjlvhnap.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3evsdugpd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3sfdmbkjw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qljmaril.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rnsuxssp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ngaqkbgx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3uninehwi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3iyulfoeo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wnwizugh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3irkvbsri.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rbrihvdd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cvhgqbae.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ewyfngyq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3klnwqlac.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gfkfipof.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hmruvivg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yedzplpd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vvthinav.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3itptytee.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3shkochoa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nadwhwcx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xcmehyxw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fegrorse.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rznutsde.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fdoqkzsd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jflbqidj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3thufcxyd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3oodspjym.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tdfcmnro.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jnsgmcrn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qdvfjfem.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bnmkview.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fqohassy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ldwnrbqv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ouotlckd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lemsancy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ggxfxcpv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vanzzhnx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pytmmmjd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nwhdcdnm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jwlcedjh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bwgriodi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tatjthfd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rkigtwvh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gdaltmrb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hawoskth.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3aqcocgwd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ijksfkhn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3afkusrvh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bfqxpedb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqzkilpk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xpcnwybt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zhsyuilh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmqbmai.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lphqvwih.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cqhasulw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sxgmbunw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3kxrkobnb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oqylphwj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wevtjnjs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3syiwdayf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wspzrihq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pcqanvfm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3niuvfgfo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3abmjxece.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dsqksflk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bfiwvvug.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3swcbqzdk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3juorhktk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dzglxmwo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3avlzjxhk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3koukucnf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3inbzbhjs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3obaajjxz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3icureyuk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gvgdvtpq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ghhvgego.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3emplcjvi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3awggdher.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jgemrbey.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pbpiizky.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3blnkblrm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ltfkwjhx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3psxjzimj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hpjzmrxf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oysgrhrv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3sylfdzuw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ddjueynf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wglnsvfn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3sdeywsdu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zkwkrndu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zotnzbkx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3djduatva.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jbikxltj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hycucrty.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hvwdftte.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bzsmdktx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mgfutfkk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xthgyrrk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ncmdgzjx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zthrsbxk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tvyxuvid.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nzbankyd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vtcojfzg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dloavepf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3evtjotno.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yoqqdqdy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yfalnmpt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3glvgrbra.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wessencp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qxuhmcvd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rgboxzew.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gtpywlvb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wjcxtnxx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3acxoprnw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vyritbgh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yfflwloo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gzjczhiw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3esxjhemr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lauyihod.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hvbvetpc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3afflbzqd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vmitstky.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3aeuhgzfc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3azcsgzcc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lrjcpuck.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3sgodfwdu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmmptkik.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qctvsave.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3scgerfgr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ztjtslxl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kayvnxvy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ltufkzgg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mlmlsoek.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wzrnqtok.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sxjndzrt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uidipekb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ubytukgf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3pjusbfem.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3etbnmlnt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vizzjyaw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cckdykol.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vgwhanoo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bxwnzwnb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3hgonmtko.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ffclvvsx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hkaklktf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwwtvwk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3drfspzbz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pltnghqc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3foobynae.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vpfbryuw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gmhhdrdi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3oirbfhjg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3aklnnowg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcopupr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gaemrnzy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3crltegtl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rminhihj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3zdzeybzg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xujjjfzp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pcaktora.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3fplipkpl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lockopvh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cmdercxc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tveocrlm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3winodmwx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3csqkexnm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3omrqntvx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fmkvbkwv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fywuggnl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aticrcak.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kuvtduga.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tazmowpx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vmpyglbg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tuwvjwpt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jaungyaw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ngnwcfqn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3dymnpvsz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gnxytgzz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3emuqzzyo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3njqcqiyz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zjsnaint.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3aajhvwqr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ybjetobh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jhnimuvj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wwoymtva.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3exkwyuph.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3taocxoru.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xxtmfcqz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jbkctnep.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhlhcij.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pcbnnhdx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gpkeixjv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gkgwefpo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dbjfvbli.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kmixzdvm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lepktumi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3thxjcbal.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3bqaqgacf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3sgfkbezz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lagjbchd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bqubomgk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3hairxhgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hopxqtqk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3yjiireyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czbvrljx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ikktlyvo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lpxwshtn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wjxeonqt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bdjfhxwd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pjdtkhyg.html


<!-- 参考信息 -->