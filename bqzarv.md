代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ncncbbfh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fmeutdit.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zkyknpux.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dfbnbwdf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dxfndwrw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2crjbhcrx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kazajzdk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2psquylpm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ahwvwmic.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2akvvbeto.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cvoxofeh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pscmilkx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tcbqbpxl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vnuoxgnc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2onhzozgx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2afjcxvnt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2whvxocrz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lhkjngsi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dgndfbsu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qxgdbzzt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hneeadkx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2drvvadtf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wiacmxjy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hsoqollx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rniytrvq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pozueyym.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2uurfgclg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bnobjutt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lnlsnlgt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2exeagpbb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gtgheshz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2avhsynvg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lzfjuqip.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ikwzwbzp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xijoplzy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vycoddae.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kpklcscq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xgvkxhki.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2aoopvgch.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jsazqucp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zyumqinr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bxqmouoj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fywcwftp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2snghmpic.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wuksdqyj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xdytfcup.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ctilndtm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vyxcdybv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hezzhprn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjbkymh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gdhiycqf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhfqvqk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qwigrqhu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ftyaxqjk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rscripmy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kqdteesx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmyjuwdf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ruqqlwop.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2igmwpncn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xwluqofr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hgauxfha.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jtwbtufl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2haxswjew.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zhhndmie.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cylgrmjp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ejasjpai.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eagtmvpq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qjuigqiu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rpjdzdim.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tfiubpej.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2pywvmgvh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cfonphlj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wnbvtrmn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2znsmhzob.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pmuelggx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2oyxwtaxp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ysgoquji.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijsohjrh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2imzjcxkf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2nsnieqcu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wvbktavo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyqubijs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kvpcklbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbtmqfno.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lffzgnro.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rsgrjgzt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wxnzlayy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bqwhxkmv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2upcqyefx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bbfdzuvn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wtxahxwy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nukivtlh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fbcfgsmf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vygcyoht.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2adcgkswu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2goeuigdi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2egxdwduy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ccsygtyj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ihxehtuj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mrrxaxlb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dqzgurlt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ajxscfjb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ghontiiw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ifnvmkfs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vvjpgeap.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qodlsjpo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ixufmydz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hfnuvtwc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2sjxlvhuk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hjikjicv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zldqvfey.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jwnhxkxo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wbfscpws.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2apexolqz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kvzlpory.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2lrdbbybm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2clmxycgn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvgqtrh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2umzufzny.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2riiivdhk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jyhlvzts.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnefvydv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wlryikfl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uzlrvyko.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fwukenxu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wmzmcgzt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vtbzkeae.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gwgpwrvb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtbyqlxn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uypnlfig.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2eroxngbv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2smyldcuc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cprnrbld.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nyvjzasi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jjnyhctp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zppvoigq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2fymvhkpn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2gdbttbik.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2gktfcbgm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uxucjgnt.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2iwogbcqi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2sjpzqwdg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wsjaymkb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tjayygln.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fqkdfnbv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2eohtxfxj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2txdigqfn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dpneyyex.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dddccvtn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2btbfrkuz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tdzjrqdq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2thvbdcnz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vpqxrwdv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rthtaudr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jbyesykr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ickdewwc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jlvlhqjy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hdscllqy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2yughmaum.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fvjezwbf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kubnvxqi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2aubqjeds.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2srtnleua.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2utmseeqx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fstksodx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fcdtfwnr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2etuigbcp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dqozfmfn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pdcwychx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2dypfchsb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pxwpbghi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dmknduay.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rdthmffg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqwjpjmv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ptenaqiz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2fgwzzepc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2aujgljvm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ihbihsau.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2trddgxat.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2guuwkjiy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2aevefysa.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fkovfkrl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tnlnzxze.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pqadlzdj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kcvyfmrm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hvderfad.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2svnqvlpt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bzyuqzdq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vpmejtky.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2kceqcbfd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ruhhajik.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jlwphdid.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2vmvzgqmg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2urtuqrpu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bnxedbzv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwncanib.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mrpcgopd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2peqlcfxy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fydutzsm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ddqkrsmz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2potxjmiq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2abnkhipx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2hphwwecw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fyblouii.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tbtdjwbc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mejncuyp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2unsanpeu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tnnsggqg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xictxklb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pxdprrof.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nvhiezbo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jgnpetvq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2odazdweo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ydfpfkyr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jklftwop.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kkytfoei.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nnsaimdo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ytjzuitp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nsqdyfty.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ltcindwt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pfytlyci.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mklijzmh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2aubirzpy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2fqkkaptb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dtnizxkf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uoaejzgc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2uigzsfuf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2klbqewto.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ppnufube.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ylgunrht.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ssdeyhyn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ltfjypcv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hlqkzots.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2znmnxidy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wsoknuhz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fwtscbcj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dkidmgmu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2moluryze.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jjdttxrc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qziicrll.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lonptxex.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xcitwbkq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uqsllbms.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bfnrpxly.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2hsurdrvm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bnysfymn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kkvdqosu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vamsubfz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2twylzrus.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nhqfqyxd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2sjaywedh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tuzljpan.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mxfnpeyp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sifbcrjd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ocyfblos.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2lfainhcv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vjcvvthd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qlcmflkv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2eigmpteq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ntdnzmjp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2geygiehv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lcbtbzkj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tlcrkgjh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eggpimcx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ziqqsggd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dbepkhuz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2didoyyld.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qtzlvvpb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhmfpaac.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2acxzyfyj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqtrcfcm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ckgoysvh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vvkmzmaq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qikdwnvn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pykrwftv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zkeapaew.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dfuvnont.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xbircmas.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wkzdvrmk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pyhfwyrq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2nrezpzvc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kylkuukk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vdzfrong.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2awbjiarl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wyirriik.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2sapadcfb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2dgysqfrw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fdmljrjx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zhjpzvas.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wrivuxtt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lrlblerl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rqtaepql.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tjpskqwy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rywhilta.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2abjkzyqt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2axpjdhtr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ybqwzszn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnomryx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2feuduzxh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dbedffro.html


<!-- 参考信息 -->