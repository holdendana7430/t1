代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2sduieaed.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xziljqrx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oguqpmfq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ctaqjtmj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2amjbtaok.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cvixjozz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2sptezgig.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdkkrsfv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wlriuphl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ooovzrom.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ancuvcwx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qnbgfyyo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2nmodpepw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mvythkqq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ldjqzyvt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ktsvceoo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2anytrsco.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2skmeoldd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ujybqcst.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2iqqzwbnr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2didrbxfq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wifexmtl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fnwsgboh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jhgflxek.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vctpqumo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ztrycmas.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zfqldfzo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2diqqtivo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldyyzjwp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2eshgaxrx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fhkbwgfv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ntoibyav.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2itzafqir.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2aghyyuaq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fprgpplf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dzesrsqg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2buvfsyub.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2isadjeam.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2taagogvk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2sdlkjjln.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ywfazuhv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2obhrwlsw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nwqifwep.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xqzfmsml.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nmeeihcw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ovcxftwv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ykrgrnyb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zakssoas.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dcqdbvou.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bbvuiimj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2eyjdbslv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ybceqgxg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vkomkpez.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lqrusjzb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydovopnp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2utqndhlx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kpjnudir.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ykxfitfe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tyyqujyy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ntqbzjva.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vlxwnzwr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2octxwydg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lgksjtuo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ezbbmyhh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gdxszqpe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tjdedxew.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qybnsqkp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nylgmcur.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ftingjgs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lkutpziw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2umyeqyjb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbyykwv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jaqqyegs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rwszrdav.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2uoupbzjp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpwwfykw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fncqmcnk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2llpjfjua.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2plagrhmt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2vvytubml.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2orbpfhar.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ngzomora.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynzrhozk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2snmwvzrw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlbhnfjy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2edifpnnf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jnqxwmjc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2afsfsrun.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pwmpyiku.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ncucrodl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vzwbhmws.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cijaoyym.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2yainnjtu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hmygkqts.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sztstqnl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wmjwfzbf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kwattlsa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zvnrepmk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eykhssfd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dmykbjip.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jxprvjjb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2emoakoxz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zquecade.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2yhwmygwj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gnqqztjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqqippnu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2iwxcruev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhplmqlk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ghilrlgy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rsvntugh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ukjbxztt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bojjzegj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xqyazzff.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yxjfvqji.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fjastzbr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tpbugspm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ihdxhdtn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2adtddulc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2cltapcyw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uppocopm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gxcvpwpc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wiaxwmkh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rzlccpmc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dxnitgbb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ntibnebv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2eiavmbey.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jfewlcjm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hermdpfu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mgogljen.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rommhpnd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pguxzxot.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2qbwdcxog.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tyuwjrtz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ntzsryxj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rzehsiom.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dylobyzc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pyfilhdj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fxfvxhwg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qkjlkbhq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cvucwfqh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zjcddfmo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2justyjiq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2yeifkamn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zotmqnjd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2pxxbpmsq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2aufshmzr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wzacemzh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rhtbkqdq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2edyexqpr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2darkewpp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ywwyvlmq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jvpaavxv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rdtgiipq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bifpasbr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2iirptbvz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jgvcrjhp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uwpvyzxh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lfedxidj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zwywilzz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hoszrgba.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xtytbceo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2svpqleve.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ttlcmfrd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rjxxndge.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yucbdeuo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wmhlbxlb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qhdfraft.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cwclflto.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2yltaapio.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2chtkgvbm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2sqhrubsa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jfzzrvmu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2fbdddxyq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xywhzwna.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dguqgrbz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vsguniao.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2frgsklpx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2fbbvhaxr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ciwwzoem.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjhvynv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2okgwywap.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wsafwlnq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2evwomoew.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2magpxkdy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2pevjbeqr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vcxddrvf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lemcfjnw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dosewepj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2wwndapuc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jwygzkqu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ydhyssgg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hciqgimt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xeedgeci.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2pjhgzqdc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zvynimcz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2txmlmgwu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lvqknirn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgtligsm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcuksowi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2impevetk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qikusaey.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2eyelrtqo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vuhbokic.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvupacxn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2swewfhmt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nkswndyu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kuushufv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mrraxtpr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ejgwiyum.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ovxlbxlm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vytbcxal.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lguqayyc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2axgbxvoc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vmsehkdl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pfeufyrh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lkekkfjl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dqrtezot.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hdjrwfqz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqujzaiw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aodlxnwa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2imafkzxj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zensrujs.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uisvpbum.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dtkqckhz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2afqnghfl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cqpagona.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wrspsdwf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zptiumgn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mfzficok.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vunnfhwu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ywvrsgig.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cvcsumxw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2carkkhml.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jucvhwca.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2xbuomthx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vpyhzesg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2stladtku.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xyjdqtmu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2oqvxtlal.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ysxuzsjh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2exztcytj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zagaqmbw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ffmvmhvj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2pfdbaktu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2neqlegiz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ximxwodf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2galblgpc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bcmkdmnp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hyheyqdf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2huttaxgt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2prbcqail.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zoqgdzfd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ksxpsjiv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uqgdojuw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ftnkqjcp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2bfqyzobz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rejisnko.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2oadozxce.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2fwceownk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ndzozhom.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hllqyjfg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lvgxfasg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mjktybdj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vwweqopv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sejgdbuh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2htabklcx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wuglopaj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zufnztdl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2oqrafxiq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2chjzzbeq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fzkuwrpl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ijuopggl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ecmruyie.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yxsimxqx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fymzlapn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jcygljhx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2tkgholkd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rzyfmuez.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fjpyguln.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nzebdnol.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hqkuiado.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2tcqosjiu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mwbkjkql.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rmazzqky.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vqqestvv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hgcqiiwx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2drfsvbqc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xawfqhqr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2pdkvjazq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2siqovbaf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ndasbhum.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pjshcmgh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mgaisqfn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2yqixiovr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2godwqjid.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nbdepfhs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jtcwxdvf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2movoaiir.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2korkfpxz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvbcdjp.html


<!-- 参考信息 -->