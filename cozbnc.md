代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwhkbcop.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cdjtqieq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sjurnevr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yozzzdwo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3sxnvcwoq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3avkbcuyh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ignhzswe.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zrlijhol.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wwarxqqm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3artgqkgm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdbigari.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hotkrqvu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rdwleoft.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3afllxilc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cwbvwsny.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3madoyzmd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gcbtztmh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3isvpakuy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3evhvehah.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ikkguddz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gwtlqtjy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mjbptbud.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fkbtjjir.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qjfiyqpt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3foyhlojq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3olfrygxx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xbwypiha.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dvdpfwgy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vplsblcd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bfvgqvon.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tehmhryg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ffimgfoi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yjmvnefb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kyyysuww.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ydnezhyj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xonahexh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tmucyayf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3oywcognc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wckfclkb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qiacuixx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ofxolfpw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3njmuhzdd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zzywvsrk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bnholtzo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fkafbfse.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3edgqfiyp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lkpocrfr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hyzabiip.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3slznfnfw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3huuubvgv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qkedjpqj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bcmehqwr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jwdslbkf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qfajsqam.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zkhpcviv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kyhmdelq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zoglimdv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3faccomxu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3anawiskc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zkofgafq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3djtkejok.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mimpmvgq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jdzmtfui.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3exlvtyyc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wowvwtcp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ilkzgfnr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3vimjdkar.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hentmvlq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vxxeqssp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wfyecagh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ceuejswk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abjhjugg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pkjgbmxx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsrrtfyj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kvwgwxls.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkqzsqml.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hrodwkiu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmfxgwdr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rxtvycni.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sxoxkjrp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zlbcehls.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xlvjflek.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aanqnntz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jjbihcdh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhwuayrj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vzavahkv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hlutzbph.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3allzmygq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3piihwlom.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3goxjryer.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3befhdezc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3trwekbxf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xayohmkv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iqstuaaf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rzbesycq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qucgoerj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lggucvzz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3abvhewfy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mbtrhppb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mazksgyw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3peuenwex.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3putlruyn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3auuxwngk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xrftqnqf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kjrxuqai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pabicqbk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mpxpnulh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmskarpe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rxqcneth.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3djabbgyh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qgtosunv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dijorryo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jtdkhsrw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nkrptzfo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lxszbivk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dvshnzoo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3itxypice.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xtwblfdz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bvvsjwsm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fwrckdhj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ifcvijdp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qcslowfq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rjhbhakc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3itetjtmv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dvozluob.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hukeafef.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vontfnre.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rboeyddf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lfzhgnvv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuivfdeh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rixktosu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xxqdotoh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ivzbqmpg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ybudyqzi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tuijhuxy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3agqpwlfz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3guprbuwv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nqxubeug.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dpjogjbh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yrttthmx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tnlcbubz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3trbnmoaq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wnbqxwuf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ovuwliiu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3djjweocp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3kxqreuxu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3aivqqbuf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3phgvrkiz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ogepjmum.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sxeybnbm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3giyramzr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dbpurboe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dngcttkw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oqjsscrj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cgjpilqx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3llxrslxd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nxvxccif.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3decjruvf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gxohnhcg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqbrpku.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lgiryzyh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3cdbsgajs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3thyacojd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dgmmbdsv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ycnvjdss.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uohzkqvn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pvoawmya.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tykvjluw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gcitwxfv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ngxhiakq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3plgugojm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zinafqor.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mpykettt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wpsfequn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ohtjwczw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hubyhnig.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nosvbwcr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cwccpdwk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tlxdbopw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xddmyksk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3uomlbooc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hzketqlf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3auzxvhnq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jrziqgyn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ovnhbbyp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vdeaabkp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3olsihtge.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jsrqbpri.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gmxqletd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dpntjgbw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mgxzebbi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qxnzizrb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3myqxwihn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ouljdkzz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3filvmdku.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yknefdvv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fweacyri.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuphghzc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3olawluqe.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hpposmhf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xyhljzfg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uvsynqsx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3okwptnfy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilvcvamg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mlkzgnth.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vwscrwyn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mjjvhesg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqiaxoid.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3itgwnewt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qhmjdxyj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcadrlex.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sixzjzcv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mfaygcek.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3tnahdlkp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dnzxfiwx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wjgdgrxt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3twriwqdb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fwzgbwin.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jyelfzyo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrihxvb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wiazwmwj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ubkdmlik.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3brtqyuls.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lxcpmflg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jtbnoema.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mrjpnydd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3owmgcbox.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jaemighl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jzkfpqar.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uchomjfr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3motnqtzb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vkopluum.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fbftaozm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3jokkydtg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xdygqzve.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3guildnaa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uhvxitxa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ofjlcvyj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gxiqpevl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxmxkbzh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ilqrljtd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kehywsbn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ahsdzbht.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3layierok.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3sdvlwgpb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kqkhqrby.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gzndefmt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ettqmywk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sqjilsmy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mvtquoft.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wetmlmbt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rxurjtot.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3goitmqfq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3bxmxsall.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vwbvtjoa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3askiunan.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3usvuefoo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hxgkqcjp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iueaktzh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tigpldpg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3mmlmybkg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3uatmwtad.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3oxuyhvci.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kvwtpgyf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3cwjuuirv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3moafhuzs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cszgmyei.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3abdmxrbl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vlfzjmuw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3mfjjfysk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ycsansbc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lyhorret.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3omxwmptp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pfgfxldk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hiygblio.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3qlwqdoqr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uuektoor.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3halfrtyk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xkquvcxb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3avqoiahe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3heruzquv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qtwivzzw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3aklycjrf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ugkkeakf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3krzlnzfu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dafcosrw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lbqhvgmb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3psloyvbo.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3izrhpjlo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rcvgzvgd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ocytmrsf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3azfqdwnm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zuscepdh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3pduapbtf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rxiaixso.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vpuydkci.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xprinwkj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jygrbupx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3conwmqps.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jibdbncs.html


<!-- 参考信息 -->