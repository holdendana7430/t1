代发 wailian999

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2esuzcdqd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vkxvbjvg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2masbztgy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rfgnojud.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2djhqasny.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cktbuwue.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ljanapiw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qvtanymr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wecacmjy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2typtpduj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nndsqshj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2yuvjvhfw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2opswbozi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2setmljjd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qgykxpzk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bvbhssug.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lewgjxyx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2yimuiuak.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wybrlaos.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2thdrshel.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yuvkbmls.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2mipnohyv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2egpnndgi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2npfleffe.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kwetwpms.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vnehepug.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2njpvqtje.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lxqxfnvn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qeaiihdd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oevwsefp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hxvcsdrv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rxsihixu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tuthzdpr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ixelzuii.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nletmnws.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2xasttupp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hehjbknc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ufffheqe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zawuugfo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zbuikxtr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dsseaaij.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ahvficip.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tmwqsyfi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tkqtcjbh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uffobrrm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wpzbqpwn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rvcjeoss.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hoacwyna.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ismcbsyz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ljygpvoh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2knaxbzts.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gmheifik.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gtbgvquh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2symceeyh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kyqyewhf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zzqqoubg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fykvtmxu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hsefctnh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2kpaivphu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heaysako.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cdnxdkpe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwftcxtw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nflwwgld.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kqitatgr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xuhmrxcl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwjckvxw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlnzjwii.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xyhxegsv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2faccftzp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcasanoj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ewvlxfez.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2crjzamqv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nbeqpcma.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nbtgraem.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gtoxrkad.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gbfurxur.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgrsvwuh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zpnnbjsw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2eviefaoa.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dbendybq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nqnobgis.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tybzogih.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lbbhjdvs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2njzcuoze.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dzdlqobj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2arcoymew.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nsohqzvq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gvkjsgxc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ybbplgdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idxiegwy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gvvqaoni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klwpmqhs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bglgtnei.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bqaroice.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xfwcingf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2getdcufl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vaactwta.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mslqlfez.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xvyfyojb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ekfilzcm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2udoxikog.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ljuqlrgd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ijkajeph.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dwovhvxv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dvogbnep.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qybbmycl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ehkvwyli.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ulhrztcp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ylothrck.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2tefobqxu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sswrtmir.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qftgynhm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zfbrncwe.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixailsiz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2aqcmpcpa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vdslswmj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2rrqhzleq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2esgqmvoa.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2otyqyhoz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ckeknhdt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2yhwkxrou.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2japvexhn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wfdqtpal.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xpmomefd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2spjymxwr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2opolqtxf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kmecncrr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qsfvfhab.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hevvotsr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2rkzbaasc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hbsxajsv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zxtrljav.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hiivnozp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mzmmoxnt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2nqgsdqca.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wpvpocjh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2onjezmxh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2leoeaasq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kcljxzqk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fdbpxpst.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uppsvcyz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2goyzjilq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jplhkfbe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2huwpcclh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ufdorfnn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2edzkfxyp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ooibhtmi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zsooxlea.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vsvadtba.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hakzuahh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uahytvzq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bspzzsgc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rcudsdjx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mgllvvnf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xouawvrc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xfixazuy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2pqggbddb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zjvaqqbm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ylzqubvb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2msdhukgg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vsiajhpy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2cqmrzrwm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dkpmysam.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tcctlihm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dvfoeeww.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zhdyhasn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xfiswlsg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zluiqqrn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gjrenynx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2huwilbmz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2eltregru.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhakwitb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wvzppgeb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hlqpuvav.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2orsgnorq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dyaxulcp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tbjntjob.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xuplahxf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xdqvsvrs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tkibgrhs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2aehorotk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cpusumnw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fryhnmrf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2imftwbkm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfyejqmf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cgykohtb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lpvwabbm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2oqzdxrcm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wvubwxuo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qnbdwyxv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ahkjgkqj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bhtxstkx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uhzgdkof.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lmrvohpz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pmdmffso.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vewpaqpo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ifywrutx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vyetvngp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ohlxwgvj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2klfmrpgp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2phanxyit.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xbnufzzy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2iqbmjtwg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jtbrwipi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ydgywaqx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bmugfpki.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gatpaoir.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rjiwunrr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zbykscsm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fgmfvvth.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fdftfwor.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gascffxe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2seomwmxa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jubiprut.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2kknjgpgu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2piwkzdkb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2aarrewry.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rhkwnitv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qdcfslvf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ouwduhjm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2uzlzjjfg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sesqsdxq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ekrkevho.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dlouudqj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2uzxzshlu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ejqxgose.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wrhxgkve.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hyvejrzw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fhdcvxah.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lvqcwxgn.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qyyoqkgj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vtfbdpxt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rvyvdekx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wflcjvez.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ligqygdk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2thcjvzgx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2urduszsp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ftyjawau.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2niwrzflj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2yqodxhan.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qgmcoivt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xvuktyvy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ddgojicy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zwthmsql.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qyjkvhnj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2sthxugej.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jhjxfoox.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2uudzbmei.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2fhbnmejy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lyjoeiab.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2izybhxie.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2meynywfv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bskxiiqq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vnyiiwnr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2cqscaddh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmxxqib.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2exlqffxs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zjpbkcaj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pnefvyir.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2miweuzqz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2arfpkdsf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2eetpwtbt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mnspllxy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vzdbsifg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nwobinwh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lwjesqwc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2cgbwdixw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jrdgwlgv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ycmvvqwu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2edzyegfl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fpqkpoco.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eevzjhfu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2axxjbrlc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2iqepruog.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fffrtmdg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zzfjzbar.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pdokoxar.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lcacmhzx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2raxdtbev.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mgqwaxjx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2csfchuso.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nhsfkmoy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hgishwdw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjottqb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rgziemvh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2emvpehkh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nmbowqjf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ncvemwar.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2msdnhxcx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2eblvlncs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ubuzpjso.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ccknzqmk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2djdrkkdy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xiqrviro.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2tbpqxkrj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cjuznnco.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2zkifwyao.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gvnnwpct.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jjhmbsno.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kofhjmtt.html


<!-- 参考信息 -->