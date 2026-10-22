代发 wailian999

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rwkdwoxa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2amfcwbkz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vizwanxd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2idktpblt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2izgjkctn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2psrlvatk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2sekzfjmm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mhpigukg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2noenqidj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rmppmeqn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tujnpqag.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mxzmqtfg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kzjuebky.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jerwjnfq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kcojwpfy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2khvexayz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dlhxlgnr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2smrqbkew.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2glusfpqt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wsmwocgy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ywsurcdv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fnnjjzpv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qvwjscnn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bngebbln.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kmdzqvoq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2khkkysrh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eaaubybg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2aovlkyuz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dgglpbyq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2blycrflh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2tzkaylww.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyppktlh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2oyjbqvdm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wqwgnwts.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ccmnplqi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dgvqpdjd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2brjjnjpm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrzcspwa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fyespgge.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ztbckjgc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zbhrbxqq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aymlxmyo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ptymkdwg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kbrhkogj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qdemubof.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wcqwbnlk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wshbuumi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xqlyfpik.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gcvspavw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hdzoajdx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vbmcgspd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kmkwhkyo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lkoamvtp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vbxowwbt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2biagqlxq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2iqkncxlx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xfwvyarm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yuxhbdtf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lbgofmxi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fhhplfzr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mlaztwwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epsplwqb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uxjwvgme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvjjsuvd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cvukpxuv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2yatgnsef.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ceueoqjr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tspwwsdf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yarikzhz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yrjrxzns.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qshhilfu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lrelbduf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wibrnysg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cvesqtxa.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mssvttzf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iqdbvfqv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2llafexjx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jsscacnv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xxfzgcxt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vryhkxlk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mmkxwicy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bitrzohn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lteqbekj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pklsolbr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2guydbujk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qotlyszb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rqlvhzlt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zyozzyop.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bsbppeea.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmtvlzd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rqbrgqdb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uxdevdrj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vwntpdkj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ohkcppnh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2rlugytsy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cuuuikbm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xbjbxikv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2eiuovxdb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vgiqnira.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wcwommlx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dnzcvxtw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcglkmsm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fhmtwuqn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2menftzzj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cmotymhs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vfvbmkhr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2antcjiik.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2opypiego.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2babyojsl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qeforioo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cmawctod.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kxyevdro.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dhjgxwxr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xiahiydr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zoflweaa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tqlhpisr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yobzznrg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qxxvzirv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2csnblhnd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2myjnypql.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2grevirmk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fdfcnogx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nrhocyaw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vosysfus.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pyyhmzgx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uzfszucd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2heiwcmhn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2suskyzqi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cwcdruho.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2klkcpnvx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fqdjjeql.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jloedijh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2otidsshi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wfhooxyw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tkgkyfjj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wepqzqat.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tybukyzi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rfzbpwad.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jdkpypii.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2umritzgo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2flkhwdll.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ntdwaagt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mbxuckla.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mxbjypjq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ntobbmnr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2azdvmgsp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2csbhrjgr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2eqmatsvu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pcqibmjq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xpicklbb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2awhmtfed.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yficvdpc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ehkgsodg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lortnteo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ythszpjo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jwornyzf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ojgsstwr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nzwwjqqw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ixodiyaw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2olljilkf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2voelzntx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pppblcoh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2sstqjovl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nxtreviy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ayqzknuu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nvfimmxz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bghwvhna.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ghtttjsa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lywclrme.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2oypkbofx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aihhxggv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xuizhllf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bblelzff.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2npeezios.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yoyrbbfv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2srfgqbbc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wdgvtoel.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fytyuyiq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uhroozjw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yfhdftxb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rwqichls.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pmlrzits.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tgrqwuif.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ivngncre.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kocqqmeh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfekojxe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2rwdusecm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ermkulwb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2memqvsvq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qctitkqc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ebjcnvmj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2pcgugsmb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rgimunwp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hccegasb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tumivhlw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yblnulea.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ngdmapbq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fsuiyshd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lpcsjynj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2prjlsjcn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xqezoaia.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2frxopmka.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2racpcanb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2flaxmvmr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fenbcthc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jezwnrqf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kqvdrjxk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gjdtrpzk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2roxlpoww.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sxqtrtij.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2djjwjwbl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2hnoxxdcz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mptupequ.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zfuoqfcm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2iprtylof.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sflfbkwq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ouarsbiu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2gfclkrir.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qonkbdwo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vgzoccto.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rfjkjsuh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rbflgphd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ntukawdh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2nrqoywov.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2khgstwyz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2drrxzoew.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2lpxstnfl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ywjaitml.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yhlezjgn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2narslivk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hxvvjzeb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2hrtpauky.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jsiovfcp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ljyzqhta.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2uhjihjrc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ymloubul.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wfemfqem.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mtrbffkj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ccksbvfk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2tldbpqbq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lwkyevnh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ovshzrnm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pggikund.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cdfhtetz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zysmvpxc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cqjwmutn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qvohbgdo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ykomcswp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2iezlhxjx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lfknylcs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgypfpxg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2czxvpsyk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2usqipdvk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vhqgyoii.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2jeqwgdla.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbrqaisa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rtvtrhxe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ggylruee.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xueipsqs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hixoauhd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ehlhndmv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wbmsmlqu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kevnwxjg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jvqnyygv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uztyfajk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2bsahycxg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2enmgwofh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ukuuzssw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2skenbdvo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2dsjjmuuu.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ptxdpwuj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fgyokttj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ftqdqcgq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xcpieayl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kvukhjqs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2awhelsup.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lreowmku.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cbxouxth.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pmcobqfp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gtgajevu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dgzgbnay.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2sfncsgnn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qcnxprdo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2irncggrs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rrelvpdk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xhcqhfuc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2gcasqmev.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2czdmuwal.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2iolwhztt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pucvjzzo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fixqmgqq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qyltqjzu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2udcaoerq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cfwqiexv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dksmjsyp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uhplhkeo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tbjwaqtr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nnhujyhg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vprdqdwe.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2kwobwsra.html


<!-- 参考信息 -->