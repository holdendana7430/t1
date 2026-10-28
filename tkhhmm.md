代发 wailian999

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gtffozteew.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.9152youxi.cn/gtgwewakec.html

[S34] C++：遍历 vector
来源：http://hz.cashguo.top/gtvzyavcvs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuanzx.com/gtefhcjeeh.html

[S35] C++：map
来源：http://hz.bjfxy.top/gttftzgclx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtcvsazpbu.html

[S36] C++：unordered_map
来源：http://hz.shuidangran.top/gtkohsipak.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtszwlygqc.html

[S37] C++：set
来源：http://hz.hfpthk.cn/gtpkpzleny.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtboyusxez.html

[S38] C++：排序
来源：http://hz.mhx1999.top/gtzkjphgtf.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtzripwwxc.html

[S39] C++：自定义比较器排序
来源：http://hz.xinyue.icu/gtyqedsknm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtzkbjmrpx.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtzrncyshw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.c1oappe.top/gtzoduhqky.html

[S41] C++：类与构造函数
来源：http://hz.chenlongwang.top/gtlkgroxaf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtjcwbksqm.html

[S42] C++：继承与虚函数
来源：http://hz.zhaomingkeji.xyz/gtuzsknbik.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtfyvlqltc.html

[S43] C++：智能指针
来源：http://hz.xylfe.cn/gtnqhkvucc.html

auto p = std::make_unique<int>(5);
来源：http://hz.shzxlz.cn/gtuyfyrmdn.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gtlmzsohgw.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtsqwgyotz.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtkcjpdyym.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gtreplwgoq.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gttcfnnuqd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gthaztqoks.html

[S47] C++：结构化绑定遍历
来源：http://hz.redwolf501.top/gtqfyarfpv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.birdmap.top/gtqzwlxpmx.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gtvhcwszmn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ppjwa.cn/gthmtdckia.html

while (std::getline(in, line)) { }
来源：http://hz.zhongyouzk.top/gtqkffuhmh.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtzxbrbazf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guannengcc.top/gtplrqbbcg.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtgbndzalo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtcpobuusd.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtbewutnur.html

static_cast<double>(a) / b
来源：http://hz.hongshengwenyu.top/gtklmlggxv.html

[S52] C++：const 与 noexcept
来源：http://hz.wangdashe.top/gtwqfulnne.html

int size() const noexcept { return n_; }
来源：http://hz.hysaishi.cn/gtfwgxpmui.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangtech.top/gtfwjovfmj.html

std::vector<int> w = std::move(v);
来源：http://hz.aibaodan.cn/gtsknpsgnm.html

[S54] C++：异常处理
来源：http://hz.ydjk.org.cn/gtxsleqcqr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aibaodan.cn/gtcpnhhddj.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtcabeiqbl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xingfuxueyuan.xyz/gtmrouutmo.html

[S56] C++：optional
来源：http://hz.jinghuilouyu.cn/gttklhsrlu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tanke756.top/gtuswcahqc.html

[S57] C++：编译期常量
来源：http://hz.zhengqikj.top/gtjhhymbrh.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gtnrwhypvi.html

[S58] C++：命名空间
来源：http://hz.hongshengwenyu.top/gthniwmjyf.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtwbpvubwx.html

[S59] C++：静态断言
来源：http://hz.meibo888.top/gtqqzgciut.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtvlliykkn.html

[S60] C++：遍历并删除元素
来源：http://hz.ydzc1.top/gturtqyfvg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guannengcc.top/gtppkkqxom.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtjblvqfuv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtsjniyibu.html

================================================================================
来源：http://hz.c1oappe.top/gtqjymalgg.html

[T01] Kotlin：Hello World
来源：http://hz.hywenlv.cn/gtxayxbbds.html

println("Hello")
来源：http://hz.mhx1999.top/gtesesxdvr.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtgsbwkgom.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.316326.xyz/gtlzglpucm.html

[T03] Kotlin：字符串模板
来源：http://hz.yuanzhike.top/gtwnjgfabc.html

"值: $b"
来源：http://hz.gzhubu.top/gtclwnfooq.html

[T04] Kotlin：空安全
来源：http://hz.ehwqpu.com/gtzaacyuad.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gtdsgacoem.html

[T05] Kotlin：when 表达式
来源：http://hz.cucudq.cn/gtqynbxdhi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenlongwang.top/gtkerkjkax.html

[T06] Kotlin：集合映射
来源：http://hz.shuidangran.top/gtfnccwhpn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ywan-chungtsiang.top/gtsweflaxs.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gtpcxehnue.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.0kj1m.cn/gtyrmvqzbe.html

