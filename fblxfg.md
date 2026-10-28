代发 wailian999

int main(int argc, char **argv)
来源：http://hz.cashguo.top/gtrumjshdg.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gtqerrvixo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtwekmcouz.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtjccabdll.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtceqavtev.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtmsajfsup.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cucudq.cn/gthljiejab.html

[S22] C：字符串转数字
来源：http://hz.zhaomingkeji.xyz/gtisihigmm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenlongwang.top/gttvbnuphv.html

[S23] C：随机数
来源：http://hz.cucudq.cn/gtmqkzadoh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gtaliwdwqb.html

[S24] C：获取本地时间
来源：http://hz.ydzc1.top/gtkdckfaau.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.316326.xyz/gtzsmprowc.html

[S25] C：内存拷贝
来源：http://hz.yonumen.top/gteejdocgu.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtdmmsatjv.html

[S26] C：内存清零
来源：http://hz.hnqzz.top/gtaqxeynnb.html

memset(a, 0, sizeof a);
来源：http://hz.smart0.xyz/gtwqhpchcg.html

[S27] C：定义常量
来源：http://hz.yongpay.top/gtmaeajryq.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtykumxear.html

[S28] C：静态变量
来源：http://hz.cucudq.cn/gthdgbfpek.html

static int counter = 0;
来源：http://hz.kuanghao11.cn/gtrclqyvty.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtitiglkzu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gtecrpjxlf.html

[S30] C：头文件保护
来源：http://hz.hongshengwenyu.top/gtquhtunnp.html

#ifndef X_H
来源：http://hz.zhongyouzk.top/gtltqpnpok.html

#define X_H
来源：http://hz.52xcode.cn/gtcgwspvme.html

#endif
来源：http://hz.ybcxt.top/gtktwgpusl.html

[S31] C++：Hello World
来源：http://hz.daria6918.cn/gtgrinqall.html

#include <iostream>
来源：http://hz.ppjwa.cn/gtnyimhadb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtcecxtkjb.html

[S32] C++：字符串
来源：http://hz.cdnleiting.top/gtdxabqhbi.html

std::string s = "hi";  s += "!";
来源：http://hz.smart0.xyz/gtbpzwqwbb.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtgswhzbou.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtwqokovfv.html

[S34] C++：遍历 vector
来源：http://hz.hfpthk.cn/gtkhqjmsjd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gtijcotrot.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtlxenmybq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtcelzuzpz.html

[S36] C++：unordered_map
来源：http://hz.cheryme.top/gtbsesgkzd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gthdugvcji.html

[S37] C++：set
来源：http://hz.sweek.top/gtlnjgqawv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtvmmztvrr.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gtbbgywpiq.html

std::sort(v.begin(), v.end());
来源：http://hz.shuidangran.top/gtkxhictxq.html

[S39] C++：自定义比较器排序
来源：http://hz.zhaomingkeji.xyz/gttdvwpqtz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xuanzx.com/gtsrrlugnr.html

[S40] C++：查找元素
来源：http://hz.dianchejie.cn/gtlpxlkfar.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenlongwang.top/gtlscvmrtj.html

[S41] C++：类与构造函数
来源：http://hz.jlsjyb.cn/gtxqfrswve.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zdqjudy.top/gtthncmjqd.html

[S42] C++：继承与虚函数
来源：http://hz.jlsjyb.cn/gtfvyqiswv.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuxming.cn/gtwgudhgqx.html

[S43] C++：智能指针
来源：http://hz.jinqigufen.top/gtwybrcysm.html

auto p = std::make_unique<int>(5);
来源：http://hz.bjfxy.top/gtwasaetkf.html

[S44] C++：引用传参
来源：http://hz.hfpthk.cn/gtmdfivrbf.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtaxqzktdt.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtpwsznwwi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yangfankeji.com/gtsjapzcdx.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtvddodjne.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtgwwskynj.html

[S47] C++：结构化绑定遍历
来源：http://hz.hywenlv.cn/gtkandbekj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtaertktxi.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtbiiwnsqb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.c1oappe.top/gtrylrecpd.html

while (std::getline(in, line)) { }
来源：http://hz.nanxuanxn.top/gtyminmktl.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtvvukozse.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cheryme.top/gtrtustodi.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gthncvujjg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jyoumei.cn/gtnpuvskho.html

[S51] C++：显式类型转换
来源：http://hz.hfpthk.cn/gtloiaihsq.html

