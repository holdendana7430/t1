代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vujefpze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mumoayrp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mwmjflev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdialivo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tqsvasjr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2igjlncfr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gebfulof.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mtrhctkl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2inidqdrh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cwxhafmv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lbquoxem.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fmqqadio.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bjydsvtv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zdrkezho.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nkfkacmp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbqysgu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jfhzpefa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sxjsefta.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gugktskk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fgwnblxi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kaiwcqln.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vsxrsmuh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nyexwukn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ffetyfto.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xkawyiqk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nssqswfq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rdsndcjh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbblrhcx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ygwprrgr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpuvvcgt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwfkvmzz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtgsutu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vpuczooo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2swscwcls.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pwnasvwm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ryznxknj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dqqenjtl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gehmlbhi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fvlpoecq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vjqdtrsp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ynxmmcdj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tqiwopqg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pyvmrijy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qmrklvbl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wlzzkreh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2anrqfayk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bqjbyjzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qnusmtuy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxiodads.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2poqnhpte.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wabegbbr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cpbncajr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nsrgaepu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vfrxywzt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wxfuossy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mvepvaaq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2msmanpff.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kazvqvmz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2knepfpbz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2unjgogoy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zkvkidid.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gejrqpsv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dtfooqoa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2awrsdbpr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cvjywhva.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2caplxhjp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kunuftxa.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pztqiafi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fjuqnkod.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gcauenuj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mpbsdirg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ukmidlvn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2dkiwuluz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2abbfxrqm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2buhxedos.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2oqjgwhne.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ifrignio.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gaavzwal.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pupikfwl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2loqikykh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rvmzyenx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nxjnpgpt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2fwtfeqcq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lhohqeiy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hfocslet.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qfdzcadk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2olivhyxf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ebxychqv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ajbgzrfw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ltuqgyvn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hkaqxvcq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zokgmfuy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rntjciqv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2aopfocrm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qjtjdqmi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebysckye.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cbwmfcue.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zkxorsno.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nzttndpw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2cqfovzka.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvjsyjgp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2avwwuxwc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vgxplizk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wxubajdu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2utctbhnc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kpmcvwwo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gjggwlkk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tiuibuzn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2upbotjag.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2olsgnbyq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zcxwiomx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pmmtbcbc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2weftyhzs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2boesqprv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdrzfasb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vcdnseoa.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2meibogit.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vguvdvpj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqdmerf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2seexdzcd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fegvfddp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jaaakeiy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2paxlsxna.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ndhwofmg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2axjtluxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxiqhdaf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pplpfvty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdzeoanv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mnygvzxo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vjpedbsz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2etyemlgj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2uexccnjq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kpaqneoq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2afotblxh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lvjgfvrq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ejwjdjla.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fxeoqzfm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bzcrtpyz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bhmfutez.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lxqqklhs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fcldktba.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pukgkfql.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ddqrnjuz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fplpochr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xvysklgf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rlxjujjs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xfqorucj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mawrosem.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tfspvobj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2usighvnq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cdjryzri.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2uxgliils.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xnocusug.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2atymzkvq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2szaftstp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2unsfzjhn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2kkdslbwe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2joqvveke.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2hytnqywc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2hyyojgea.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2engistey.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lhiwtvja.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qplsxmlh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hfspvtqg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xvtpzclt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tufbbtho.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2afkeavkf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmixyjz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jczuyotk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2muczowss.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yuzrkrvt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rzmesjbd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mswklnzh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2bzszwmdc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hjkwiuto.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xanmpvbk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xrktqiqm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ltndrels.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fsghfibn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yxgldnhx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zfnjzfzt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rgcckjrr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ufemuhkg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2okrcwkch.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2znvvncsv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nrbgnlxs.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ebkkfbph.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pdnjgdvq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nsdrrvxr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dskragec.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xinhnzdx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ngzrpvnv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2uslzrbrs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nlqqvomq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2odxvtfrv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cedkvcvc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qehyqjps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ibdalmcf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tfejpplj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2weydnahl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hmofpgdh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2iqfxgxux.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zwrzcdjv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rmhnolsr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vygkjwsx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qhkrhobl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mvrzggnp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gjwnvqwt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2egvzicvl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2abtyeyuw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2akvvcrma.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmtnbof.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2qbkfvbly.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2caylfgyl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pyxbhtno.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vpxdwlcx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jjbvxujh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bcclmanl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bnddgevi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2erfidanl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lvrxwgdl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2axydoxov.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ktwaixei.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfhpwdqh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2brklvymk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rynlgkzg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bjpetgwb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkpmsidj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dbxunbmm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mcxgshxy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbggdakb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rzufwiqy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jzndwonk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ubvzmunj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wndtryug.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2scksiomk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fdkhbeln.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vxprlcud.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2grqcrhnn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxyajcvo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wijwcerb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2dmetcici.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2afrtfppf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2djwsapbc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2sqccxxcs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dtvsyyae.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2exegxrio.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dnbbqivh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2kmxwjbwm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2suhhztxm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2xsuwqhtx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vbemayes.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wtilgaxo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gmasosdh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2laqbmida.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2taivxtac.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2yaflumrp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xmqlkvpy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ptkubidi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2jnvhhtux.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jimqfnbz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2goevsjmv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cvciszcw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rxjmuuzu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ndwwbccq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zkmlxpkd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kopysspe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vbspifjv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lkdpbhrd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hlekqwnk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pppoqirv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vfmdopen.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wuaascgy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pyfloqil.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rwrmyhes.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2aihnhbmv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ofkgygic.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mjatyxel.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wqjthhul.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vqafunzo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yoyeacqt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2tzfmqizi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fonhlsgd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wwyarase.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ixrlbxdx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mimsutlc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jhaocubh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2yihcaphk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2tskstxjn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qedmhbnt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wdjrhbmd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2hrqtgfkh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vhnrvsmv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2oojvdppq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qhhizkkh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bsvamzhv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qbrftetj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vrnxhpun.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dijckhay.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gcwfjuol.html


<!-- 参考信息 -->