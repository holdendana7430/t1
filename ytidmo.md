代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.zhiwuduotai.top/gtzapgcocz.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtganbohhy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtwhpnfaeg.html

[S05] C：字符串长度
来源：http://hz.bjfxy.top/gtcqojpcif.html

strlen(s)
来源：http://hz.svipenyu.cn/gtovgrbdxu.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gttpdyyyws.html

strcmp(a, b) == 0
来源：http://hz.jinqigufen.top/gtwddrcpdp.html

[S07] C：数组遍历求和
来源：http://hz.svipenyu.cn/gtvfklumtj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guowangkeji.top/gtntfgtoxh.html

[S08] C：动态内存分配与释放
来源：http://hz.hnqzz.top/gthpksvfgm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydzc1.top/gtnfiwehvm.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gtxnadtqco.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dashuyun.cn/gteuqvtevv.html

[S10] C：指针与解引用
来源：http://hz.yvedp.cn/gtigichntc.html

int *p = &a;  *p = 5;
来源：http://hz.smart0.xyz/gtvbflufpa.html

[S11] C：逐行读文件
来源：http://hz.cucudq.cn/gtxhhqtoeg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtfdflxlfb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gtbtjoljqy.html

fclose(f);
来源：http://hz.yuxming.cn/gtgdmiufgj.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtdznxfkfg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtsqewkklr.html

[S13] C：宏定义
来源：http://hz.shangyingyoupin.top/gtnlfyuhve.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtatckmnbr.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gtwrhubgge.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jiagoushi.top/gtofybstss.html

[S15] C：类型转换
来源：http://hz.svipenyu.cn/gtoeuuxkmo.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtaeudzmvh.html

[S16] C：位操作置位
来源：http://hz.ppjwa.cn/gtnxixrjeq.html

x |= (1 << 3);
来源：http://hz.sufxvd.cn/gtgbwufnxs.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtfqafnkss.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtozkafamz.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtxkrhqcra.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtbwcmodob.html

[S19] C：快速排序
来源：http://hz.gotoacloud.top/gtzfhnafqh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.andypj.xyz/gtgwcerjvc.html

[S20] C：二分查找
来源：http://hz.feifeiyinyue.top/gtsgthufha.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtblujuslf.html

[S21] C：字符类别判断
来源：http://hz.chenlongwang.top/gthpjwwygq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shuidangran.top/gtdbbeawur.html

[S22] C：字符串转数字
来源：http://hz.xuanzx.com/gtmuplvvlr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtzieezzku.html

[S23] C：随机数
来源：http://hz.shanyushiyangtech.top/gtrbgyczby.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.mhx1999.top/gtskemmrjm.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtycezynbf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cdnleiting.top/gtrjzsdfwz.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtubtgcwlm.html

memcpy(dst, src, n);
来源：http://hz.jlsjyb.cn/gtnwnhmrct.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gteomidifj.html

memset(a, 0, sizeof a);
来源：http://hz.yonumen.top/gtqmahzlug.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtojokyfly.html

const double PI = 3.14159;
来源：http://hz.tian-w.cn/gtolaevffn.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtpqtxmssc.html

static int counter = 0;
来源：http://hz.kuanghao11.cn/gtvgsgpuin.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtonwuqbqk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydzc1.top/gtxyfgabco.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gttqzltcky.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtwwckktuw.html

#define X_H
来源：http://hz.cqqwz.cn/gtyzbwtoml.html

#endif
来源：http://hz.shuidangran.top/gtfypuchqr.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtfniezdhm.html

#include <iostream>
来源：http://hz.vqdsnc.cn/gtxkbmrpje.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtewaatrej.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtnzsijuxe.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtbzvrqgnm.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gtsqfmvtcb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.feifeiyinyue.top/gtukpuuobf.html

[S34] C++：遍历 vector
来源：http://hz.cashguo.top/gtrlbjhgua.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtjscbonhj.html

[S35] C++：map
来源：http://hz.yuxming.cn/gtfqveznzg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtgsuzwmwe.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtemjgkddv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtwqjbykzv.html

