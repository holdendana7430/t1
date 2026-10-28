代发 wailian999

[S37] C++：set
来源：http://hz.guannengcc.top/gtrfvaetjx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hysaishi.cn/gtiiwhrubj.html

[S38] C++：排序
来源：http://hz.chenlongwang.top/gttbbkaqoa.html

std::sort(v.begin(), v.end());
来源：http://hz.smart0.xyz/gtqpaltxpm.html

[S39] C++：自定义比较器排序
来源：http://hz.yuxming.cn/gtftfxgzak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigufen.top/gtrzyvvugw.html

[S40] C++：查找元素
来源：http://hz.ydzc1.top/gtgidfiddf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gterovijjl.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtnbddrtfv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhiwuduotai.top/gteyrvkpdc.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gttpsfgcwv.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtwqrduvkg.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtocpsvspq.html

auto p = std::make_unique<int>(5);
来源：http://hz.cashguo.top/gtisnqazzg.html

[S44] C++：引用传参
来源：http://hz.yanxiufei.cn/gtuvloecxv.html

void inc(int &x) { ++x; }
来源：http://hz.yj202588.top/gtleqzomnq.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gttujgohnk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuxming.cn/gtemfbnoxv.html

[S46] C++：函数模板
来源：http://hz.cheryme.top/gtskwaagrc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yueranfly.top/gtgczqedbx.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtocnxfimo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtpemlqtaq.html

[S48] C++：逐行读文件
来源：http://hz.jqgfzy.top/gtswfymyzm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gogol.net.cn/gttwabfmol.html

while (std::getline(in, line)) { }
来源：http://hz.pycfn.com/gteuhrmnes.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtfhlmfpgy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gtgnybcmaj.html

[S50] C++：格式化数字
来源：http://hz.jiagoushi.top/gtrawedcll.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tanke756.top/gtdjjdclap.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtdmfzxgwn.html

static_cast<double>(a) / b
来源：http://hz.tianlin.xyz/gttwkotdzj.html

[S52] C++：const 与 noexcept
来源：http://hz.redwolf501.top/gtwjidykxh.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gtsutxsmbz.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gtggcnfzpu.html

std::vector<int> w = std::move(v);
来源：http://hz.gaohongyu789.top/gtqyuwnmys.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gtauzwjrit.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gzhubu.top/gtbszxrgxg.html

[S55] C++：结构化绑定
来源：http://hz.xinyue.icu/gttwekgwto.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.mhx1999.top/gtlyyqemix.html

[S56] C++：optional
来源：http://hz.pengpengdd.cyou/gtteyqsura.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj202588.top/gtlddwwrvl.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtvdzawlnx.html

constexpr int N = 10;
来源：http://hz.gaohongyu789.top/gtwbsfceyy.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtatrhekka.html

namespace ns { int f() { return 1; } }
来源：http://hz.tianlin.xyz/gthbpjofqv.html

[S59] C++：静态断言
来源：http://hz.hammf.cn/gtmtnohknr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jiagoushi.top/gtthykokss.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtcrqylghs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtxewjlpuo.html

================================================================================
来源：http://hz.chenlongwang.top/gtfugdzffi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtbxflduzu.html

================================================================================
来源：http://hz.yonumen.top/gtzsdsvgcl.html

[T01] Kotlin：Hello World
来源：http://hz.zhixingplan.top/gtlnbwxkgs.html

println("Hello")
来源：http://hz.tanke756.top/gtfvgguerd.html

[T02] Kotlin：变量
来源：http://hz.iojbl.cn/gtnfcdmnlw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gtlfayuylg.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgufenzy.top/gtlkvmrndf.html

"值: $b"
来源：http://hz.jinqigufen.top/gtuzmsecul.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtefeoztsp.html

val n: String? = null;  n?.length
来源：http://hz.xinyue.icu/gtkofvdzvk.html