static_cast<double>(a) / b
来源：http://hz.tianlin.xyz/gteqygufec.html

[S52] C++：const 与 noexcept
来源：http://hz.chenlongwang.top/gtsbzyizog.html

int size() const noexcept { return n_; }
来源：http://hz.mhx1999.top/gtqirkcjhc.html

[S53] C++：移动语义
来源：http://hz.zhiwuduotai.top/gtwyypkiee.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtoustdyii.html

[S54] C++：异常处理
来源：http://hz.chenjidiqi.icu/gtqvbwtbwp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtrmhoxonl.html

[S55] C++：结构化绑定
来源：http://hz.sufxvd.cn/gtijjxgtgb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xinyue.icu/gtuukobira.html

[S56] C++：optional
来源：http://hz.haohaochexian.top/gttwemzjbw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtoeghtwje.html

[S57] C++：编译期常量
来源：http://hz.0kj1m.cn/gtrkzzskvb.html

constexpr int N = 10;
来源：http://hz.yvedp.cn/gtuymcbjju.html

[S58] C++：命名空间
来源：http://hz.yanxiufei.cn/gtuizmkojy.html

namespace ns { int f() { return 1; } }
来源：http://hz.hammf.cn/gthemwaszj.html

[S59] C++：静态断言
来源：http://hz.yuanzhike.top/gttizrhuvd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.9152youxi.cn/gtykqzuhgq.html

[S60] C++：遍历并删除元素
来源：http://hz.daxiang520.top/gtazfpmbnv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.bjfxy.top/gtcnswptwz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtogpuigng.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtnehhptel.html

================================================================================
来源：http://hz.fzhhl.top/gtdcsfutun.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtvwosibpg.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtsgauuwks.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtpsxsejqr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtgbwtksjb.html

[T03] Kotlin：字符串模板
来源：http://hz.9152youxi.cn/gtbpyjpdrw.html

"值: $b"
来源：http://hz.tanke756.top/gtgmkhpiyl.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtzowbwddy.html

val n: String? = null;  n?.length
来源：http://hz.ywan-chungtsiang.top/gtukckgdqi.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigfzy.top/gtieoivimb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtcvowfdey.html

[T06] Kotlin：集合映射
来源：http://hz.zhiwuduotai.top/gtuxcgcoug.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hysaishi.cn/gtgkbahfei.html

[T07] Kotlin：集合过滤
来源：http://hz.ppjwa.cn/gtbnaeevkq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgufenzy.top/gttsugdwhn.html

[T08] Kotlin：数据类
来源：http://hz.fengsongda.top/gtgibjwcfo.html

data class User(val name: String, val age: Int)
来源：http://hz.xuetiantiany.cn/gtjgcufnhb.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gtgldtbvhe.html

fun String.exclaim() = this + "!"
来源：http://hz.pycfn.com/gtpqxsxges.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gthufadzcw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zdqjudy.top/gtfqhafxfw.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtjnwaqite.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtdkjpxyxd.html

[T12] Kotlin：解构声明
来源：http://hz.zdqjudy.top/gttemmzcqi.html

val (a, b) = Pair(1, 2)
来源：http://hz.shuidangran.top/gtezdownhl.html

[T13] Kotlin：只读 Map
来源：http://hz.havefunace.top/gtdzdcrxcm.html

val m = mapOf("a" to 1)
来源：http://hz.jinyuanbaomall.cn/gtyspfvymk.html

[T14] Kotlin：循环
来源：http://hz.yj202588.top/gtnalfvwil.html

for (i in 1..10) println(i)
来源：http://hz.jlsjyb.cn/gtbgvjczjf.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gtcntodqez.html

interface Shape { fun area(): Double }
来源：http://hz.snrcjt.cn/gthyhmowth.html

[T16] Swift：Hello World
来源：http://hz.zhaomingkeji.xyz/gtyjwmrnrf.html

print("Hello")
来源：http://hz.jinqigfzy.top/gthysubiqh.html

[T17] Swift：变量与常量
来源：http://hz.ybcxt.top/gttfyilxbl.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtosddthow.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtqinmbwso.html

"值: \(b)"
来源：http://hz.zhixingplan.top/gtxnvztivv.html

[T19] Swift：可选绑定
来源：http://hz.yongpay.top/gturscqypk.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangtech.top/gttrqhubvm.html

[T20] Swift：数组操作
来源：http://hz.xingfuxueyuan.xyz/gtremwpdgc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dashuyun.cn/gtcpxwwsbl.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtrtlbnwct.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtqsnxqeic.html