[T08] Kotlin：数据类
来源：http://hz.yangfankeji.com/gthupqhebw.html

data class User(val name: String, val age: Int)
来源：http://hz.aibaodan.cn/gtqkhccelm.html

[T09] Kotlin：扩展函数
来源：http://hz.hnxiangtu.top/gturvzjosv.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgufenzy.top/gttreliogf.html

[T10] Kotlin：默认参数
来源：http://hz.daria6918.cn/gtneeteaqd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangshuangyany.cn/gtvioproih.html

[T11] Kotlin：协程
来源：http://hz.tian-w.cn/gtrlaozofs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtkaeryuth.html

[T12] Kotlin：解构声明
来源：http://hz.havefunace.top/gtxznsvzbi.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtgcvfpcdd.html

[T13] Kotlin：只读 Map
来源：http://hz.pengpengdd.cyou/gtrndpdbvp.html

val m = mapOf("a" to 1)
来源：http://hz.zycfv.cn/gtdzzvraiy.html

[T14] Kotlin：循环
来源：http://hz.mhx1999.top/gtnphectqe.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtjyfncvgs.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtclhxnhfl.html

interface Shape { fun area(): Double }
来源：http://hz.daxiang520.top/gtohxzlmag.html

[T16] Swift：Hello World
来源：http://hz.yonumen.top/gtmenyjvpm.html

print("Hello")
来源：http://hz.yvedp.cn/gtqwztuhed.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtejdazvxp.html

var a = 1;  let b = 2
来源：http://hz.feifeiyinyue.top/gtpwcratug.html

[T18] Swift：字符串插值
来源：http://hz.smart0.xyz/gthaaalvxx.html

"值: \(b)"
来源：http://hz.xziqi.cn/gtzvvmxbpn.html

[T19] Swift：可选绑定
来源：http://hz.ywan-chungtsiang.top/gteuugoqhk.html

if let n = opt { print(n) }
来源：http://hz.shangyingyoupin.top/gtzraocivg.html

[T20] Swift：数组操作
来源：http://hz.jyoumei.cn/gtcwmnynmp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgufenzy.top/gtkzltyckw.html

[T21] Swift：遍历
来源：http://hz.yvedp.cn/gtvfmnmxfb.html

for x in a { print(x) }
来源：http://hz.gogol.net.cn/gtmvnrqcrz.html

[T22] Swift：字典
来源：http://hz.smart0.xyz/gtzgftexcr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gthxiznfna.html

[T23] Swift：函数
来源：http://hz.mhx1999.top/gtmigsmuwd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daxiang520.top/gtbxnxlxwv.html

[T24] Swift：闭包
来源：http://hz.ydzc1.top/gtntkskqrh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gtunaroono.html

[T25] Swift：结构体
来源：http://hz.tanke756.top/gteopbcjzm.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gtcjlhqgvi.html

[T26] Swift：类与重写
来源：http://hz.ehwqpu.com/gtunsxkypq.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gtvlviamou.html

[T27] Swift：错误处理
来源：http://hz.hywenlv.cn/gtzcswrxiw.html

do { try f() } catch { print(error) }
来源：http://hz.hammf.cn/gtueclprev.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gtozqkrume.html

enum Color { case red, green }
来源：http://hz.quarkkingdee.top/gtyvdrfwyw.html

[T29] Swift：guard 提前返回
来源：http://hz.fzhhl.top/gtjyzgnxfp.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtvfflopyz.html

[T30] Swift：协议
来源：http://hz.xuetiantiany.cn/gtztkwpczf.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gtkowuzafs.html

[T31] Lua：Hello World
来源：http://hz.chenlongwang.top/gtbviwayes.html

print("Hello")
来源：http://hz.xinyue.icu/gtapklqjeh.html

[T32] Lua：局部变量
来源：http://hz.daria6918.cn/gtmtfctvso.html

local a = 1
来源：http://hz.hammf.cn/gtbpqfsrbk.html

[T33] Lua：表（数组）
来源：http://hz.jinqigufen.top/gtljgooptq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sysykeji.top/gtnmpphraz.html

[T34] Lua：遍历表
来源：http://hz.zhaomingkeji.xyz/gtrgugpcnb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hammf.cn/gtwgjgasfo.html

[T35] Lua：字典表
来源：http://hz.jinqigufen.top/gtzwngnaim.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yanxiufei.cn/gtesnnclie.html

[T36] Lua：函数
来源：http://hz.fzhhl.top/gtuptxhwpp.html

