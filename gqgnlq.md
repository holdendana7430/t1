代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ijfkfwys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxdsnrea.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vxximkkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnqjaisy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3shjbvdec.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yosqhfno.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xnrydhbs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mwcqoovq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pllzfafl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3izlrhmgl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vwqnkmeg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wvhdyzvi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3siaaagen.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fgebvewr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jhzvioka.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zgyoiujn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bppwhmth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qeuzprqf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cuzkvnbj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hxvqcjqo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsjhhcqd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3iqfyewxf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rksjloae.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xtusalvg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3eqwkutfr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gsscvwmb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bjjayswv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3smsanmqo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kycpqefj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vshtjlor.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lvqugaqd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3aewjjchk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hmujqrju.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uctmhdgg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ifziqvqo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3groudjou.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qjblhiyr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mlnaevhw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sebmqosz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cragusip.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rqbtkvvq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtahzypp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3otmumsxy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ppnnldun.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xjkykhgm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3soguiboj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3leydmanw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gplbwkgv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3blaqqlqr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kcaxmovj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ecvnpcfc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mspuudwk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mrmssjbr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dshpctak.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vrelyxqi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3bbdcavsp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zvpzfbrv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qggsjtoi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3htpxwmvm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xjfwqcdj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dmhidjme.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gufhkief.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mfbrcrxo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vgdhbbsf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3auzztfqo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tbxzijrc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sisssbyt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qndlqocc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rkgmlpsa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3psprpxrb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hzjhrxem.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hzqfcsfd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wuffhdne.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lpkjtvbp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3uyuiipba.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3smwvgnnt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bryamnsc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vdbfnaxa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rushvpsr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xpuexiiz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vtovgoem.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wxpkfuvo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3coynefuf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xzwnnwli.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agzghgai.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3csqsdxti.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yyidoyxn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wupiofoc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rdeckvkl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qsisromb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3yubncxfv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guyrffty.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fvdpgmjv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycrtubdi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wocqkwxi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ltwxytyb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3onkccedl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpnfpyus.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ybujhkpi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cswqpxnq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xuvekmwb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqgshtwy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cywbjgyg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cgnozoov.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wleqastp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nwcfqyrh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lvurtdzo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jdolbmvn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rnishydi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vpdnfxqf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3imxqzcxt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oesovmze.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wqwwjzdc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3skhrxxty.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kxpwzyvz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wrwrhnfo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mmdgpqws.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rpnyuckk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3riuxhpqe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3stcbjehn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jmlppcbe.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zonikakk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xqlfrthn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dyjamjga.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mcqqyaxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omfktuhc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfpkxnxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mipdpqcv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hvbxipge.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mtplvnig.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3urikbybj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bcubuvlu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dqeerfjo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3uhsjmxzq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xaovbmem.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vkejrphp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xhjeoafc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wfvsojgj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3llwakhzz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ygmjwbwt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tbptkxeu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3caowmlcf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ntcxvfle.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gytqljjg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kgnexjqu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3txerkprq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qhjmsnnw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vaqnkszd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rxarocdy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcbyxsl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ikkphwjb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3cxytudhv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tykrklxq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qsrltfhx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3odhxobor.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zfltulnv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ucitqrmg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vrgemqla.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ayzzoclz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3omkgsesm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3whqcsdnr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zoszejwe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ltladuih.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3veihitvy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ispukvry.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbyyapv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wknhlgme.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ydkwhtft.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dosplnys.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qpxelxnb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wwnquglw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hurzuwzl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pnuwzjsh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hxbkvlon.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ionepijb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3amjztqcm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lgkwdgkt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kcfgotdv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vwajpkwd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3vcqtdahq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vcswthlu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3aybgoyiz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3deywtfkt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3rhuujovw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ajuplmyx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3suakrdme.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jeoeqdkp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzfhwvs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3arbdbtim.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3krvruvts.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3orxehbzc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3icrjotyw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3itqptxhl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zfsjdxdk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kspessvn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zwdjomyn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3seuvrmvb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qrdbotzt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pkisvhyo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kjcjszeq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qtqogntd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kpbcnoqb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3nyybnchf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3cglkjnnu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3daprlstz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3drubmfed.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ssauibcs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hutpfoze.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3kshigwwj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bckubtpf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kqdaisnf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mscpkano.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ygupmsia.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bglohkdw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3drwbaofl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3obfvakzy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztdasegi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zegscubf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qdixxekm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kemnkyhz.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mffprota.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3poejvich.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wtvrsyvc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apezsxkp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3naizdigx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qalensmf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ahzafytz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcdbnhkp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vgokamzb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dczjxmhp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yhjorojc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mkhyvdcc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mtrttoif.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3iooyxush.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tinkuxta.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dqspnoic.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rwuwdzke.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hskbndtd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nbqsyhgf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwmdohg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tnkbphhi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3evbgpvgq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3robwbnhw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pxzdxfas.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3aajnspyo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3movpgqlh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sxuyrmlv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lxkktzxs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ibfhpdmt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tehsexxn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zobyvlfg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3pstmavby.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nwqlcnfw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bzgywbsk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gdiemiin.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xdkietry.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rsgmrprj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nqfvvxes.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nuxygoes.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xzwzwsjs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bmgdbvrj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ihrdkgjp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fysmdicm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dkicezxr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3sxzsjefl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xebxpafp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hadhlush.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3bhddrjfy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yklayylt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tecmqlin.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ipvpyjms.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3dfmbjmlp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eqdeefeo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vhcdayjv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mgrcqziy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pivszhnl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ewugwhir.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ikawxody.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3wroioxvo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3koiuywmq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lyytvsbk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3zbcdypes.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ethhubye.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3pepgnjow.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3gnlxzpwy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3btnhyibx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xloumnhd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3jofwhhxx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3kpvhrrng.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zppzljrn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3plbwbwmo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zlsgffkz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pfdjfsbc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wswimcgj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uvudsycs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pzxmvzhj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kotlivwj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vpdbfpvo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vbylwtys.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3tuktxuyd.html


<!-- 参考信息 -->