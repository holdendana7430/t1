代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hffgzznh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2daukgzle.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ktytznro.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ukmgevhf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iwapsamu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wzwljbtt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lzuxfbja.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2atqqcrrr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hugcfizb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rkefibzg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pwghgjrh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sxxivsvf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ljpeqhpx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ofpxtlcb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tlksvokn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ljavirpv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kjoqtlta.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2psnosasc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xzlbtslq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rcoifblk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pwjjvnoi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jbwoanev.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ekjdoxdc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fexvdqkl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mmrnytpz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pflxiztg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kkggwkxo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2obbskomq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2uelyzmlk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lfknphor.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2btfxfjsc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wmpjcwmt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ebnpkrfc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jsfnfptb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rsuuduze.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wmclhvyz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vvjeaemb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ebzjwbsg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qojgmaev.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2aymdzpkr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lwjfweco.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2alrahfiz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2blvnpqpl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pcjwzyjd.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kbelhjwy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tbdjptoe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2djqoglut.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2omohsvle.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mtwnybsf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gaasnxaw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ndresdif.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gqosufgv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rojhzgtp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mabargvu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jtywchdr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2csvlrvud.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ouklvqzd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mkwtvcxn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rmfkexqp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2abaivvit.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2sorxyqcw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2khunacbq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2guttdlmz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pvguhitn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zkllsvri.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qtkljjia.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vpuudhsf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dwawruza.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2skpdwrzm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2prlachas.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lhgxitsu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2sknrbpen.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gbllrrqn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2etelggsy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zusaaqqr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yetcucys.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zwbhzuik.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pselufyp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vgceqdjs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2trigfoow.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2snrlqlxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olkvhqwh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbnlmwrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgrcstyg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2papedwrc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qwjuezqw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kpkaxsbp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2yernmwwt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vdlmzvoj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2owjyqjts.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ucftxots.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lwiauosa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qkevsrcv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2eecwiwuh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rnwkuyad.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ljjlacjq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2edjkcpll.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lkpxazrp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gsizusmf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ouczdrxa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2efsepxwv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kztvltxr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nathudvg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dylqllon.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ygtvksgo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tighpxxh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2poziccwj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvvadgae.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wczeboir.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qztrrypi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tpqlalbt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lhlzegex.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pvjjwxms.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uvwkbxvl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qzlaqwmu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pgvpwrpk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xggagpfm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qpxmuwoy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2yxcglttg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ncyllqft.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nhbmxtyf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwokvxc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rqeyxsfj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2svmqfevw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fpiwzwtl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2imjjjqfq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2txqdybbx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2evpzfmff.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ymebbifx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vfjujmtb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zijhbxee.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2crjlfohn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gckxqtvu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2boqyziez.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ryhvwskj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2iohunkxs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xnpyytll.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2llwqpspi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jugyymrs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dazopinu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xydyxjof.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2heldrwzl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rproztzv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ywbqtujb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kmtohmua.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2uhtmehvi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ockgilus.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ofgpsiji.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vdmyvblp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ucksozpr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2phgbqijq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hwsudbvy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kgrzuxeq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ynoxxdts.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ozwtbamd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2uipsiijp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hjaqtooo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rnggeakd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gyomsnlp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xpiibmcw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2afcvylsw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2yskzhlvi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ecreilte.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbjqxunm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zqipbreg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nnpghtrj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xihglmba.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xjxtosqf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dfbbzfkq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mftatvit.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgavnymr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jxiuegcj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2puyowets.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bgtxwavl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2meadkhoq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mozqkzmi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bswkdyvp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ckqpzuiu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2yfjucknb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzdffizv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tmcwpilv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wizgpntd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nofuyawi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvzihzsn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tngbxjvl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kmjseape.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ojgetgdi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xwinmtja.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jwrhtndm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tesbrjqb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2drosfhmn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ioohifjq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ulpdcykh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kdfopwpe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fonthvom.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgumufsw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hyaptiro.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fzeszqcx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mwftftza.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mpubhbfu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qcyjqpal.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rajynjxu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bkpedtlj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fyemyvlm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cfnpargx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jyatnhhd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dbbydqkb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ogedrwes.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2nqbmhreh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nxuuxidx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kgfbwqat.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2cjuhjtnk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vvxeqtsb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yzhoermf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gzzjlhtf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lkurokwp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2rxcqxdcs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qmkbyixq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qofinhrn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nttualud.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2aptumvnj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2fqceztkt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vwpkwjpv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hlahbqfr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ixschrot.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oxyyzmyn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kwzqtdzi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2noromzvk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xmslwalo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ivsknxfc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fzasrryz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ipddvjtq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jbrewlno.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gbnowmbz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zfdfsrhb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ipkiyqrq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2afwjqpbk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2atjcdqgc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ikzsjqzc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2chrghykf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2cwmysryl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2deyagnzp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tlkwwtie.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2uqyeueat.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nzirclsb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qvqbiyyb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2goqxuelq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2okubkwej.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tuelbsvc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jbwjltle.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rionktkw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rxuwncmq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2admtsygd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zpbclefs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ajbfmdzn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2flbpewtg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yfiizmoa.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2aczawzkp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ritczxty.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pzocfrlc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2fcvrghtd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qddwjitg.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2dqpysfjh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmoarac.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iqcfajuy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ohgnjaeh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2acnbtnbg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxtqezva.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rdgqmztx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cfetjegt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tdxmramx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xiuoaacg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lcqmwsmc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2okubbkto.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wqwsciyl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlirpjbr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2apbecbzr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2itqbyhze.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xdwlqtxy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hmidexhc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2epmqomjh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ismzgdhj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2scstnrkp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ufmwlngq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kzjazliu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2osubhfmn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2obaspzfk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2phmgvbhp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jtcvucdy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2teawtrsh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2kgbafnsf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bljxcsce.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2umakxitz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lernkeli.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nstyrqzn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dprcprfe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pmgzxqxs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjxhkkt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ibidokmd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2oqeejind.html


<!-- 参考信息 -->