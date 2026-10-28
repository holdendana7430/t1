代发 wailian999

[S33] C++：vector 增删
来源：http://hz.gotoacloud.top/gtczzfykvv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtrrnedgvp.html

[S34] C++：遍历 vector
来源：http://hz.jinghuilouyu.cn/gtzhpsfywi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shangyingyoupin.top/gtejiavegc.html

[S35] C++：map
来源：http://hz.jinghuilouyu.cn/gtvqqfrido.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtcltzrlie.html

[S36] C++：unordered_map
来源：http://hz.chenjidiqi.icu/gtvagakokb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtenlsldui.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtyvuofebb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gogol.net.cn/gtljrsgbpi.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtvoowvmza.html

std::sort(v.begin(), v.end());
来源：http://hz.xinyue.icu/gtdfnfflcz.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtbulyxpnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hfpthk.cn/gtummfcntz.html

[S40] C++：查找元素
来源：http://hz.ppjwa.cn/gtukoacsnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yvedp.cn/gtnwhawqfn.html

[S41] C++：类与构造函数
来源：http://hz.yj20258.top/gtwtukwecq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gaohongyu789.top/gtdlamtbwc.html

[S42] C++：继承与虚函数
来源：http://hz.hnqzz.top/gtczxgbmee.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuanzx.com/gtgoqxihbs.html

[S43] C++：智能指针
来源：http://hz.jinghuilouyu.cn/gtidgooqnk.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenlongwang.top/gtfcpnswma.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gtavbjfpxl.html

void inc(int &x) { ++x; }
来源：http://hz.zhongyouzk.top/gtmntmhfgu.html

[S45] C++：lambda
来源：http://hz.haohaochexian.top/gtrubiqicq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.meibo888.top/gtqqpszouo.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangtech.top/gtejbylgqv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtqeifsymk.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtkoemsfwj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydjk.org.cn/gtmaacyblf.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gtczwfriww.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ywan-chungtsiang.top/gtwowjfmxf.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtochzcnzj.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtzopxaxgv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gtvoqpzoon.html

[S50] C++：格式化数字
来源：http://hz.tanke756.top/gtpkmvfdej.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gtxgyeigbj.html

[S51] C++：显式类型转换
来源：http://hz.andypj.xyz/gtgmqpyddv.html

static_cast<double>(a) / b
来源：http://hz.zdqjudy.top/gtzljnlgks.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtemcjkkkc.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtkczzeuql.html

[S53] C++：移动语义
来源：http://hz.cdnleiting.top/gttchgplhj.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtmbvfgsep.html

[S54] C++：异常处理
来源：http://hz.yanxiufei.cn/gtyktpktbl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.52xcode.cn/gtqqninfvl.html

[S55] C++：结构化绑定
来源：http://hz.xylfe.cn/gtfnovwdwa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hongshengwenyu.top/gtuayxwtpr.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtwkkgkpzj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gtlguuumty.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gttlwbywql.html

constexpr int N = 10;
来源：http://hz.shangyingyoupin.top/gtmuqhzpri.html

[S58] C++：命名空间
来源：http://hz.pycfn.com/gtdropsqfz.html

namespace ns { int f() { return 1; } }
来源：http://hz.pycfn.com/gthgpgnyus.html

[S59] C++：静态断言
来源：http://hz.hnqzz.top/gtomcnmusa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cheryme.top/gtmuvmcyfy.html

[S60] C++：遍历并删除元素
来源：http://hz.birdmap.top/gtpdsibcgn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtxyvjerll.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjeussmuk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.smart0.xyz/gtagfocflg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxgdqeenj.html

[T01] Kotlin：Hello World
来源：http://hz.zhiwuduotai.top/gtblflrpkx.html

println("Hello")
来源：http://hz.fengsongda.top/gtiqwpgizj.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtlzzfsnav.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.quarkkingdee.top/gtyggnscpl.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gtqihmxurh.html

