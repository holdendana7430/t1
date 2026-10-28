代发 wailian999

[S35] C++：map
来源：http://hz.smart0.xyz/gtpeuvwzrw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gtrvpjnjng.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtdennyzjt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtndxndcwl.html

[S37] C++：set
来源：http://hz.haohaochexian.top/gtfuefssvf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yueranfly.top/gtksgolahh.html

[S38] C++：排序
来源：http://hz.zhaomingkeji.xyz/gthzjkbaxf.html

std::sort(v.begin(), v.end());
来源：http://hz.fzhhl.top/gtumrxdmma.html

[S39] C++：自定义比较器排序
来源：http://hz.sweek.top/gtxpouyqtn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cucudq.cn/gtghztvwhe.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtzfirfqnc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtbkkqsobl.html

[S41] C++：类与构造函数
来源：http://hz.hnxiangtu.top/gtkkxwktrc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.c1oappe.top/gtxoholifn.html

[S42] C++：继承与虚函数
来源：http://hz.shzxlz.cn/gtlshrefpc.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gttcysnofo.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtqpkshsvd.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtsgqdjzmc.html

[S44] C++：引用传参
来源：http://hz.yonumen.top/gtyozztfil.html

void inc(int &x) { ++x; }
来源：http://hz.fzhhl.top/gtmtsvsykk.html

[S45] C++：lambda
来源：http://hz.jyoumei.cn/gtivldmmer.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jianghu66.top/gtoxrfboxc.html

[S46] C++：函数模板
来源：http://hz.hfpthk.cn/gtlhdszcjz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydjk.org.cn/gtvrljucbo.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtnykzmaum.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gthvhrwxhm.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtgvloctrs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigfzy.top/gtnjltkfdr.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtfbvvyzus.html

[S49] C++：写文件
来源：http://hz.gzhubu.top/gtcmuctcoh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fzhhl.top/gtwngpktfe.html

[S50] C++：格式化数字
来源：http://hz.dashuyun.cn/gtkvprllbr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtyvobubzl.html

[S51] C++：显式类型转换
来源：http://hz.pengpengdd.cyou/gtvwjnutfu.html

static_cast<double>(a) / b
来源：http://hz.ppjwa.cn/gtbplduejm.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtzdoqblib.html

int size() const noexcept { return n_; }
来源：http://hz.guannengcc.top/gtjpzifana.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtdrvyiyrx.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtmfhqikmj.html

[S54] C++：异常处理
来源：http://hz.zhoulong.xyz/gttcnsndmz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.quarkkingdee.top/gttpfoupar.html

[S55] C++：结构化绑定
来源：http://hz.redwolf501.top/gttdektjak.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.52xcode.cn/gtaijwtrui.html

[S56] C++：optional
来源：http://hz.ivvv.top/gtbfhmwyyj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtlqglmmez.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gtqguwdbav.html

constexpr int N = 10;
来源：http://hz.svipenyu.cn/gtyxtoidwt.html

[S58] C++：命名空间
来源：http://hz.ybcxt.top/gtdunrplup.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtlqtdsevw.html

[S59] C++：静态断言
来源：http://hz.redwolf501.top/gtgwthtusq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxuanxn.top/gtdndvhgvh.html

[S60] C++：遍历并删除元素
来源：http://hz.zhiwuduotai.top/gtfghjlure.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtcwsnsbcn.html

================================================================================
来源：http://hz.chenzaomai.com/gtbolrtfet.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gttemajivz.html

================================================================================
来源：http://hz.redwolf501.top/gtyhsfpqac.html

[T01] Kotlin：Hello World
来源：http://hz.ywan-chungtsiang.top/gtnlgdfdub.html

println("Hello")
来源：http://hz.guannengcc.top/gtuimmhvei.html

[T02] Kotlin：变量
来源：http://hz.zhixingplan.top/gtajcxowts.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtkdymvzfg.html

[T03] Kotlin：字符串模板
来源：http://hz.cdnleiting.top/gtnuuuanao.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gtfdvrkolf.html

[T04] Kotlin：空安全
来源：http://hz.zdqjudy.top/gtarjfaysc.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gtfzbqefje.html

[T05] Kotlin：when 表达式
来源：http://hz.c1oappe.top/gtxswjfonv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zdqjudy.top/gtvafsjuzb.html

[T06] Kotlin：集合映射
来源：http://hz.jiagoushi.top/gtkighcsxn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtujuhmcck.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtmoombiwp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gtimujjoqx.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtoayklvdm.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtvolhsrji.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtzvwgvutu.html

