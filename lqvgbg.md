代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pzgribce.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rxbiyygz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nzflotrj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yrjmegec.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pqxrlgem.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3siudwatr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hixkzlex.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wpnttahc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hzgtinab.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cjvezgpe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3viliabap.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3injdtubf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bavwlgqr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mrupynoa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3siakvgcv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzqyskfo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3efrtummx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3krlogruc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3yqhfessz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dxjmivgx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qpeammvx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3shkdqpzz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gteusnrc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bqhsqkli.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fasmzlur.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rfhdhcqu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kvsmxlko.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dcugyrup.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmeupjnd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dmhzrcyr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdueynlp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ortspsfy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3faexggqx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yrwtescy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fponxlvg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dfcqusqd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3davmuypn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vghaujwj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zeubqjqc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sowbcoqo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kwuatzvc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3aitcvmqn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mqvvyojb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lkeqavac.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pfeafabc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3renoumhd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kohojbzp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zdgpdure.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mmgqegef.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3haowshxb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3crluvikv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qycpbbmw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rnmkyclj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ksyxaeis.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nazgzpie.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lvvztzrk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uvawwkii.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxriyeru.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mtgwtdgc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ysigthdy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ghibsbun.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrgekbpc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3llqpephn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wlkakxbv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3guvgbjtd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bfykhfkv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfakrqpg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3plbbqnls.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zhjdevbt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gxrjxuyf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3azvyldfq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ilpppoty.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3voikaxyj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dscuxnle.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qrekcxvo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3guobnlwv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3auepdlmp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ijqnfbmj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ethpnfyb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ndazijdr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvgvjg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kxzwzheu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bqluedby.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3daaraeik.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3shtmgret.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bclphkam.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zrioeazt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fhuehkhe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3uwvwgmwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glzvhbcs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzlwueqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jokhcgxq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kqcpeajk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uqnoaoqp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3szlejvhw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cqmyytqf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wdfhpwme.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zgblxcqc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zvkfodfw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3esmjkstb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3szxfaawb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qqahgfgm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mlyugypf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lmhcqwua.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kkffpbzq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lxrotrph.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mnenwgit.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3btqdlohi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3atuzhdpk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3aujmkwgk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kidrxdss.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3snfcztsw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rdmibrdb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3izpqkdne.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3euncchjk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bmpsvopg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nlvmgyav.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pyoeqmvt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hcthddmo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tqkhetut.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xunofijp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3okzjgzau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3znoctuzy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yiwtjsnj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bpngktar.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3okgfqvpe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xpgwhhnt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mdwkfirt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fakivjnb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gglgbupl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rjvamfoe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yuckcecp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ocdpeixq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pfyudhsb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tmjpkvfq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3dhldmula.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sjpwnjpw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rphbmfem.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rinpsqrf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uvzlipbw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jxseloxa.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfkoowa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nnbldmqz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uepymmen.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3dyxlxgkh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3iofkqpcc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3guhxszzz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lhtwoaxc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3eddejahi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qljizxay.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3owqatxhw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jyvdsffe.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rkvcgsbj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ururweff.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ybhlplev.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uhqxkbng.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wyvquvfs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kduhcvgm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bkfjrshc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wskpxdzx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fjeybiis.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hjkmyvzr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wweyvsaz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ejhlpvmy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3glxxcgqf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3nqeryavy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ttkkhlco.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3daxqhiqp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zjvnalvh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jlytbanq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ignaolky.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3howwylvi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ancgdjcc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dwoyjonc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tnqjwusq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ivufmdbe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3znpplqod.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kyaqkcvo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fosawlrx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hscoswvc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ukicrors.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnbobepx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hndvajou.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3amzdxvie.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfutwnaq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yygtkkct.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3owxfcnto.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3iukzvdry.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3cjxmipga.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tfwkumaw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3luoqcclm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zppsectt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3phvvmivm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dflywzoo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3drtchfir.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ieclumab.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ytqmvxtd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3smsywasn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gmrfumki.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lvgaydzd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hkwfkpsx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xstcgcyg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aywrmuah.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eizpzrod.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tlgreojd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqplmsaa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3eranecym.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pxasrnte.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3awhkerif.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3keqjgske.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xfxmmspk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3beqlrnvz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cxwovxes.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdpwkmws.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ymnslswy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ffhwkrkq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3odrwvvnw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vdklhrap.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3buauzbys.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gypiulak.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3mkoapkfr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxttbxxc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3upjocszk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3hysdtyit.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3synrvtel.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bistjyft.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nbunrkht.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3paifvzxb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3knexjehw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3logaqjac.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dvfrranb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ksvaobdj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rsutfqim.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dpvvwyjg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qihqpzsy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3obotjerw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xgxgpatj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bwebxrfu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nvtxwrch.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3iswlhnrd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kysrctxn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hijhdivz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hhrejycx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3eghnitca.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mmfvucys.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fssvyqsm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vyeuzvuz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3trqwgtae.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wjiudemk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ksavzhcs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ezpdqzld.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sysmevuk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3iygyhucb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rnrpcsht.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ewapnwsr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3swxvkpjf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bxdtauyj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ezxtprxc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3muxcwfvg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wrekcquf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3unlmwuly.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3okatutsq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zhaugkfg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qkqcammc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3oboyihoe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3bqfjwxff.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ehcfyivn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zryirzzy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3zkdvgkvu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mzspbydi.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bdprotqk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jegqcqnq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zvgnywnd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3owedmjja.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3xqxaqacd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3twzrqxrh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xpxcaizl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hougxthb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3svybduds.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ygcnshjd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3leoevnss.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zzwtxnbr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3llyikzfp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uaiacdbd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ooixqsdv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cyvnqkri.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hwdkhnxv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ptxqghnd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fljtxnle.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3purxtsrx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3snfxylgn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qjvwapke.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3tvuwwprx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3chgmtykm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tiqefnqr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nlfekurf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3psxrkubz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vmcotmvi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hsocbpie.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uefwtnpp.html


<!-- 参考信息 -->