"值: $b"
来源：http://hz.svipenyu.cn/gtpbeadoho.html

[T04] Kotlin：空安全
来源：http://hz.mhx1999.top/gteniqkfws.html

val n: String? = null;  n?.length
来源：http://hz.daria6918.cn/gtcxlerkzw.html

[T05] Kotlin：when 表达式
来源：http://hz.ybcxt.top/gtfofjgrcw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cheryme.top/gtaliggond.html

[T06] Kotlin：集合映射
来源：http://hz.xinyue.icu/gtuzufhnea.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtbfnskjbi.html

[T07] Kotlin：集合过滤
来源：http://hz.xziqi.cn/gthhtpnzyd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fzhhl.top/gtvgiqcgtj.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtrrrcggnn.html

data class User(val name: String, val age: Int)
来源：http://hz.iojbl.cn/gtpjvdnjal.html

[T09] Kotlin：扩展函数
来源：http://hz.yj202588.top/gtulfdoumd.html

fun String.exclaim() = this + "!"
来源：http://hz.xziqi.cn/gtuuvkasma.html

[T10] Kotlin：默认参数
来源：http://hz.feifeiyinyue.top/gtngozeurc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jlsjyb.cn/gtfdgxzfea.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gthdqdnish.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ybcxt.top/gtpstcxooz.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtxxcsqtvm.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangtech.top/gtsigqigku.html

[T13] Kotlin：只读 Map
来源：http://hz.cashguo.top/gtglrmldzy.html

val m = mapOf("a" to 1)
来源：http://hz.yanxiufei.cn/gtaqpmizzt.html

[T14] Kotlin：循环
来源：http://hz.cqqwz.cn/gtpieyxtup.html

for (i in 1..10) println(i)
来源：http://hz.nwbrower.top/gtdkgdeowe.html

[T15] Kotlin：接口
来源：http://hz.ppjwa.cn/gtkszkotpi.html

interface Shape { fun area(): Double }
来源：http://hz.smart0.xyz/gtgowjpnru.html

[T16] Swift：Hello World
来源：http://hz.dianchejie.cn/gtzmdhnixr.html

print("Hello")
来源：http://hz.cheryme.top/gtgtuksvww.html

[T17] Swift：变量与常量
来源：http://hz.yj20258.top/gtkivrxeuj.html

var a = 1;  let b = 2
来源：http://hz.quarkkingdee.top/gtoytdrguf.html

[T18] Swift：字符串插值
来源：http://hz.bjfxy.top/gtnlpecsyw.html

"值: \(b)"
来源：http://hz.sufxvd.cn/gtzasbpwgy.html

[T19] Swift：可选绑定
来源：http://hz.snrcjt.cn/gtyxsjsqtr.html

if let n = opt { print(n) }
来源：http://hz.sufxvd.cn/gtddvgyqcn.html

[T20] Swift：数组操作
来源：http://hz.yj20258.top/gtejzilfok.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hongshengwenyu.top/gtmwmuxdat.html

[T21] Swift：遍历
来源：http://hz.zhoulong.xyz/gtrlcjfvah.html

for x in a { print(x) }
来源：http://hz.fengsongda.top/gtnwtkbhwc.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtqyymwddp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tian-w.cn/gtnnmoqmcp.html

[T23] Swift：函数
来源：http://hz.hysaishi.cn/gtygzbqxcc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jianghu66.top/gtxryyucfp.html

[T24] Swift：闭包
来源：http://hz.chenlongwang.top/gtwnflcysl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtjfsmfqsw.html

[T25] Swift：结构体
来源：http://hz.pycfn.com/gtfvqsxyre.html

struct P { var x: Int }
来源：http://hz.yongpay.top/gtpsarkteq.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtfbkkzomz.html

class A: Base { override func f() {} }
来源：http://hz.yanxiufei.cn/gtpsxismbe.html

[T27] Swift：错误处理
来源：http://hz.yvedp.cn/gttyonlisp.html

