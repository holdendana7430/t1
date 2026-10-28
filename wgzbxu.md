代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtpvqzavxg.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtzvmsrdug.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hywenlv.cn/gtyuqbgjgn.html

[S05] C：字符串长度
来源：http://hz.cucudq.cn/gtarbqitbp.html

strlen(s)
来源：http://hz.jiagoushi.top/gtgfjwxbrf.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtflvxidqc.html

strcmp(a, b) == 0
来源：http://hz.ppjwa.cn/gtgpkecdku.html

[S07] C：数组遍历求和
来源：http://hz.hnxiangtu.top/gtelvireve.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtqjnljisi.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtdpxjbtoo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.haohaochexian.top/gtmipjokyr.html

[S09] C：结构体定义与初始化
来源：http://hz.gaohongyu789.top/gtvlktygep.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuxming.cn/gtquhjxixm.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtandturvj.html

int *p = &a;  *p = 5;
来源：http://hz.jinghuilouyu.cn/gtrpcqanbn.html

[S11] C：逐行读文件
来源：http://hz.yvedp.cn/gtcgdufame.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258888.top/gtkqlwmksg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.9152youxi.cn/gtevhuvlbj.html

fclose(f);
来源：http://hz.nanxuanxn.top/gtwzyimocl.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtvybvecbr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hywenlv.cn/gtfhlbseoj.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtcfsyfdwk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtsnaaioot.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtxopuxslu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangshuangyany.cn/gthbldkzec.html

[S15] C：类型转换
来源：http://hz.yj202588.top/gtikchaxhk.html

(double) a / b
来源：http://hz.fengsongda.top/gthafadbzs.html

[S16] C：位操作置位
来源：http://hz.zhijiandao.cn/gtxeaumjzq.html

x |= (1 << 3);
来源：http://hz.bjfxy.top/gtkwmbqvxw.html

[S17] C：安全拼接字符串
来源：http://hz.mhx1999.top/gtynxkbwiq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gtqfinddyk.html

[S18] C：命令行参数
来源：http://hz.zdqjudy.top/gtcxkmalfz.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gthbvmlboa.html

[S19] C：快速排序
来源：http://hz.wangshuangyany.cn/gtkhyiqbit.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtkeqwfxcd.html

[S20] C：二分查找
来源：http://hz.svipenyu.cn/gtoirfynzt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtwayjltad.html

[S21] C：字符类别判断
来源：http://hz.jlsjyb.cn/gtnfnflomo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.feifeiyinyue.top/gtnnokkvqm.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gtnmshskld.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtnfbpofrw.html

[S23] C：随机数
来源：http://hz.wangshuangyany.cn/gtonmxdlki.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shzxlz.cn/gtorgissic.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtnrzmhijq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtldzstagi.html

[S25] C：内存拷贝
来源：http://hz.chenlongwang.top/gtqhocjteb.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtxsyvgqtl.html

[S26] C：内存清零
来源：http://hz.zhengqikj.top/gttgcugjps.html

memset(a, 0, sizeof a);
来源：http://hz.svipenyu.cn/gtokezkgur.html

[S27] C：定义常量
来源：http://hz.ydzc1.top/gtlklgxevt.html

const double PI = 3.14159;
来源：http://hz.zycfv.cn/gtudsatypz.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtbtdmqbih.html

static int counter = 0;
来源：http://hz.hywenlv.cn/gtviretxaq.html

[S29] C：变参函数
来源：http://hz.hfpthk.cn/gtwwykynck.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtkfiyilyt.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gtuiyxkajx.html

#ifndef X_H
来源：http://hz.vqdsnc.cn/gtavhyylwf.html

#define X_H
来源：http://hz.daxiang520.top/gtyyefknhz.html

#endif
来源：http://hz.316326.xyz/gtnvwmuuah.html

[S31] C++：Hello World
来源：http://hz.sysykeji.top/gthyfpjvsa.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtutwbjrdx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtwwusccpp.html

[S32] C++：字符串
来源：http://hz.guannengcc.top/gtxxaoxhmt.html

std::string s = "hi";  s += "!";
来源：http://hz.cashguo.top/gtyxsusvty.html

[S33] C++：vector 增删
来源：http://hz.jinqigfzy.top/gtedzsebwj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhaomingkeji.xyz/gtpfclsodl.html

