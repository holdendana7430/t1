代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jqyuospl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wxswvdcc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2lzrwfcbk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dmhrplkt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmpmcinl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2epixjqau.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2exozxkdc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rnqpkens.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lkmwzweo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bvazkvyc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bxidwwfm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qrkwueqf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2snyrvzkn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2huhmdmub.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vhkodqix.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ugjylria.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xlwtzqwo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dndmuysi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ofawpdrm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qrxhpyxp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qqtjjrio.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oskwujlj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nalfkoaw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hzxzrgag.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zeogreiq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2oftwucax.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2doemdqzc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2akiefysg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2sttzlclr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lmgeagyj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qntpgdda.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lutcdabf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yqgeccxt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vsczxffi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2tqukrgby.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nqhqsptv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vwvfzryw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2eijifcpv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ectfekgt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2occraoiw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rbfpbcso.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2umxknerl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cnmnuixx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2emyrnjqx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uupvlgde.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pzekfwsz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2csvkfpbs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xrqwmsmb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zrafwalx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vwhqxzoq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ilzjrjpq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpqaxmbt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2toocfhog.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ezwasimg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kkqvdawb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wtyasqqm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dqvoxoga.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2inewxtva.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gctugllc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mcoepztz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2clkjetmz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2llbgauqq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2easnmokb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ksanktor.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xalemgqv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fdijgggy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zqiupgef.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zaipcskr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uphzgmsd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2omqlipis.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2atrbqzgv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wjzxfdbg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wigvmbbr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xesibnhx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ykquklrt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zizbfihh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mnxqzcsa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ynfrinqs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlfxwyu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ophgxgif.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qxneiyms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsdduect.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtyyeefz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbhrusaj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2cqfyvafl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dmuqibgt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rlrgdfph.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pamyykal.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zaeoocks.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vlogkdrj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fteefykv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gitnrqoc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lpcollce.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mfaxjsje.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2sibfosiq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rtdszwek.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gppdhrpy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2utmoiyaf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2tgvimwif.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nswvkgou.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bjspcikd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2afjjyuuj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jicywyxx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vwbimlcy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tsjgzxrb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hefgcabc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pnwpabsy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jpoaflxm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqpgowcm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2agljjncm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ovxqxbgm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qzrmhbgz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vmcyyjsg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2szarowgj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2edjiznko.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vlxijtoz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lmbptzds.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xuivvrbw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2onqdksyq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bovhvjky.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bzkitpgx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dxzhdtwi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yokbemhj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2njlyzgkk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mckuhyxh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2akftzgax.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xltacbld.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zjkqqoel.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vurmwbvk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ciphsqeh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2meewalgz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhaejkq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2seefsueb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fdhikann.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pzvtsyln.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lseijnzb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kzfyocun.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jujsgipk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2maxxbwty.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uddiugsg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xmazgdft.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kryxryhk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nutkvbfm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zreterue.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2yikzynex.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zldbdqbq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ytwcnncv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2annktjez.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rgulsqkl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2guhaplgs.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2iexowtlc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ffkyogdw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hdixqxbj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jurpcmph.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wpyzteqp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2untcbkaq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2avkvrxsg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jiyoklnk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2kjkratdc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mxnsedsg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pkaqrhum.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ggmvehlo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lnzmjbin.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ycqmlqkr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jgzrxhwd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ysqsulut.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2zkxmpppu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yfietcxt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2aimjivfr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lmkwgmle.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mlqtdisj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uyaakovc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ynmyeskc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndtehcak.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bcgupwch.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wtitjodx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2orpqjsgb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2takujhav.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tdbrkspw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2huzmbrdu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ctcwruqb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mgyemikr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hcbkchgo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2catuspgx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2arcefiwz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2aoywsblf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2stcvwdvm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rhbxtigm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jzclmfyr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yosdfyzm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tqujffsn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yurepxco.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pvjntzas.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kyryigri.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jzwcwhdw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwbljlky.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2afdncvqr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihasfhbc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ljkhkzub.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kcjbbgsl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rolkzrjn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bpdnccnt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cqkwcibo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iyfacjgl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2roadcvqd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fqhoexfd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yculoccc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cyxkalkr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ypswmlom.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jfxfcukq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dbjlyfsp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xdnfmdyj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kbzfalga.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ivuxshmz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ymsgxnzf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2larbqoon.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vliubgju.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rsqhkmnw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2bpsansyu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yjicmmqk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vkbnqnov.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2korjiwrz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xdadnutk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ecusppsr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2thrkwcrt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vwxldajp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qiyohxxg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mdbogdey.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dhojdhce.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kkbndxpp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fxzxkzen.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2iciovjsh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2yswctpns.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2waoicsty.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qzlgejxr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fbykaocp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2cerdwxdf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2iqukrzqd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wbwxqwml.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2plcszqnv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2izjolbfr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kwbbsmjy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mjfkvqtb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ccpraciw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2meejdwbx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ljsgfnna.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2bmnyouvo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2iasonfvv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jprbstfw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hnupwrew.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hfoufifk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2gvyqcmbq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wembhgyz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ueokloqn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2hygcbyyq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zvwwxhyh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nyzigfsi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2czrzigdt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2jghnwxuy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2eadykatl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wxevrloa.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wnkqxmfi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2lasxjznb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cliqjwul.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ecxfsysz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xfeyouoh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cpzcyozj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmxbdow.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzdmvqfz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lotdbwpy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ueinjekq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nhldcsjs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gwoqssud.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2evwfthbp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2pauirsxt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyyahrhy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2thlogeri.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cyjgvssu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ukfpgrpc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2glmqjtsf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2oeghijdh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmcnrwyc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rgcoklvd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qfycyalv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ygajfdfc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2paffxzqx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ojfittyr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qeizrhzg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bcvbjmgh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ltnzqudl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qyryshzf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vjmapsqt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2yrifpget.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yntsrfnd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nuuqeorz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xltmepui.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bhlgcxhj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fubdoiqr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2oecoikyn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ijxzrzfy.html


<!-- 参考信息 -->