function add(a, b) return a + b end
来源：http://hz.zhongyouzk.top/gtydfbdwwe.html

[T37] Lua：字符串拼接
来源：http://hz.nwbrower.top/gteayorkto.html

"a" .. "b"
来源：http://hz.ydzc1.top/gtrtogvfpp.html

[T38] Lua：条件
来源：http://hz.xingfuxueyuan.xyz/gtnpeymmpo.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gttqjtohsg.html

[T39] Lua：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtgrapreou.html

string.find(s, "%d+")
来源：http://hz.yanxiufei.cn/gtqsaolmzk.html

[T40] Lua：元表
来源：http://hz.ivvv.top/gtglqncepa.html

setmetatable({}, { __index = base })
来源：http://hz.smart0.xyz/gthvxqokte.html

[T41] Perl：Hello World
来源：http://hz.xinyue.icu/gttpukakgo.html

print "Hello\n";
来源：http://hz.xuanzx.com/gtsljolowv.html

[T42] Perl：变量类型
来源：http://hz.pengpengdd.cyou/gtvcuyibiu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sysykeji.top/gtdqgyjyjh.html

[T43] Perl：字符串插值
来源：http://hz.zhengqikj.top/gtrgcnyemh.html

"值: $a"
来源：http://hz.havefunace.top/gtjohvghwi.html

[T44] Perl：条件
来源：http://hz.dashuyun.cn/gtxrbftkzq.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtmaybqcdw.html

[T45] Perl：数组遍历
来源：http://hz.jinghuilouyu.cn/gtyderevxj.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gtvhcthyca.html

[T46] Perl：哈希操作
来源：http://hz.wangdashe.top/gtaeolwfwc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shuidangran.top/gtpcdartir.html

[T47] Perl：正则捕获
来源：http://hz.jinqigufen.top/gtxpzlmgqv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jianghu66.top/gtgkdsvfyb.html

[T48] Perl：正则替换
来源：http://hz.zhongyouzk.top/gtifbnaxpr.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtjixujfkc.html

[T49] Perl：函数
来源：http://hz.jinqigfzy.top/gtwfujaalr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yuanzhike.top/gtqngtrkgs.html

[T50] Perl：逐行读文件
来源：http://hz.sufxvd.cn/gtqfefekoe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.snrcjt.cn/gtxinwscla.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.svipenyu.cn/gtmomhhkzs.html

[T51] Scala：Hello World
来源：http://hz.tianlin.xyz/gtcafaivze.html

println("Hello")
来源：http://hz.ehwqpu.com/gtwgvbpsun.html

[T52] Scala：变量
来源：http://hz.jinghuilouyu.cn/gtlpbefpgq.html

val a = 1;  var b = 2
来源：http://hz.ivvv.top/gtjddxjrug.html

[T53] Scala：字符串插值
来源：http://hz.meibo888.top/gtzoybraun.html

s"值: $b"
来源：http://hz.yueranfly.top/gtkfqpazvq.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtbhfrzvyp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.bjfxy.top/gtpqzbpkad.html

[T55] Scala：集合过滤
来源：http://hz.yvedp.cn/gtcdxoyseb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ivvv.top/gttdvpjwkv.html

[T56] Scala：样例类
来源：http://hz.nanxuanxn.top/gtsoooccjy.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtbxikycdu.html

[T57] Scala：模式匹配
来源：http://hz.52xcode.cn/gttljnrljr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fengsongda.top/gtuzqafwqr.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtawiwcppl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xylfe.cn/gtcmcaguta.html

[T59] Scala：循环
来源：http://hz.aizwys.cn/gtvcdwwrxl.html

for (i <- 1 to 10) println(i)
来源：http://hz.aibaodan.cn/gtbubsqvya.html

[T60] Scala：折叠
来源：http://hz.sxryk.cn/gteidrltov.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtxdvsxath.html

================================================================================
来源：http://hz.andypj.xyz/gtlznkrlmc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtqifncvys.html

================================================================================
来源：http://hz.ydjk.org.cn/gtpeicpaae.html

[U01] Py：创建虚拟环境
来源：http://hz.zhongyouzk.top/gttjylqbcz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guannengcc.top/gtiymshrgl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenjidiqi.icu/gtmmsxoisp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jlsjyb.cn/gtqtrwvtka.html

[U03] Py：加载 .env 配置
来源：http://hz.jinyuanbaomall.cn/gthkjwdemq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.guowangkeji.top/gtzlfvzjfg.html

[U04] Py：变量调试打印
来源：http://hz.guannengcc.top/gtdggdazfr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tianlin.xyz/gtbvweeamb.html