[S34] C++：遍历 vector
来源：http://hz.pycfn.com/gttrsylemh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gtszlpsunu.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtyoqvqvko.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtrqizjplx.html

[S36] C++：unordered_map
来源：http://hz.tianlin.xyz/gtmducajve.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtktkurwnr.html

[S37] C++：set
来源：http://hz.yj202588.top/gtmzrcffav.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gtuxcwmqib.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtuoenbgwa.html

std::sort(v.begin(), v.end());
来源：http://hz.gotoacloud.top/gtnzqetmzx.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtcxsjmyyn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtivjfjkhr.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtmhorvlkx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yueranfly.top/gtfevmgccq.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtxizqoxdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxinkj.top/gtaekwuemw.html

[S42] C++：继承与虚函数
来源：http://hz.svipenyu.cn/gtsqbsrtwd.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtekkqojeu.html

[S43] C++：智能指针
来源：http://hz.xuanzx.com/gtrlxmmxvj.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinyuanbaomall.cn/gtmrlzecdl.html

[S44] C++：引用传参
来源：http://hz.hysaishi.cn/gtoszedyej.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtrlkfzjoh.html

[S45] C++：lambda
来源：http://hz.ybcxt.top/gtjtpijehc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtmcxbbfay.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gtawcwcass.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtrdouurih.html

[S47] C++：结构化绑定遍历
来源：http://hz.daxiang520.top/gtdqyrscel.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.9152youxi.cn/gtsdubhatk.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtktpuncpr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xziqi.cn/gtzwfuryyl.html

while (std::getline(in, line)) { }
来源：http://hz.aizwys.cn/gtszhykbmx.html

[S49] C++：写文件
来源：http://hz.chenlongwang.top/gtresvuoeo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shzxlz.cn/gtvrdlhxpw.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtixmixxrf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cucudq.cn/gtxybcdeyt.html

[S51] C++：显式类型转换
来源：http://hz.yuxming.cn/gtwtbsxnnu.html

static_cast<double>(a) / b
来源：http://hz.yuanzhike.top/gtfweuakvr.html

[S52] C++：const 与 noexcept
来源：http://hz.guowangkeji.top/gtbmskbqtg.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gtkmvrkvyx.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtxvvtskba.html

std::vector<int> w = std::move(v);
来源：http://hz.zhixingplan.top/gtzqzojmff.html

[S54] C++：异常处理
来源：http://hz.redwolf501.top/gtyincvzjm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gtpljjxqlh.html

[S55] C++：结构化绑定
来源：http://hz.ywan-chungtsiang.top/gtguqdutov.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gthqeranyh.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtkfgdmlrz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtjedytapn.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtseaylxix.html

constexpr int N = 10;
来源：http://hz.guowangkeji.top/gtqvtehmus.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtspuyhzma.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258.top/gtiqvgtucb.html

[S59] C++：静态断言
来源：http://hz.316326.xyz/gtndcsrbsq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtkrvujzqq.html

[S60] C++：遍历并删除元素
来源：http://hz.yuanzhike.top/gtehrxhleq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hfpthk.cn/gtnvqwedvp.html

================================================================================
来源：http://hz.xuanzx.com/gtgdjjtoya.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.redwolf501.top/gtqvicttus.html

================================================================================
来源：http://hz.jyoumei.cn/gtutnbaqxg.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gtvoevdvgl.html

println("Hello")
来源：http://hz.quarkkingdee.top/gtqgxgfwdq.html

[T02] Kotlin：变量
来源：http://hz.xylfe.cn/gtsseqomvx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tianlin.xyz/gtqivosfjy.html

[T03] Kotlin：字符串模板
来源：http://hz.pengpengdd.cyou/gtefnxxadi.html

"值: $b"
来源：http://hz.yongpay.top/gtllwiwysr.html

[T04] Kotlin：空安全
来源：http://hz.wangdashe.top/gtnknbjjtn.html

val n: String? = null;  n?.length
来源：http://hz.ydjk.org.cn/gtzxstvmuv.html

[T05] Kotlin：when 表达式
来源：http://hz.fengsongda.top/gtutttyfwq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtgwufwkvu.html

[T06] Kotlin：集合映射
来源：http://hz.jinyuanbaomall.cn/gtrofqskmk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtcmqdvmud.html

[T07] Kotlin：集合过滤
来源：http://hz.tanke756.top/gtzizyipkg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhengqikj.top/gtjskxlbcv.html