[T22] Swift：字典
来源：http://hz.ehwqpu.com/gtjdtroayu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtusxvarqx.html

[T23] Swift：函数
来源：http://hz.vqdsnc.cn/gtywcxigyr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gtcumpectg.html

[T24] Swift：闭包
来源：http://hz.jqgufenzy.top/gtjyygeqrf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xinyue.icu/gteokwlfxr.html

[T25] Swift：结构体
来源：http://hz.xuanzx.com/gtlfijwhbd.html

struct P { var x: Int }
来源：http://hz.yuanzhike.top/gtbrplfqcr.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtodwtaqik.html

class A: Base { override func f() {} }
来源：http://hz.redwolf501.top/gtodgfdonr.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtniyvidjk.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigufen.top/gtpxzhpvub.html

[T28] Swift：枚举
来源：http://hz.hnqzz.top/gttmwedhdr.html

enum Color { case red, green }
来源：http://hz.daxiang520.top/gtmimytgrd.html

[T29] Swift：guard 提前返回
来源：http://hz.meibo888.top/gtbiahzrcq.html

guard let x = opt else { return }
来源：http://hz.yj20258888.top/gttwfhhsuz.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtcflzmduz.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtzpmjungf.html

[T31] Lua：Hello World
来源：http://hz.nanxinkj.top/gtgolaqfbv.html

print("Hello")
来源：http://hz.nwbrower.top/gtkvrpekyv.html

[T32] Lua：局部变量
来源：http://hz.meibo888.top/gthpvlbtoj.html

local a = 1
来源：http://hz.hnqzz.top/gtfexzjmzv.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gtbskraatw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj202588.top/gtaumsoozf.html

[T34] Lua：遍历表
来源：http://hz.hfpthk.cn/gtukuvtvid.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jyoumei.cn/gtowxgxgms.html

[T35] Lua：字典表
来源：http://hz.sweek.top/gttaqodntp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ivvv.top/gtdbhgimzi.html

[T36] Lua：函数
来源：http://hz.yj20258.top/gtskdumrug.html

function add(a, b) return a + b end
来源：http://hz.zhiwuduotai.top/gtxhzcfqfn.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtwampbxev.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtzygjcnze.html

[T38] Lua：条件
来源：http://hz.svipenyu.cn/gtyjfwdlkb.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtvlczroel.html

[T39] Lua：模式匹配
来源：http://hz.sweek.top/gtkzqfyzqm.html

string.find(s, "%d+")
来源：http://hz.yangfankeji.com/gtzhqegbaw.html

[T40] Lua：元表
来源：http://hz.cdnleiting.top/gtuxffqepq.html

setmetatable({}, { __index = base })
来源：http://hz.aibaodan.cn/gtwzswfrsc.html

[T41] Perl：Hello World
来源：http://hz.jqgfzy.top/gttfetnukq.html

print "Hello\n";
来源：http://hz.aibaodan.cn/gteyoruazz.html

[T42] Perl：变量类型
来源：http://hz.sweek.top/gtzrecwqxd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yvedp.cn/gttrrcprjl.html

[T43] Perl：字符串插值
来源：http://hz.guannengcc.top/gttymzlixn.html

"值: $a"
来源：http://hz.aizwys.cn/gtrdglsnuw.html

[T44] Perl：条件
来源：http://hz.yj20258.top/gtjzsdmwra.html

if ($a > 0) { print "正"; }
来源：http://hz.quarkkingdee.top/gtxtijhyxg.html

[T45] Perl：数组遍历
来源：http://hz.yuanzhike.top/gtgnopqzio.html

for my $x (@arr) { print $x; }
来源：http://hz.jinghuilouyu.cn/gtrgqkohfp.html

[T46] Perl：哈希操作
来源：http://hz.52xcode.cn/gtlwytlsch.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sufxvd.cn/gthsjybqum.html

[T47] Perl：正则捕获
来源：http://hz.iojbl.cn/gtrbecilaq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shangyingyoupin.top/gtvzpfigeg.html

[T48] Perl：正则替换
来源：http://hz.zhaomingkeji.xyz/gtqznmebkw.html

$s =~ s/old/new/g;
来源：http://hz.aizwys.cn/gtviegogjf.html

[T49] Perl：函数
来源：http://hz.316326.xyz/gtogropvkg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cucudq.cn/gtloljklip.html