[T05] Kotlin：when 表达式
来源：http://hz.jiagoushi.top/gtjatiplve.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pengpengdd.cyou/gtkywoiklx.html

[T06] Kotlin：集合映射
来源：http://hz.sufxvd.cn/gtdikeriop.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangdashe.top/gtucvuioyu.html

[T07] Kotlin：集合过滤
来源：http://hz.shangyingyoupin.top/gtpfziyckv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtidwsxjdu.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtkwotlmoi.html

data class User(val name: String, val age: Int)
来源：http://hz.hysaishi.cn/gtaqymqdqo.html

[T09] Kotlin：扩展函数
来源：http://hz.gaohongyu789.top/gtfcpjrkzz.html

fun String.exclaim() = this + "!"
来源：http://hz.iojbl.cn/gtceavbeoq.html

[T10] Kotlin：默认参数
来源：http://hz.jiagoushi.top/gtwcinobtn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.52xcode.cn/gtoosixuvk.html

[T11] Kotlin：协程
来源：http://hz.ybcxt.top/gtnolzcnuu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.9152youxi.cn/gtglzahigq.html

[T12] Kotlin：解构声明
来源：http://hz.zhijiandao.cn/gtmxmxaqyz.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtinoegcnf.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgfzy.top/gtnzoiqdcj.html

val m = mapOf("a" to 1)
来源：http://hz.sweek.top/gtuskzvyil.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtoysdobxg.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtrjsjshpz.html

[T15] Kotlin：接口
来源：http://hz.cashguo.top/gtuvjdozxg.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigfzy.top/gtonifxwjb.html

[T16] Swift：Hello World
来源：http://hz.havefunace.top/gtmnddezgj.html

print("Hello")
来源：http://hz.iojbl.cn/gtssxqcxdn.html

[T17] Swift：变量与常量
来源：http://hz.zhongyouzk.top/gtgaatwudp.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtydrzjfxn.html

[T18] Swift：字符串插值
来源：http://hz.cashguo.top/gteggcntlx.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtdfbykohg.html

[T19] Swift：可选绑定
来源：http://hz.jqgufenzy.top/gtvjxlmdjn.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gtbkzkpznl.html

[T20] Swift：数组操作
来源：http://hz.haohaochexian.top/gtrmyaksce.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xziqi.cn/gtqkljbzsd.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gtocvortcv.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gtlkpyrhan.html

[T22] Swift：字典
来源：http://hz.guannengcc.top/gtjelsnvpc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shzxlz.cn/gtifklzmus.html

[T23] Swift：函数
来源：http://hz.nanxinkj.top/gtzfgncybr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.quarkkingdee.top/gtzwodnwmz.html

[T24] Swift：闭包
来源：http://hz.cucudq.cn/gtwfxcgeri.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fzhhl.top/gtfwzkmcyx.html

[T25] Swift：结构体
来源：http://hz.guannengcc.top/gtlvsmkbwf.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtmfthzdwe.html

[T26] Swift：类与重写
来源：http://hz.sysykeji.top/gtgwzfrckh.html

class A: Base { override func f() {} }
来源：http://hz.ywan-chungtsiang.top/gttxarmykm.html

[T27] Swift：错误处理
来源：http://hz.zhengqikj.top/gtseqndkpl.html

do { try f() } catch { print(error) }
来源：http://hz.jinyuanbaomall.cn/gtgkskodaw.html

[T28] Swift：枚举
来源：http://hz.pengpengdd.cyou/gtrfrgecax.html

enum Color { case red, green }
来源：http://hz.ivvv.top/gtiwlpqphj.html

[T29] Swift：guard 提前返回
来源：http://hz.xinyue.icu/gtdfgpmmfp.html

guard let x = opt else { return }
来源：http://hz.fzhhl.top/gtxgyilbsr.html

[T30] Swift：协议
来源：http://hz.pengpengdd.cyou/gtvjbhzeac.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgfzy.top/gtpukunimz.html

