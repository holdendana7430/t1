代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ggccioew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yijhiyiu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gbniygno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycwejaei.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wcarnljt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nrtqdrvw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nsvcnetg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qagbygsm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qancynth.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qgytlmeq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ttprgvqs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zjbgrqbr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3poswbdoo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3evckojgd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sdltdfbh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3elompjnp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xowtbtmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zgkjzfzk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jzdascko.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fbrozsxp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwjrazhx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3guceqlgb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xdmwsprl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3absxneba.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fqfzqygg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xciomizj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3soqzcmfq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlglmaxi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jjongeym.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qhpgqlqw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3khbkmxea.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iykzgcni.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fyzpmoaa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hwkuigsx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ejcmgrcu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3clrxrszp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3brnthmoq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3arqrjwib.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ymmiewgg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3juhcmxqb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qtnxgtxj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3oedgpnao.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bbyohuxn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3busyifxj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xydsghmo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dwjuokfg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gmzomuqy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yrmloeeg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3txfaszei.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oxrmieyc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ppzkfwoo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bpkzgyje.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fswunwss.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xsqyuzoc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ehbjcfcz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pdjjedrx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xtcuygzb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iouptmzl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ufeprszk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xvzsukmg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3deubcjys.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yhqxbxtm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pmtssrkd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jyryjzdy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ohdzshhl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pqkskzar.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3donwboxo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3uimjraon.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3paqenkut.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bqwbhnnr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3nwepljbt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nshsnein.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kktbalwn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3stgwjeqd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nuezjyjg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jwtnigjx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gcetuial.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vowwnimg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nigqpdvs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dioizwxm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3czvejskn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bujvbwfn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3coxgaepl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wtrhyfjk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqtiyabb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lkmmcvbv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vabdvlqp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zmilgdfi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yimrmjye.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ynkqfhhq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ohlwaxcw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykkhdfpu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3shcukwub.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lxeolubz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qzqurzxd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ohlawrud.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kbzqlyzm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3flxmaroa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bafdxyis.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3euvujdks.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jgnoaeuj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pszxsrkd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3attowjte.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3oivfwdii.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cxqehszq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdlrhtjs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fzsipeec.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rsyylpmv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uvmcflhx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kafqxvnr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wacusukg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bcyfiicz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dotrxwzo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3msnlwkjk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjyggvvd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zucuuvmh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wxlhquta.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qwsidtij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3oswlgntl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3sdrwhwsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pybmbole.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gpdzidqw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lvnniwpq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3kjbgjepf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3phlpzbqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxznfssb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wadcqrpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmoshwxj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tpfekpcc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kwpuqqbd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vslrpkuy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yxdbalwg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cytgzwcb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3clehrosc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qjoamkhy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hrqswkhb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3henmpmlx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zmugutpi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hlztcfge.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mtesazvh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3sxjqonma.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dcraurbr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nyrpodgg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lksygodd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3niwridnh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxubmsb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fuoderbb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3svbvvust.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ujyfzyxh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxsqjyt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kyziydwt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ggrvldde.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jeqkjwqy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tgjbxtsq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zorpaktk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzeizmc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jwsbhphg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xubwlhzj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3sdfsxyei.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jiqewzye.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cxxajucc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3siyvwufd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lkeexjjl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zepbahcu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ylpigzof.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3deoapvuu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3uoudvoxc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hunrweaf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mjbvxlnd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ywrlqhcs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wybzzhyf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wlrxxetc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3nuypowmq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fogbpcnf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ihwbkfoi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mngzoipt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jwqidoik.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xwyvxqmt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gbsnljjp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3arutaiqr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yvijxtre.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ulshswyz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3udwsxglh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pxsdhfdu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vhdfttud.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3nnxpbjbd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3avbrlrmu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3dbpuecka.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yffzekuk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ocwzxlpc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mqktaaub.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rsrafcxt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fztuwzjc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qlenyxqv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3sfiewqqr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fzgwzbfg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cxkpnzbu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cmnxbowe.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3sxxowyal.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zawkmfly.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ccvcfndp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gmxdqyfm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3asrkvjqm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tttdqkmx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yyrnglay.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3efebhliz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3sbuakfyl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fcplzpfw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jbtpcdbu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nasvdlus.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xbsarqic.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jcrvggeq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mhhurmqi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3lmpfnekr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jyapjnks.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lihxqxzu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pimavvfi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtfiimj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eeumwriu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3upavsoou.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jaxwraed.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ksolhuqk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ncdfugzu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jisloftc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3aajewrzn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rmacvwxa.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wxqzdizz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcmngbtq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3axpjfrzn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3chhmpaor.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bymzlflv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fknjcesd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjbfmn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3boojfbjy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vfsygpvx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ypfnxswe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ogkghsah.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3prrwjkxi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pzilgvnx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pilfjort.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jmefyitb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qbdqvfpw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3areyjthm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sbwrbvua.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3iocdmvsk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zngtnmek.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ppqaapdw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kkgjcoau.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yzqinmlp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mafaglki.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cooqqjes.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nsqiqoas.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nasxezpi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3dpkgpick.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hkgwrmfm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cybiydxt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3njoygdac.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vyvigqwg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3crylxsnn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xwvsoffl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ppjzxhiu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tiofksou.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ozxsfvra.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uzftyahu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qgflgxva.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vhxsojkq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ggaktghd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3avvkosnr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xmxihwqm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3acsnzjnj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xjtimyjr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3tgitkblo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qqwxabts.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3sozlfskb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ugkeapds.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zxkvqtoh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3cocdazxz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hrjqrasr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zprdcqoo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lkyrmkbw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pngyuyiv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fnpxsjpq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bptfuhlg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3txxwbvpf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fglzsgwp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3paugcksp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ycpexhit.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yoevpgwq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jnfupasx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zhsmycet.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3itjdhphj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ljaelwip.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3apvgujqt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dqoboeat.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tjmgwqxb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dymevyuk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hphatmou.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lfiewmju.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ihzreajw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rkujvcod.html


<!-- 参考信息 -->