[S37] C++：set
来源：http://hz.zhixingplan.top/gtzpttcmfo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtqscxeeob.html

[S38] C++：排序
来源：http://hz.daria6918.cn/gtzlhsdopj.html

std::sort(v.begin(), v.end());
来源：http://hz.yuxming.cn/gtesaojgtb.html

[S39] C++：自定义比较器排序
来源：http://hz.yueranfly.top/gtnhzxkeko.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zdqjudy.top/gtiylowqbi.html

[S40] C++：查找元素
来源：http://hz.sufxvd.cn/gtvfgkntef.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtoqghpuea.html

[S41] C++：类与构造函数
来源：http://hz.jinqigfzy.top/gtokizlvcp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtrcqjzuto.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtlqcqtwul.html

class B : public Base { public: void f() override {} };
来源：http://hz.316326.xyz/gtosbrbuzn.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtygyjqywn.html

auto p = std::make_unique<int>(5);
来源：http://hz.mhx1999.top/gtxceagdgb.html

[S44] C++：引用传参
来源：http://hz.yj20258888.top/gtjczsjjcd.html

void inc(int &x) { ++x; }
来源：http://hz.pengpengdd.cyou/gtxhrskksw.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gtxywkjqbo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gaohongyu789.top/gtbxvgucah.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtdzexajse.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtcnlxekkx.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gtvilvoalo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jianghu66.top/gtxmkdnlwx.html

[S48] C++：逐行读文件
来源：http://hz.xuetiantiany.cn/gtlbtthptk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yongpay.top/gtuxyreugr.html

while (std::getline(in, line)) { }
来源：http://hz.tianlin.xyz/gtgebgssfo.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtsdpqbgjv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtbndzkjix.html

[S50] C++：格式化数字
来源：http://hz.ywan-chungtsiang.top/gtrcaukmow.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.redwolf501.top/gtidpovpsp.html

[S51] C++：显式类型转换
来源：http://hz.jinghuilouyu.cn/gtqdbozwhi.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtmxdwymmm.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtyhbtlxum.html

int size() const noexcept { return n_; }
来源：http://hz.sufxvd.cn/gteprsvzid.html

[S53] C++：移动语义
来源：http://hz.zhaomingkeji.xyz/gtiomvesoo.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtruwhdrqm.html

[S54] C++：异常处理
来源：http://hz.dashuyun.cn/gtayelipnf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenjidiqi.icu/gtttffwyvz.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtmsuxnocm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hammf.cn/gtztvmjble.html

[S56] C++：optional
来源：http://hz.ydjk.org.cn/gteabdelkd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hysaishi.cn/gtebpozthq.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtloppecal.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtebczfqor.html

[S58] C++：命名空间
来源：http://hz.jlsjyb.cn/gtlmlqckxr.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtmprlluvz.html

[S59] C++：静态断言
来源：http://hz.tianlin.xyz/gtrcsiwfpz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gtkhxhnpwn.html

[S60] C++：遍历并删除元素
来源：http://hz.hfpthk.cn/gtrufpdcja.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gtzvlpyvfd.html

================================================================================
来源：http://hz.ivvv.top/gttxbocizu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgufenzy.top/gtytdakznz.html

================================================================================
来源：http://hz.316326.xyz/gtezsqgixv.html

[T01] Kotlin：Hello World
来源：http://hz.wangdashe.top/gtlrfzyqdd.html

println("Hello")
来源：http://hz.meibo888.top/gtuitjaeov.html

[T02] Kotlin：变量
来源：http://hz.yj20258888.top/gtaiwaistf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.iojbl.cn/gtazqscmxf.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gthrfvadzj.html

"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtaxphbsag.html

[T04] Kotlin：空安全
来源：http://hz.chenjidiqi.icu/gtrlbovsjv.html

val n: String? = null;  n?.length
来源：http://hz.sxryk.cn/gtyflouoew.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgfzy.top/gtdlbggndq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fengsongda.top/gtrrvaxhic.html