[U05] Py：列表去重且保序
来源：http://hz.shangyingyoupin.top/gtsnajggqh.html

list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtqdhiyzpv.html

[U06] Py：合并两个字典
来源：http://hz.feifeiyinyue.top/gtutpzhvqf.html

{**a, **b}
来源：http://hz.mhx1999.top/gtnmjamxid.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangtech.top/gthjodnupj.html

{v: k for k, v in d.items()}
来源：http://hz.pengpengdd.cyou/gtnloembax.html

[U08] Py：展平二维列表
来源：http://hz.0kj1m.cn/gtuibltuto.html

[y for x in nested for y in x]
来源：http://hz.svipenyu.cn/gtgtpdewxo.html

[U09] Py：字典取最大值的键
来源：http://hz.chenlongwang.top/gtfdnqcyam.html

max(d, key=d.get)
来源：http://hz.yj20258.top/gteoxjzerb.html

[U10] Py：按值排序字典
来源：http://hz.zycfv.cn/gtkyxmumlv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhongyouzk.top/gtfcaqqrey.html

[U11] Py：生成器表达式
来源：http://hz.pycfn.com/gtnermglcl.html

(x * 2 for x in arr)
来源：http://hz.ybcxt.top/gtkotsinjm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shangyingyoupin.top/gttjyvegzs.html

Counter(arr).most_common(3)
来源：http://hz.fzhhl.top/gtqxcgcuxj.html

[U13] Py：固定长度队列
来源：http://hz.tianlin.xyz/gtsfrhsuvf.html

deque(maxlen=10)
来源：http://hz.c1oappe.top/gtsqebvqzy.html

[U14] Py：分组收集到列表
来源：http://hz.jinqigufen.top/gtjtqhywlb.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtpuuabcki.html

[U15] Py：高精度计时
来源：http://hz.jqgufenzy.top/gtcjkphxaw.html

t = time.perf_counter()
来源：http://hz.cashguo.top/gtviqxmbxb.html

[U16] Py：命令行参数解析
来源：http://hz.ybcxt.top/gtqnbzqpaa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hnxiangtu.top/gtkgsirlsy.html

[U17] Py：初始化日志
来源：http://hz.meibo888.top/gtugfwmqhg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gttrqtapuv.html

[U18] Py：预编译正则
来源：http://hz.daria6918.cn/gtovspowro.html

pat = re.compile(r"\d+")
来源：http://hz.zhiwuduotai.top/gtmzfaftuf.html

[U19] Py：正则替换带回调
来源：http://hz.iojbl.cn/gtgvfpnwwe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yangfankeji.com/gtovowmrnc.html

[U20] Py：缓存函数结果
来源：http://hz.dianchejie.cn/gthjzzyjkf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yuanzhike.top/gtxfertwzk.html

[U21] Py：自定义上下文管理器
来源：http://hz.ppjwa.cn/gtpremzeyv.html

@contextlib.contextmanager
来源：http://hz.zhongyouzk.top/gtoxsxioeh.html

[U22] Py：矩阵转置
来源：http://hz.hnqzz.top/gtvtrgnuwn.html

list(zip(*m))
来源：http://hz.jiagoushi.top/gtjbnuvsrg.html

[U23] Py：分块读取大文件
来源：http://hz.meibo888.top/gtyspmgjio.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hongshengwenyu.top/gtmtyrrmvo.html

[U24] Py：路径操作
来源：http://hz.andypj.xyz/gtpkdcuutg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhoulong.xyz/gtwkavdsoo.html

[U25] Py：CSV 按字典读
来源：http://hz.ehwqpu.com/gtqqysfoym.html

csv.DictReader(f)
来源：http://hz.cashguo.top/gtsuelgpky.html

[U26] Py：并发下载
来源：http://hz.zhiwuduotai.top/gtxqrhsknd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cqqwz.cn/gthliqefqa.html

[U27] Py：异步 HTTP
来源：http://hz.yangfankeji.com/gtuezvogjc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.aibaodan.cn/gtqwcdpkpz.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtvdecxyyu.html

UserId = int
来源：http://hz.ydjk.org.cn/gtcefifiij.html

[U29] Py：属性校验
来源：http://hz.guannengcc.top/gtabssyqzu.html

@property 与 @x.setter 配合
来源：http://hz.hongshengwenyu.top/gtwqbbjbjl.html

[U30] Py：数据类
来源：http://hz.gaohongyu789.top/gtnokbeuin.html

@dataclass(slots=True)
来源：http://hz.ywan-chungtsiang.top/gtiqcgfcmc.html

