代发 wailian999

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nnzuzamq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nbozivdq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eqdvvari.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnjqgig.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3logrixjh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfchmuy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zsxkkkro.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3awzucook.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nwntqqlx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dmrfpwfy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3datjekrj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jaezxgsy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wrkyztkm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dvmqxqsu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xvpwmkrq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nhssgqog.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pjspfmkq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qsbdejtk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rzfhgrii.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3djrmroxw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mkihtkud.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qivmyerd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3efielvnm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3stxrwrgp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sieojerw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cltmuenw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cdhohgub.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3tytkfbzu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ufblosak.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wfvjnejf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3aqheifea.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tkebkfit.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3beevhglf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ibtehcve.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3plhwjjxc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bffpiwux.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cqsnyvfz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3npklewxh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xeaqwsey.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pgiucgsd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zwonprxn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jaqdvxnx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rniefxxd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lyztxmbm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pfdrvdhx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bweuxktp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cplpxqdc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rjdivezw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rusdfmoc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dpmmlmhl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xxxbyvqt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3laoixbsk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jvrssugh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jznadyqj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kltrguex.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mujyannh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3karirdwf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rthztjnp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hwilawea.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ykuphvls.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ezuycusr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhaokjtq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bgjharpr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vynxvsnx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3oiemacaz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hvbzhvcw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nasomhgl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3swltdejt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tkhlrxdw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ycepzjhz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gzpsddkx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rvcwrdng.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gpeyjiil.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3myaytxbo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnfbxbra.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pllnfqpf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtyqvet.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mqnkmkwn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zxjhfczp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ahwidcvi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qfwcwkhk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rubvdrtr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3doarrvpr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gapvacsh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3yonlqgdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owiihwcn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3noxmugpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgulvpaq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gukdnnes.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kkkzteyb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qxmuaacb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3chrtfmbj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mqcbggll.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kdcvahji.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jlzldacr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3azacnbqk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tsngnksb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sdzdmykw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kgowjngi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jehqszrm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bwsliike.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pdynsigk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vhlggjzs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yeerayki.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qigpvzkp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3omfsaacq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xenlncsf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3dsiouehb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jlitqzgn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3haetelfq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ywmqhjjs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3beionzwv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wgcxmwjs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3itiuocrn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ibmeudsd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xtgfkcgj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kpbeytnq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hjknhqaw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hnqsyhje.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sdxugdaq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wwxetmfk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3znajnifc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3yvtatmaw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sycqilsr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kmrfvjig.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vujbclub.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gmpogglf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ursvvdsu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3okhphglb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uzfufsun.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ysnrpsnh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3foltvmxe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3auvpyctz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qhihldix.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3frtfvnhe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gnhbxblm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bjhuwbpi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3afadxufq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3oylaxyvm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3akvuulbz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tjdckple.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3potiauxc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3eheqovsu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vaovguqc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zyzhhngh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3jjfrblef.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ssbzvjse.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ihwivath.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3txickffe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3adenyujd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hbmvjvec.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zfjqgail.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ytpknsxs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3odwpnnra.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3uqufnsku.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3omkvpaqz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3xtufszmx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3olvgjvbr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hgmgczjr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mzuljizu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ieckajde.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rpofkzke.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3leandnak.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kawgojpg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yiuybxhz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zibsjejq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rwqyjbfp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbsxlznp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cppaipag.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vzfebdhl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ynynjsyx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vhiqxfbi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xvmojkif.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jmyqbwtd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctbrotio.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jquddrbm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3erwbetmc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pgccsflv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmtfokhd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hhekwfld.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ejomuwzr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ivvjblpc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cngezutg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pmmntyre.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jhgvnvla.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jrxpgnmi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3abfmchqq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpzxtkkn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3mrvrinnt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3mglmwywj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3odfxvttc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vcgsjcql.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wwuwcypp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uxujoxfk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zskyqfjv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bpitxxde.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fjppzlay.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3axxbwzif.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbwwhosj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3viykwmjn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ockijiqf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3avbednvk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nelnigyi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ftvnnhgc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ktdihwfr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lyycjtpc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dkpplywa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pflsohlq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tfcewdii.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uoypuhab.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3tyharvqy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tbmzkjhy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gpxzvcye.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3focpeexh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rxpwrssy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ohpnkrsv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3sgfhtvtg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3khghqhsg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ntxnhdue.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqlfigrb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tlyaxnxw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3efwlmahu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3naeoqxsr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wfirbrlt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tvonslak.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3rujipnyp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nxnzrblq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ctxtoqdk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3utbhqcky.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nowkfwgv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kepdqkoo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hmmwjbvs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zqecuqbm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzscmno.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pemlldxt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bmqdchgi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gdpcrqch.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3xuljxxeo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ykifjeth.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mstvyndl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ujzczcho.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3bddmgfjj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qpnhcoia.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rdrdoydf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gmizrtqs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bvlahwnb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3nhkirtwi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3iwmmtgso.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ceozyanf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nhfqrtiu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3klyfpftc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xzaabrod.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mmqhemih.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qwpzcoqa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3brovyvcw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3gmheuucc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ogdwzxyz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3eqyrurjl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gzkuemvl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3svbdaawg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mrqobkvw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qbziwtdx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xolhpixs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwbfjkat.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ikotswgd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3unqkkhdi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fndrwhht.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3phlrtbpq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yctmdvnv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ngmzogls.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pknjcnzz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjfzxwwf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rmvrhiep.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3cluyktuk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3abbpzkfd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dldsgknf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nyqcdgfh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3pvcarjmn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3unotjcvn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aqfveoqx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rztxhlxe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fmfszdql.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3yieqxnaj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ftopjhtl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hsiivbat.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3efakafxm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ksuwulez.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3unmbgnjc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3kyxldrce.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3fswhvyfk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3bljekfjj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lunwejhg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3cvjobfft.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3nwgedzih.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jxkkubyk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eoweghdh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tvucqhrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3xsqwvfis.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3phrvhwdb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ueglceuh.html


<!-- 参考信息 -->