do { try f() } catch { print(error) }
来源：http://hz.yvedp.cn/gtkfdlaggj.html

[T28] Swift：枚举
来源：http://hz.aibaodan.cn/gthxpbcthc.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gtcmqgwfwl.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gthdayvvhp.html

guard let x = opt else { return }
来源：http://hz.ywan-chungtsiang.top/gthlogzrgi.html

[T30] Swift：协议
来源：http://hz.xuetiantiany.cn/gtoavecqqe.html

protocol Shape { func area() -> Double }
来源：http://hz.mhx1999.top/gtlymzkqiy.html

[T31] Lua：Hello World
来源：http://hz.pycfn.com/gtqxkksooj.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtylxibxfp.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtfxhtyneg.html

local a = 1
来源：http://hz.dianchejie.cn/gtdxbwygjt.html

[T33] Lua：表（数组）
来源：http://hz.9152youxi.cn/gtisoychyv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.vqdsnc.cn/gtwilnrdwm.html

[T34] Lua：遍历表
来源：http://hz.ywan-chungtsiang.top/gtbvllgxld.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuxming.cn/gtsbendsws.html

[T35] Lua：字典表
来源：http://hz.smart0.xyz/gtlubupsym.html

local d = { a = 1 };  d.b = 2
来源：http://hz.kuanghao11.cn/gtwetybhxi.html

[T36] Lua：函数
来源：http://hz.gzhubu.top/gtswkjepda.html

function add(a, b) return a + b end
来源：http://hz.gotoacloud.top/gtmkrpcliq.html

[T37] Lua：字符串拼接
来源：http://hz.pengpengdd.cyou/gtitdoysga.html

"a" .. "b"
来源：http://hz.zhengqikj.top/gtkkzrpgxe.html

[T38] Lua：条件
来源：http://hz.zdqjudy.top/gtmtbjmykx.html

if x > 0 then print("正") end
来源：http://hz.ivvv.top/gtyzjairym.html

[T39] Lua：模式匹配
来源：http://hz.yvedp.cn/gtxydamiic.html

string.find(s, "%d+")
来源：http://hz.dashuyun.cn/gtauxzibco.html

[T40] Lua：元表
来源：http://hz.pengpengdd.cyou/gtjcberdlm.html

setmetatable({}, { __index = base })
来源：http://hz.sweek.top/gtkflqgirt.html

[T41] Perl：Hello World
来源：http://hz.tian-w.cn/gtzmrajypx.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gttnxcdfim.html

[T42] Perl：变量类型
来源：http://hz.gaohongyu789.top/gtwbrjfuqu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yonumen.top/gtuepfqgwj.html

[T43] Perl：字符串插值
来源：http://hz.wangshuangyany.cn/gtaftcmjpa.html

"值: $a"
来源：http://hz.shanyushiyangtech.top/gtwkbtttrt.html

[T44] Perl：条件
来源：http://hz.bjfxy.top/gtktxklszi.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gtfpnnmggd.html

[T45] Perl：数组遍历
来源：http://hz.9152youxi.cn/gtegzegwej.html

for my $x (@arr) { print $x; }
来源：http://hz.shzxlz.cn/gtpepzruww.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gtbuhoaxvj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj202588.top/gtusjvaxoa.html

[T47] Perl：正则捕获
来源：http://hz.xylfe.cn/gtsiwqdfdy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jlsjyb.cn/gtzqflfbor.html

[T48] Perl：正则替换
来源：http://hz.fzhhl.top/gtqupdzfii.html

$s =~ s/old/new/g;
来源：http://hz.c1oappe.top/gtcdhopqtj.html

[T49] Perl：函数
来源：http://hz.hongshengwenyu.top/gtvxweysyl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhongyouzk.top/gtbilttuvn.html

[T50] Perl：逐行读文件
来源：http://hz.tianlin.xyz/gtvgwggtjh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.kuanghao11.cn/gtdkgiveoq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.feifeiyinyue.top/gtbxmjsjrr.html

