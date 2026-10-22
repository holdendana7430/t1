代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uwbjxnqe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rjibwtgs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yntnkfxq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xgznoakp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nswowary.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cahgdfwa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xayrtkmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioyzrpoi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfrhizxi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sbsdcysc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxclqiac.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2giyjyjgn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bzmnktok.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2olmulnco.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ntncskqk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ufvstxqt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cflwvkwt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jznvbtgq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2eyeuqvlb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xqlzwuhm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xqpxzbgf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iuxtyehy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lbdnlyeg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ytkdrzyb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ivkopjtw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lrckuqqk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jwdpnfib.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ubbfvdtu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pxrjxdbp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xwcsqflc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cztrdnvh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfsxxdaj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pirzcppt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lelbmkff.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oafnvnhs.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dztfvqkk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zudczbsi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nzyvbdjc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2imvkfcxa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2erwskzzi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ououbxvd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwrdyfok.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2limzemap.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2efigjcpv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fdhunntf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sbxgznul.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2kyxnmvqu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbryxwx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2satprwcp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ggsfiqkr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2npvdkrvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2eygwxotd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xurhmumb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rgiyhtnf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ecmbimhx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jwmqqudg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ylogtfqu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmcmhnk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2irttpczf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pwjgduob.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lhdpvieg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2skiqwpae.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xnjetost.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2txogpuwd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dnqgnkva.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lmebyryd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oqioisbb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jqupwqwg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yxnhtpuq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iyqmqtwg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2eoaocfdi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2osdhupjv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2glzrjveq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vjcnoljq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xuvcicuv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sbpofrmu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2hdusfhlb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2usgeschy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjlazefp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mwhxpizh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ddgjhmhq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bkgkbjng.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ciosyazi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2kkugwbkr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kictczut.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zuwxxdug.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2iadlggsr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fegafrmu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ulfeqayz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zkzurhcr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ksoislpw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dtxjtlpy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eyubioyf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2cgtgzrqx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kjkbshbo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gughpllz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2biwtrnrd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dmknyzpb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2opjcowhq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fqmizmpq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2iicmxfpu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2melkshij.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kgevmwzw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2coedtekm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovbeydjg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2atrqldjf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rcdohwik.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ddprqwpa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cadjxtff.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ltfbossp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pnlduuqz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2moektfjf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2webqgzsz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2djkgilbh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zeudbnvz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wgrxqzhb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkarllii.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ccylhwtn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tbxicnwv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hcmplxcc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2imxxnvru.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aiptgxkf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2twtgewmq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2aclluuxs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2anydiiml.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qeikuipj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxwzvrb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tyvdzhyq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ifurrcwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbujflbn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yiicycbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmzjqvcr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2todkxgvo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2glszzesw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2shmykfbv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tacvrqsa.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2iyieguzj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2atxuekpx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lythjvvv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2noausdex.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qcucnwxt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fszitsyg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2icbnhohj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kwwnyngi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pbepddvy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lompytin.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mcmffsry.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rcxrcpdj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xrkbzigx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gwfdjreg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fqoazqqx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rhkobzug.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rjlhmqvc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jdldzkfn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dvoccrdh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2uecpfbhu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vxastlya.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2optiwgyy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rslwcshr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fpmgypan.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ivmfpuea.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2okuokdrs.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2phyeqqdl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2nxebzohd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qhezkbje.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cqgpnwqw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dxegamdr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uyyyalrq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2akdlxpmk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ykczniat.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2acvewzyg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2uycpyccm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dnqvxhlj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2pqrqvbba.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2fvayfmxd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ukhrifqp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2oojzyezs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gqjuvcik.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2aeoladdy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jxoswzux.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wahimmrt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2tjxaochp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2eetuqwpx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zztxzcxi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dfpgeofx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hqjiskzp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2znfpfdkq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dwvmmjdn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2cyqfzjxq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lsfweigz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2kwwgqpzr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nzrbrtjx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hnxuejqu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tjxjsfvq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jncimpxg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lrueoojj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2smhwxrbb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2crpqvqvn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2owybymwy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bhxmthky.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zjejbuyw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hpysnipf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ajmezwfe.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vjjowapf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bpmpbwxw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wwgjrsne.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cujajuhc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ipvgqsyc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uflujiot.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nomqdfxn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tffrhbfx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aubfwecd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fcbvhuup.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rdzxbpvh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rdbeszuj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ghfshokd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zkhpcngb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wujhjcoq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxpjpuew.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wuhpglwd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfhaexbj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yczfhrwq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gsrogowy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ungnahxr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dhgondbj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2flnzurjn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2sqcimmah.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtqlcunk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pstjngbr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2kxnjsogk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2khnmliqg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2entccymi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2guawsmrc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2paeggtkr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2avxumqbb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ieccljen.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bclzgxlw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qpkwmsvc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nxikpolr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pjzbvvmu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2acokbtol.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nkpawimb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qqnwmpdx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lioboxnq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ssukxntr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zapdpgfi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2thyuzdgi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sjqudfvp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ivteapxp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zitxoxzx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jfendirm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2vcwmwjyd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lfljgiaw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2orhtwtcp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2msvnnajp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uqndjogc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2xxawctqj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2axpobwdz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ivrwdcwt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mcjwdltf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dyyuxsfl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gathxbnh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tzomotoj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgjmfla.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gbnxekab.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2gcwffsdw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ozroylzg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2uqotgpon.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2rngqymal.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rhmdbwqb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2yjhdvlxz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mmzdeccg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pabwfopt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mmqpdauk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ccainjhf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vbbycmgm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lhuameqc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2knjxipoz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhyqbzfo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wkowofty.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zazptfsh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2mzixggrq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bghvpbdg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wgablcmf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2adtedeeg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2altutxlw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vnwoklqa.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vexrqwrv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zmxjpijr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2scdiqknz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ceqgyjtw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2elzcuimi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xceacrme.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zkdesrqd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zkshecjx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wctzftms.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2aptatkqx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sdhuveaw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2eqsisdip.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2opsdecey.html


<!-- 参考信息 -->