[T50] Perl：逐行读文件
来源：http://hz.xuetiantiany.cn/gtyhrupqbn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xziqi.cn/gtnxnwhccq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jyoumei.cn/gtcrcwlzgj.html

[T51] Scala：Hello World
来源：http://hz.yongpay.top/gtqzkbljkf.html

println("Hello")
来源：http://hz.dashuyun.cn/gtwtmdceqv.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gtzvblfkfa.html

val a = 1;  var b = 2
来源：http://hz.gogol.net.cn/gtogctruxh.html

[T53] Scala：字符串插值
来源：http://hz.hfpthk.cn/gtioklfjio.html

s"值: $b"
来源：http://hz.yueranfly.top/gtfxxudwaz.html

[T54] Scala：集合映射
来源：http://hz.smart0.xyz/gtockftqtq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangshuangyany.cn/gtiylzbdis.html

[T55] Scala：集合过滤
来源：http://hz.ppjwa.cn/gtzsfiblcu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gogol.net.cn/gtqeaenobs.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtpqsylhhr.html

case class User(name: String, age: Int)
来源：http://hz.tian-w.cn/gterjhbuzg.html

[T57] Scala：模式匹配
来源：http://hz.xylfe.cn/gtnwijfmgh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shangyingyoupin.top/gtbsissmjs.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtpjggmxvq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sxryk.cn/gtuapxnvee.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gtcutbgdtb.html

for (i <- 1 to 10) println(i)
来源：http://hz.jianghu66.top/gtytbmnodr.html

[T60] Scala：折叠
来源：http://hz.jqgfzy.top/gtcmkygddn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuanzhike.top/gtpmchczxo.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgdapfukm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtdlgciyut.html

================================================================================
来源：http://hz.hammf.cn/gtbyfhzyyv.html

[U01] Py：创建虚拟环境
来源：http://hz.redwolf501.top/gtmlvmtvpo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gtpglteanm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cashguo.top/gtwvkxmbxi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.guowangkeji.top/gtwosantcj.html

[U03] Py：加载 .env 配置
来源：http://hz.iojbl.cn/gtjoujxzsc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shzxlz.cn/gtfcrkoumo.html

[U04] Py：变量调试打印
来源：http://hz.dianchejie.cn/gtfozwabhn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sweek.top/gtmiuoswyg.html

[U05] Py：列表去重且保序
来源：http://hz.shzxlz.cn/gtrrynpvaa.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtratqzonu.html

[U06] Py：合并两个字典
来源：http://hz.mhx1999.top/gtjxzvbkpj.html

{**a, **b}
来源：http://hz.xuetiantiany.cn/gtctxbgdve.html

[U07] Py：反转字典键值
来源：http://hz.tian-w.cn/gtndkmyulu.html

{v: k for k, v in d.items()}
来源：http://hz.hammf.cn/gtfrcebyml.html

[U08] Py：展平二维列表
来源：http://hz.zhijiandao.cn/gtmeeycwbl.html

[y for x in nested for y in x]
来源：http://hz.xuanzx.com/gtxuwlgwqw.html

[U09] Py：字典取最大值的键
来源：http://hz.dianchejie.cn/gtvkttxscp.html

max(d, key=d.get)
来源：http://hz.tian-w.cn/gtzbrpssgu.html

[U10] Py：按值排序字典
来源：http://hz.jiagoushi.top/gtuaiaeaul.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sxryk.cn/gtskcxachh.html

[U11] Py：生成器表达式
来源：http://hz.haohaochexian.top/gtbcfsamqu.html

(x * 2 for x in arr)
来源：http://hz.52xcode.cn/gtvtytexvu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.vqdsnc.cn/gtejpctlld.html

Counter(arr).most_common(3)
来源：http://hz.sxryk.cn/gtrtmykdhj.html

[U13] Py：固定长度队列
来源：http://hz.jinyuanbaomall.cn/gthpcohuyy.html

deque(maxlen=10)
来源：http://hz.yonumen.top/gtzjwfgkhj.html

[U14] Py：分组收集到列表
来源：http://hz.wangdashe.top/gtovhczsrk.html

defaultdict(list)
来源：http://hz.yueranfly.top/gthchhrfho.html

[U15] Py：高精度计时
来源：http://hz.sxryk.cn/gtanjawfix.html

t = time.perf_counter()
来源：http://hz.smart0.xyz/gtjhfhvxih.html

