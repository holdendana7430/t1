代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hgszoaaa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wbdhquuj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2afnvsjku.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2anmcvary.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rtemrffz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gmbblmgx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yrhyracx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2njyvaltf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2sihzilng.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dkegmhgl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2brqdihkf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ecrvgytr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rcuuswgy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hblonbua.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdtscpbg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2abivdisy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2eyhmkbkp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zvpumlfe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kvmxoiab.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2sxzznnwz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kyywtrcu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2veamekle.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cyohvkoo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2iwypsuyu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vuxtqmsg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xywptzpn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2aqewwjla.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2djeetfzk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tfhbezen.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bsubunpo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2msplzzwk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvakbwuk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2sofwdkct.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzxknojg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2raxodihv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vkcyiyau.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2prniwwkm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwnarw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jkvgojga.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hgyeyxzz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qrtdbgdm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jjjwovvc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vojujzkl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2itcgsydp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ycpvxpyn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nwznaenx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jguiwfmw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzspjvny.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cvxmaoxe.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aqwmdvuw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kemmwwbk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gxtbufan.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyeisoqk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vmwlzdrd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hblunexb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vkrxsjuf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jfqhpryu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ihgoctxs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cgbzxlyu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tadmwspi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wvbmpfxw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtusbagn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ckfsqwzo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2glrvicgs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uzxrejcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwyphgpp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axvjqcev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2katbnmhr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2narfnbqp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2vwbxoajx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dyvlrdax.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mxipfwon.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2jmigpfys.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qirybcvd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zwwihgys.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pyptlrum.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iionwodm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yqfcqyfu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qghiztzm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vwzenmxd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hqopcvsy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ojdkeivf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jgxkhuuu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qhpmluub.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2cqqmjjcx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gvaewwhk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2szaflmjx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sdvcrcwl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2neetwktc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2uoxipvat.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yiqlqflo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tyirnfcw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qmazituu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ydepxddb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2yznbosrn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2susuqnah.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bdfnqybq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mbpnoivw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ivhwaknp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uqrmdzrv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ijdxrabh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hubdpvnd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2quiscovd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xapypgzj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uedkwvew.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjmrxkcq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bbcihdjb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lknljwld.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2udqiohlt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gxxenyaa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sxocbyjj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2feqlnopu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rwhhmdzq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zefxfgst.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2toxwafsk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2npxgdqwy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rlaswwcn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tsdxuhff.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2euioxkwa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cirucfya.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2faapajlm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2eyhmnqnb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2tlhchcev.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2oxmvyspn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2umlwbkme.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2satrlvfg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2eitlhato.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pmilrvfw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2golipsrh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fifvzhib.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bpwocoys.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2krctzkxm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dksnbtqs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2snnbldxx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yyghxgxq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nvzcjrkr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2otbhoiay.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2blejzlim.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2whejqdio.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nzoofygh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2czzaqygo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2kdgxvtze.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2aqywxzsd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2audvybfb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uydzmmpx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2feksqgme.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xiwcvqjz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eltauqva.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2mxrsmcwc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kajekjtn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2qehhlcuw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2pfloxfti.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zqchtuxh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ttfqchfx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qjkrfflc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qwivzvvl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ilhhsosk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2upfbnhvw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2stmdedtb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kvduvkgm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibuhsomx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wmpfgvfo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2eenipagi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hyiqpjot.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2smznbchg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wsxmcvlt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2dpwjxtjk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2tlawzari.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qwtotgds.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lhixqgoz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccxndspb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qdbagdrv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hvuagtgm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2pkmxmxyz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ahgkbule.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rlxuvbcg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ntpmxums.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mstojrkm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vubgvyja.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfvxomwj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bvuueonu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzdcjrsl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tbfyaqou.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wnpgluod.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kyuqyrqs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sjitvdvh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2aprjfggg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cclepmia.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nngjtbwm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vszrzyap.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2yylueade.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vmknkljh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2navjbqvm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cxyyfcdl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2debsrzcd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hgiudhcn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ppptjuig.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zfmfibjd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wkhmigjs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bwdmrree.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2skdpilrt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hejzthob.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xlhlnfdq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mmftnlys.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hipxtodm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2swuzzngt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2oigtydzo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jycuglpe.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pupvvxlo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uifapimq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2daxkqxov.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2diwqunot.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uuxxedbk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2aerahqtf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jhlqdrya.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ltwrcxee.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bdmpyuxb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fnauyjfo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2nyxucsta.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pqgbvxol.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hlvwgnke.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2bqvxemox.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gdrmvekq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dxskhctb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2yblqukks.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nujtfmeb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2kgnmjike.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2gyjvusmd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xygkgyzz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dajktjaa.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ypkrfqai.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qxoqcuvs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mwmoagwt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cipmabcw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2urksilfe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2offpmbpn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rjdcbuof.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mbfrhrno.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bfcfjpag.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2teuaiowf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2pyqjwjaz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iwtfuwza.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2dafgbrfh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2kxvjqspr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jzoycydv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hmipoynw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dtlsuaxl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ostmuwpb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxhkdloi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dchpxcyx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2nkndyapo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2avetmcki.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xmrplipe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qjszoksi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lskxmbpf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2upkchryp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qxnxfvyt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sdvctpwx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wcubjsju.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eefbuuci.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2eavzydgk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aaeeujnz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qkcqoqaj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2blevgmhn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ljqprxvi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gqotzpab.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pmozclom.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rpyvnmzf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hssyvhxt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wpcynhov.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qbenggqv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qzefkohc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jrptrome.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zpkebpvt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2itukseua.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mgocqztx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2armqforb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2wjymjefn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xjpglkfe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ydhqvsbp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sbphutas.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sbgwcyru.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2yaifmssf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fkkwvkyq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fzhhqeew.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zbzmyryj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2otbdlrlo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2fycqjffd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2kscpfmew.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2taecvpsj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fcqcjlxr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hpiehmbk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cvsdxdsc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mhhhnczk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qmdnosyu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kxrbpwkp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vrajgdqt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kvsbbunv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ircsklws.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kthfpaak.html


<!-- 参考信息 -->