fun String.exclaim() = this + "!"
来源：http://hz.jinghuilouyu.cn/gtfzlluarb.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gtdtisrxah.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cqqwz.cn/gtiuzrqbmq.html

[T11] Kotlin：协程
来源：http://hz.jianghu66.top/gtihecghaq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenzaomai.com/gtxggizwwh.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtdiokyoni.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtbruqvksv.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigufen.top/gtvfdwzook.html

val m = mapOf("a" to 1)
来源：http://hz.pengpengdd.cyou/gtvjukhqpt.html

[T14] Kotlin：循环
来源：http://hz.yj20258.top/gtlzcpdame.html

for (i in 1..10) println(i)
来源：http://hz.ivvv.top/gtyhpysrbn.html

[T15] Kotlin：接口
来源：http://hz.yongpay.top/gtwinyujvr.html

interface Shape { fun area(): Double }
来源：http://hz.dashuyun.cn/gtgcapgmoo.html

[T16] Swift：Hello World
来源：http://hz.ppjwa.cn/gtjcjvvrcm.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtugasbfxq.html

[T17] Swift：变量与常量
来源：http://hz.aizwys.cn/gtrnqqdrkj.html

var a = 1;  let b = 2
来源：http://hz.jinghuilouyu.cn/gtwnmlebuq.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtacikimoe.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gtentxhqbu.html

[T19] Swift：可选绑定
来源：http://hz.nanxinkj.top/gtsvgvbqep.html

if let n = opt { print(n) }
来源：http://hz.meibo888.top/gtonkrrqxs.html

[T20] Swift：数组操作
来源：http://hz.cucudq.cn/gtwulzrccv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ybcxt.top/gtfnixlivd.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtqbnuuzrm.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtshwaaxai.html

[T22] Swift：字典
来源：http://hz.cucudq.cn/gteuhpumey.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigufen.top/gtwktshdpj.html

[T23] Swift：函数
来源：http://hz.xuetiantiany.cn/gtoughtgyo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.iojbl.cn/gteczoiurz.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gthcekpfsq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.pycfn.com/gtjpevctqk.html

[T25] Swift：结构体
来源：http://hz.hongshengwenyu.top/gtyhrkeafy.html

struct P { var x: Int }
来源：http://hz.dianchejie.cn/gtzhhlubgo.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtagrceczt.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangkeji.top/gtexqgqill.html

[T27] Swift：错误处理
来源：http://hz.yonumen.top/gtsvwkjsjm.html

do { try f() } catch { print(error) }
来源：http://hz.wangdashe.top/gtcqanrvkv.html

[T28] Swift：枚举
来源：http://hz.gzhubu.top/gtfbblmarf.html

enum Color { case red, green }
来源：http://hz.birdmap.top/gtqcxmclxb.html

[T29] Swift：guard 提前返回
来源：http://hz.nwbrower.top/gtiojhtzyg.html

guard let x = opt else { return }
来源：http://hz.zhiwuduotai.top/gtqguyquxt.html

[T30] Swift：协议
来源：http://hz.ehwqpu.com/gtbuuegpum.html

protocol Shape { func area() -> Double }
来源：http://hz.zycfv.cn/gtmxyhagih.html

[T31] Lua：Hello World
来源：http://hz.sxryk.cn/gtgbexjqok.html

print("Hello")
来源：http://hz.andypj.xyz/gtyeawqwof.html

[T32] Lua：局部变量
来源：http://hz.quarkkingdee.top/gtfnelauab.html

local a = 1
来源：http://hz.aibaodan.cn/gtasfpxnzf.html

[T33] Lua：表（数组）
来源：http://hz.andypj.xyz/gtaisoyyul.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jyoumei.cn/gtohncryhg.html

[T34] Lua：遍历表
来源：http://hz.ydzc1.top/gtnimvxaxr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xinyue.icu/gtuzwrvmwu.html

[T35] Lua：字典表
来源：http://hz.ivvv.top/gtrhhreqwb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenjidiqi.icu/gthqdgcfxf.html

[T36] Lua：函数
来源：http://hz.iojbl.cn/gtvdgradig.html

function add(a, b) return a + b end
来源：http://hz.zhaomingkeji.xyz/gtvqwievoo.html

[T37] Lua：字符串拼接
来源：http://hz.fzhhl.top/gtdnuqhfvt.html

"a" .. "b"
来源：http://hz.shanyushiyangkeji.top/gtlntflhst.html

[T38] Lua：条件
来源：http://hz.sysykeji.top/gtdaaofgey.html

