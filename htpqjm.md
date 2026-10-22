代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2harmilvt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hsjuxvew.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dlrbmgpp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xeikodjt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bnxlmuem.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mvbrpycj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qldoyogz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fiigjunv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gefkmiru.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ebejajlr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cmjwdfdd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zjgplykp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vjhuxbzq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ejhufjnw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kyulpmvt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2kpmtfeub.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ewdiadeg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mbsrdned.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ooetpqvl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mgnhhpii.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pictxqcx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qyrxzzyr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ogkpgnnz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vdduzmnw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2estgtdoo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2domzuhff.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2poojtyqw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqzsrviy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2roaqrbnl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2myldlwkp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iyjqjcza.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zddaimvr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vzywqwdu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lkukmmvu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2alwmpqzi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fpenxjpq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ecsmaljr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmiokkfe.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yjgvxmor.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zddncjpz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2igmqyzwo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cfsdasxv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ymydisbh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxpcminf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nyoeitsw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gzvoequx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bqljdxwu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rtkjlzso.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vvoadyjx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2asmbsodv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qenijsio.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kwrjtfii.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vdfbskth.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iflakrew.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dkcpbffe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2juxcmcbr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zxlrmnix.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zjhcrzng.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuiygpi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2abmblojx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uwbloaon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxubkqie.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2irsasldy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mllvazqr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yhjjnzkn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ffkktgog.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cjmybffx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zdkdqwjv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dgpqzfjs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2hvvflgjw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2aiudadxh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gchnxawq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2occsgzdc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2asmpejyf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lcufhqti.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2toqgztlj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vznkfzjf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2drbxqzud.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kbdwtgxk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cwbeowoi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ahzaosrc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2yylylwsw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ksijmicy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pbgnfgav.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mjhxdvoy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqeapobk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ohvtejro.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrfikakq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2svslfibn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vkfeuiss.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2denbnphb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rhevidnb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mfkxhsdt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2amvtmtti.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yccuhgii.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2oldtwzng.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vlhbuodj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nvuwhnka.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zilkmofy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fdrqugtk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2frusekim.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fscdzttw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cgehaxgv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2opvrmwvz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gfpdktrx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cnrbhbko.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xyiuonci.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ixgfcqux.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmhqhrno.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ywlhwszu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2rurrjwtz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vohexdcy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bkgfazuu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2njabvios.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nnafzlkx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zofwdngf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2efmaehmk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2oukblccc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yaqgzvma.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dyedgpse.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ursnrdnh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bnstuwlr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jnasvchm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rdrcnkzc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dpdyajlh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2altbqpdt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2csbpgmql.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2okrrcsed.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ehlnfgvh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pokoxklu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qxyterww.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zokkexsi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xrtzdmgm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mqorompt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pwmesmhq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wchlxwfz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2eavxzrjm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xnhvslod.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tcgnderh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2emltwnae.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pazrpzcy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tsqlrsmw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cvqmprsk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ongtjunc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2orffqcpp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wirrkicl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2aleiachu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uzpubbds.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vrlxfstn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jdysrwle.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2thlvflmf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2htfyowde.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubazhbir.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tucazxzd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cwpgwwgc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fhbfxxsy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2isjhrtuw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2lmzwpmxn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zexpzehd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wequkhto.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2quiitbcu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2sinkwfmj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2gcazcoce.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cxgfmcby.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yxiimbix.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dquwghlm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qytypofs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2khaheiqi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cjyoilri.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bbxqkkrr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nzjuorut.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kwgxhaik.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bmbimoyw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2atccdntb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tknucsqr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mtemqaau.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2esbqfgwt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ixxmcotm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2nydvholk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2stgyoxwk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2sphzuyay.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zorzoani.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xyqokcbl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fmtaatnu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tiffstel.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sfcpwuyx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ahplepjt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zicsvmjl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xkmpxzbw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qkmyysgj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ivjdrfaj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2swugsxvr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bxpaaetw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjthzvde.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kcmxcdto.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hpvlukcp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ixbgmxij.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pdhkrkev.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dhzxhlmq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pmvukieh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pllobppf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bhbteljc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2daxifgfg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2miillkfj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zvizhqwj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nfwmcgdx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wiyweobp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jmvzgykj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2tintmrys.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ugataigx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qixsalnq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wifrkaca.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ycyeqjgq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xiikbmqv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2gnjtuwak.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qczxywpc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ozwdsuxg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ghnwknsf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ejdpmmrc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ynimxxnj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qgfoheal.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jjjyryki.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wrtvucit.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rfhbznja.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xxujkufw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ncrlzfsk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jkweejda.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2sousvtft.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qoeszedv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tuhtaxvv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vmcscryg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qcqnhrtc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uhkiydqs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ecnrmkkx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nfkafnxl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2sneeupfk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xsvvlydp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xanrfadi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2uktmqvrk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hwxmlzwn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2puzlxydr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2otmdplje.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2kplpldkp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ogjmlhyl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wssmbjkd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ouyouwaw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ymxawvfp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbhyqmp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ibkrqhuv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lcsshfuk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvherdaj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2liuvywin.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2imqbweda.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pxtwesqh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2iexguopn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmqgjdze.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2whgnmvag.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2acavmyqw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2tvklbyov.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qwdlhvvn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2txalawds.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xawxyuhw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2iodgaibd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qzroylae.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qcziieyx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fomywrsx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xwthrbvj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ddauxhjq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hhntghkh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ekjibedf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tdsytfel.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjruzcml.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rjawlwnn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nlsarjhk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pncvtttp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ofkdjjuk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xgxcnavq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjzjou.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wqjjzppq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fzvbtash.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2okkpbzkn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2djfngixy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2chfchkld.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xlukvhva.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rhesufuw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ghrfjjyd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pitfrxwi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tezvtoix.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jzbcbtmb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2buwmpqle.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2heyeokid.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmtjrtxy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xyekfcpk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xcswrvyt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bnzicacp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xomskznw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fmftexyx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qsloqprd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2mtrzshpc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2cchibepz.html


<!-- 参考信息 -->