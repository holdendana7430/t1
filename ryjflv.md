代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2klubxunr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tfuyxvse.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ytinkjjy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vcbpmjtu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nkxgmqmu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uifbystn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2twuskhqh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2htapzrrf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qdmrqamb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hiaraqzq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2atmxehyo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xeuolifj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xkimyixp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pzfwpndb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gdsfccfl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sadnkwjk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uumuvnyt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2djseeyfg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2atszzmkc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjdlfjrn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rklqfnyf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rkilczvk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yzlvydod.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lupzhuhw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2svfnlrbc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nkwpjasx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bdsytoqk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cwcqrrsi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nsbtohvo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gxfpxzmo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qfirybjl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bnaqmawi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aesztmuc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qqhztlsy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fvvnsvov.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qtxjxkuv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ichhjgve.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rcqcotos.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kzuupztt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2phbyfnle.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2btgvbxgx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2eosizozj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wladumtd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2asxspbeq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2uexxrmob.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2sogyqgfu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2swtvlxli.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjceuvjm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2tcsiygxd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pwgcjivr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ecrirhuk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2aqfifqyw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bctgqrle.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxjsqxrz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2powazfaq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wnpwdvkp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wouqjbfr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cqvcpasr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tofphpbs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lgkkhazv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nenrtytw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ehxkcmom.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mlmndluk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2brmuvagm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fueizerl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mibijpgi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2odkciofl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2yrafrcto.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jrywftmp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gblxfbai.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ynxnwqpo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2wqottfyo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2cjestmyh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hwhtxooo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2whwcgfih.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lxndovpx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gxhktgfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxdmzkjg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbatgjul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jreschmz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2pmvfnizw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ubqoxlbe.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2yvsvhwbm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mdjkpbri.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mtmwozgc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zjzvghmt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yjcgtjjb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2halszqiq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2uwmcivef.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hwwjwudr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uuojcanx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2oybzdeir.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qfkbcuxi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dsymyzzr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ghjveqex.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rbsrhlbb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zrtttbfb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rrbarwhn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gixvwfga.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lfhbdqcb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qflucxxl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fzgcmjja.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hrntalvi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihygzjrr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bwmyoptq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sdwjhinl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qwxcirox.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2facmjehq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tmnwflfh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2sslvrceo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2qluwktui.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vgwvttcb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dvcscugj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgxmomi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lxpaglta.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sjsetahd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2casmhapd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfalsedj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lsplcowg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rncrgdpw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lbuxikys.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2izuyxybi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fhrrsviu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vdotfoiq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wklncwlh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ymonevvx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bkskzxcf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kibhnnjj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ajhfztme.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ovhhpnui.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fxbrtelb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2swszgvyi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kthtncwd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dhtfszin.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jtkeujac.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lbaklhps.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2uskktcbd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fiqsttkb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ipxxvkrd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zsxuklye.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2izxggjue.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zfnbzqew.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rzhejgsq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gycsolnw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ipjqtkez.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fyathevk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ncqqbiub.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fhimndrs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bcucqhhg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rupgblpv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eueinpnt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fcfaziqx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2izwrskdk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ybcqzwub.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qcruvxnt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bikzniui.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yvmgpzbs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2udjrgipn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vhlrgyzi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2glogmkao.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jtfmiecf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hrzlkicw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2smcpygzb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kyzvyhrf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rvxdoipa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xwcsngxg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mrehxytb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2auocrunr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2qwpwnrhi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxowlucr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ammjnwzt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wtircohv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmhnugtt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gaasqsfb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wpxauere.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jwwitkci.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tgyfdrbm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2dqixzfpe.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2shpwfkpz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zxjkwkxw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pgpbvnge.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wvyugxxf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmabqoaj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sudgwqvn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qcruoqbm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wcgprtss.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hejqfped.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mzkxltxb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2cjcovxvw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yztwrvgc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ydamowvp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2luulcdxa.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qqwvonux.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2aabmwico.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yasvwixi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2snrykbtd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ovsoeltd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xqqcrdps.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2sqtlhsis.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nliqeril.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2slegpojj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2iepdaazd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2komyokre.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2dgxkkzlk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2krsanmwy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ovzlfpaa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ezznzjwd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2sdjaagbb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2cqzvllaj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jwxroxnm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xsvokyej.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhtjbusg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lrixduyx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2oqohevao.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wosuriob.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zsknlggl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vwgrxuuf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gbjdjxzc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dsmitnzb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2oebpbltk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2weszrxco.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ikvbrpjn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2yhqnmvlb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kbnxpmjm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vanalzjo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kdusufsq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxtmqtqk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ppfgryzn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rcidodol.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2scatuznq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wxetnrrx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pxhktowp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fpodpbws.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jzrlirdk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rrqsuqpx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xspqaddp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qqxevndo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qehwtmbf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2msvhcukz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2agqrqbxp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jcxjivxv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pekolxvz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jycyufbi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2amtpqjqi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ktwjaubh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hgpnamrg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2yeelydre.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rkkobbmb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xxpoxtij.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gcirnkdr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cdetbepc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2prcmgrpj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2goujcivj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hpjeomwy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pmwkcfuu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2jtgvxxcr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zqtmmakw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dfoijahb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ajdkyexn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dqwrugar.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yzeeuzra.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bsfufyci.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2upbwwhgo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wurhofht.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2efauwoxs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mhgmvxnh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tzzygdwx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ssvvtans.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zigxaher.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lfprmsmh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zdyrcthf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nxssuygp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2eedovmdi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2upeoddxd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bggwifkn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ewbquobr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2thzpqnpa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ayjfwawk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2rkyggrli.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pfoaniig.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2afiqgynu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wgacheta.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hcpmuvun.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nwnmuifs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2nhzworbu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tmsurjcv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2smgxosle.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sygqogux.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2obllvita.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fkjvxevi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2amimqier.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2kygkicrf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aagswxko.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2enngczzk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2aodtdvak.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ebbreyij.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ihvgeufh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rrhtlwhs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vnxggzpq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2gcerirwa.html


<!-- 参考信息 -->