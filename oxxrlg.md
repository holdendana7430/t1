代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qncjtede.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ajzpeeoi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ggsmnukj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2izcbrxom.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2angqtofi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qldanmrv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dwocmsrm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2arszvyqa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xbncoiba.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tuecklyq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ijvrbqel.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ukfrczyz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2loenarxj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mixfxewn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vhxbjzjw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iapebzje.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vcicbzym.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skonbbiq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fpajaeqz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vstlmyln.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jtulytnk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qiwwjitt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fkppggda.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ldtfnqrm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gdtguaxg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xmemczmr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yzuqggjx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2sffsuxzx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ykyijunt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ymyzohnb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ukzyebfv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pnrhwrda.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2virqykmy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2cwzwhrdy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wjcmfhsg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aayvqzzu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2oujvxhmp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nwcnxxsg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ufurtevm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2csuhygns.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qhaabmgc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hesutlhn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mtnhswrc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uorahapw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ofrcvsac.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2mggziabm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qzsaajpy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qkvlbvmb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ifvrxexk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yzgonhvu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2prefqenz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pqxgzupi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yvafbipv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kgiljbpo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vyvlxcjz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2slbkzdzb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ofxbsajs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nmwudaxw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ptiwbprv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bghgmrfs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hexvaaib.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yyqxclne.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rzgnoxxt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2byposndx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iaxwttat.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2uyscqcbt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jljomjby.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tstokewa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ukwmbuiq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2clplldbs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qlnrlrxj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vloznnpb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hqpcuqzl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2goqeclgd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wfifgcup.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2obmombtb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2owlhjafi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mlidnvhk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ijnogmjh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoypejbg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ulmcsjbf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ajtjljxf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ccmzvyfh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agnrazxr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ehdvampu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2llapumse.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ckkhzwmc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nhjipmyi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfvsbxzu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cpdlnete.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2okgymkdg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mecbtucp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fjtjaedz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cxbywbss.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zynjuwhs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2gyostfaf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rplgbflp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2akhjuwwr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dguzxzqw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pxoaccis.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsaazhmk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uxwrsgtn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2pjmzwfqn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wpvxftfv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yimxnouh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ebvhpdzb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pcgsovjl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2twtzymmh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2unhrvzym.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2txjljmzr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qmfmxhxd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ponzklrh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hvuftzij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndbsmpvf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oruodald.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxfwktdu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ykwscsvi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xwrmfonm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ljllnjqq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sjydzoet.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fhssdtml.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ssudgacd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2tucyoueu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zfvrwwdq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2adawexgb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hpdtnjxy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2yvbhfnjo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nzvweepi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kvmfueki.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ntuunwlz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ldoljxep.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2bdrvwspk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nusfxuks.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2yguvqcav.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2knvttmpa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rtkdrkko.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rdcuheyk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gyywuxvj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hotgcpho.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gokruzvp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lidbtkaz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uwjiatty.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qmtgiiyb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bwrcohnr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sfknbgfz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hkigsgfo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kdlykxun.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xqgwothp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tsdhpblw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vntzyvcy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zevpojla.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fqhvrhhl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2krjtuooz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2doxvdvjk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2sfdgpbiu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xpojkgey.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zpdzjrto.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bhljwlhi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rjwrlril.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hlihofvs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjrytxyk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lyirsboz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cgwijimk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vldbvgie.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oihelvik.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qcgqxtvl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fyvllfjc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vkqgzfjn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ibtajajs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uuojljxj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2chllzzvw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ywixcjqb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2odfliwhb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dqdfzvvw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2snpfjfeh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lgohptlm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2llmarjad.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2uxhatzlx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2sbsxhksz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2usuomkcs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2svhrpkky.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jcwienwe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zrvsdnac.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2crmbymtn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hxjmzsin.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ggvyigkp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zfcpntzg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ftcfazmf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ktxdfjhf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kigulzvq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bfgrvxog.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ydxmgpgl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vodlxmei.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2gjmvscrm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pafxghyj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2omnrpwqt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2glfzjfco.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mrcntedp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tzpnwajc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vhdlnvip.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yodbzfoh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jujssfew.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jhvhseom.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hlrzxwiu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tjxnsfqh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2swlyuxsi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhfdowjt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mydrrkcx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2milxykfa.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vbwfzujn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tadezxrj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqmkrjlf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xihmlskj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kerqvpui.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2endtwlly.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbsxlzcf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fwdtblzu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2oxgsxrua.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rfuypgvr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sncdzwuw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2chexwusq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2sxpjjsrz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aypyivtg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2qmvofwbt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mjjlrjln.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2duldzjon.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lsrsbqbo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wdtrfnfa.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oihfhmnd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2nfhnomvx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ymbnskow.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2igeaucca.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2utgbmcok.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nrkzvetf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2aklbxwxr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2nvczrmdd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2saiqogbf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhfsqolt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xeqehwmt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2itdnonda.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hgkesmck.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aebwflmp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kojejxkr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xwvoakps.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2iohbpaaf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wdtmylei.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2awartsec.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2sliumhyk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kyiicsrd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xvakeoxm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2srpvibrs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vjegyduu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rpyytmnx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmukgkiv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kkrpcawr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2taumrvrl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jacfduyg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lrilvqxx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2yhdjhxnj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cynaeumi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kmhgpgzp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bqakddwp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2acyczogy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cizzkvvj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gvdtgrqy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hmsclwvg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ykajffpp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2psjnfgfo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vfbickmb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2inkbyiwg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pcajhnrw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2jqshcaut.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2znosdrro.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zzzvxpew.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cxuasfdu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zybausnc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2unqbfygg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pzujkbvk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2tlskxxua.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lwtygsdy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xbzvwxoz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cufqhzcc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2cdkhnpuc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2czanpmpz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hvgjilue.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bitmuebv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kakxwdwc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2akpryvjl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2btefsosv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mmculkia.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ftltmztx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mxokgves.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ghsinbuy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oiqzbwhb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2oayhbhho.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vhndcxxk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mhigggem.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ooldjvrw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bsfmhxdw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ttztguzb.html


<!-- 参考信息 -->