if x > 0 then print("正") end
来源：http://hz.yanxiufei.cn/gtwgrljkkl.html

[T39] Lua：模式匹配
来源：http://hz.chenlongwang.top/gtjidsyshc.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtkvslzzjd.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtkotamesi.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258888.top/gtrbfgqrzl.html

[T41] Perl：Hello World
来源：http://hz.tanke756.top/gtlmalbium.html

print "Hello\n";
来源：http://hz.zhijiandao.cn/gtikjowpsb.html

[T42] Perl：变量类型
来源：http://hz.wangdashe.top/gtfsmbwfjk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangtech.top/gtbgoajwog.html

[T43] Perl：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtgvgeczxi.html

"值: $a"
来源：http://hz.hfpthk.cn/gtnxzxpqcj.html

[T44] Perl：条件
来源：http://hz.xingfuxueyuan.xyz/gtgrnzuhey.html

if ($a > 0) { print "正"; }
来源：http://hz.bjfxy.top/gtazitbywl.html

[T45] Perl：数组遍历
来源：http://hz.meibo888.top/gtljhzgzab.html

for my $x (@arr) { print $x; }
来源：http://hz.chenlongwang.top/gtrpmboehj.html

[T46] Perl：哈希操作
来源：http://hz.quarkkingdee.top/gtcgqvmiit.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhixingplan.top/gtymcnsbym.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtckhaexqk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigfzy.top/gtclnjkjdb.html

[T48] Perl：正则替换
来源：http://hz.pengpengdd.cyou/gtzzvammbr.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangtech.top/gtopoysuiu.html

[T49] Perl：函数
来源：http://hz.quarkkingdee.top/gtonxanjym.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.bjfxy.top/gtmrphmfbg.html

[T50] Perl：逐行读文件
来源：http://hz.wangdashe.top/gtevcsycpr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.52xcode.cn/gtpcucyzho.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hongshengwenyu.top/gtspzpzmnb.html

[T51] Scala：Hello World
来源：http://hz.vqdsnc.cn/gtovewjcrq.html

println("Hello")
来源：http://hz.birdmap.top/gtkbbxdpgw.html

[T52] Scala：变量
来源：http://hz.nanxuanxn.top/gtqbpfwaxc.html

val a = 1;  var b = 2
来源：http://hz.guowangkeji.top/gtjgvyopka.html

[T53] Scala：字符串插值
来源：http://hz.tianlin.xyz/gtfltfwdap.html

s"值: $b"
来源：http://hz.zhiwuduotai.top/gtzrhxqtbd.html

[T54] Scala：集合映射
来源：http://hz.xuanzx.com/gtfibhlixf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ybcxt.top/gtsowncgzq.html

[T55] Scala：集合过滤
来源：http://hz.birdmap.top/gtikxrjzqg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenlongwang.top/gtiitxtosa.html

[T56] Scala：样例类
来源：http://hz.gaohongyu789.top/gtqapltbuf.html

case class User(name: String, age: Int)
来源：http://hz.guannengcc.top/gtcegacdnq.html

[T57] Scala：模式匹配
来源：http://hz.nanxuanxn.top/gtnfrndihz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shanyushiyangtech.top/gthdlxpdrv.html

[T58] Scala：函数定义
来源：http://hz.pengpengdd.cyou/gtzvahvmzi.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangshuangyany.cn/gtubfnuqam.html

[T59] Scala：循环
来源：http://hz.jinqigfzy.top/gtehasjuuz.html

for (i <- 1 to 10) println(i)
来源：http://hz.smart0.xyz/gtbnyjbcxm.html

[T60] Scala：折叠
来源：http://hz.gotoacloud.top/gtlaaxwxxo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuxming.cn/gtjajjdgpf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzailicsr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xingfuxueyuan.xyz/gtflcdpclf.html

================================================================================
来源：http://hz.hammf.cn/gteloqtqpn.html

[U01] Py：创建虚拟环境
来源：http://hz.xuetiantiany.cn/gtmbqqifad.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gthxadgjum.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xylfe.cn/gtsxbuuopr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nanxuanxn.top/gtktpgbmaj.html

[U03] Py：加载 .env 配置
来源：http://hz.ivvv.top/gtnbedeouk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yonumen.top/gtopeoauho.html

[U04] Py：变量调试打印
来源：http://hz.9152youxi.cn/gtktzaodyh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.316326.xyz/gtcujmucmj.html

[U05] Py：列表去重且保序
来源：http://hz.gaohongyu789.top/gtrdviwmvl.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtcpydanmg.html

