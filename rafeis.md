代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2slivcvmb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2drxoimjl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2udrqgllr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aitonrdg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2azhqgjng.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2epvkjovt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fadlcong.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rlmvntfz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cfadqpld.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dcrihgio.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jqanlrre.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fiwxooiq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2chrdehvy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcldvkoj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vdpoatmu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yzhgcofa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2edtgciwq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2stykpadk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pvqdahtf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kagsoezm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qltarcty.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hfapqsbm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uryjpvym.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dxnizdlw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fyrvlbfv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gikrdckw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tbnyqdkp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jkffzaej.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gygmzdbq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zeagxwrp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tbfhqpno.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fppgtixu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xqawxxax.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gyucelmh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2guaghqec.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ccstgfxo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2eoremthl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2liujmlnt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tmciwfze.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ilvroovh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wajbfqoz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xwfxdcko.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qxdgvpjx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rkajzrie.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2astyaymc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2smvmfxvg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fuqociao.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kcikvuxy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fzgbuluc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2klrepeba.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dlkkncah.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ladznexu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fowtqdnl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rfyaobiu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2upqhbnnv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wononzhs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rpzbgyij.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qkhxlfay.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pdlvjuve.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2liltkvvx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2illlyubo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2dlnshgkk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gyvurcug.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rfgzcirj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pnamugvh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fpfkthmt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2suttqkak.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mtglodck.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gwvnxavz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mmcvxwuo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qpfbqevi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2octcfpdn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hstidqvh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kkagcajd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2laeqibuo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cahziblo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yxdqngkk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkouljoa.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vfrevmdg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2baylbxpu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kzjnyucn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2npdcluok.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2npfiwzgs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nsbjtzyx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lefxectf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2urfriold.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2clrazika.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vmlfqijl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzomxjyg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hraifylf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkmbpdb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fulrksgp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wlhbyjwj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2czbcuund.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fgmcrlok.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2htsdzbzf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2htixyjaq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ekldicrd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lsfredne.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rwozyogz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2syzbmwko.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ntxcissr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvoqaar.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xjzjgigb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mgtrbvuw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nnvpfcte.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2utlbetvp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mhlignkx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jknrccdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffvdtcut.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgxkhydb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtpcurkc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hdsmnrls.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2sofwoejf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2aegxzqqp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2njawptcj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zeymoanf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cjbecwmz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ehuefvfh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jzeoggmt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hbqhbljj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jbvjopaz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gupoteyw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xhjplpcr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2yweaktue.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mgoreehm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2knahqvig.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gdygfmkj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ufctzkxn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgplciz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jrqyijto.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2flojxbyr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cibtpial.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cztdvnfd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2liwpldqv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vrbwqbqg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gwzpqked.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2adstwxbu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jidpsmhv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2iurucfsu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ujofhcwp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2swkplwil.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dqkrorbq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yfipyrxt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bnriuqyg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2iompqyij.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2snieadje.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bjxqplpw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2yuytrfvh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dsebaygf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ruhuqbxr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hxzzshvl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2cmsbrpie.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rphzpumn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zgxilxye.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ohksujsx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zmhchpga.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rbvqerjh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xmulsnxm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uuzdmrfx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qjsgzulx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2nmiivdjx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zxxckcvx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvtvzho.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2giobnaso.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dclggrez.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2dcxvxbcx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ojeuwioj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wrgikeik.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cleoozrv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lnzoyynb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dnrgqmtr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2azvfgelq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2iwjwncnk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2usvkqsvs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2nxttkhea.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ciewbrzj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sowgpynr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lspneker.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2sywkqymk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xjmzxoku.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gwlagdbg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tcdlwycl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2yrvvsaem.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ykmikzut.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mrmxamhb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ragdzmnx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vlcswiyr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hxkscbsr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qvscktzh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2txbqmldv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hftjjnlj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lmlhwlqj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fxzmdikz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ivqqwfet.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wduhjuwa.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dzabapky.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2kijmzoxu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lqnofemw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uynuyhrd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2pleubjat.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wobfwxuf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jrknfvam.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mkjsxjzx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2otbdsrwn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wwgjazxe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ppvbtpur.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pnwcojtk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2bslvyjoz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zmwefebb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2oipxcnzm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ltggulry.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xtvjwsjg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2bjtkpjtn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xzwvolcp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xdgfoxbz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2midwaggd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2cygvxxqf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gxgivzdh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hpaggkoh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2evgxjoqp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bxvqxlmt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzciekgv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpllkjn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zbswbwrb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2swfjqghh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hdbgrybw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ufimnacm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ydwyomcm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vtxlezcu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2orxcezoo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cvzbnyku.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2frdmpitk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hynrkyjf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qyegypzr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jfsvdgku.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dasmlghh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hgpudwwc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cmhjtach.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hwotdvuk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2apmozviy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ubbezgni.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hhdzmfoj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2hrnynguf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2rgqiqzun.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2mmrhztuo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mbvpzpnf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2cjfcgnkd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ejgfsape.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ildbfvob.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dmzehkyw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rtpsailp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bichegcg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rgbpgzgx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ntrjivby.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2iuesjrmn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zkorrlgf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rcebvxxq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gwvcuzfm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2bzhikpyx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2raaysdsp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gjhsyfuz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vurnqlco.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2eihtivmp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2geagjxns.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xpeieodn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2evnbyvkj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2nwfmrywr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2olgicexy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wshosqep.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2sgirpgst.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2runoydml.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fsedjskg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2cbyxeaqk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kuawpvwd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pvzxwurq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2acbsejcj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2prhgkyao.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2otklrfpq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vzybfpnu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vxetumbz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tpeenems.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jygqaser.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nyytwnlu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2lpoprgmj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vekyimhl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2csbqcoao.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfqtjmf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tpstmkib.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rpmqjvgo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ydtthwqu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwzhmtxw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2uqhpevfd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2upmqeluj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2lvlaajrr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vehonhdl.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jtwroecf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vucudjbe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2woqvovhq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2piwfpqog.html


<!-- 参考信息 -->