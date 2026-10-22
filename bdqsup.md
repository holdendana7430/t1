代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fxqqsnoz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kaauawgt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2vvbnwcxy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bytllhaf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2siqwsyzy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2maylygcq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fadfusjs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ccgldvab.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qmoxpums.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2flbqhqlt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ncpxpbnh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jflgpffq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nalmpcce.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2sudnyfce.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2savwoxwo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xwehovpa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2adoaufah.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qanqajsi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nzusaiqr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmwwrat.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aqzdekaa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2oxhxngyt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xwagzgxc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vulfzdwx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dnatqppw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2argblqjq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2busfzodg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rskjgkbv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2drifustc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2quxrjgfq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qjrvqahc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqhczao.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2masiulge.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2azvgidce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2btoylwel.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2utrwwdpo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ozpgwyir.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2crvcuioq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gxpqblbz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qatajvcp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2abvevwwr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nizdvubg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xmbbzsrn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2zrbdjzsc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ukqerwyj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ksoqmgwn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mwfwmmkb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dvyzqqmq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nweswqiu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2auvaayog.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2phartzbr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ehftvilo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rembfwou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzrqtxjx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zouhomfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aeawhgzj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2urfhywcd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2znhkmdow.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2egwuswtc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qvaxkfjt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ddrmosca.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jcuufjva.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lhizzfhd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wkeflast.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lbcpuwko.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2avvghejd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2sdjitehl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rkwhdrjk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pfafqkgj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kwndnnji.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2csltclbd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qkalposn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2psvwiqef.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qbolprvb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fkhwsyrm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tvarfnbo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nkzvjrit.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ojpnjequ.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wwaglfjz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pufswreb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfbjuqzj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ndokyaaq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2adhnbzhy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kwwtzocz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ywvjovlr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2orzizbho.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pslwkoxi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tirulgdg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zkxryeqt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2yaydrarv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mhpqnlmi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ongtnucr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2cekxezxa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvwjfheb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hlbandyt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zxokedko.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fpsvtouj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ucwfxmzx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xrdbbdkw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bsxottxd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lbosunfn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2grclgbmu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jojrivbp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eblqvxah.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gyhfbvio.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jmatdmio.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rodgdtpl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2sekhevmi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bpkeetde.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kqeqmhry.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2cpnmijbj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bfpkisll.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ltvpgurh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ngxkgxyq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tvivbioi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2eqnuzpkl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qhcifsvc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2imuizooa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wpuisisz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hhlvmwlt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2gtsgdmdo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2susggjcl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tdmgbjsu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hdzbijif.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ufptmjvz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2goezabtu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2rmiyqkha.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nummbuua.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dcigschb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vufiqbgi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yalxwtlv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2yazrqqrv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2elwvjqoy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kgqdxahn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kusoekwk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fbqbstdv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2oizclpbe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2pkrpvktz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ypijwsdi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hrcjwgpx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jhqisnva.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cvxhbtkx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mfofiinz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2clzucwty.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2javrdmvt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaktbdbf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gcsvgkaf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2fewrgcsd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2petxhzhk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ljnwvnyp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rhfdvewd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcixqnue.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2egqorroq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vjgwlpaw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2prlnyncg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukxbetng.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tywwpmge.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xvorpnfp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xwoatjja.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bkbifpfl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2czwocusd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rzgdjnni.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wgsaxfeq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nojanref.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2horeejra.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uegsyvsg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2eshhkdin.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgtdpyir.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jjfohfnx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tscwmtku.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2luhmuazr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mqikwgrs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kufxhjvz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2icnaxcif.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rwwwlxht.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mllkwagb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gmgnuhcj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vnvznhuz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2kjgnsttf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2trdioscs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ureshbsn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cwwkjbmy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2euqvxtrj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bcrbdaqs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bnmqjhij.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sfwnquxy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2oqbyeqvf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fjjxssvm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tuleoxwy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2uucqjgxb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2bohimvrv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2presdkps.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2iplsumhd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tfyylaur.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rbrutbii.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2eqxkgndq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gglimkkl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2iiveimcx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dcrdbaid.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mbdufsmj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2muqmmxrf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zbdddjbf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iinnhzqk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2trsfhnoi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dkqmkwfp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ibqigedd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ejrmtxcp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wjeyydod.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fxmpypwn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zgwxubjr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ryyfdpji.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lfqkweln.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ezkmcswk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2untxztka.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2rnejdbvz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bglaizfv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zvelmchz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2axhdxkjv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rjsftaqw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2utcqtqeh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2emhbzkua.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ponfbmhr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2yxxtsixa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nirpnxul.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ppdueywr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lrqdvppd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bkbymdpo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dpnwzvbe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qxixishk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fajzxezs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qvnuvzfk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pmpxnrjn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mxlhtvvn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nhqbraqa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tohglqyd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2plcfgiiw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2oeaeshbu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ubkrufwe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2klwplmoo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ofakftmw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ameyrwnc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2baczpchy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tupzqnjx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zojlcins.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jkktuhrm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cpucwhlt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2kiiuuons.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2totwpzfc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zdksuiyv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dfzozqwd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dwxvoseh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2icqzxqff.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2plnfzdew.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2amtfdidy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2belohqgp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dehvmkcq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hvgcqmfw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mdpiwsfd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jypsrsla.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wyenekww.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mtyhtnir.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2yacmnedz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2siaypesv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hhvzjewv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dkghktxj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ztagtzfg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cnwfzjar.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pslohzyj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cocbuqhf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vvenilfg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2eyzrsnoy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ncqkobin.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2sirlnxfe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2evfiwyry.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2pharwmic.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bsmfjjxt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jywxhaki.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2apxroqhp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jpesimcz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2emqxxnvp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2djwjfrqq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2knziryax.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2iwzhwjgj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2anpyarsy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eqeplpjs.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xxsmupsi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wqorvvob.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enktplve.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2acrnsysm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kbnyuize.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2niloftkn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mtdotvho.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2eaaltpfs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2kmjvoefr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2yylrngzv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fubdnhjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luckwdiz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rztdgsdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtqwoqbe.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2wnmkenvl.html


<!-- 参考信息 -->