[T06] Kotlin：集合映射
来源：http://hz.ybcxt.top/gtukfsquyi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangtech.top/gtuyqfdsqj.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtwqolgcew.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ivvv.top/gtmizbvwgl.html

[T08] Kotlin：数据类
来源：http://hz.zdqjudy.top/gtwuvwmalk.html

data class User(val name: String, val age: Int)
来源：http://hz.shangyingyoupin.top/gtkrccdzwf.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtgkdcimwo.html

fun String.exclaim() = this + "!"
来源：http://hz.zdqjudy.top/gtmwjsezmj.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtckafhbut.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtcosekxim.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtxnunuedj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shanyushiyangtech.top/gtarptyrhl.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gtcdqcsfwo.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gtctvnrlvq.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtvymlvwcy.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gtbuhdypul.html

[T14] Kotlin：循环
来源：http://hz.meibo888.top/gtqsqylrgf.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtfspswlzu.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtuvtvwbkt.html

interface Shape { fun area(): Double }
来源：http://hz.gotoacloud.top/gtiddlplrd.html

[T16] Swift：Hello World
来源：http://hz.sufxvd.cn/gtpwrztcap.html

print("Hello")
来源：http://hz.birdmap.top/gtpiqrvrgm.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gturiqkvcl.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtywlvtdyh.html

[T18] Swift：字符串插值
来源：http://hz.nanxinkj.top/gtwbmnjwlg.html

"值: \(b)"
来源：http://hz.0kj1m.cn/gtkfjblkcq.html

[T19] Swift：可选绑定
来源：http://hz.quarkkingdee.top/gtbogbunuw.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtgqybutar.html

[T20] Swift：数组操作
来源：http://hz.jiagoushi.top/gtkvmpkgqm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gtydqxardq.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtwpazufgb.html

for x in a { print(x) }
来源：http://hz.gzhubu.top/gtiuxupbqa.html

[T22] Swift：字典
来源：http://hz.chenzaomai.com/gtsjfqnzbe.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxuanxn.top/gtltvixmyk.html

[T23] Swift：函数
来源：http://hz.nanxinkj.top/gticcvcsbz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtswqtubnt.html

[T24] Swift：闭包
来源：http://hz.feifeiyinyue.top/gtytrhrfgs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtaziwroyx.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtoooofnse.html

struct P { var x: Int }
来源：http://hz.xinyue.icu/gtjcuolrvk.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gtgrbhoobz.html

class A: Base { override func f() {} }
来源：http://hz.sweek.top/gtfmzemcvi.html

[T27] Swift：错误处理
来源：http://hz.xziqi.cn/gtwfucyprs.html

do { try f() } catch { print(error) }
来源：http://hz.jyoumei.cn/gtdtrqzijc.html

[T28] Swift：枚举
来源：http://hz.jinghuilouyu.cn/gtjzbssikl.html

enum Color { case red, green }
来源：http://hz.zhiwuduotai.top/gtvcfajjde.html

[T29] Swift：guard 提前返回
来源：http://hz.sysykeji.top/gtneocqzma.html

guard let x = opt else { return }
来源：http://hz.yonumen.top/gtwxqulzny.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtckemnhjk.html

protocol Shape { func area() -> Double }
来源：http://hz.jyoumei.cn/gtujzfdzpq.html

[T31] Lua：Hello World
来源：http://hz.0kj1m.cn/gtvlrmesya.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtsflwuytt.html

[T32] Lua：局部变量
来源：http://hz.cqqwz.cn/gtpwqlyxfv.html

local a = 1
来源：http://hz.ehwqpu.com/gtjxzeiggx.html

[T33] Lua：表（数组）
来源：http://hz.jlsjyb.cn/gtgrhvgpmy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jlsjyb.cn/gtwaqzroau.html

[T34] Lua：遍历表
来源：http://hz.guannengcc.top/gtgpndssbc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gtsdueywmq.html

[T35] Lua：字典表
来源：http://hz.smart0.xyz/gtpivzpekr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.iojbl.cn/gtlzohxgmg.html