[T31] Lua：Hello World
来源：http://hz.jqgufenzy.top/gtasyreerc.html

print("Hello")
来源：http://hz.ydzc1.top/gtyowladgq.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtuejzrqdj.html

local a = 1
来源：http://hz.aizwys.cn/gtmbltjkkf.html

[T33] Lua：表（数组）
来源：http://hz.zhengqikj.top/gtultksunz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.birdmap.top/gtftkoxsur.html

[T34] Lua：遍历表
来源：http://hz.smart0.xyz/gtedhjrhrh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhongyouzk.top/gteardoist.html

[T35] Lua：字典表
来源：http://hz.ydjk.org.cn/gteodizpzr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangtech.top/gtvzcqgcxy.html

[T36] Lua：函数
来源：http://hz.jiagoushi.top/gtypabwhyh.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gttkrqefmu.html

[T37] Lua：字符串拼接
来源：http://hz.zhijiandao.cn/gtshdhqusv.html

"a" .. "b"
来源：http://hz.0kj1m.cn/gtkfjxkkna.html

[T38] Lua：条件
来源：http://hz.fzhhl.top/gtzpncasog.html

if x > 0 then print("正") end
来源：http://hz.mhx1999.top/gtdhkpfauo.html

[T39] Lua：模式匹配
来源：http://hz.ydzc1.top/gtsikhvlqe.html

string.find(s, "%d+")
来源：http://hz.havefunace.top/gtrjhdrgsg.html

[T40] Lua：元表
来源：http://hz.nanxuanxn.top/gtlykxfhet.html

setmetatable({}, { __index = base })
来源：http://hz.wangdashe.top/gttkfrtpnj.html

[T41] Perl：Hello World
来源：http://hz.chenjidiqi.icu/gtqgvlwghy.html

print "Hello\n";
来源：http://hz.9152youxi.cn/gtudjagkeh.html

[T42] Perl：变量类型
来源：http://hz.havefunace.top/gtsbahukgl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cheryme.top/gtrhfbcqae.html

[T43] Perl：字符串插值
来源：http://hz.smart0.xyz/gtgsphaohi.html

"值: $a"
来源：http://hz.jqgfzy.top/gtorccfrbi.html

[T44] Perl：条件
来源：http://hz.shanyushiyangtech.top/gtqzsfjvby.html

if ($a > 0) { print "正"; }
来源：http://hz.meibo888.top/gtsukvuybn.html

[T45] Perl：数组遍历
来源：http://hz.hnqzz.top/gtenprioun.html

for my $x (@arr) { print $x; }
来源：http://hz.redwolf501.top/gtiddynyql.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gtsbdlsiod.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinyuanbaomall.cn/gtprcyesxj.html

[T47] Perl：正则捕获
来源：http://hz.meibo888.top/gtwedmmhwn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.quarkkingdee.top/gtuehalwlb.html

[T48] Perl：正则替换
来源：http://hz.nanxuanxn.top/gtstezzmbr.html

$s =~ s/old/new/g;
来源：http://hz.daria6918.cn/gtyjoliism.html

[T49] Perl：函数
来源：http://hz.jianghu66.top/gtsqtpmsgz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj20258.top/gtcepqyzmb.html

[T50] Perl：逐行读文件
来源：http://hz.hammf.cn/gthjakgzbx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtijcictkx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinghuilouyu.cn/gtlnpthvwb.html

[T51] Scala：Hello World
来源：http://hz.guowangkeji.top/gtvnrfjphr.html

println("Hello")
来源：http://hz.pycfn.com/gtqwliulny.html

[T52] Scala：变量
来源：http://hz.ydzc1.top/gtjbprxiea.html

val a = 1;  var b = 2
来源：http://hz.zhaomingkeji.xyz/gtflcqspaz.html

[T53] Scala：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtaysddocs.html