[T08] Kotlin：数据类
来源：http://hz.hysaishi.cn/gtfgvvekpz.html

data class User(val name: String, val age: Int)
来源：http://hz.guannengcc.top/gtdmnlzxbd.html

[T09] Kotlin：扩展函数
来源：http://hz.jyoumei.cn/gtghfedrlu.html

fun String.exclaim() = this + "!"
来源：http://hz.tian-w.cn/gtcxrkngmd.html

[T10] Kotlin：默认参数
来源：http://hz.zhiwuduotai.top/gtnpbaeepr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.snrcjt.cn/gtaeczykdo.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtdibqmxur.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gotoacloud.top/gtlmaaywbh.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtxdaqsyhw.html

val (a, b) = Pair(1, 2)
来源：http://hz.jiagoushi.top/gtryxzptmz.html

[T13] Kotlin：只读 Map
来源：http://hz.zhaomingkeji.xyz/gtdsuxzkif.html

val m = mapOf("a" to 1)
来源：http://hz.hongshengwenyu.top/gtrgrwgbmh.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gtedwwsngl.html

for (i in 1..10) println(i)
来源：http://hz.yj20258888.top/gtabzokxrr.html

[T15] Kotlin：接口
来源：http://hz.havefunace.top/gtdhdnjzxf.html

interface Shape { fun area(): Double }
来源：http://hz.gzhubu.top/gtxajpkpdv.html

[T16] Swift：Hello World
来源：http://hz.sxryk.cn/gtleogintx.html

print("Hello")
来源：http://hz.ydzc1.top/gtbxzjddfm.html

[T17] Swift：变量与常量
来源：http://hz.snrcjt.cn/gtpgwglabw.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtrxkeegyt.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gtamlyswcp.html

"值: \(b)"
来源：http://hz.cucudq.cn/gtejryaeqh.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtywbbssfy.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtgdredeiw.html

[T20] Swift：数组操作
来源：http://hz.redwolf501.top/gtsbeymslw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhiwuduotai.top/gtmznfdcnp.html

[T21] Swift：遍历
来源：http://hz.zhaomingkeji.xyz/gtnvlsdeuv.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtzccxhggt.html

[T22] Swift：字典
来源：http://hz.cucudq.cn/gtonzzieht.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shzxlz.cn/gtqhjeqvfg.html

[T23] Swift：函数
来源：http://hz.9152youxi.cn/gtfaqzxnbr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gtfgfghjnc.html

[T24] Swift：闭包
来源：http://hz.kuanghao11.cn/gtespfhodh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cashguo.top/gtuefiebzd.html

[T25] Swift：结构体
来源：http://hz.havefunace.top/gtagbqsqhv.html

struct P { var x: Int }
来源：http://hz.aizwys.cn/gtgvuxiysd.html

[T26] Swift：类与重写
来源：http://hz.fengsongda.top/gtluzoxwqz.html

class A: Base { override func f() {} }
来源：http://hz.316326.xyz/gtywcksrec.html

[T27] Swift：错误处理
来源：http://hz.guannengcc.top/gtfmedywum.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtswvbhuxc.html

[T28] Swift：枚举
来源：http://hz.tianlin.xyz/gtepjmseol.html

enum Color { case red, green }
来源：http://hz.316326.xyz/gtujcqsbhw.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtvubohsku.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtzefrvjgq.html

[T30] Swift：协议
来源：http://hz.guannengcc.top/gtmferhijy.html

protocol Shape { func area() -> Double }
来源：http://hz.haohaochexian.top/gtknubovax.html

[T31] Lua：Hello World
来源：http://hz.chenzaomai.com/gtndckoiwz.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtdmylnnna.html

[T32] Lua：局部变量
来源：http://hz.yj20258.top/gtnslpiqmf.html

local a = 1
来源：http://hz.ppjwa.cn/gthkphjmpd.html

[T33] Lua：表（数组）
来源：http://hz.cqqwz.cn/gtclewohdq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangkeji.top/gtjgyaoceo.html

[T34] Lua：遍历表
来源：http://hz.sxryk.cn/gtuqvxiuwq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.havefunace.top/gtxguhyfvg.html

[T35] Lua：字典表
来源：http://hz.fzhhl.top/gtxqzmhbxo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtjekuksms.html