[T36] Lua：函数
来源：http://hz.vqdsnc.cn/gtsktmsrwz.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangkeji.top/gtrjewfdqh.html

[T37] Lua：字符串拼接
来源：http://hz.yueranfly.top/gtbchtbilk.html

"a" .. "b"
来源：http://hz.snrcjt.cn/gtamfxvaxq.html

[T38] Lua：条件
来源：http://hz.ivvv.top/gtkvwovyvh.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gthufdnpnd.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtxjxnevds.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gtttsznwfl.html

[T40] Lua：元表
来源：http://hz.daria6918.cn/gtknerfbtj.html

setmetatable({}, { __index = base })
来源：http://hz.ydjk.org.cn/gtkbyigwbm.html

[T41] Perl：Hello World
来源：http://hz.cdnleiting.top/gtvwlbormk.html

print "Hello\n";
来源：http://hz.yueranfly.top/gtkioiwhhz.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gthdkpnklx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhiwuduotai.top/gtglnykhxj.html

[T43] Perl：字符串插值
来源：http://hz.xylfe.cn/gtsxqljrgm.html

"值: $a"
来源：http://hz.bjfxy.top/gtttpfmxrs.html

[T44] Perl：条件
来源：http://hz.fzhhl.top/gtnsgjjwky.html

if ($a > 0) { print "正"; }
来源：http://hz.guowangkeji.top/gtvrirwtbw.html

[T45] Perl：数组遍历
来源：http://hz.hammf.cn/gtjbmjlsjp.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtrluwpcpl.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtfathqccm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sufxvd.cn/gtcxlmiepz.html

[T47] Perl：正则捕获
来源：http://hz.9152youxi.cn/gtsjjqbypi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhixingplan.top/gtncqvjlso.html

[T48] Perl：正则替换
来源：http://hz.ehwqpu.com/gtajdukahr.html

$s =~ s/old/new/g;
来源：http://hz.xziqi.cn/gttyvocdyd.html

[T49] Perl：函数
来源：http://hz.c1oappe.top/gtzdhftvpk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtpuvwfnfp.html

[T50] Perl：逐行读文件
来源：http://hz.xylfe.cn/gtrlzsaron.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hnqzz.top/gttafvqmul.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenzaomai.com/gtbfglikjd.html

[T51] Scala：Hello World
来源：http://hz.andypj.xyz/gtluguxbyg.html

println("Hello")
来源：http://hz.ppjwa.cn/gtzozzlfdn.html

[T52] Scala：变量
来源：http://hz.pycfn.com/gtgdqpotyx.html

val a = 1;  var b = 2
来源：http://hz.guannengcc.top/gtdvpedzpa.html

[T53] Scala：字符串插值
来源：http://hz.tian-w.cn/gtiuofzwmt.html

s"值: $b"
来源：http://hz.jyoumei.cn/gtzsnaftlh.html

[T54] Scala：集合映射
来源：http://hz.fzhhl.top/gtpdkgoupl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zycfv.cn/gtycpkdwoc.html

[T55] Scala：集合过滤
来源：http://hz.zhoulong.xyz/gtgkkufsgi.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tian-w.cn/gthwbxzfub.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtayyitnsw.html

case class User(name: String, age: Int)
来源：http://hz.gzhubu.top/gtsiqlorhm.html

[T57] Scala：模式匹配
来源：http://hz.feifeiyinyue.top/gtiwknpyyf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.dashuyun.cn/gtkuscrgud.html

[T58] Scala：函数定义
来源：http://hz.sweek.top/gtqftlbvzy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtsalsuucx.html

[T59] Scala：循环
来源：http://hz.tanke756.top/gtluavigks.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtranbtipr.html

[T60] Scala：折叠
来源：http://hz.ehwqpu.com/gtodiaevyc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gogol.net.cn/gtlxqaryna.html

================================================================================
来源：http://hz.ehwqpu.com/gtlvyakwqe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtkqmxtqtc.html

================================================================================
来源：http://hz.chenzaomai.com/gthzwumagi.html