s"值: $b"
来源：http://hz.xuanzx.com/gtrhgscwde.html

[T54] Scala：集合映射
来源：http://hz.sxryk.cn/gtxgpwatgj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnqzz.top/gtbxqxdcff.html

[T55] Scala：集合过滤
来源：http://hz.zycfv.cn/gtqugdgohw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hywenlv.cn/gtqtncojhl.html

[T56] Scala：样例类
来源：http://hz.mhx1999.top/gtuhevrtnk.html

case class User(name: String, age: Int)
来源：http://hz.chenlongwang.top/gthqzckazg.html

[T57] Scala：模式匹配
来源：http://hz.cqqwz.cn/gtvgwrxmyk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jqgfzy.top/gttkrqazwv.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtpqduglhu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtcpkeycoo.html

[T59] Scala：循环
来源：http://hz.chenzaomai.com/gtkmsgufne.html

for (i <- 1 to 10) println(i)
来源：http://hz.jianghu66.top/gtrppjbems.html

[T60] Scala：折叠
来源：http://hz.mhx1999.top/gtjjkyoxhj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtapywvhao.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzrnvvnug.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.iojbl.cn/gtvlhdnxdl.html

================================================================================
来源：http://hz.yuanzhike.top/gtdywmiekw.html

[U01] Py：创建虚拟环境
来源：http://hz.ehwqpu.com/gttkxxzoyo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jiagoushi.top/gtexhfsvmi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xziqi.cn/gtnmvydvrn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.redwolf501.top/gtzcoxtaae.html

[U03] Py：加载 .env 配置
来源：http://hz.yj20258888.top/gtyppchhij.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yanxiufei.cn/gtchitlalf.html

[U04] Py：变量调试打印
来源：http://hz.haohaochexian.top/gtspjorkrp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinqigfzy.top/gttxwbgayu.html

[U05] Py：列表去重且保序
来源：http://hz.jyoumei.cn/gtsuxqjwpr.html

list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtegmzoaou.html

[U06] Py：合并两个字典
来源：http://hz.birdmap.top/gtxxpccliz.html

{**a, **b}
来源：http://hz.yvedp.cn/gtcjkvpikb.html

[U07] Py：反转字典键值
来源：http://hz.fzhhl.top/gtgubjikrn.html

{v: k for k, v in d.items()}
来源：http://hz.cdnleiting.top/gtgvgpvncc.html

[U08] Py：展平二维列表
来源：http://hz.ppjwa.cn/gtfnvmbwfc.html

[y for x in nested for y in x]
来源：http://hz.zhaomingkeji.xyz/gtfvklmdly.html

[U09] Py：字典取最大值的键
来源：http://hz.jyoumei.cn/gtmgryswtt.html

max(d, key=d.get)
来源：http://hz.hongshengwenyu.top/gtbxzyxunw.html

[U10] Py：按值排序字典
来源：http://hz.sufxvd.cn/gtocctnlvt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yanxiufei.cn/gtmlfosgmr.html

[U11] Py：生成器表达式
来源：http://hz.ybcxt.top/gtztlogvso.html

(x * 2 for x in arr)
来源：http://hz.smart0.xyz/gtaipqhdgs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.svipenyu.cn/gtjwvgyrnu.html

Counter(arr).most_common(3)
来源：http://hz.gzhubu.top/gtwfrytsdv.html

[U13] Py：固定长度队列
来源：http://hz.daxiang520.top/gtwncwzwld.html

deque(maxlen=10)
来源：http://hz.guowangkeji.top/gtczcetiwt.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtjcxpqjdd.html

defaultdict(list)
来源：http://hz.chenzaomai.com/gtrsumuygm.html

[U15] Py：高精度计时
来源：http://hz.havefunace.top/gtzsrzxkkb.html

t = time.perf_counter()
来源：http://hz.chenlongwang.top/gtfhvxhwcr.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gthkbqjknd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhoulong.xyz/gtxhfoardt.html