[U06] Py：合并两个字典
来源：http://hz.iojbl.cn/gtrhncgwkh.html

{**a, **b}
来源：http://hz.shanyushiyangtech.top/gtkezuqdut.html

[U07] Py：反转字典键值
来源：http://hz.sufxvd.cn/gthplacrlx.html

{v: k for k, v in d.items()}
来源：http://hz.wangshuangyany.cn/gtygnbobar.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangkeji.top/gtifxaqjaz.html

[y for x in nested for y in x]
来源：http://hz.fengsongda.top/gtwffaiweq.html

[U09] Py：字典取最大值的键
来源：http://hz.jianghu66.top/gtulventmu.html

max(d, key=d.get)
来源：http://hz.jinghuilouyu.cn/gtolrnqcim.html

[U10] Py：按值排序字典
来源：http://hz.pengpengdd.cyou/gtczwgtjwp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yangfankeji.com/gtvapaqdut.html

[U11] Py：生成器表达式
来源：http://hz.meibo888.top/gtbezyiirt.html

(x * 2 for x in arr)
来源：http://hz.gotoacloud.top/gtqeojhmgc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.bjfxy.top/gtjrncyfsc.html

Counter(arr).most_common(3)
来源：http://hz.tanke756.top/gtvulovhcb.html

[U13] Py：固定长度队列
来源：http://hz.cqqwz.cn/gthttnnvyn.html

deque(maxlen=10)
来源：http://hz.gotoacloud.top/gtulezcpzo.html

[U14] Py：分组收集到列表
来源：http://hz.chenlongwang.top/gtyrzsfafe.html

defaultdict(list)
来源：http://hz.mhx1999.top/gthfugkugr.html

[U15] Py：高精度计时
来源：http://hz.tanke756.top/gttowhfojz.html

t = time.perf_counter()
来源：http://hz.cashguo.top/gtjpktdvse.html

[U16] Py：命令行参数解析
来源：http://hz.hammf.cn/gtgbbzsdkh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aizwys.cn/gtvrtuhzea.html

[U17] Py：初始化日志
来源：http://hz.hfpthk.cn/gtnlqchgmr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.9152youxi.cn/gtxsbrfpyh.html

[U18] Py：预编译正则
来源：http://hz.nanxinkj.top/gtatlynyki.html

pat = re.compile(r"\d+")
来源：http://hz.zdqjudy.top/gtrumswztr.html

[U19] Py：正则替换带回调
来源：http://hz.meibo888.top/gtzabzwvjx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtsxddjcic.html

[U20] Py：缓存函数结果
来源：http://hz.0kj1m.cn/gtmxrzhmnd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gtnzizuuin.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhongyouzk.top/gtstariqya.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangtech.top/gtbmvysoyz.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtwyxddket.html

list(zip(*m))
来源：http://hz.yueranfly.top/gtgvpbewbo.html

[U23] Py：分块读取大文件
来源：http://hz.vqdsnc.cn/gtlhwueska.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinqigfzy.top/gtfubapjzr.html

[U24] Py：路径操作
来源：http://hz.ydjk.org.cn/gttbqghyii.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cashguo.top/gtfzwhvslm.html

[U25] Py：CSV 按字典读
来源：http://hz.zhiwuduotai.top/gtmtvzzbsz.html

csv.DictReader(f)
来源：http://hz.yj20258888.top/gteaaagtxv.html

[U26] Py：并发下载
来源：http://hz.kuanghao11.cn/gtxpdikhuc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hammf.cn/gtiyuemmmz.html

[U27] Py：异步 HTTP
来源：http://hz.ehwqpu.com/gthmyavaoy.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ywan-chungtsiang.top/gtjdtpnycw.html

[U28] Py：类型别名
来源：http://hz.ivvv.top/gtwcxedxvb.html

UserId = int
来源：http://hz.havefunace.top/gtiphjthok.html

[U29] Py：属性校验
来源：http://hz.daxiang520.top/gtqdgdlxft.html

@property 与 @x.setter 配合
来源：http://hz.gaohongyu789.top/gtodwdbfnf.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtdzpzwtqy.html

@dataclass(slots=True)
来源：http://hz.nanxinkj.top/gtwmlddlzk.html

[U31] Py：单测
来源：http://hz.jyoumei.cn/gtjywwhyyc.html

python -m pytest -q
来源：http://hz.sweek.top/gtkpforcdp.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gtkrybiisx.html

ruff format . && ruff check --fix .
来源：http://hz.yuxming.cn/gtjvtzkhik.html

[U33] Py：打包发布
来源：http://hz.zycfv.cn/gtyaimjdcb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.redwolf501.top/gtoziuxgsa.html

