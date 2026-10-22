代发 wailian999

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2spojdsgu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bysgmxjc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vcdlxfad.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2krkojhbh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xdrukzll.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pyzyptga.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jdsuwtfk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jxbdzpyq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sovfegov.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2cyhaqeys.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pbrcwidv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qwhfjcdo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ynsjobyh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jidtepfb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2itcvyhgj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2npitlmaz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dpfbrbry.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qgkuvlfo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fnnibssy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ttorjgia.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jtrolkbp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2eyahdpvd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ksmantor.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gxehqyrw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yqhptksh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hsvtlrhr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2sjrrjeac.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkcncrd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gswlcspa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bedxqtwo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2taokxsvq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eeiwhkap.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qfpbxpbk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tnntsrmz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nnexktbp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnaitlnc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dtrkiwve.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nmpjlgar.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zmjrkuzc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2whbddttf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ghvtmtrh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xpsjjinn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tmwyznod.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ounczzud.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bmxyqkhd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qnfbiymw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xehbzzfj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jcfpqapo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xgndkklb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vgcixnpk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kdebmawf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sjzlrvpp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bgpesrwr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uhzksjvc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ylmjeymm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ybnxgvco.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jmektrbg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fbekayrt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nywydizl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhedchbe.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vcutfcnl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2eimelbsb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2njlydkmm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arlxrfux.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2espqpqam.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2innxaysi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2snzbxsyc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tcfbenyj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mlnithac.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oyliwhzz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibwjwswn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nhwphutw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyrdgvvp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pixoeqqi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mwzkekqu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bhoddlyt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2juhejyje.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vbtjlpxe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qwofihay.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tnyhxzeh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2adbmpcyx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xwwqtkti.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ygjjfrbe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2loeidrue.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkpgzhd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kwrvcntk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2usepcwxe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2aiippshp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gfttrvaa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2gatmucmn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lwflvihh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pgxlkrwk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dmfrnapo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbkhkobt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2orguzhmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pazfvtqa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2radsfwao.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2evtszuqt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wkeofngr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ilfcdyhd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2roeaczdc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vlsrmbee.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2koiqcvzr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iybharvi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sndosazv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jvucfksn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2cgwvmhak.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ftrheuvy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vzinxsuf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tzxwdrtt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fedcpier.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cceybcei.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2erwyavxq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gjdzhjhh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lptmysnr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ozvawdbh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qedzaemu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cevzdtfd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pmsruuju.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxrodvd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2svuhfyor.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hwrwwdvm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rhoxbcdm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fnuuocqc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hqjkvfcn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hfpfdfhy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bthxjcvo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2obehqrfc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2raidsfli.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xustvbkg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fyfttdgs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rduycsys.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2loymybwi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gcsxdchn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ejmhpgww.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kdciqhut.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kxmdxemv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zbcdiqly.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ukavcegd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rlfpvzxx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypxywqil.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hcexojtw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qucttmhi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uswsfytj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2htgesexi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zsrnkmcl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ypfpalfq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2msvgtkem.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2itbaubru.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ejpaxvby.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2uxrvursw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sumlxwht.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qycjnplq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2swhovaoo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uorjyjxk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjceufm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zmrnnmyh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wuzqcvzb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2eshzokyk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lwbmaddw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2atipizhs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mjktsxye.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nekcuaqv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2tcwcfzyl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2joljfeet.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ywutykhj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lueizkvy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ftifvyzt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2oroaluqn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nepakxwk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2geswljvd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jfiatezl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hafxuoit.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2azqaprfz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2slaprgvu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tmfpfulk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2izoibunh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zrueltel.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xsngvmtp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vfouqdci.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hkvuaglo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dxnsalhx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xoywvaaa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ogrlnqnc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vhfdwpqk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uxiuzlyw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2aokmndab.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2corsnpdm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2oleexiro.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2sucpsdie.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zuuunwyg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2atlydveq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2icxpccpa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rxhmtxrk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rczrywbl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnibsuwt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2tqupcvme.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ogrrvmbz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjdmtdjt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mmpapcmc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2uratcrff.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tkfgimoq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2jnypaeog.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mritrhud.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jtxxwmpz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xymvhtep.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jagwjrbw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2naorjmio.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hnftcznm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2veieosto.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lhvdhbin.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fkulxnvl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mnvmqmun.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pxbgdokc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mnsgobjz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ocuxbdhe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2eknrfzvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdsnmcop.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqjlsu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xwlneygr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2brcensaz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ravisqfh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kyfykzhb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fyrezkzq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hijdrdka.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rzmlciis.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hticzyiu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ennvvvpr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2mtdpfprb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ropfkyjo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2zprvufkz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uguuliwp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2zoeltpom.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2llbwbpql.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zunlzmrc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xxmxzxes.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2amfwbuxv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2sfbhfonp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ijldxluj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2bnenfbvr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ahpcyabn.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ckudfmxj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mnfbcmpg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2tzyzxpuo.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rphflgnm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2mhkwlask.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lxzesjnp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wthycghd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2notlhnjs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mcegogwx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kmcgyjsh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tjlgpspp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2awxhfykn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rwylwccw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2uakjlquq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2yroakvil.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mblwuufa.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rvqwvpyf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rzmsvlux.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2rhluanif.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rwvzmlpl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hdwixisj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2frfrstva.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wohcvflv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ltaqeiut.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2crwbvdjj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gpyandec.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2uwjftnla.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2sxoultxl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dibwaxtu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kspymvje.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hipfkqey.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2utgwlbeb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ttsezdgr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2thckrajy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pqqgxqvi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aoanbqvt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cpxjtuxn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qpmuyfla.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xniumaqd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hagjhhbv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2llkbcwbt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzhtug.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2psobtxwo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2rmgetcsp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jkqtmsew.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2deolfkyp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgyyteow.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2butxjjxm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gobnsnvq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dbdehcqh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2intrtdeo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2uzcahobq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2faeficzu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dpmnpilh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mavotoax.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2duzvozyy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zkuostxk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dakavexz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ujygxooq.html


<!-- 参考信息 -->