[U17] Py：初始化日志
来源：http://hz.zhijiandao.cn/gtygtcktlw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gtqpibrfjq.html

[U18] Py：预编译正则
来源：http://hz.havefunace.top/gteeosdoba.html

pat = re.compile(r"\d+")
来源：http://hz.yueranfly.top/gtbxdisaug.html

[U19] Py：正则替换带回调
来源：http://hz.hammf.cn/gtptvsuhdf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.daxiang520.top/gtnwmjmmfq.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtbvfcleft.html

@functools.lru_cache(maxsize=None)
来源：http://hz.bjfxy.top/gtppigoddk.html

[U21] Py：自定义上下文管理器
来源：http://hz.52xcode.cn/gtkcwysjqv.html

@contextlib.contextmanager
来源：http://hz.xinyue.icu/gtvusqsqqq.html

[U22] Py：矩阵转置
来源：http://hz.havefunace.top/gtklaoroke.html

list(zip(*m))
来源：http://hz.redwolf501.top/gtxfofsjkp.html

[U23] Py：分块读取大文件
来源：http://hz.zhaomingkeji.xyz/gtxhmfqavu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guowangkeji.top/gttgufgcjv.html

[U24] Py：路径操作
来源：http://hz.jianghu66.top/gtagulsxsr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydjk.org.cn/gttohzhkea.html

[U25] Py：CSV 按字典读
来源：http://hz.shzxlz.cn/gtkhkkddag.html

csv.DictReader(f)
来源：http://hz.pycfn.com/gtbnacjvph.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtxpdhhtpb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yj20258.top/gtjdafnunw.html

[U27] Py：异步 HTTP
来源：http://hz.yvedp.cn/gtduszcrqk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zdqjudy.top/gtqgdmkysy.html

[U28] Py：类型别名
来源：http://hz.gotoacloud.top/gtlkjjhzga.html

UserId = int
来源：http://hz.xinyue.icu/gtwgiebndg.html

[U29] Py：属性校验
来源：http://hz.xziqi.cn/gttocramwq.html

@property 与 @x.setter 配合
来源：http://hz.kuanghao11.cn/gtieuxttnd.html

[U30] Py：数据类
来源：http://hz.jianghu66.top/gtoxjscihd.html

@dataclass(slots=True)
来源：http://hz.jianghu66.top/gtynyqscwl.html

[U31] Py：单测
来源：http://hz.guannengcc.top/gtagzytmep.html

python -m pytest -q
来源：http://hz.sysykeji.top/gtxovwntky.html

[U32] Py：代码格式化
来源：http://hz.birdmap.top/gtbanrxpaq.html

ruff format . && ruff check --fix .
来源：http://hz.cheryme.top/gtqyvyyjqv.html

[U33] Py：打包发布
来源：http://hz.shzxlz.cn/gtcwgjjxbh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tanke756.top/gtnlfcpqpw.html

[U34] Py：判断编码
来源：http://hz.shzxlz.cn/gtlprgtbli.html

chardet.detect(raw)
来源：http://hz.ybcxt.top/gtnceauuww.html

[U35] Py：发送邮件
来源：http://hz.9152youxi.cn/gtpgktpvzn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.0kj1m.cn/gtrlzletlq.html

[U36] Py：定时任务
来源：http://hz.sweek.top/gtlyjdavkk.html

schedule.every(10).minutes.do(job)
来源：http://hz.aibaodan.cn/gtkpxmaqve.html

[U37] Py：读写 Excel
来源：http://hz.zhengqikj.top/gtqlywedsn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aizwys.cn/gtbmmbqnbj.html

[U38] Py：获取脚本所在目录
来源：http://hz.yj20258.top/gtkbdtzmsv.html

Path(__file__).resolve().parent
来源：http://hz.shzxlz.cn/gtepladqoz.html

