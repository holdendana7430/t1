代发 wailian999

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2roxlshjk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnjyovv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mnrofubh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2brcgxhdz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bsoxgriu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqbbalhb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pkgdvwcz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xyltytsf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2apxvhhwm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqtgcrd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uqqrhqlb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2toglxgub.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2aogckids.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yzwgdfpx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xazcqxcc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jgojoxzv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mmwpcjma.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tjdjvdql.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cuovhxei.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oymjwzmx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cyfgvrre.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2lllazvfe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mfocmrsd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2civfhbec.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2roftkxia.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dyxefcwd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fcmjwqtb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lgezkvhq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ipkjdvex.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xxszssiy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2descbrby.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bonexlpw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ohndywah.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vdraovzv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wyxwqjnf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2lvyugncq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rbexrlig.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cgvxfnjs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zcaywytr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rlamzyao.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kmvfqcow.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eohrdkyo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2haunthrz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xprkzibl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wycapkns.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2prfatpvy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2iyugmfgy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2oislnbxc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gdmdqpts.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mukztvds.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cranqquj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kqiuhhln.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hbmhqouq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2itqhudvg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bxrpwkxd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2toxuxues.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kbmgyjpq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sjmeewvc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2weeokvcb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tuhzjfnk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jxqnwpev.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kzcuenek.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2caqcnrtp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rdjobuyv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hsjjygby.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ucbujycz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jylqyclt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tscifxqt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ckyjsjkn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqohlikd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2iowemamu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snlptltr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2oycodkvm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2lwxfvvgi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ecmuricj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bfaplbwy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uaosshow.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgxofegi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctbozqzf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2grbeviwr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2udyagovi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2briundvj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lvygzdan.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tyosxfuh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2orkfzevb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bfabtjcz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2atbagnph.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ticofzww.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oxfkusps.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gxremaeu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ulojnepl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qxvbvztm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uqasogom.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ehdaqosv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jmhxmpdq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bsseycvo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zqzhqxjl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2lvlyiggt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kpalbebh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ffnsrlug.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2njufwlhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptcnmkae.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gdmlpdeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igrwbues.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zilmdrpw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2oudnqzlk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fhoryhol.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ainwftap.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wgbjbcqk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bizvlwjp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2twrawphh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mywumpvv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ilydhxsg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2quppwnsx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2tndwudcu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mmixoozi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2alazhclp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tyivmszg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nhurgwvy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fdhyimyn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xsivfjpy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2capieqhg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vjtkfjmh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2krzvxjxz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qevjyehf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ornjpcsn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ydrqonum.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjvsomt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2poktcfym.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2rzsflrai.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jwmuppgz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zbkmrgti.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qlzqcyai.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xlydwgoy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ovutzcfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2orstuumt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lnhsnour.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kicatgls.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2snxtjgbd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2woocawjb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vlwveokp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjrqjfyr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fjtzjsnc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hhnqvkvs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2oywsdbtu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2szjfmvil.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vrsoazab.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2eghduacu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzrhfmby.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2goyklnyt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2toksfqvy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2doghwmcb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mdljowfe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bisyeugi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hllmwwsk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vjnltopr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2cldmwjbi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2unxdwfvd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yvjigrot.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ynwfevlk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vdocrgnb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mhrnhxsg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2htvfslnx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mmlojenq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gytcwuky.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2oohiamvx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ptoiiorg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ssozzclq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ugblmivg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2uopjsevw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qplqfpyz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2aqpimwdq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2fgrrwjux.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2snlluekh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2msspcfcx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ssbspxjn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2misooztx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kjrcxaok.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iajfnali.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2olnnhmld.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2byvugoct.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2emoazzla.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2imcjiicx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yeehczbv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ucrtghle.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dtuddsoq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vfqzmmtj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2suwzuadf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rfepyrug.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lcfcobli.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uqryneyn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cobotkom.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2hvyqfnzk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dorltrez.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qiublmgr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ucrtsioc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfmqnsft.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ztjehmkg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mbjqxtkg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yljdedlt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qtwlhoxh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fxunhatd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2iidtyqzb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fhcwmlwu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zywzblqr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2evlpqbea.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2czqqrgxb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nrryiqrf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hirciyuq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rxkumetm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mkxaceqm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2efxoropu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jwcmlcom.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2svfsicor.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ulgbbdwn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2losczvek.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sjjpmiri.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mzlmfydo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nigeyrav.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2beoxaavf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2rriapuyz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dbjlqmln.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cwhhuqcg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2uqunyesu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vliestvo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2clxfesie.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pyztpusr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2oeuikxkd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jxxkfaxw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xqyvxhrs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2whkxltev.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2cwtimfnr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2bnukvadz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kpwvejyu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2niluxbtq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2wvmmztsw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2erkjmpsn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fcucernj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vyuliohc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uyihqbvk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gqkohtbc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fxvhxlkz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nreexrar.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ledrkbhj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2anisbwaf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pfdfrsqv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bfytxrok.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2saaulhgr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jdbidlbx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ghspizua.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhurzxjc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zlpvlebz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xmocalgv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ygowbeaj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uvtlbntl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2kxwodkcc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2svvagiif.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2auqroftk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lwrkxpgn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fcbaccep.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kedjyvzh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hayuimhf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qznyksmj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2aobsjsen.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zupjqeoo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jgavrvhb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dchfpivo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2veoilekr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2bsggjvha.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rewbhsoq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zmlleuqh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2oqqwwyhy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2exntpzmn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hngiasxy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rqnouyye.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2etkvrgnj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xixsyeny.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pknzpbzl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2oyxiytni.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qupujrnb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2bazvykyn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aeoruqxe.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hlyqkgdk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aaypwykc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gxhwormt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wmvfvwmz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ggxowact.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2irpjqfxt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ptmrtemx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2qhuandsx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zlfwlsmw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zxblujju.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qddqkbbc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sgmfzxuw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qqzjxxjv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjsfbapq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qorhqnwp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hfjupcdb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vovxhjqm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2uroedcql.html


<!-- 参考信息 -->