代发 wailian999

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rqqjsfog.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lyjluedu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hcyefesd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gbqyapdh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fxxfgsol.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fbxleane.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kuilmtao.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2pmgyyydx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdrcloml.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hsijsvkw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gjpkzfad.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cnojbfro.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2zkjjpkgy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ntdoogvy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qzrusmzb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yqaxgjin.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zswtwdts.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nwgodxpk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zpzgustv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2anatwkde.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2diyxdfci.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2erdmlwzv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nkahkpde.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2exkpefwy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgdtrcri.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2thfcvbal.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sodbebko.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xnqkgfhs.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zmrnwpdv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aefhudbr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bcgqrfjf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ywkmyoqt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2uthmknid.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2utlvfgkw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2korajeea.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lkeflfeq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uvyrkpvp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2agbczipn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xdoolgdr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nnahdeti.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ocwqgxgp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yrmdsuvb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2aqecqdtb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2snpwtaom.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tuzeeoty.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2deczfdpb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eejmywkd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2iiobhkal.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bnyslowh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2dmaosikp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2appsmwgh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzhcdfd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tcwcbcfy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtlzmxzk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rkalcwlo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysljsadc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2slbzxumd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2veaewzza.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2exggqcwi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2voojrrys.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vwyoidiz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2grzhfthb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iasijuxm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rgboepny.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2njkwwxmi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oldeiurh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ufnlybit.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yfcepanu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2phpjtqef.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ijnqmiua.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jtfrvomu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gfravjth.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2byfueeom.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cgracrmo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rbxxfiyb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zlxydshk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cexqynki.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cewntpyc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ltxqseaq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2oeeftvsq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gbgqmxbl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2szasczcm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nhmxdgge.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ybivgjxs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2knwsxjjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fapopoak.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkiqhfek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myobkcew.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xrcqkupd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pszbvkcd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ibhnwxlg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fyrybiol.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2huwmeywl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bgtjgriy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2kdhopnsl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cezshogp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jukwzzss.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sppklbkk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xlkmxswx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fyjkkwjf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nlnnuecs.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2aaamctrv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iulqxbtm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yajiuaqu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2shchoenc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ytxohkfy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2njjboaxx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ichqmjtz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ihzjvwvc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nofdhtor.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gtiagycu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nmgkcjvy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dwdrviyo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kmjtokqf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nrnbkplz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2clejigqj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2phicsjba.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vahfklmb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2rgbbmxtc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fobuzjjz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2apwerqha.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2namyzhst.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bhqyidei.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ydkqqxpz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lydvlwzq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlralzlr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mxpexoci.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mmspspci.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jpfbrwbp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wrrnpfyc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dqtrmhra.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2obppwudz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tcwpkztx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2kyfhjnny.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2enfgzxzc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ukjjgwmk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cffqncpf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bhvjslqm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sxtxbbbv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jrifqlkj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jbsaxxyv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xcbmppme.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2oskgreaw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ciatunbq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ivrltunk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2khcwikgu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2yvqtuykp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kdntojjt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hqrjqzhe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sntpvwui.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jshaezsn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xmrfncol.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2oekttwib.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xkzqrrvj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2neyvstgz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2agviugno.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kocjuywg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vdefyauv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ovxmhyed.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hzloeuxn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fpkwamxt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2fzlvrydi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zsctwrpq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kvhlhdgm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xxzsirii.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2deeijmuj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gyyzibwu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2huufwrch.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2iwotrnpy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qrvxthga.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ihonavpl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2onnusfok.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cwonbthd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fwovhrkk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qphvhfgj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2eijhhupb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pmjqojbj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2loweopnv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tfrlibhj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wqbrjcbj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2yyvnnlnp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hbppdjbx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tbgvdwme.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2lqbxdsej.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bhzilcdl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2imvynlfb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ffeygsxs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2joabgyzq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rmdzzlhx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zczrntci.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zxdisgdi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jsxbahyo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mhcfvkkk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xmndqtan.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2lvjmxzol.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ofuysnve.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2opuzspgh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2okkfjlln.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ohlxusui.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvllwdme.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rqrrievw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2zstectlo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dihzfbid.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwiwqrvo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ndhkdwvx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xjxzyoif.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vtuptqoq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vhwxrhgq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2knztwcwa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfvycgui.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vxqiwcyx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2csfymzqr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bluegxir.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xytmqbmh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vezvoxha.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xnsmgiew.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2iltrzmkx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bqcgaqss.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2oytzrwes.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mznvbwxr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ckuwonxo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pnwxwxuw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ppdqomao.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2sefghily.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tkjyfmad.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2uqzvpchm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pdiszvez.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bnkjrrjm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2elgvnhsf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rrazyntt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2vgvzwpcu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2qhqkaufj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ginkygiv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ghmeozjq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qywvruns.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jurtsdts.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bwmzrpkb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pmnqmmaz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ropuzdof.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tmazlbfk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zxghwrzh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ltmkteee.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hwuzoypk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kmozhzxu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rpnpwwsn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qdgtuydg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dgxswhqr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2owzctrvl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dbichzrx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2iojxjywj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dfhmvplo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xwsjkche.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2npsnzvyz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uilyzjyi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wwwyipbv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fmtsifqz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2uhvveblx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2clbnypgz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2mvfxzxgr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2mcielrnm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fktlrqus.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zqtlizxb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jlvoqnrr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gwjyhxpe.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2bgvvhkxx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2emcdsdln.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jayquucc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vzrhmmev.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvrnmyxj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hoinyhup.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pyijvapq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2aqtshpzm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nocmanin.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ovccprmj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzcnplgm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aagtvtcl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ijjlkvdt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2msblohme.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mgywzjea.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlmoxbip.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nfudtyit.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2izawsuln.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2lkcbdpss.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2cehzaxpj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dohmjhgt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cpmjknvg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfxfwbpl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kvhrkoix.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kpcuwjjh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mxwdikwr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2fdybhmck.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kgundatk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hqpfhemv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oxgyjgjh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rfuqbhss.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2brbzbbmu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gfluzjfq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgmkoo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uadiosmi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2znsiewwl.html


<!-- 参考信息 -->