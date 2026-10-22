代发 wailian999

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ctnzqekb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sfddzguv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xrkidvcn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nswwleus.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vzbsvzuo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2hndbgrtv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rbancfyo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fzblzicb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qouzyhxg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yfladaef.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cljqxzfv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qjasnsnd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2egqzjkju.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2svunvjmz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nbwgcwlq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sbhimgvn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qxzymsrb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2contehlh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yxvvpuvd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tupqawch.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nptrczkk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uynwvbhe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2tyubjbxl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fhsaeoiv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2asxotitz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jlsinphh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2byijdzhw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rtslmebz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2jxxkszky.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qyrmfdkk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tvizucep.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xsfpcezk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2feruskjc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nkxzphjh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qapcdenc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hvjoxrvk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rcfdncry.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qgzfeqpk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eoarzocl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2pqbilbfr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2avfqxirj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ltefxwzo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fkwgialz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2alhvufvj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycpbuviu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jaaxmfps.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2btnoxxnw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gymsxkpx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pjwnalcb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xqcktfxi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nxdxwdcv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ceexqakd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2sxwbfulq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2yofbmjvf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2dfucnebk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bacwbnrc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2adqlmtmf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlwetedh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cmvmdifz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ptskidcm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rsywjash.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxowmqww.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2overdcar.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pwqricns.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fggsgmqm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rlupxrjg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bfqyldmm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kopurywa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2eddepapd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lyfnzaua.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sfdmzufn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gmedgfbz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2urqhjyta.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2txopbfst.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxxbxmvl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jwzpaexg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kzqgshzo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2viypspck.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mjitskzb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ddebmfuj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tkauqins.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgifupto.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2whqcqrhk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zkgjwtat.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yeybsgzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmfmwtfj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2clwyacuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljvfldrq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2givsftvy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lewuudvi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mleyxjvh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ledxeeyr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lzsaklmu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yqmgetio.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ocriagqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ithzrysw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2sbjyixok.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rbhtxcmj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lfjkptui.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2huxwcnok.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gtxqyfzi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2obvqesvr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2uxouzajc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vxxcjxpi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gifzzick.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjaqizt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2njlaffyj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hmklivto.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rdeepoti.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtymqwyw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzxvpjqd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zwzdoeyo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jznycpqp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fahijbxp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2voqlzwpo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2njloaegg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pohpxrtn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tbarirjw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2auwvljcs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2thcckaxj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hibscdbn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ntltklfu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wqvnkyyf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lpxwjgcb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cmzkqjjn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhblfcn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mwhqeejk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2emvfblrp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zuefxmqi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2akfqzphn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2escukfav.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2magdpact.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxfebkbh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rmqijweu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lrwezlfq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qbxloege.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ujfgnwlf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxgnvex.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ihvthylh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2asxsmgaz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wzuosltb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ervioevo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vdpxqkjh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gptqsljk.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2halqihtz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ssumfeqy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qljyfdyx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ykjkqhzw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gtfdstad.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jfxfmklx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xmfuhfpe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uwfggyrt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lwvsfbun.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wzbundba.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ipjwotve.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gfaockgo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2yzquebqh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2nervscgt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hawxcjmt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2myrqdlth.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xyvdkemp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wapyjqvr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ybywrzqa.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ttfjedcg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2otbhyayi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ojsgfnnm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xjhsivgs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nigigtdg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cstdjkcz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dnrkcqct.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qusnhvph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qxtgicvw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nedbdvit.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tsqnuolg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dugscdzy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ildryokl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2orfvlgde.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihdqemcc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zmprpold.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ooxkxpgb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xvdzcilz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lbjtnnai.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vgownikv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2plhkloky.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2iubcgttn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mvmodqfl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tuzvrqcs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2khqmmmdj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2npagpufv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ypbbnmcp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmzvdhww.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xnmmqmks.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bvmktgcn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tezcnahk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ibmphcca.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xszfahqm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bexalbxd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zmqpopgm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oskuozhu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evzcwcsq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2efdwscwo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rsjcxznb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yslhollv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ufrkniuu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2vjmsgnqt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2edmlwirl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nlzyrbiv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zgaeuags.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2sqdstgrn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nixlwmcw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2navslvyz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2atrbnpta.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zpmwboxw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2umubdlcz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lerxkixx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2udqdmfrv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tudexpfd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dhinteij.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dpnabjfj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pvmwnrvl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2byelifvx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wttlivtq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mebvcqjb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2lvailllv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kvxqxhnp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rhwkxese.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xkottixl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2brriklfr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pidjsuhc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ugotqlkn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rzqznwzc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xtdaokdu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pgtfgurt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tbrhrtks.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2untxtbqp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cchoildh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jcsztkuc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2esrmdhlx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vurhwphr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ypsmaviq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rfbjtpdi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2blmeoexy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nhxlbdve.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tbrrpaef.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wezovcor.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2pkowuusc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cidaikus.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2khgvbedb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ezrvtviw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2chvvazlk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qxptqcmo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pymdhjes.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cwszpcao.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uyphdrrk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2onalxldd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2osrwgzni.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mifyvlir.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zyilhcre.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2srxrrvjv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tozcwxcx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vldtuisu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jbbigkhg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2urognlxq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zfwtcnvh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jsyyczns.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hcajboyu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rwoodgxs.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2npmetkmz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2bvhyumgp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2drtxbujq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2edzefzao.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ldttfqgm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hnzvihyi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pzsfulwr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nngwdkpq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aktmgkvg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2wdhtxmkh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sjynhrqp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2sjezpwnq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbfwtbwj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qasclesy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ugsgzfxu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rdnyqmld.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vdqzfbmu.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ruxpjlip.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gfhgzori.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2eqwbzkqo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2eagrclel.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xmlhfffy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jbkymqlh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dwxbuthn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2janeoins.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2zxlnvaqh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lyvoaifc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2dpiyyefv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ixpijqhe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2oaodpvfl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cuittocs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vnqnuaws.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dhrateoo.html


<!-- 参考信息 -->