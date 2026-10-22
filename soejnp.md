代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jtrcbeje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snbsehlz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jhrfzzbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyyaoovt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxoanrjm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pmkdotbv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qxjltcpa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jhyrbacs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2okvtthnu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iiinxyoz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yzazqxlc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rtwfgdlr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fgygcmro.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zrffizrx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mnusvxad.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2avzirfpg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2moenvdss.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfdrbwbs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kayegtcq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xfztcgnb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfyvdzed.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tifocomh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tvtdtiut.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2krswexgd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wraoikfz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2grlsfays.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2elygvvoc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfbirze.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2orijzbsj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2keczolaj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gkqwijtd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bybdyipo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qxbtoryr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jfobhmfj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bmmjwhuq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bewjqgnd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ttjvlfbi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2krflbatp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wctrvnfi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2donquadz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lfzspedg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2olbbozse.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nmoshvub.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yfnqcczc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nlbhabcr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yijhehwk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2riuxfrzy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xazaxjpu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2acwdmvgn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hefesnwy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cdtljgcp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tnlelrti.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ygqtrmev.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2raacopxp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2stifqnwh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ifcreczp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ospxngoe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlsjlelf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sekkyvly.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nttwaymo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fvuffzvm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bxoddhmi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jemvdohm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2acwqzdah.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xczmyfbh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gsisgofa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2croqkvkm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftlydrrg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fwfcfcrq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wbkksrmy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hzrfwzha.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2eiridqpx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jruxcilc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cyivyrqg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gaziyvwx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bygekhvu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jwlucobf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gpoiinxm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cbdejrhf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dkkfhalg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sxteltba.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vdklvzqs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zruhfeli.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dkebafhq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dgbjskws.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rqqarjnv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ciyksvdg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cxphmclg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kgeolscz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oolzzxvl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yqoojasn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swfyyamx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2znqqpkmh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2lgszjndl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2thjclmba.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tysbynpw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2lixflzmp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2eealrulw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ixlfyvnx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dkoucart.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfvnkqda.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2drijatgp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pugqepui.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mkyqyzuy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rntjkeii.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nrovurnl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2etcfnjtk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yinuptag.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aztiftck.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wjbxelhg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lzbzywyy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gyrdyxls.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqpfexog.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pkaegzih.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kklsdcuk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2akvqjtem.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2csdpbhce.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cflgvnkx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gjnwaczm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2poddmnqp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ulfnvisz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ymaihxqd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oakhurhy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2glstnypx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ndxjjgqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duhnmugd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2onoxeopa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umqxwngn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2cluhptbb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vihzwkvi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2paxathlo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jpfjkvio.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hzysitcy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ogygpeym.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ufydzlht.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2itvlxvwd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2enacakgb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bbrturhu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2guolfljd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xqozxues.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uzixyovx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zgfijskh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2unirqaxz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wyiczirw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2pwnbzabc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2buhbxsvt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fjuncfzl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vhexcwlg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2biyqjgtr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2owtpgklq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hgwwwhpp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhgacwel.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xshpxeja.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rwoqzemj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ppynosyz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kxdrxxbu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2brabgefr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2njplixvj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jvziysmf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2oiprujig.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zyhopwbu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tznaffkk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2gyrxoyiu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lgpqzskv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2efdkpfws.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyilkbkn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ytfnleao.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ynroxbgn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ucrsjpfh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cacqcwlr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vmevhmhm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hywzwppj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijrkvzeo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2bfrhycrd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mjdzkcoz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cwdfcfpd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hngrzkpw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2iaiyejij.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zbosrzel.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2icakkjyz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qtgllpiv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jrqassch.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2hfiwtnqx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jdxfzdvd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2isrzyozl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2onjawvjs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2drzlzybc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2depqxhjk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2pewuuzca.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ktzlbdmf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yapgjywa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tooihzgh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2uyifymcg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qnrtanwp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zncvjoyy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gkfjncco.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jyamgnvp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qfaosjyu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nnkdhtqq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ecpuobuv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mmlykhju.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ovivacla.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2uashvxpd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2texuqztx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mndsubfn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nfkuzdry.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2uxssxdzz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqtrudm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fwhrbsuz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2oxobvegr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jnlijnid.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kiypzvof.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ocymmidy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qlbnxugd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wikqdptx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gnqnhjcr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nxgacmsd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxsqvaip.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ghofvkmi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ymnobcxm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qizqhuah.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2zyscovcf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mrmttsvl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knuqyihy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nxdmrurc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hvxxnkyu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pwdvvwvv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thjqrkoz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ljhpdece.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vcyeaqjh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kboypgcn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2svqzqhbm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kyrvpdpd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lxyhspou.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2finlsovd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2eiellblm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2oppzgbeb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qfngvlxr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lvnohpcg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zmezbwxj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kbefjbmw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jfjvnjwz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2erfzecsi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jttkarun.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2japasrlp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vwlcpqwq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mstyxnvi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2luszvqcm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yzhzrjsh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cpyplkob.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qtsopwhk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2wxxsbyie.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gufhswku.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2utrxjive.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2orqwypyn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tfwetdvx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2sotgcqah.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cuiryrme.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hchmwqzn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mjsymadr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jzzdxbzd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xodffctl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pintfjjv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ngropxkq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2afodgrgk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2sasibhhj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2neropign.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2yzhqkknc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iqovjovh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hgrdmfxx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2seoitjvs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2divykvrl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bqbnoocy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ujrpqltl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2doizijes.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hugxgkfb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2gzkoeuxp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2sjtpdhxs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rxsnpraw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2edmetily.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2msmesior.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2pwlozfrv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wfxpmnit.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2patxucxc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2nagprpbu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zfsscmhz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ektzrhrp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xxcqfeen.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lpltpjwq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kogvoftb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qraunlac.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qqugcxzq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nrvvfmtn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sqtkkkvl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xsvwpbrw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2gcnlpinl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2stmoawhf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ycedawmy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2srlcminq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bzicribk.html


<!-- 参考信息 -->