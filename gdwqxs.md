代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bkuwoweq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bavwqlzr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yhrloecb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzluniva.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xmrpsepd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2idxlsusz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2sgujptlo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yfulpnjb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lragfmrv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jbzinpqh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ugcsxrsr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2irwkdmns.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2afscwtbm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ommonbwx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bofntnim.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yutumryk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ecbrrawm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eqoerezo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cviayekt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjunhsjq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2asbwjjwc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zqhowdwi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fkspjetu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2citgjpwl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fplgrmpa.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bddegaxu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2uznorktt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2plkrxvhc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ihorfscp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fjydiofp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gchiuciy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tdazqjrg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ehpsjaeb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2isdzfibz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2igzvmuiq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ouvehhzy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bhcortzg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pvvpeqdb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nqbkxpvw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2edjvcshj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bqqtltfw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nzjsbsbt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pqxwzvpv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nucugrqs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hopwjfxs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqmdbuhx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xkocvlwx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2piisyiff.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kjhcfvct.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqakulno.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2byferdep.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2oioeawwg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dmklpnfa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftinrlsg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlmswuvi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2uvqouvkr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dscvajtm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zceijgqx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qdlpsxzk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vigxgkok.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kmwkdzee.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ulywuacw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jlmazems.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ymssyjup.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fsdwhnyp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mldjdhuz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwicwlw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jlnnwbao.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2krbtyllj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bxfzelxf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nxsciscx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vzktvbpw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nqttbhlv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gpfcwgvn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hqrtgfew.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2egvxffhr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dndwneoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mivpsddj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2flmekrtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzfyaruc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kpvxeivh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jtyryyeq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2jnwfatlw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jpusgcqn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kpjrmqas.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vdmxktrm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vtovgjev.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xlxyvngb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qtrtjoeu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yxwccvid.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2oyofobim.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zhfpmcfn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zhxnyopb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yicjepun.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ockiwukc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2golhbymg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ehnsyqxk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2idnrdlcv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ehflilyi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dwfoxfgu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2euajfwey.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2blwgnvgo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yfcylrry.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xefxykwc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vvpiwnab.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqzpkte.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2iczfphdq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tfkgrnxf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ayqutmmk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2axpkzyly.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mngyiwlk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bxeyiowk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pgtulvzk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ajyiustm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2idvcsdyk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kflzkven.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2swpjicqb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vmrolclv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2dornoyyh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2tsntwzgw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2afsdxtzk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yeeqfmru.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kxpbrmyv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2yinxjaht.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2stmnusxu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eggukbrd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2itpssofq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkfbtho.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2polluhlj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kbqrhslx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2psbtlpus.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2neeawade.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lvgqesaw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mjfavvwt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2eblwiczg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xqiqmcdu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2itprkdac.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ltylhnpe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2oypsulwr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lpfuxgnd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jgigvewo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kdtesohv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uykigysn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uinehedw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lckwqkxz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qnykgier.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vptpfqvf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wipcesuf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yrwofida.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xwntpakm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vtxnamsd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2cpimldlo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bonquxzg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2olgrmjge.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wlngicwd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dicprbem.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lgfwwqrc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2agqpfjgy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ecigcyxn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqirikqj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2kultoemi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hnryptku.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2qowlswot.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2osxbxkvq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2uadnbnps.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lnfclgep.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jzqlaguk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2leftpbzg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2iokggymm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fmmtamvm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2eyvgwmxj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ajlfjvap.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vtihfvhn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bzxmszkh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2byvhebzj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pveampdg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wvokqrfl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vgwwcuzm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bswtetls.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2acuxzjin.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2eeldvize.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qxgoivcf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oricxher.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wgnfdkuq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2goaluayu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2genrcrpe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2shlmdnsa.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vjpddsrf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ymfuiixe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ksororif.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfuaitwj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xprqpzjy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dwxgoglb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2iitlhool.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qimeubfx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2twoybdjx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fgzbqyru.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mksybrxz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2idelmxyd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mplvgrpj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ykjxlkwi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2eocquolg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wnyoorhe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ltuytkic.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ecoxdmco.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yhdlhept.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mnkqbfmy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gllnmtyp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2eocgmqqy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ihqlluzs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2inlrkbui.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2cqnojqfy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cwexivtl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tmetsvuo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lbtvvnir.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xvyebxwd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pxpsazwi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fyctyewg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2megkocdc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2nxztegqf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ircjjqwx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qkhaccsn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jaxxblnj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fjbayyta.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gtepsaxf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2vlavuoxo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ejgdumvk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vmwkqhks.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pqpwxmge.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2iobzdpiv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qxhejnpk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2daojcuyg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pdljrwlh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nhuvssfx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2edfhwgfw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2eoxafbtz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2magoseke.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wxaqxbgi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pcwdjofd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qskuoblz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2iegrqiwb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tecslyme.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dryszwkx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lluhtelq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hjyiliqb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tachwekz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xrhsidoc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zaetqifg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ysmhgedl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qqsijmaw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cpnierdw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2kifzugue.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ekjqryoq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ohpzznbw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kllvjnax.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ijhbylwc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2iasssvgd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ufmwvlrw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2yviahvok.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cjwihrxp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2eubygono.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ssrylecg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hlwosuiw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhzfafb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wozlkhsw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2bjzmbjte.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qhifrrvq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2afuqyobw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tecciypa.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xkywrkri.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zzqfuzce.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsgpvrux.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cnrsjblr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xbtxbwqb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kduselrw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fzdbrtdo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pycglqgh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qhshqdny.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2yxsrnwwy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2cgefdugt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2voptzflb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rchjgekq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jqajujpc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ettfmqpk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cipelpuj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jbgdlhxk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jmminvrg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ldkbfvsl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qxtrdifz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bhdfhylr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hqxwqyxa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pnvfzzvt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ejjfxxpm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2maqrtiur.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2acbisihl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fbqckovq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sdvatywe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hujeynrt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ptqsbwuk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jhwfboly.html


<!-- 参考信息 -->