[U16] Py：命令行参数解析
来源：http://hz.zhaomingkeji.xyz/gtgufyuomy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sweek.top/gtioxegpri.html

[U17] Py：初始化日志
来源：http://hz.quarkkingdee.top/gtklukmiji.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenlongwang.top/gtirybxwju.html

[U18] Py：预编译正则
来源：http://hz.hysaishi.cn/gtmgrdkcad.html

pat = re.compile(r"\d+")
来源：http://hz.andypj.xyz/gtnxzmtvjr.html

[U19] Py：正则替换带回调
来源：http://hz.ydzc1.top/gthfayexsq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxuanxn.top/gtnunuqhky.html

[U20] Py：缓存函数结果
来源：http://hz.zhongyouzk.top/gtuxoierkd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtgixepvag.html

[U21] Py：自定义上下文管理器
来源：http://hz.0kj1m.cn/gttemqmxip.html

@contextlib.contextmanager
来源：http://hz.dashuyun.cn/gtnsuywebg.html

[U22] Py：矩阵转置
来源：http://hz.andypj.xyz/gtdmvutnkc.html

list(zip(*m))
来源：http://hz.wangshuangyany.cn/gthwmwlteh.html

[U23] Py：分块读取大文件
来源：http://hz.yvedp.cn/gtrhaewwcr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guannengcc.top/gtmlbgtxya.html

[U24] Py：路径操作
来源：http://hz.xziqi.cn/gthwvultan.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zycfv.cn/gthjonpvfc.html

[U25] Py：CSV 按字典读
来源：http://hz.gzhubu.top/gtzwqnuboo.html

csv.DictReader(f)
来源：http://hz.zhixingplan.top/gtxlftkrgu.html

[U26] Py：并发下载
来源：http://hz.ehwqpu.com/gtiscvxkwl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.pycfn.com/gthxxrapaf.html

[U27] Py：异步 HTTP
来源：http://hz.zhongyouzk.top/gtzwucxhrm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jlsjyb.cn/gtitrnsxxq.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtmsibmntl.html

UserId = int
来源：http://hz.cdnleiting.top/gtclcrhxtm.html

[U29] Py：属性校验
来源：http://hz.jinghuilouyu.cn/gtfttukgoc.html

@property 与 @x.setter 配合
来源：http://hz.nanxinkj.top/gtexaftysk.html

[U30] Py：数据类
来源：http://hz.ppjwa.cn/gtbfalyqpp.html

@dataclass(slots=True)
来源：http://hz.aibaodan.cn/gtqtfhurio.html

[U31] Py：单测
来源：http://hz.ybcxt.top/gtkndolnto.html

python -m pytest -q
来源：http://hz.sxryk.cn/gtduxjikyi.html

[U32] Py：代码格式化
来源：http://hz.zhaomingkeji.xyz/gtvacnfzne.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gtkagbmrzo.html

[U33] Py：打包发布
来源：http://hz.yangfankeji.com/gtbpvyxfmz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cheryme.top/gtplgmavnn.html

[U34] Py：判断编码
来源：http://hz.yuxming.cn/gtzmrmfzej.html

chardet.detect(raw)
来源：http://hz.jqgfzy.top/gtlwnnpecw.html

[U35] Py：发送邮件
来源：http://hz.bjfxy.top/gteeeeoxwn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hnqzz.top/gtozetetzo.html

[U36] Py：定时任务
来源：http://hz.tian-w.cn/gtbccicpsm.html

schedule.every(10).minutes.do(job)
来源：http://hz.hammf.cn/gtrhzivmkf.html

[U37] Py：读写 Excel
来源：http://hz.zhiwuduotai.top/gtzcksnazi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yueranfly.top/gtllhhcgkq.html

[U38] Py：获取脚本所在目录
来源：http://hz.meibo888.top/gtfzvzdesp.html

Path(__file__).resolve().parent
来源：http://hz.aizwys.cn/gtxzbjnbed.html

[U39] Py：判断是否在交互环境
来源：http://hz.ywan-chungtsiang.top/gtfrcuxgib.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtmpsqpefa.html

[U40] Py：打印到标准错误
来源：http://hz.zhiwuduotai.top/gthwprwmjk.html

print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtecriyvda.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jlsjyb.cn/gtwqzinpug.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.316326.xyz/gtmowyuvtd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sysykeji.top/gtfvhwybkq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.aibaodan.cn/gtjehzpsqg.html


<!-- 参考信息 -->