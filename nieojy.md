代发 wailian999

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fsmrwhyy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kklseejw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsydqlyx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2llwejcao.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sajhbywa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2aozujtoy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2blmkpqlg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2hzcptore.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xekxdukc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ayfpoogv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2iilvsjwc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kmzuzrse.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ahkrrvkd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2veidwrda.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ravaguwo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ayumfuib.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ypfsakdh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jdffgmth.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cjyugigj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsmblcmg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jdxafczy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvmttlqc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iwvpvant.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pruxpvwl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xpoozqqo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmlllnjg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2devcuodv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jjrrwaho.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2aiclxmrw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eyutlisb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ljcqofyd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2grxposlh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2atajyfxq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vyrwpgue.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2atdnflus.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2umvtkjvt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2darvaicm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jtgndafz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gnulcqjb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hgeioxdd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tvbscnmi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ntdcvdto.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2furpuvpi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hlvakdzx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cbwlumif.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rcjvryik.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wozaywnf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bpbztkvp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mpfoehof.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ifsharam.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2adxroqlu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ppfgzecc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cattsrzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukvescrt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bosbylsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqjrsfwk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rwbigaqo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2axlmtvyg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2emrcmszr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qhbszain.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tthzadzm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zsnoroso.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lzldtntw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2kgpxubnx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xcyjqkpc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rgbpnxqy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2haqziazj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fkczscaf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ynujvrap.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ynxxisud.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nirvaucx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dwwqerli.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2avaqbnhi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rdmbrlde.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2chdzlzve.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aasfgvij.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qvqyhbfk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shumwocf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nnadfliu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2teqbmmoo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bnxthxms.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wposqipn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ekebsxyx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2drtramgc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wblndcip.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bqyfflbo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ffyehfqq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kmonwyzh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cyswuewq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bpnqszss.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tergkjlw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nelavixl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2umqigqzu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fmdempig.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mnwdmwoo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2atiirlsm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zhykpspz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2imovtwos.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ilqifyfm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cvsvbtst.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkvtrltj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qlzykkzw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2aowzjnjf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2becbhaxv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bszuumjm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzzrjqa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rahggwod.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qvugahzg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lcjjfsfc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wifjivlf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rqmrfvzz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nksoxixx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hbeatuox.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yosenrug.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hdzrfjaz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cdjhwrbp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bjovjswj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kxhfbltf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gxbsfzmw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lnbilifi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rlgjubfn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ohvplxef.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ukawohnz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2agsegjio.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gxitwjjh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2mchidnoq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mfwvdyfh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lmtuuijl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2uqbchvxo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wuirsghq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ewavlfrp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2oygaohzl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nizpgyia.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wujehwze.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qxepuhvx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ittefrfa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jimphkwl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ipsrwqff.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2odsodotc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nbrnmcck.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pgqrvdjs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jzrvegzu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfqkmwtq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mbdcqiad.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2dqprpitu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2otegxnjt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cukjvduq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qznatqmx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rfensefb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2dhdcxkhi.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jkjxmfzb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2djazvuwv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2iajykmuj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2iaxivnus.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ghbwjfad.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbxoljar.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qgkvbrhn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nrnleodt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qawgbfle.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2prkvybvq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jtiihiwt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2sniaqpni.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2faesvyin.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2flholkwq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jnxqvagt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2anrrzucj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cmztebpy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdvsmfr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cmdhieyb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tfcpxaic.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2tgodjsxn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yhovhrde.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dajltoxu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fdebjvtz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wnchfgnq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2pmukewsi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mydxznqq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tpxpnhga.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nxzbspas.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2cyxwulou.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ytvtebyp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pxseeflb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cadktxoi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2onhtzcmr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qckdyjmq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gcruafwm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2mbttggma.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2igzuguhg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ravwrvai.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2uyohaawz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ymerkuap.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lgixybbt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ttgtfyut.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dpznmztt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hlrlkjjh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ywmreqeq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zfhbpqgw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wtoeazjc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2pulzknwk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gdhhacmk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2wwjdyxio.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2unqpyxwp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2djwwchuu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mpihbneu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bzdlezee.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nhhhrzqs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pcorozuq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2klrkcxka.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xytugonw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tmeyevbb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2akoxerhs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zpoeellc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2blktcbte.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bagrxnzx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bdhtcvvi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ctnebciq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2koyczeuy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vuydetcr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ldizbtam.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ehzllhkj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tpkaeoxr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iwtaffzf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ketptuap.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cfsvtgoa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nwtwxbwn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tknfxlyl.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ogigmbpi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2etcxhhlu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cbplpvev.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nmtwcsau.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2tthbtoyg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2arsdndxz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hlwegrgp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kiavtpah.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cfpshewu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ygclugyf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jnnxtqho.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ysgjqscx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qcnpeiwq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hgumgnbp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nhgcpxiu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qtkzacql.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xngrmowl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2segbdglz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wucqrunu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kxyfgpbx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xylynukp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxorkeek.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nqukvodt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nbbollug.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qbpnztkl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ruqwbnrq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2hfexheai.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2knkkijei.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bzfaxsjx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lchqimoh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jgwlydma.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2epebdwxt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ifgvresj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qgjyonma.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ghauqoxr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2pblczgsm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mzgkgzxf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bprweeiq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vffqwnud.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2utopzijb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ovlmkrgy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xlhsqkmy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cmswjgjx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2udmikwsl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fsumffta.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ahpzblyr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vadqcywa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rnezptge.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2unumleqs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2hbalzhlm.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zsflihvz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rehqjtqo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kjctcbsk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zjiyrfnd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2snrgoozr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dxbuxsnj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fhcdpncw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vjjzzfvj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fbqphxxt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sabasvpx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pvdgfdza.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qdtqcqqe.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rxkbqifs.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2wehwgvvl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nbdigsqy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mksixgay.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zxfrfkmg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2hecsppii.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2vaermlvp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ftcuyryl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igfhkxtw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tujiihbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltyvetaj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ltlxbpcv.html


<!-- 参考信息 -->