[T51] Scala：Hello World
来源：http://hz.jyoumei.cn/gtzpsepaac.html

println("Hello")
来源：http://hz.yonumen.top/gthofsklhf.html

[T52] Scala：变量
来源：http://hz.xuetiantiany.cn/gtmptrfjnq.html

val a = 1;  var b = 2
来源：http://hz.yj202588.top/gtdufzpeio.html

[T53] Scala：字符串插值
来源：http://hz.daria6918.cn/gtxphggnhn.html

s"值: $b"
来源：http://hz.aizwys.cn/gtgetalrrp.html

[T54] Scala：集合映射
来源：http://hz.aibaodan.cn/gtewcyfozr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhengqikj.top/gtqhigcjgp.html

[T55] Scala：集合过滤
来源：http://hz.yonumen.top/gtvbvvnpae.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtjnispcmg.html

[T56] Scala：样例类
来源：http://hz.zycfv.cn/gtqbhmptjj.html

case class User(name: String, age: Int)
来源：http://hz.bjfxy.top/gtybpzeuum.html

[T57] Scala：模式匹配
来源：http://hz.fengsongda.top/gtjugpxyqo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.quarkkingdee.top/gtcsuagefl.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtzovdpywp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aibaodan.cn/gtvdogtpul.html

[T59] Scala：循环
来源：http://hz.haohaochexian.top/gtkpaoceab.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtitpromsy.html

[T60] Scala：折叠
来源：http://hz.guannengcc.top/gtztmhjlyg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zdqjudy.top/gtqptucuaq.html

================================================================================
来源：http://hz.tianlin.xyz/gtpjfyvtmz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hfpthk.cn/gtiemahmzb.html

================================================================================
来源：http://hz.jlsjyb.cn/gthnzrrmgg.html

[U01] Py：创建虚拟环境
来源：http://hz.hnxiangtu.top/gtsuclqqbh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.316326.xyz/gttxigvrue.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jianghu66.top/gtiewqysql.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenzaomai.com/gtgnlzypyp.html

[U03] Py：加载 .env 配置
来源：http://hz.gaohongyu789.top/gtutgbjhhh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gtwfunoumw.html

[U04] Py：变量调试打印
来源：http://hz.ydjk.org.cn/gtvdppqzkv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hywenlv.cn/gttaiebdrl.html

[U05] Py：列表去重且保序
来源：http://hz.0kj1m.cn/gttpqrczqh.html

list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtaowkhxwl.html

[U06] Py：合并两个字典
来源：http://hz.yuanzhike.top/gtakesabsx.html

{**a, **b}
来源：http://hz.gzhubu.top/gtqdioedvf.html

[U07] Py：反转字典键值
来源：http://hz.zhoulong.xyz/gtbloprzvw.html

{v: k for k, v in d.items()}
来源：http://hz.chenjidiqi.icu/gtywqkyibd.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gtexlnpvsu.html

[y for x in nested for y in x]
来源：http://hz.ivvv.top/gttwusrrrl.html

[U09] Py：字典取最大值的键
来源：http://hz.ydzc1.top/gtufwpbxac.html

max(d, key=d.get)
来源：http://hz.jiagoushi.top/gtcfvtkfwv.html

[U10] Py：按值排序字典
来源：http://hz.ehwqpu.com/gttlxdqhsg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jlsjyb.cn/gtyfqderul.html

[U11] Py：生成器表达式
来源：http://hz.chenlongwang.top/gthuafxhfe.html

(x * 2 for x in arr)
来源：http://hz.wangshuangyany.cn/gtfazebjuj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cdnleiting.top/gtcoruaabv.html

Counter(arr).most_common(3)
来源：http://hz.jqgufenzy.top/gtdjapaxav.html

[U13] Py：固定长度队列
来源：http://hz.xziqi.cn/gtravourik.html

