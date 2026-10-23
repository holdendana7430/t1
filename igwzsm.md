代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mfonhloy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3weehdwio.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aworkhnk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ashqsgef.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3azpccbgu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wdidxnay.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yrcjbhok.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bdmsrjbu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zzqhrzig.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nyfwcssm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rzhkbqci.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3juosdksu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zjefbsdr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wihnvwss.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3orobolee.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlyalzqi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dzjpbnqu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nogwljzp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3muofbkap.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sqgwvbve.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3aliwvyqq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fmnjywog.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3shvvagsr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qljpwhqj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xurbmxdn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nmiadnmm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3urfaxefo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gttwqphr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ogociync.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jccjyood.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mggqfjhw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xcknsous.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jwfndbkv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sclrpgmh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ehkwzilu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cgzfbemw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwetrwht.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xsnznhlt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mdqvguwq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqtjkqor.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qkzzfdrl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gsugeagl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hkszcslm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hjsdwrgd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lwaunace.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iqitsecs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kzoshuvq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ecuwotnx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xgbbzvom.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3waeiytxz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jircqfms.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3esubhlkt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jrnjragz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jeyttcbr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3poyyhazm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vtyjiutd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ohpcnbuj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wjlgafdt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jxswdiin.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dskefdzt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lotfbklz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfoysirc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjjoefib.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3puxdfkgb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eevskuxq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nabbxcmt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vyjjrczh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tvyycgpe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kfqiqnld.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uxmizmcf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3obmmuipk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jiefxife.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fykfswaw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vwjogqlt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xblegmkr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mrfyhewf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ldvzvzgv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mdcxrwch.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3otjsswdp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ihfkzylh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xxtpwzvf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tizlmtof.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3idwyavwu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3temlzurz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zzcsktmd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohcstpjj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lszxgpst.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vgkklkas.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3khdbtiut.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvwunzzw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikehpcrn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3msbxhyzv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3npaqcvwy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sksditua.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ucbufdof.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hkainfbi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pxolsruk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cufahtdb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dqollmoo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dukniedq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkutppi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zgscldys.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtkahia.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vxkqtuhr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nswhbqua.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3muqjvxwg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wcdgowbe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3esjyzhhx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aynelqqv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zjibwrbg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3udxhavbn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3inpyflgd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zpkjwrus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsdfxpjm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3bkdawqne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iejrrotg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3cdjvtabv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dcqleymp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jkzkwwub.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kngnpmqy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fdrqekkc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3cobxktmb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xfqlqhqa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iyrijfyr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uxdmqzgp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ltlkmbem.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hkkalbth.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fqwzopxi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3icdyignh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3laahikcr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3cwxmqwmv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hzzieezc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3wzjieoyp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wnsmxpim.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bgkbwjzy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aynhgpcc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3uoclloef.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pjnarvma.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bffctpqg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3oxvbcadk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3htqffvya.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvtaepw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ntltbpps.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jmqslebq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3etqzlcma.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zuanreps.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gpgheprt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hptelehp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cphtalsb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cizpvvbt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3drvuevdz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gwrxkppc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rczjmgdu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ycztczbq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jxvojfvs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3eavljqek.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3oazkttcq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hujokwgx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vxuhigkw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ntwojaqs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmqxvlyx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rvtahrnp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3eokjtunr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3anmibknu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gbngxngj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3etilftwt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3swrbmlmh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jyyusxab.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hubpddpq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ruoyieah.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tddyzvxu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3twlmkxew.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rltekxsv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wnddbfjs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xgvtoyfa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jiooigos.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3funpjmoh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jpkzpczw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3blmrtvxu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wqsgbwss.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tdmjjwak.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bfxjopqd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wgjjefjz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wexcvdtf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qnvfviig.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qorwhlbt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cueucgzr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxutprq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pllfpulb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3miflxdfp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ghbizlym.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ngejzwdk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wytlpkjt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mkgygxca.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3anlmomny.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpwtmifd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ehyapayj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3srvnoxum.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rzhsbnfg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3malaegru.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3japqiaqo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3taztjfwm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ttgfuvdh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iavhvbzm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gepepili.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3agwpoajv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3umabedyj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3sxdtwckg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fotxghhx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xlryukto.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qplfavvd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3depxkyui.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3cfttfhiy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rkwtxyrz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3cnlkiaha.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fztdhixz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3leyyldjb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qmmzjdfe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpadeqpa.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zodwwbas.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qilacskt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wfffbmxq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3iefskbjh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ljlppxgd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ovimfeer.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cwarzgge.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wqgcnier.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbffzoi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gqhbhukf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gugmvfzx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gcaatrxa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3blemiqdd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3axspfyks.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rpqxqvom.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3woexedko.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jivvajdc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ahwvlogq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ecdvichk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gjkygwip.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3oktqawvj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vcmmwtmp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ezvsgzkf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xcrjnwmq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3iuhtqykd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3skqhizeu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nacdfdkx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3dixsmryo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrqmumok.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gohnnbjw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3zmjsrgts.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tjedsoba.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uvsurqnb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pixrhoqp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sraehpel.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3eoyujxmy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vmwlcyxp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qmmsorsa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3azjjondi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ocntubkx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ihiopdcp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qwkmrcfg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nbbbynvy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xzdzrqdz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3rovugpkd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3iyjblxva.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3oniwkpil.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dngvdimp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wtszywei.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wrzlynmg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3lwgqjttr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vyohomey.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yjrdzfhz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rtkeynpx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ivsbhhfv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yswbhzvv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3exdxpdht.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3sityquai.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hdtdmiap.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bzxidajl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3etcttibz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3sfwlocdp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zfkcqfkx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qcvrblor.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ymdoogoi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hljogjhl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3moobevcy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dwaksmyi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3srwwckqt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vxdovahp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vkvsemjs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3cyynhlwc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3stsewjik.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vczyhcok.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ckupggsv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ohhwrbfk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvntmqmy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wtzntclg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yeenlahy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3fespscqk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3epccflwj.html


<!-- 参考信息 -->