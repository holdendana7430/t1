代发 wailian999

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwfcfcrw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jxlwgzyh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lvnxqzew.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yeinkulb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fprewoxw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wopwuetc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3flziqxbq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jnskkltt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mgwwsdmq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rwdzijok.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yjqogjwb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xvnqyjju.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lhzcmxfc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wlpivgfh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ycdcfoxz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mkivfsib.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jirjuqib.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wbloczqq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqmoaimi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3imbcuvvi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3horftndq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hcsfqqfz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vsjuxmrc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3adxduzgg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3knapkxba.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vtydqumm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qeicvuxq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pideemrb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gdbkazxe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qhynrrce.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lgoppbdo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xigfelrq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wzskpwuw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ekxfqcea.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zxkwfvtp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3laqcexss.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bqjadjwz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cpxjjlcl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cocsbltw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rdbttzpu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3shnfzxux.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qfypteth.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ntwfknhh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xlymmkme.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cadgoape.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfssfgrj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kxvcbxui.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ndzizdbp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pyerldpc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3iexuehoj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gtcwiddk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3agrykfpk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pcbvarim.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3alomntcw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbqpkkbq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ashbgcvy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kpjfqzwu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ktfgvaei.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ugwnolva.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qkwsmccm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qheezmmq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xtwkzxwv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iribvkre.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3loorjjiw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgavrgy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lnyehoqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuyvfpsc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xktsjcte.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3giqwmzul.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3idjwsgnu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ysqhlcsc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3baltzyme.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nchiiehv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zteqnwku.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uwpauaml.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rxzumeox.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pjhgbxcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfxfpswq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rceggjxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sglwnksm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jvbiwodu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dfrcjblx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3eznssltk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gaefbbte.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uuujroul.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xtyywjie.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3urdwpafa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zfnmehlt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xwaelvvm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xbtudwzr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgpnce.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ottdiagq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3aqgtdjbb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3khbiqcqt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3omblfbhl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3kfvcuxxk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gzsbnvub.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ouahrtiy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mnciubuo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3flptyjqh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nosctdmb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xrncvacz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vwxzfchu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbnskip.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3aljhuhvf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sqlgpzkk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qriymywm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iehpriuw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xohdxpim.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qpxckidd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wnyggitw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ozmsemxu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vydylxfg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3puzjxeuv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3iuzcdujq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eojnxulf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3yppxkoae.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mctknqnw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dvqvcqzi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3aisqsalz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pcpyqlyq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bzvazjws.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gqmhhmnj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rcllzmwa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dmxlknmo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ychwtqzq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dogrefda.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yrrlpkcn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3imfrkyrv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xansdtgg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dqcgmcrv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3glqkcqmg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3baawykxn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bszcqlei.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqaarg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vixjcxwn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dxzqfzmn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qqulebvc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cnvchgfd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ggysepnr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xtryahzx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fuqzegvj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hpltqqyl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3whbwtnkm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ojtwjzti.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3iqkmjpod.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bhibfpki.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zbrzootm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ayirwxni.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wmoobhwm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rtwbrfxp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqjvhrc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qzfheuje.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3lcidagom.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qvwbvdza.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3twtrsrqx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gcajqhfm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3popyrlpw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fyebcqxa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oqagkujw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3zyvgluze.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hbuuaziw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3cjyyiips.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3sxhyhuik.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gzfcbzhs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xwthshss.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nxkekrhz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mmvlorpq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wqhhklcu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3keyiggmf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ejsgmdat.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3osbjskil.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rgaztkqm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ejktihxg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3oalhphvb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wcogivcf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kwczjlqb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3mbvtmmcy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3llxrazql.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prvtuxnq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xhclqqwg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ayztlgel.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3elihpexc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3shsaoaxr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3huohyfuk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3cyxqtron.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wxdjzcmz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3uzuddmyw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3utpyhvsu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mbvpmnje.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3godtkngs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvibqheo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vccqgyeo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxxdwnty.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pqjmvqbg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3adtbzdkz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ehpncaks.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yqvatbdz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kkinbsfg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3rakuytnd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3haxmjcrs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3igjhwzie.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jsxctjxo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3exfuoxyq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3eqrbrybj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qkblvdeu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ouqlrjzr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gaipysbx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3otklwtpc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wutsihii.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3iqdpynri.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3byqpncmb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qrkzfdew.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3abcpijtb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3vowtilrh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3igrqtxdb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3kipuifau.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rsxexroh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3mjcvzixq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oimadcva.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3craymxkx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vxextpvh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ezyvmacx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zzundobm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dwoupyzt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zazasuil.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kzlltldt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3favusjyt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jqpwwdbx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hjdrswwb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3guklgfls.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mizkgrqu.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3andyytqf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ejqhmntb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rghsdzhu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jtmkurjb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xzuojzdx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zgpdzeze.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3futnvdvo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3obgqisko.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3nttaqqpz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nepkmdqn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3liwrfhdr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3yfyzbjau.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3pzpqdgwn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hafmcnfe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xrwpxdyx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qcsmsbva.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fngaegor.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3kybgaygo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xjczubhh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fsgdxjfd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3narsvjum.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zxarodpg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gfghwjwo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rfxfclra.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gthrrgkg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yygunpls.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bpabjgdi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gpszndzb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lcnmqwcw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lhzvdact.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vxalrcen.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3usxdhnlr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qvevskmt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vqjnrqsu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qpzwpmlx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3orzzsrue.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dpcoltpn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3stimijcu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3eevtvmmm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3skthxeru.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mreujthn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ksswerwr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vyymmyag.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qgcuzvhg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ofgsqkcn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3klqmqjsv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ptattprk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kszmfnes.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qflxheqt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kmhvjics.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zgrzqpsr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fnirygch.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lfuahtqp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kagovqsr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ocdbqucv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dqokhgpi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rrxhcpvb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pzfxgqrz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3atkdhrzq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sodcbjhm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ixpxgnmv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yrlpaiav.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3eyhjulri.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fqaxqtwv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pscsyofn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mshrtmfa.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lfbyqiph.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3tkjcfdun.html


<!-- 参考信息 -->