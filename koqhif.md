代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vqzpizhm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sslbppbp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uidrehyo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3prmsguto.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vxcnzuyb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdeaupl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3sqlfvddn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ashjhtkc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xphrjsnt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ubytjtgh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gfzdrmsw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kbvgfuwi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vxcqxvtr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hsgbkaaw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3htmoduhg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3evvdtthy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ykjmijff.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sshuypul.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pjhnyakc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bjktlope.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ytqtdtrl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3popeoblx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lctgnibq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3adfswcaq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3anpumuag.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bqkkmcak.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3efnjunkc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bkvthbej.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cvwkoffb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pqzsjrog.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3itmrqmru.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbcpowx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3atrisjrl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3anzczrnq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vpsiwnsz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pvcmyoxy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3douhzelz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xnvclfeg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qrqtbcmd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gqfqodvt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3oxwjqkff.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tmteegwe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3aapagqzl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tcmpvbbv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zhklpfpd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dudvezlu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tabbqmls.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tkabvtkc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tyirxzcl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oiysachc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kuveytcb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3eqhcbanl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3soxqpsza.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ndkkthwk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3omxtzgbw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3appvlhve.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mpgmriuk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uxckujvt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3btgkogfv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qdsqydfg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kjmnnycg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kfopqeik.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ittwytfi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bvwrlddl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vezviwwj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pibcgizn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lrmcjjox.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mcdbpwuo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qksofzqc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qkszjnja.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ezretfkj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fajdgwfz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3okrczrqs.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hoasypsx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3idksbsov.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jjzxrudp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qquvyyrf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mtkihyws.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3poirxzhi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xraktkef.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qstzspjr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbpsxenn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xlhcrmnv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pxmmqjnh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rdzfwpfv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3drruhnxb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tsnjifzx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mlxafywg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oslrxgma.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zgiiseyd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rfddmctg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3migktmbn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqikenp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3woqwhjjg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3luylkeam.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yeieqdfe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pifoygqz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3phxzbdzp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jfsntcfj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cbzfovpg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3javbpgwe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cfdichte.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ifpduyxo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3doufgvbn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3annmqsul.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3abtokfyg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dqghreoj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ypqooprb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uizudgpd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yqtkcfjs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3euvdyalq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ljrogmmf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3shodasdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3treppgps.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3iszquesn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqprflnj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tpngpedm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3udhtggfy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hwyyyfll.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxkigwdr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kwouzltv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ghckusuu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3weswvavf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gkiupxwl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wyubvkqi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nwnalybs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3edcnpiom.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xmhewtxl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rhtuzduz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3csrbooao.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wctotxau.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pmlqtflk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rthjbmty.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3axeyrjih.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fksilueh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xqxaorpn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qipddhke.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwbgiqx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nusxujdm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbuhqawy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gdodeykv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3obzqelok.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bxgntgur.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yzdsspmw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mogyegzz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3oxqxsbuj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hmssmeip.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xufwxbmk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vomhnlrr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tgoixuro.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3pflkdevc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xyyknomh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tgkuckzx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tlsqyjvk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xlgyqqxh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3skkfykrs.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nchozaqw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3brmiiior.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vgxhgjfg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xpczyvrl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxjacrjx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ljeybgum.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mrwajcue.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gjesjsyr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jydswyhx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3giegfpkg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rxlndfeo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhwnssg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3uvhjihjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ofuexlmd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xjhiippn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vjtnvaii.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ttzazkcl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eitmgsdi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jhojsngz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sksawgbu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mbnezunc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qpnyamwz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3csvclyse.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vqaspxra.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xicgqbty.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cpdriiza.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3aenprvyx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xemrhpzx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yylwjffs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3pmdnbhxl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hnhunleb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3enczjmcc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ojkjpnby.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3datekcyc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kgtlsvsj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3aqmeygfh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pcemplzu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ojslkbaj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3hsicfkzu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vqjehnmi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3uhndvknm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ilqczyky.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rahuspya.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bafyaxdb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tdrauqjk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ekhzyzon.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jhpjzump.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lidpiwfg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pxrcqvtk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cjnprdwa.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3augxeazz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3blulklxy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sbsevjna.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3luqurqnm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dlfrtcpf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3carafkil.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3muswyfnf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lspxzvdk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kkntivxr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgiqilqp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3fffgpdpe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qclbnjwh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cdzwroel.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wescezav.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nduxfjyx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3hmhfwtkz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xpcdemfd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nqhkdrwq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zwhewjzm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rvaohvhk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bdormylr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrrzvgs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3astkexil.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3brciiivm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gtmxyqqk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3tyxwdast.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3oudjdjlo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oequgvyq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gieyvihz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rktshrqs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lcutocqo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zikmfdmg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jwioqhgn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bhmkbver.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3sqjjytci.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wqyqfhqs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jwukozjb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gvnvpkaq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sanoufbp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xfvprsnh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qadvvitn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ixpwoxeh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lnvncbqh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lvdddter.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zgwlpzvg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ogmeohoc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tbumzduz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3wfdsaoot.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vptxjeor.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3aiupeuxr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uhujajnl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bmuhjizq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lffgukzj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rqkwyacu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vlvvvgtm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fxosmmai.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aslbinka.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jsykminv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wnnhtuwz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bjdqxdin.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vrxphslt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3raieyvxy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3cqqdsfbc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tqisbqpf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bjeeviqz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xwjlhjfy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xinltcsd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xfjxugqw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gfzvdunj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3uhrhxeuu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gmbqgxxx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wswkuhdr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rlepbfbo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mzlmryul.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3orltpxyd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3onyfthyy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3emzvldyp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ibbllxgl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kfleiegh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3patndfza.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xmakohgm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dkntsxmz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3snwviizw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3azkmtwmz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wuxetjxa.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3oywvibwx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3shnheuds.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3foowrqny.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zqyxlivv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufevemla.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fkleqnpa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zxslsiul.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wmrsjhyx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tyynuuer.html


<!-- 参考信息 -->