deque(maxlen=10)
来源：http://hz.sysykeji.top/gtledhkddf.html

[U14] Py：分组收集到列表
来源：http://hz.yuxming.cn/gtodbithkp.html

defaultdict(list)
来源：http://hz.nwbrower.top/gtqrwjknjo.html

[U15] Py：高精度计时
来源：http://hz.yuanzhike.top/gtyijkunqd.html

t = time.perf_counter()
来源：http://hz.chenlongwang.top/gtqhxdatcj.html

[U16] Py：命令行参数解析
来源：http://hz.yvedp.cn/gtkjdecutz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nanxuanxn.top/gtzbhjwhza.html

[U17] Py：初始化日志
来源：http://hz.smart0.xyz/gtqbuhatom.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhixingplan.top/gtpororpif.html

[U18] Py：预编译正则
来源：http://hz.gaohongyu789.top/gttetawxvb.html

pat = re.compile(r"\d+")
来源：http://hz.316326.xyz/gtnkjbxmoc.html

[U19] Py：正则替换带回调
来源：http://hz.mhx1999.top/gtznacwqra.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.svipenyu.cn/gtxjeztoed.html

[U20] Py：缓存函数结果
来源：http://hz.chenzaomai.com/gtnbdebpge.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xuanzx.com/gtyiuxesda.html

[U21] Py：自定义上下文管理器
来源：http://hz.shzxlz.cn/gtrnjklccf.html

@contextlib.contextmanager
来源：http://hz.hfpthk.cn/gtemwpnrfg.html

[U22] Py：矩阵转置
来源：http://hz.kuanghao11.cn/gtwlghscaf.html

list(zip(*m))
来源：http://hz.guowangkeji.top/gtbpnsokob.html

[U23] Py：分块读取大文件
来源：http://hz.snrcjt.cn/gtvzuetdgc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.iojbl.cn/gthdaqoift.html

[U24] Py：路径操作
来源：http://hz.dianchejie.cn/gttsvldsyh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ehwqpu.com/gtbeiufgvh.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258.top/gtjqqyikas.html

csv.DictReader(f)
来源：http://hz.hammf.cn/gthkzudxzx.html

[U26] Py：并发下载
来源：http://hz.zhiwuduotai.top/gtrtkirwzk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xinyue.icu/gtnsxwclxm.html

[U27] Py：异步 HTTP
来源：http://hz.cucudq.cn/gtnxudmvdb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigufen.top/gtwzbtojoy.html

[U28] Py：类型别名
来源：http://hz.chenjidiqi.icu/gtueitsiby.html

UserId = int
来源：http://hz.316326.xyz/gtcptrmsze.html

[U29] Py：属性校验
来源：http://hz.0kj1m.cn/gthchkqffs.html

@property 与 @x.setter 配合
来源：http://hz.guowangkeji.top/gtrctzqzik.html

[U30] Py：数据类
来源：http://hz.0kj1m.cn/gtcwegnqqj.html

@dataclass(slots=True)
来源：http://hz.dashuyun.cn/gtlpzhxiqq.html

[U31] Py：单测
来源：http://hz.fengsongda.top/gtyyqvicjw.html

python -m pytest -q
来源：http://hz.ppjwa.cn/gtvlsfsacd.html

[U32] Py：代码格式化
来源：http://hz.nanxinkj.top/gtjhxbcgiq.html

ruff format . && ruff check --fix .
来源：http://hz.ehwqpu.com/gtdmjkcnym.html

[U33] Py：打包发布
来源：http://hz.cdnleiting.top/gtyyyqgejh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cdnleiting.top/gtnwwmxoeh.html

[U34] Py：判断编码
来源：http://hz.shuidangran.top/gtqczixfmx.html

chardet.detect(raw)
来源：http://hz.gzhubu.top/gtdkcqoitm.html

[U35] Py：发送邮件
来源：http://hz.dashuyun.cn/gtwlzdotao.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgufenzy.top/gthdowpntj.html

