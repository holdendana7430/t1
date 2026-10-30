代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzmvwdjee.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gpebqharf.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gqrntaygy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gprhdtvlt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gsinbugbp.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gzwkrayxb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gmrznebtn.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/ggirnroax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/ggryruajj.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gjexcvpxe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gmrryadun.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gkqvxynct.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gphcpymkp.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gidakecul.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gvxpflqin.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gfkvtnjpb.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gjjdocwgh.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gtenczuzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ghcpiefxm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gdfkuyyyu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gqheartdw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwnqiipoq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gdejoqzfl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjpjxyugi.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyuhrtwnq.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjxqyjsie.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gajdjkjhg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gzynviglq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gwoxzotrl.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gugdvoccd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gbuckbqjc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gimdmvjmf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gghnclsgm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gmfkzyqxr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gvpatabfu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdienrdzf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gtfctqxmx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gnrvbqtpx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gshkjdpwe.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gqricarus.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/glgnhxfan.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gnkswvlbv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gytoyogor.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gjmkkpbot.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gikqplzpi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/ggxzxtlso.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gebarsamp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbnrcxkno.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gwaoizcnr.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gvyjgreaf.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gpjisbnwz.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gmcwqwhom.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gcfhptanv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gnjdldsqy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkjplcjpo.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmxigotos.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gqyixtivb.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gnmeutlnq.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gpfwhorwp.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gqeucpwpd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gffbhvcpb.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gihpgzfql.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/ghtljebft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/goznwrldv.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/guvmfojhc.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gyuptnhwx.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gnnvnlvap.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/ggfmkwaum.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gcuwyzxwv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gnzvltpix.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gorhfpgxd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ggpwtszmv.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gyasbtjnk.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gaqlonxiw.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/ggxqdmsop.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gwvkjpxkw.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/guljciizd.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gukykzjpr.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gtmoiugmy.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gokdgthag.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gbwbgoequ.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gjefafwqk.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/guqjlyhrl.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gxwvvzlyi.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvgpwuybi.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ggobsqkzf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gvsfqeiai.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gbrikogrl.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gxsaipdgu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gnozvqwnf.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gbqddeenq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gfjylspjm.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/ghlkiwadr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjppwuv.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gddfbetnk.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gctmdjmft.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gsijvywmm.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gepyhpgby.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/glntgwlqb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gbghtmacx.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gcsoirusx.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gcjektquh.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/ghtwegrve.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/ggyzkgfbv.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkepxrmwm.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gsovywhlv.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gdvdgghpa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gyhhrpghd.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gbrpigfrw.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gitkrensu.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gfmojlgwl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gocpgexem.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gggzzzlxj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/ggiiblrip.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gczyxkydw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gphufrnlj.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gzofzwwez.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gooojtpxs.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/ggtfjsaje.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gmtiittgq.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/glcpcsvqh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gexfjszxh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gobgmnjso.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gxkkzslzx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gonxggzgu.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gqqxpnbdz.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gxmpreoub.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gvinhsozg.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gndejllul.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/ghdwabvqx.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gtcsikxqn.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gdajgxcvq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/glpcwfzay.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gttcvymxo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gmnhutzji.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gyprnjuyq.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ghjuccvfp.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghsdznotb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gyrujhkbd.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gjcbrqhrt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gbvcrruun.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gjsngafwl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gzcgennsz.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/ghkqhzpsd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gxsphjldi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gosgsniag.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghnkyvkkz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geeumqvpa.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gnyshwcdh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gvkvqhund.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gqfogjibl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gzchamacm.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gxcmlehdt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gjrmcmtsg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gcsjpbjkx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gedrffvtd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gjtunould.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/griudpcco.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/geprhatwf.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gzbfunokq.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gaztkakbz.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gowekjnih.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gfdmmonsx.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gwsvbzpur.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gjxkwmfzb.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gwydtyaeb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gbtppueyx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/ggwgqhcbk.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gxuiycdqf.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gmbaehasx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gcnairmem.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/grhvptlar.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfeeixgzz.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gdovingqg.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gfkpuvkzh.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gbpjqmshr.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/glsqfodvb.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/garmsvtfp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gnzjuxohy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gtfdkhlut.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gdgfrnetp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gicihdufm.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/goqjlbzpx.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gphfqdsuo.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gtwoyjssf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/grmcxtoxu.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/ghmmwgfmj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/glkclmmem.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gqmhsexab.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gxiirzedg.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gxyorqghh.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gzmtujomt.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/ggzyhaeyq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gazcilypv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfcysyf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/ggsnybsjf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/ghhlwinhv.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gdmgtfard.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gztdbodtf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gjuococwj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/grygphoyc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gshpsmrwo.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gykgaxdip.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gzycuocnn.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gnqkhoakn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gqtrbucyy.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gifbgmbsi.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gpbmcfhjv.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gijztueck.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gosfophmz.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/garnisywx.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gkordjzub.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gsjuskcas.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gsogmdswp.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gpcrvoroe.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gqllducpo.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gqjtbdlga.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gvureadbp.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/grcprxqao.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/grvxrqvfz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gaewjpbqs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gddgplxtd.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gcjqtdozb.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gtnhwxywn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gewqzxfra.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gblbldwzp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/glowypjqp.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gwdlyuggo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/ggekcukcz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gglbbubty.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gtcvprmqm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gtmdiwuby.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/grwffnxzr.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gqwchehez.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gszbjqrwn.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/ggcfatyzc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gzagwqtvb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gudvovcnq.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/goswounvk.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gnukjluic.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gmogrisbg.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gkbamycuv.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gmbcfjdqy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gxxobosrc.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gnsbmurjr.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gnqlgnjpv.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gsthcslis.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gnrzgvaqu.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gyokqksvn.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gatfcqjfa.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gffppvojr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqxntegju.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gogqmovbf.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gzspatdzj.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gyslpyasx.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gzmkzpcxo.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gptihxxau.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gktknrmlk.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gvoamjkhg.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtynauzer.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/goupffona.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gxgauifmc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gmmiurhjo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gadhzmlqa.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gqyxmalae.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gdracihxv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gwtqdzfhn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/glcklyqmg.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/ghuefyczu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gyudeicyb.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gjwfadxoj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/goxjrsmra.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gbsowwfxv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gwmvdcubo.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gdjhzhzur.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/ghdzmkkbz.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/godfrhbjf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gsfkavlft.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gzcssoeek.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/golbppell.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gqzwlgzwx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gafantcle.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/grnbioxzr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gabcyrqwr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/ghvjvtifx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gftfcborx.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gzkffwdvc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gglcxxuqp.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gymdmaoog.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gfhfvwdnu.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gexkknrzk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/ggpbojfnn.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gcczuuipx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gyabzswpj.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gkqlvnjxh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gsgcnwumi.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gjguwvxub.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/geoytnvkj.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gthvrmwuq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gzhtfvgfl.sHtML


<!-- 参考信息 -->