[T36] Lua：函数
来源：http://hz.cdnleiting.top/gtoclgwwcg.html

function add(a, b) return a + b end
来源：http://hz.zhiwuduotai.top/gtfpdajfnp.html

[T37] Lua：字符串拼接
来源：http://hz.aizwys.cn/gtcygoyebh.html

"a" .. "b"
来源：http://hz.52xcode.cn/gtsxxegxln.html

[T38] Lua：条件
来源：http://hz.pycfn.com/gtcbgwidif.html

if x > 0 then print("正") end
来源：http://hz.wangdashe.top/gtajfvafji.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtmdqqmpnh.html

string.find(s, "%d+")
来源：http://hz.zdqjudy.top/gtefeifgpl.html

[T40] Lua：元表
来源：http://hz.xylfe.cn/gtprnuddcd.html

setmetatable({}, { __index = base })
来源：http://hz.cucudq.cn/gtkdoyraby.html

[T41] Perl：Hello World
来源：http://hz.andypj.xyz/gtkvxpmfvu.html

print "Hello\n";
来源：http://hz.shanyushiyangtech.top/gtnvfxicgg.html

[T42] Perl：变量类型
来源：http://hz.fzhhl.top/gtuikkmlrd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gotoacloud.top/gtlckxbgyy.html

[T43] Perl：字符串插值
来源：http://hz.fzhhl.top/gtihdfbcff.html

"值: $a"
来源：http://hz.sweek.top/gtyfzqswzl.html

[T44] Perl：条件
来源：http://hz.cashguo.top/gtqrvvfnvh.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtofbqwuxk.html

[T45] Perl：数组遍历
来源：http://hz.wangdashe.top/gtmdrssomu.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtwvgvtchy.html

[T46] Perl：哈希操作
来源：http://hz.yuanzhike.top/gtqvsctfxx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtkkojtlrz.html

[T47] Perl：正则捕获
来源：http://hz.jinqigufen.top/gttuccjiok.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ivvv.top/gtbxyoinpe.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gttsnghejp.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gttegwfnsm.html

[T49] Perl：函数
来源：http://hz.aibaodan.cn/gtfjwakayg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tanke756.top/gtalxozcdj.html

[T50] Perl：逐行读文件
来源：http://hz.smart0.xyz/gtcyeqzuax.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.meibo888.top/gtvpdmggyz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nwbrower.top/gtjkdgjste.html

[T51] Scala：Hello World
来源：http://hz.zhengqikj.top/gtibwjgiup.html

println("Hello")
来源：http://hz.gzhubu.top/gtdzgjxjxl.html

[T52] Scala：变量
来源：http://hz.zhixingplan.top/gtunnxmzto.html

val a = 1;  var b = 2
来源：http://hz.birdmap.top/gtrltaufxt.html

[T53] Scala：字符串插值
来源：http://hz.zhoulong.xyz/gtelyvgthe.html

s"值: $b"
来源：http://hz.shzxlz.cn/gtmjrjbbai.html

[T54] Scala：集合映射
来源：http://hz.daxiang520.top/gtyzzgvjrr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtxbrcmobd.html

[T55] Scala：集合过滤
来源：http://hz.sysykeji.top/gtxwqbdsdy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtyvhakbgk.html

[T56] Scala：样例类
来源：http://hz.zhixingplan.top/gtjcvbmmec.html

case class User(name: String, age: Int)
来源：http://hz.meibo888.top/gtrpolyvlc.html

[T57] Scala：模式匹配
来源：http://hz.aizwys.cn/gthpwpdipm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daria6918.cn/gtpepycixs.html

[T58] Scala：函数定义
来源：http://hz.yangfankeji.com/gthmsiwoki.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ybcxt.top/gtiqbozpfz.html

[T59] Scala：循环
来源：http://hz.mhx1999.top/gtuoipdyyj.html

for (i <- 1 to 10) println(i)
来源：http://hz.gzhubu.top/gtgjgwcvdb.html

[T60] Scala：折叠
来源：http://hz.hywenlv.cn/gtcaojjpco.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shuidangran.top/gtlenpxujv.html

================================================================================
来源：http://hz.gzhubu.top/gtsdlmpxgm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jianghu66.top/gtdrqeafvi.html

================================================================================
来源：http://hz.kuanghao11.cn/gtzpppqgzq.html