[U01] Py：创建虚拟环境
来源：http://hz.tian-w.cn/gtphrwgkmt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhixingplan.top/gtycovpddo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.0kj1m.cn/gtmsldymwc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtwxgvosky.html

[U03] Py：加载 .env 配置
来源：http://hz.sysykeji.top/gtnxweptot.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.redwolf501.top/gtuhshnqie.html

[U04] Py：变量调试打印
来源：http://hz.xziqi.cn/gtkpjulnxl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.smart0.xyz/gtrtdwugzh.html

[U05] Py：列表去重且保序
来源：http://hz.zhongyouzk.top/gtddmdyxgm.html

list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtxlrlxomp.html

[U06] Py：合并两个字典
来源：http://hz.meibo888.top/gtwafgfgeu.html

{**a, **b}
来源：http://hz.daria6918.cn/gtupulalhu.html

[U07] Py：反转字典键值
来源：http://hz.chenzaomai.com/gtsdhlxwvv.html

{v: k for k, v in d.items()}
来源：http://hz.daria6918.cn/gtxphvqegj.html

[U08] Py：展平二维列表
来源：http://hz.snrcjt.cn/gtkclckzgp.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtirvreoir.html

[U09] Py：字典取最大值的键
来源：http://hz.jyoumei.cn/gtwworukwr.html

max(d, key=d.get)
来源：http://hz.xingfuxueyuan.xyz/gthzbmheeg.html

[U10] Py：按值排序字典
来源：http://hz.hywenlv.cn/gtapbtvwrq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.mhx1999.top/gtcdspjiov.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangkeji.top/gtatettbej.html

(x * 2 for x in arr)
来源：http://hz.havefunace.top/gtppclsuuy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.kuanghao11.cn/gtsaucybzr.html

Counter(arr).most_common(3)
来源：http://hz.zhaomingkeji.xyz/gtovsdbxrx.html

[U13] Py：固定长度队列
来源：http://hz.redwolf501.top/gtsasrqjkj.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtdhxahmiw.html

[U14] Py：分组收集到列表
来源：http://hz.tian-w.cn/gtcwwjwgxh.html

defaultdict(list)
来源：http://hz.zhiwuduotai.top/gtzbwqomoh.html

[U15] Py：高精度计时
来源：http://hz.cheryme.top/gtkvtpsiip.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtxigkvgal.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangkeji.top/gtgsskuhky.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yonumen.top/gtwmvsguqd.html

[U17] Py：初始化日志
来源：http://hz.ehwqpu.com/gtdtscuoql.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgfzy.top/gtbrnregob.html

[U18] Py：预编译正则
来源：http://hz.xingfuxueyuan.xyz/gtudvktljr.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gtjzizqfwy.html

[U19] Py：正则替换带回调
来源：http://hz.guowangkeji.top/gtculibmrh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gtpgidihpf.html

[U20] Py：缓存函数结果
来源：http://hz.dashuyun.cn/gtvaepnicj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yonumen.top/gtjplhgcxk.html

[U21] Py：自定义上下文管理器
来源：http://hz.dashuyun.cn/gtkennuhgg.html

@contextlib.contextmanager
来源：http://hz.yonumen.top/gtjanospzl.html

[U22] Py：矩阵转置
来源：http://hz.smart0.xyz/gtwbimkgmr.html

list(zip(*m))
来源：http://hz.xuanzx.com/gtnhiehzca.html

[U23] Py：分块读取大文件
来源：http://hz.yangfankeji.com/gtqfoxzoej.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shangyingyoupin.top/gtvnepncyl.html

[U24] Py：路径操作
来源：http://hz.yongpay.top/gtnmuvwzep.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gzhubu.top/gtnxwlqtdn.html

[U25] Py：CSV 按字典读
来源：http://hz.shuidangran.top/gtsulwpvtc.html

csv.DictReader(f)
来源：http://hz.hongshengwenyu.top/gturbxtrpu.html

[U26] Py：并发下载
来源：http://hz.0kj1m.cn/gtklqmggaf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ehwqpu.com/gtxefhavjc.html


<!-- 参考信息 -->