[U31] Py：单测
来源：http://hz.guannengcc.top/gtwyhqococ.html

python -m pytest -q
来源：http://hz.cqqwz.cn/gteeiajthz.html

[U32] Py：代码格式化
来源：http://hz.cdnleiting.top/gtauzrovna.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigfzy.top/gtpkkjdqjv.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtetpjhcmw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.haohaochexian.top/gtinhsifpp.html

[U34] Py：判断编码
来源：http://hz.snrcjt.cn/gtfjfxyfkn.html

chardet.detect(raw)
来源：http://hz.havefunace.top/gttzonthou.html

[U35] Py：发送邮件
来源：http://hz.xylfe.cn/gtrqcoexod.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.iojbl.cn/gtqndrspnx.html

[U36] Py：定时任务
来源：http://hz.mhx1999.top/gtmrrgmpcg.html

schedule.every(10).minutes.do(job)
来源：http://hz.xingfuxueyuan.xyz/gtyjmkrgvq.html

[U37] Py：读写 Excel
来源：http://hz.havefunace.top/gtldhclkjx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cheryme.top/gtzerwwrfa.html

[U38] Py：获取脚本所在目录
来源：http://hz.snrcjt.cn/gtfzhvfhbx.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gtdndkhfyp.html

[U39] Py：判断是否在交互环境
来源：http://hz.nanxuanxn.top/gtjnquztbs.html

sys.stdout.isatty()
来源：http://hz.9152youxi.cn/gtdtmlbpbk.html

[U40] Py：打印到标准错误
来源：http://hz.tanke756.top/gtltcgismv.html

print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtywzksocd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gzhubu.top/gtpudjrwdo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xingfuxueyuan.xyz/gtanbzxssn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhijiandao.cn/gtjfqrlubu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhiwuduotai.top/gtixzwvqka.html

[U43] PHP：声明命名空间
来源：http://hz.yonumen.top/gthzbgnobm.html

namespace App\Http;
来源：http://hz.nwbrower.top/gtjchrlxan.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258888.top/gtlrfxhuas.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gtntvakjld.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydjk.org.cn/gtvbphvtyy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.kuanghao11.cn/gtagqomyik.html

[U46] PHP：可空类型
来源：http://hz.tian-w.cn/gtvblgzybp.html

?string $name = null
来源：http://hz.meibo888.top/gtfnckkpsp.html

[U47] PHP：联合类型
来源：http://hz.kuanghao11.cn/gtmtvfhztn.html

int|string $id
来源：http://hz.haohaochexian.top/gtiaiwxtfq.html

[U48] PHP：纯枚举
来源：http://hz.andypj.xyz/gttuohrjgc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xziqi.cn/gthnxjtwer.html

[U49] PHP：只读属性
来源：http://hz.shanyushiyangkeji.top/gtvhhhskfc.html

public readonly string $name
来源：http://hz.iojbl.cn/gtbamyylnb.html

[U50] PHP：构造器属性提升
来源：http://hz.sysykeji.top/gtfzdtcbwy.html

public function __construct(private int $id) {}
来源：http://hz.hywenlv.cn/gtpmzhlgtp.html

[U51] PHP：数组解构
来源：http://hz.nanxinkj.top/gtvnghjmaq.html

[$a, $b] = $arr;
来源：http://hz.yj20258.top/gtrtzpyvhi.html

[U52] PHP：箭头函数
来源：http://hz.wangdashe.top/gtydgzhoaq.html

$double = fn($x) => $x * 2;
来源：http://hz.hywenlv.cn/gtvbbnjyql.html

[U53] PHP：空合并运算符
来源：http://hz.tianlin.xyz/gtloqzuxtx.html

$v = $a ?? $b ?? "default";
来源：http://hz.tianlin.xyz/gtpqdxclqr.html

[U54] PHP：空安全调用
来源：http://hz.pengpengdd.cyou/gtobxeyaza.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtwncdeakq.html

[U55] PHP：match 表达式
来源：http://hz.zhixingplan.top/gthsrfofcx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yangfankeji.com/gtbpheulni.html

[U56] PHP：命名参数
来源：http://hz.jqgufenzy.top/gtvssbsjik.html

f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtbmepmlgc.html

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangtech.top/gtubaemdmj.html

"值: {$a}"
来源：http://hz.daria6918.cn/gtqaaevjxm.html

[U58] PHP：数组三件套
来源：http://hz.bjfxy.top/gtnzeftzjm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.iojbl.cn/gtydfwkwon.html


<!-- 参考信息 -->