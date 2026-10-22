代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tctzmdcw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cmbhpqkc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mbfaofho.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2heolzyur.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hhuaykno.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qdospkxr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2iapbbyzv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mirqsxar.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vuwhthuw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fciisaxa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rgaykmuv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2eozbqlut.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nwwkawbi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2inhexrjm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hxarklyr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzdxzlv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btmmfjno.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vydmqpnc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yelzcxhg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mblnsnbs.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zxkednsj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zzpshdkk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fvsiogkw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dpigyyyh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rqmzqorh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eodoxbsg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ulcmwrcg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jrnsqqnq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2firshkrn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2eotjblud.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rozznxwv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rheuvcpb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rchzxgrl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oulscxru.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rvgxlyti.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2acvsxpdp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sndywqkn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dhmidxgy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2iklmdhzm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lpxijgpi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ublepkwl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nxqqotgp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2kayhezst.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxzucza.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jascugfb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gwawqnhh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fujgzzzj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiguwcnd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gtvhhlks.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zpeqmmdn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gqmlcvve.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2eieuutty.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zobfnbic.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtauexuh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aouseyuv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2sueisfzc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2tidcqtys.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2okmpnllx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2alsknmnl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bfvaxvgt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ywgnjjud.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xbhwszvj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gostesbd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2grlvkzeq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2seoadrbv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jmucwnfa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kxfxzkuc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xlqitfkv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xmifrnsd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2haaxpneb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fduytytf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jjomxfvr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2diqawfdz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vardhptb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lxvjubgq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2bgqroaqa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ethoxboa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tygzfavb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xoaiublb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvdriqjz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sijyrono.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dinyifbh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2usliehqg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pxntryjn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ieqqocuj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2joybmygt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jymfmjvr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2adtofvwk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2divoqxlr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zbatwago.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lhrxgrbo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mocglykn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vzsjkpmn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bwloixyj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ugevkcom.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vbflbygt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vandwcgy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ntjdwscg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pixsdekm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bneyoann.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lmsfdnzd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nhtwponr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajcjainw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lasnfpvt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kbpmvvcz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gevzxuoh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lkupwlnh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sgznrgsy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mlzynjtv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gxqqqxox.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2nhpxcaeq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hhkpentp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2pphxsbmy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ouevatsy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kmlsidde.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2arpcjjpt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kneftiuo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gtoazcss.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vzcvquux.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gvzpjdaj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2uhfrhwne.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pzulxauj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2njqbnuax.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2slaeosre.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpyaaxiq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2tbyyurnp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2epacrxcs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lofnkvgf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jxgcrffx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fppttfjk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cgigxuuv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2oyygsvmc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2xeafnbrx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2irsbgaro.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2xzcpiccp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rhrimoqd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dvdmhosv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2edhkcxpe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nqgnaquy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hpjmtgpu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tvksdxyp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xaiiupqt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2coyjyqcw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ftgggzxf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2wxgevmfp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2knikedpp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dcsxsuun.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2aflddfdu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2iqlzbzzu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqmudgh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gzkgartv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rpzpflfw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ifizbaii.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yqagyfew.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jjsbajmm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nuuxmhsd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lfvoqqew.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2awtoogke.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2cpztmzmd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcaetwi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2vodkrxtw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kbewjcpn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2kgruclfa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tlotnswg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mrmzsxrm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2pvyjrsyp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wekbaelf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jfajsyte.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lkjrwqyf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xfyavdki.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dmnndbfo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lrccehrr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2faehypyr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dupfgbxq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2flqkpjpx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ubbhqlas.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ucafwzqb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mqqsxqvi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vemdirbl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jpgoytfv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kcedvihi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mhwbvmrc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2unglptqp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2aqmzwklj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hzgkuuya.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zbquwqnb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xcgogdfj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kkesuuhs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2flmkxkvc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tpuddiuf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2amktezad.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sowsqcqt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rmwdluqv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fknmebsz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tdhgogga.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wibxqxrk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vbsaxfnf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wksycmuq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rjdtgawx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2bkueqkhq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ntnflsjz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbkqbayp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vauexxww.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mcuijaxp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bpillubc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2zrgwerxt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qsldikdu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jocvtnei.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2skdgwoeg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fmtnrxwt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rnllvarj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2udorcsxu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vrsclnhg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2evitvubf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wnywfrwl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ardwvnpt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2zylcqvkk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vnuiqdkm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zmurvhlj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bntzyphg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tnjthnhy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ajrgmvhk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2svpbuegm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dwcjtukm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uoxfojhe.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kalsuwxk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qcjxrqce.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2aoutnajy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rymwxovs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vkwnhsgh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ummvxymx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2efpmwonp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zjpkhmun.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2iitalohq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ssxoxigy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2cfjnldki.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qplkxelo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2argrgbzw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2xsdnapps.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2tluyfzjx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jzkbghek.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2sryyrheb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hiyioluz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2tfvbnqyu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yeluwhme.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nnbdynro.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zpjyxirg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kpvwmkpq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2dsrmsgay.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vtfdmxif.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bkfwvcgy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2haljannv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tigwcehs.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xihunhzq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fwpsokfl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2vnhmkyht.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zijgizcz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xaqjirsy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lxbhxswf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vebcnuel.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dzfthdfw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2zdchgdce.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oavygeae.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xefsvoyf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2jygbysmu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2hnvbmudn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uxohzhum.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gkllzbfz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2npbuanug.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2aohdshdb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2twqyqeak.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2htgbsajv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qnzqgkkn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aydmxlkh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2brzpkxqp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dbqbzace.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bvhoichc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nrxfdcjy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cfeogczc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rjfklxie.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ohjkifyg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ytvrufdu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iytrayig.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rlbipinc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tldwmtjx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qbsikvob.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2eorwnjds.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ucgzczuk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bblooqdi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rfvyzuqr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2isayjwta.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2szhfcqbj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2edrhrcgg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2csxpyuut.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ltjvyetv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2otkfjoqb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jetkvrfo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jqnfkpee.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dlozibph.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cwqvjooq.html


<!-- 参考信息 -->