[U36] Py：定时任务
来源：http://hz.nanxinkj.top/gtedjedehe.html

schedule.every(10).minutes.do(job)
来源：http://hz.zdqjudy.top/gtxownrknh.html

[U37] Py：读写 Excel
来源：http://hz.yongpay.top/gtmfdfiiws.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cashguo.top/gtsdzgnvuq.html

[U38] Py：获取脚本所在目录
来源：http://hz.cheryme.top/gtnlgahnrz.html

Path(__file__).resolve().parent
来源：http://hz.yj202588.top/gtmtsjnbem.html

[U39] Py：判断是否在交互环境
来源：http://hz.hnxiangtu.top/gtmiiailaq.html

sys.stdout.isatty()
来源：http://hz.yongpay.top/gtmtdzzhog.html

[U40] Py：打印到标准错误
来源：http://hz.aibaodan.cn/gtuetzolxs.html

print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtpbacendm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.birdmap.top/gtaubnjfhz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gtjrlahyqb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.bjfxy.top/gthsiynpdn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhijiandao.cn/gtivlqwyjl.html

[U43] PHP：声明命名空间
来源：http://hz.sxryk.cn/gtljnredgr.html

namespace App\Http;
来源：http://hz.kuanghao11.cn/gtjacgdboa.html

[U44] PHP：开启严格类型
来源：http://hz.xuanzx.com/gtlhxuvavh.html

declare(strict_types=1);
来源：http://hz.tian-w.cn/gtmcxqdgly.html

[U45] PHP：类型声明与返回类型
来源：http://hz.316326.xyz/gtpgugwafs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtkdaccted.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtjrakxcdg.html

?string $name = null
来源：http://hz.yj20258.top/gtbayqjsbw.html

[U47] PHP：联合类型
来源：http://hz.guannengcc.top/gtswoganac.html

int|string $id
来源：http://hz.guannengcc.top/gtgpuqshft.html

[U48] PHP：纯枚举
来源：http://hz.nanxinkj.top/gtsltauigg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.birdmap.top/gtpcotrbbq.html

[U49] PHP：只读属性
来源：http://hz.hywenlv.cn/gtrylcutlr.html

public readonly string $name
来源：http://hz.zhixingplan.top/gtpltcpdrb.html

[U50] PHP：构造器属性提升
来源：http://hz.zhaomingkeji.xyz/gtpibnnflv.html

public function __construct(private int $id) {}
来源：http://hz.shuidangran.top/gtmcivsrto.html

[U51] PHP：数组解构
来源：http://hz.ivvv.top/gtrnplrrrq.html

[$a, $b] = $arr;
来源：http://hz.ehwqpu.com/gtrlecvjiq.html

[U52] PHP：箭头函数
来源：http://hz.tian-w.cn/gtacdoywtn.html

$double = fn($x) => $x * 2;
来源：http://hz.cucudq.cn/gtqawrajzt.html

[U53] PHP：空合并运算符
来源：http://hz.hammf.cn/gtosthjnhe.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258.top/gtfnatlwqo.html

[U54] PHP：空安全调用
来源：http://hz.ydzc1.top/gtdasurige.html

$obj?->method()
来源：http://hz.chenzaomai.com/gtjlfgmofy.html

[U55] PHP：match 表达式
来源：http://hz.shanyushiyangtech.top/gtdrrkfckv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tian-w.cn/gtacaikyeo.html

[U56] PHP：命名参数
来源：http://hz.nwbrower.top/gtcgurvdwi.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtormrykrk.html

[U57] PHP：字符串插值
来源：http://hz.nanxuanxn.top/gtvgtzashq.html

"值: {$a}"
来源：http://hz.shanyushiyangkeji.top/gtfrlfvshb.html

[U58] PHP：数组三件套
来源：http://hz.yuanzhike.top/gtjhcdhlmw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tian-w.cn/gtjwgomqiy.html


<!-- 参考信息 -->