[U34] Py：判断编码
来源：http://hz.gogol.net.cn/gtpkakpgcm.html

chardet.detect(raw)
来源：http://hz.jinyuanbaomall.cn/gtcfwjqlqq.html

[U35] Py：发送邮件
来源：http://hz.jyoumei.cn/gthenrhvmr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hammf.cn/gtjnhnrvky.html

[U36] Py：定时任务
来源：http://hz.snrcjt.cn/gtgsfphplc.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnqzz.top/gtjantynle.html

[U37] Py：读写 Excel
来源：http://hz.haohaochexian.top/gtnimuvzms.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.fzhhl.top/gtantaftrd.html

[U38] Py：获取脚本所在目录
来源：http://hz.xuetiantiany.cn/gtpuqsktra.html

Path(__file__).resolve().parent
来源：http://hz.tian-w.cn/gtmhlnmmct.html

[U39] Py：判断是否在交互环境
来源：http://hz.jlsjyb.cn/gtjiyigiyr.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtsvsjdoql.html

[U40] Py：打印到标准错误
来源：http://hz.guannengcc.top/gtgnmgwobh.html

print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtrlwylqpt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.c1oappe.top/gtqfkgoznz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigufen.top/gtwombsgzm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pycfn.com/gtfbhienhx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.bjfxy.top/gthhbloavm.html

[U43] PHP：声明命名空间
来源：http://hz.gotoacloud.top/gtjhhzqauu.html

namespace App\Http;
来源：http://hz.cashguo.top/gtvlycgzxf.html

[U44] PHP：开启严格类型
来源：http://hz.dashuyun.cn/gtwoetavwb.html

declare(strict_types=1);
来源：http://hz.jinqigufen.top/gtpkzdzizd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.chenzaomai.com/gtpwqxnhsu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtnvvywkxx.html

[U46] PHP：可空类型
来源：http://hz.pengpengdd.cyou/gterarvofp.html

?string $name = null
来源：http://hz.chenlongwang.top/gtebhzegil.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangtech.top/gtnnmqfror.html

int|string $id
来源：http://hz.wangshuangyany.cn/gtpquzaptf.html

[U48] PHP：纯枚举
来源：http://hz.9152youxi.cn/gtlckbkadr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.quarkkingdee.top/gtkscuhitq.html

[U49] PHP：只读属性
来源：http://hz.jianghu66.top/gtsyjlpiyi.html

public readonly string $name
来源：http://hz.wangdashe.top/gtgjjlitaa.html

[U50] PHP：构造器属性提升
来源：http://hz.meibo888.top/gtdsgumekz.html

public function __construct(private int $id) {}
来源：http://hz.yj20258888.top/gthgnamgma.html

[U51] PHP：数组解构
来源：http://hz.shzxlz.cn/gthbyrcame.html

[$a, $b] = $arr;
来源：http://hz.nwbrower.top/gtmsvqnqln.html

[U52] PHP：箭头函数
来源：http://hz.jqgfzy.top/gtwtvrdtou.html

$double = fn($x) => $x * 2;
来源：http://hz.tanke756.top/gttrmchzvy.html

[U53] PHP：空合并运算符
来源：http://hz.xinyue.icu/gtewcekixq.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangkeji.top/gtevegbvgh.html

[U54] PHP：空安全调用
来源：http://hz.c1oappe.top/gtbcrckcvg.html

$obj?->method()
来源：http://hz.hnqzz.top/gtkhjbccqw.html

[U55] PHP：match 表达式
来源：http://hz.daxiang520.top/gthwjkgbts.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.mhx1999.top/gtbaicftcs.html

[U56] PHP：命名参数
来源：http://hz.jyoumei.cn/gtcnthhmvz.html

f(a: 1, b: 2)
来源：http://hz.sweek.top/gtggwbfebh.html

[U57] PHP：字符串插值
来源：http://hz.tian-w.cn/gtlgcgjpzz.html

"值: {$a}"
来源：http://hz.yangfankeji.com/gtkylqxtlw.html

[U58] PHP：数组三件套
来源：http://hz.daria6918.cn/gtfheynizh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shanyushiyangkeji.top/gtqdtkuoac.html

[U59] PHP：自定义排序
来源：http://hz.snrcjt.cn/gtamqwcnio.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtmvkqlhoy.html

[U60] PHP：JSON 编解码
来源：http://hz.jinqigufen.top/gtxuhjfdly.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydzc1.top/gtceefpunq.html


<!-- 参考信息 -->