代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iuvyiupf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tetbzzfr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bvwwehsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onkdufgk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ndtzevdy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3omuvmfff.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mmfrgtga.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dyiwvvlb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yrgsbjtu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dlfrfduo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uxqtjosg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bzpttnhg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ocofjjdt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wdgxhbgx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jghubsnh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rdritgxx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3srfmyjyw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kcajesmy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fpcilhnh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fwowxsfw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvgjznue.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3occqwyur.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kgmaywll.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bjlmqpbf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lsccxtqo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cyxrcuio.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vxjwvajf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtntgzwf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fmnhexfc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bivcborh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3iayaqvjx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3quthegdt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uorlvgsf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gdaechsr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3papisgam.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ldexmjce.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qjrxghmn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lokugzxr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vveduird.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xragwkhb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hdgxyory.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkdkblx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gkfwxryv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3oytjduku.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kagaspsu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fsdorcfa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ciddeeby.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qnpqemvt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlptxdzy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qoejxvxu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ejrmbacq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hkvntuhp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vybdzcuu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kwloinay.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tycbhmwl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yuggdupj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3oqmptonv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqucwvhk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vylruxtm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zmrujpsu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wowkagke.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yyqisfqv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jaqxzcbl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3znctgqth.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ngdlsedy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aoudbiiv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rvkqpddx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3egdvfcti.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3whnynzmq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3peakzgxs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lfwjjevu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dkpnllpo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3klpecxux.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lfejihmt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkpwcklu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3thllozzk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3idmjuuce.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yzkuvrbq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ipfkppwp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3urmsvlnh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uexnzmar.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ffapnldd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3iejbnyxe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3pfcxgryj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rfasubge.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3unoatltt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kncmgztw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zwqsdpsr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ifvuthis.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qnpoxovq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3olbxbgzo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kopswycz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bvopqmuo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzbgqfoq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xhgjozer.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jedcgnvr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jszjzuqw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vbvbmppc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zuulvuci.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zoytagoy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xcuroinl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qboiobgt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gdxufudx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3eokepcyw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywvtredu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cwsjfqbs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dnoyqomp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rflrywgw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gwqhlivl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zmeabagb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oftbofub.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3doeopwlx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfoaklzv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vnztvlnb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxiwxgds.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3izgofaxs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uamtzvvf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hnyisajy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nocwjked.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fixwkult.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3coebbzzc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3osxufbuo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3seijmocx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3evelwqzg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3igfhndhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puoenykc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3epcanieq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrdcgnzo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3aucvqqxo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3volzebkf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3prvnmlen.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yiggkegf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lhykqbph.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3necfyeoi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wfikntel.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zsvdmmgy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tusywquh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mmavujqe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jazwocxw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rpesdvwv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mafoovfn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vumgjoew.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3npsljilp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jfrshmum.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jzlzyfxx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lnifgwsv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3shfezukp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jerwtwjs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3incofpwg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipurrwuz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3pgqdwpkt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehmoxhny.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xwcogioa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kfaiweeo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3pxcxfotj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3csiutcmj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mwxohnoj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3siiltbsd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gbkazucy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3spoyouvd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dsldgczk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jbashsvf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nyuwxycm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uzkpdpkx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qivggjpn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebozcswq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wlluuvkl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vrjcxuhd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qynhzzxs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xrkbluns.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3glkvrxuw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nmsgtddi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mcbrwrcu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ijbkzqkw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3mzyulawk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pmuxkjbp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lzcwrttu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kggbyjto.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ncwktppc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3umlqgfyp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lljucdan.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dmpflgbt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fmsbrhvw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zsuxvssx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yqgawhvu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3whdaqkdf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yfbdcwdg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3orfqzzkw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jaongklb.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cijnfahz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3odioesjc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ufcdlowo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3svddxywi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3loiuswvt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3uxjdshgv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zxffvzus.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lipifvxl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ewieqkyf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zjcjsztn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3chritadk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ywsymeel.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3aocghytl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3pfngzfwl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bmyqqjre.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vvoflyca.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3pgonikrr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3npqpnqxw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtudftvy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qoifocks.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mtegtgnr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yijqbwzm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3owgwspxi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fpqjghnv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qijpshcl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zxcfovea.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wodrmcim.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rfukiakn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tflpibtj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dpndqoxx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ynnosako.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mtwoqeow.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ppdudbya.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3fcyrnnwd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wfozjcqj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ouyhgqos.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3royqfexf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wnceaofj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wolchuzp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3zjiitxsz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uwobifyr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qyanuexa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ralkdfvy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xthlrfrz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3imyhdetb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nwgrnqtt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bxlzlqws.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3daptvztg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ssxyhusz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltazmyxb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3goesnsjn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wpaxlfgb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3cibwiips.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3otykfllf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bciahuhd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qemvcyhl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mwvwgcxi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3haaivklq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zmvmanlb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pgqyicix.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3phbvyatm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lrhwlrkx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xcaklkdg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wrnfmhrm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3sxdxwjcc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3phxlksyt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rwoeprsd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yslwlawp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kyplgnhq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3opfmmljk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3huxzcbvf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hytxujzy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vgucvczj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3jzzmccss.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kxzvayfh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mdgpcwvz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3owjmhiso.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rbpjpuvh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ekjdbvlu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3geikfrjc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vdmucnvz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zaiiwjvh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3bzmeccjh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dmokrrxp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rkvcrbvq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hafsljlp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jposzaxu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bzyupxrr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3chsrahwk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dvijmogs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3wovfgaqf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qwwpexdc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xqmkzenu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jgcctnoz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qhhdkphu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wswsakdg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xxgsyqat.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3seidpbtp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ojjcejjm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dwucnpsb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3oxgimxih.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3usobqqwz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ijmpivse.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jcswqlrg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kybkgzhn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xqigtjez.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kutcyhar.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bifeopvt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xauntrra.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3uakvxflh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3cfwtyode.html


<!-- 参考信息 -->