[U01] Py：创建虚拟环境
来源：http://hz.haohaochexian.top/gtwqwnzedm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinghuilouyu.cn/gtdiaovxcr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tanke756.top/gtkzvyzopw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gtuseuivfm.html

[U03] Py：加载 .env 配置
来源：http://hz.yongpay.top/gtwgecbwnc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258.top/gtskmtyebz.html

[U04] Py：变量调试打印
来源：http://hz.mhx1999.top/gtoufzrlah.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tian-w.cn/gtmkxxrgst.html

[U05] Py：列表去重且保序
来源：http://hz.yanxiufei.cn/gtkvhognhw.html

list(dict.fromkeys(arr))
来源：http://hz.hywenlv.cn/gtvxybrtsx.html

[U06] Py：合并两个字典
来源：http://hz.ehwqpu.com/gtegqsenuv.html

{**a, **b}
来源：http://hz.dianchejie.cn/gtphslmbey.html

[U07] Py：反转字典键值
来源：http://hz.zhijiandao.cn/gtnbadaujl.html

{v: k for k, v in d.items()}
来源：http://hz.hfpthk.cn/gtzmzbjglh.html

[U08] Py：展平二维列表
来源：http://hz.fzhhl.top/gtqhdtfvlz.html

[y for x in nested for y in x]
来源：http://hz.zhiwuduotai.top/gthupqzppj.html

[U09] Py：字典取最大值的键
来源：http://hz.xingfuxueyuan.xyz/gtulpgbont.html

max(d, key=d.get)
来源：http://hz.tanke756.top/gthdzxuoxz.html

[U10] Py：按值排序字典
来源：http://hz.yueranfly.top/gtbovbnjzr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yongpay.top/gtajhrmcke.html

[U11] Py：生成器表达式
来源：http://hz.jinyuanbaomall.cn/gtnfksgqtj.html

(x * 2 for x in arr)
来源：http://hz.gzhubu.top/gtqwxwbunh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yonumen.top/gtmvuwhdik.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtpyiiayrv.html

[U13] Py：固定长度队列
来源：http://hz.fzhhl.top/gtwelgragr.html

deque(maxlen=10)
来源：http://hz.yongpay.top/gtbuuizzwz.html

[U14] Py：分组收集到列表
来源：http://hz.daria6918.cn/gtpdtagkms.html

defaultdict(list)
来源：http://hz.nwbrower.top/gtgqqgdijh.html

[U15] Py：高精度计时
来源：http://hz.yonumen.top/gtyxertmpl.html

t = time.perf_counter()
来源：http://hz.jinqigfzy.top/gtbntevgpv.html

[U16] Py：命令行参数解析
来源：http://hz.chenjidiqi.icu/gtkqhfvhfg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aizwys.cn/gtmpzhrnlq.html

[U17] Py：初始化日志
来源：http://hz.chenjidiqi.icu/gtmzxdrwht.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yuanzhike.top/gtyfilwrtc.html

[U18] Py：预编译正则
来源：http://hz.cheryme.top/gtnsqwijmq.html

pat = re.compile(r"\d+")
来源：http://hz.ehwqpu.com/gteqfduwzk.html

[U19] Py：正则替换带回调
来源：http://hz.guannengcc.top/gtmgaxruha.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nwbrower.top/gtphgsrsej.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangtech.top/gtmjmcjggi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jyoumei.cn/gtppjvpjws.html

[U21] Py：自定义上下文管理器
来源：http://hz.ybcxt.top/gtaczyhxtn.html

@contextlib.contextmanager
来源：http://hz.meibo888.top/gtdxtmipip.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gtirfbkaof.html

list(zip(*m))
来源：http://hz.cdnleiting.top/gtkrpsvisg.html

[U23] Py：分块读取大文件
来源：http://hz.chenzaomai.com/gtyhxbxdtr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cashguo.top/gtbasmyncz.html

[U24] Py：路径操作
来源：http://hz.pycfn.com/gtfwhzdbjn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tian-w.cn/gtvoxyjevp.html

[U25] Py：CSV 按字典读
来源：http://hz.guannengcc.top/gtgkgvdmli.html

csv.DictReader(f)
来源：http://hz.jlsjyb.cn/gtndgmcqld.html

[U26] Py：并发下载
来源：http://hz.fengsongda.top/gtxyjhxtvu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hammf.cn/gtogcshtvb.html


<!-- 参考信息 -->