[U39] Py：判断是否在交互环境
来源：http://hz.cheryme.top/gtbseyjpgy.html

sys.stdout.isatty()
来源：http://hz.birdmap.top/gtsopgrrub.html

[U40] Py：打印到标准错误
来源：http://hz.fengsongda.top/gtryenfqty.html

print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gttexqadzr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj202588.top/gtmgnofohy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.quarkkingdee.top/gthauarxyd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gtdlgbsimi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinyuanbaomall.cn/gtodoccllw.html

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gtlvuxbdvs.html

namespace App\Http;
来源：http://hz.9152youxi.cn/gtzzckwcfq.html

[U44] PHP：开启严格类型
来源：http://hz.tian-w.cn/gtwgnisebw.html

declare(strict_types=1);
来源：http://hz.jlsjyb.cn/gtkctcriar.html

[U45] PHP：类型声明与返回类型
来源：http://hz.vqdsnc.cn/gtpkzscafb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtbgqrmvee.html

[U46] PHP：可空类型
来源：http://hz.ywan-chungtsiang.top/gteuriulzi.html

?string $name = null
来源：http://hz.cqqwz.cn/gtdgcttjuo.html

[U47] PHP：联合类型
来源：http://hz.kuanghao11.cn/gtgkxbmmjx.html

int|string $id
来源：http://hz.wangdashe.top/gtqryhuarb.html

[U48] PHP：纯枚举
来源：http://hz.mhx1999.top/gtrlpjlbul.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtqerqibhp.html

[U49] PHP：只读属性
来源：http://hz.shanyushiyangkeji.top/gtwnxprrfy.html

public readonly string $name
来源：http://hz.jinqigfzy.top/gtwxvffdbl.html

[U50] PHP：构造器属性提升
来源：http://hz.yonumen.top/gtktaezxwo.html

public function __construct(private int $id) {}
来源：http://hz.jinghuilouyu.cn/gtyzrcezrj.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtfujwylce.html

[$a, $b] = $arr;
来源：http://hz.gaohongyu789.top/gtgrevzebt.html

[U52] PHP：箭头函数
来源：http://hz.andypj.xyz/gtiphduqpe.html

$double = fn($x) => $x * 2;
来源：http://hz.zycfv.cn/gtyqvwdmza.html

[U53] PHP：空合并运算符
来源：http://hz.shanyushiyangtech.top/gtnvtanlqu.html

$v = $a ?? $b ?? "default";
来源：http://hz.cheryme.top/gtkryawxzv.html

[U54] PHP：空安全调用
来源：http://hz.yongpay.top/gtqpakienb.html

$obj?->method()
来源：http://hz.gogol.net.cn/gtjvforpdl.html

[U55] PHP：match 表达式
来源：http://hz.hysaishi.cn/gtxcdcnnru.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydjk.org.cn/gttwpfnzzh.html

[U56] PHP：命名参数
来源：http://hz.xziqi.cn/gtebmckejh.html

f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtgywdqieb.html

[U57] PHP：字符串插值
来源：http://hz.sweek.top/gtfwazxpsz.html

"值: {$a}"
来源：http://hz.yangfankeji.com/gtiajsfrlk.html

[U58] PHP：数组三件套
来源：http://hz.chenzaomai.com/gtxnmbqiyl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sysykeji.top/gtfxwyoiij.html

[U59] PHP：自定义排序
来源：http://hz.daria6918.cn/gtvdqlhwhs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sweek.top/gthvczpksz.html

[U60] PHP：JSON 编解码
来源：http://hz.andypj.xyz/gtsppkrhkp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shzxlz.cn/gtqyraeskw.html

[U61] PHP：正则
来源：http://hz.52xcode.cn/gtnjrlrazg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gtanfbmzxs.html

[U62] PHP：日期对象
来源：http://hz.hfpthk.cn/gtkhdegomh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hywenlv.cn/gtpieamlmg.html


<!-- 参考信息 -->