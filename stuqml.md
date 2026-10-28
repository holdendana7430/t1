代发 wailian999

strlen(s)
来源：http://hz.fzhhl.top/gtkkfbsafd.html

[S06] C：字符串比较
来源：http://hz.mhx1999.top/gtwozcpgmv.html

strcmp(a, b) == 0
来源：http://hz.snrcjt.cn/gtdcofexey.html

[S07] C：数组遍历求和
来源：http://hz.nanxinkj.top/gtmoidikyq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangshuangyany.cn/gtnonrxfxw.html

[S08] C：动态内存分配与释放
来源：http://hz.mhx1999.top/gtmaslffbv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtjpsvzjry.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangtech.top/gtxiaegbke.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtqltqctoi.html

[S10] C：指针与解引用
来源：http://hz.hongshengwenyu.top/gtcrrkepwh.html

int *p = &a;  *p = 5;
来源：http://hz.ppjwa.cn/gtyxwtodlz.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtgaysjkav.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ivvv.top/gtrwtcdkey.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cqqwz.cn/gtnehmjroo.html

fclose(f);
来源：http://hz.gzhubu.top/gtlxsizeoi.html

[S12] C：写文件
来源：http://hz.yueranfly.top/gtinqwvtbu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgfzy.top/gtmcjowijy.html

[S13] C：宏定义
来源：http://hz.yueranfly.top/gtasimdbsc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.meibo888.top/gtkgzvnryj.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtfavchqxm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtyhilowzc.html

[S15] C：类型转换
来源：http://hz.ivvv.top/gtwamlnxkz.html

(double) a / b
来源：http://hz.hywenlv.cn/gtatxporlc.html

[S16] C：位操作置位
来源：http://hz.hysaishi.cn/gtuicqcbdo.html

x |= (1 << 3);
来源：http://hz.jinqigufen.top/gtapechuib.html

[S17] C：安全拼接字符串
来源：http://hz.bjfxy.top/gtviiopehh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnxiangtu.top/gtngsbztbz.html

[S18] C：命令行参数
来源：http://hz.shangyingyoupin.top/gtwlxzwqcl.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtovmhljdj.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtkngydpkr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtxeporfwu.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtchrbknrh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtccpidesa.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gtdknkdeln.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.birdmap.top/gtkcvkmagn.html

[S22] C：字符串转数字
来源：http://hz.shangyingyoupin.top/gtzxwlltud.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aibaodan.cn/gtqwtjukqv.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtxprxzttx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtdjsbqnpa.html

[S24] C：获取本地时间
来源：http://hz.zhaomingkeji.xyz/gtbdmgrbpf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtuaorseey.html

[S25] C：内存拷贝
来源：http://hz.hnqzz.top/gtnpfajfzu.html

memcpy(dst, src, n);
来源：http://hz.yueranfly.top/gtepilrsfn.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtbtoizpcv.html

memset(a, 0, sizeof a);
来源：http://hz.zhongyouzk.top/gtiekscpxf.html

[S27] C：定义常量
来源：http://hz.xuetiantiany.cn/gtzbmpvdkh.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtckgirsvi.html

[S28] C：静态变量
来源：http://hz.jianghu66.top/gttjhnohex.html

static int counter = 0;
来源：http://hz.yj20258.top/gtghgklswn.html

[S29] C：变参函数
来源：http://hz.ybcxt.top/gthtkrbtus.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guowangkeji.top/gtlpoggptj.html

[S30] C：头文件保护
来源：http://hz.aibaodan.cn/gtzkhxsirv.html

#ifndef X_H
来源：http://hz.aizwys.cn/gtngqcgcvl.html

#define X_H
来源：http://hz.chenlongwang.top/gtlrfbivde.html

#endif
来源：http://hz.ppjwa.cn/gtrfppisos.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gttjtmsunp.html

#include <iostream>
来源：http://hz.shuidangran.top/gtltsppnej.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtvwfrcqpc.html

[S32] C++：字符串
来源：http://hz.jqgfzy.top/gtbvvtafvi.html

std::string s = "hi";  s += "!";
来源：http://hz.cheryme.top/gtbplhlpzb.html

[S33] C++：vector 增删
来源：http://hz.sweek.top/gtlubzomba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nwbrower.top/gtaukrnohp.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gttiepturn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenjidiqi.icu/gtzvmgeipw.html

[S35] C++：map
来源：http://hz.yongpay.top/gtduzgmbxf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtzmedovtn.html

[S36] C++：unordered_map
来源：http://hz.yj202588.top/gtrvgplzzp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gttuyfjtgq.html

[S37] C++：set
来源：http://hz.andypj.xyz/gtzrezfxmf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtolowvqva.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtqemizvpn.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtdvpppdpg.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtyzubtaaz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtnodurorp.html

[S40] C++：查找元素
来源：http://hz.pycfn.com/gtgjzcrewi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenlongwang.top/gtwkiemrhb.html

[S41] C++：类与构造函数
来源：http://hz.dashuyun.cn/gtdnskfjgp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtfdgownom.html

[S42] C++：继承与虚函数
来源：http://hz.gaohongyu789.top/gteobwugpm.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtuoocmztf.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangtech.top/gtfkgljezv.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtojgtvgpl.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gtcemnpjtd.html

void inc(int &x) { ++x; }
来源：http://hz.mhx1999.top/gtucsbmjkc.html

[S45] C++：lambda
来源：http://hz.jqgfzy.top/gttxlbivlu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.quarkkingdee.top/gtfqdiboao.html

[S46] C++：函数模板
来源：http://hz.chenlongwang.top/gtwkvvchde.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sweek.top/gtpznosram.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtdvrvzemr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zycfv.cn/gtpubtshky.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gtjrppkzqb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxinkj.top/gtolqnzbxn.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtwngkrerq.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtglqktihw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxinkj.top/gtemrqfqlh.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtofvbahdp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gtawupgiza.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtiohdiwxa.html

static_cast<double>(a) / b
来源：http://hz.yuxming.cn/gtmlpbuksy.html

[S52] C++：const 与 noexcept
来源：http://hz.shuidangran.top/gtuwtugjmf.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangkeji.top/gtscvqpojv.html

[S53] C++：移动语义
来源：http://hz.gzhubu.top/gtcmlxmgwj.html

std::vector<int> w = std::move(v);
来源：http://hz.xinyue.icu/gtprxombey.html

[S54] C++：异常处理
来源：http://hz.hysaishi.cn/gthdyitdhg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jiagoushi.top/gtxbrynljv.html

[S55] C++：结构化绑定
来源：http://hz.jiagoushi.top/gtcztjuqjc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guannengcc.top/gtvuaftosa.html

[S56] C++：optional
来源：http://hz.ydzc1.top/gtetlhsbwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gtdpfxkcqo.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gtpwkxjszv.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtpfybbwjv.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtlucftwtz.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtsowkgfur.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gthqzahsxg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtlgvqknlx.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtplbattyx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gtpsrebvty.html

================================================================================
来源：http://hz.daxiang520.top/gtoggtkoyj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gtauywnzby.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfdmbigru.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtzmmslyjr.html

println("Hello")
来源：http://hz.cheryme.top/gtyrizsbri.html

[T02] Kotlin：变量
来源：http://hz.tanke756.top/gtuuhjkwut.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtlnyhiath.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtyubtowmz.html

"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtftepvkov.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gthtfjsokx.html

val n: String? = null;  n?.length
来源：http://hz.yangfankeji.com/gtkgsdilvw.html

[T05] Kotlin：when 表达式
来源：http://hz.dashuyun.cn/gtdgtacedk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtrbkyzpsq.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtdxkkejrx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jyoumei.cn/gtgkzjbymi.html

[T07] Kotlin：集合过滤
来源：http://hz.hfpthk.cn/gtddyoexkr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtrdqmvoaw.html

[T08] Kotlin：数据类
来源：http://hz.0kj1m.cn/gtasgyzkdg.html

data class User(val name: String, val age: Int)
来源：http://hz.yj20258.top/gtpzoujacn.html

[T09] Kotlin：扩展函数
来源：http://hz.ehwqpu.com/gtcbreupix.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gttsiceeku.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtcwsfuawi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuxming.cn/gtascxposq.html

[T11] Kotlin：协程
来源：http://hz.cqqwz.cn/gtfkubjkxj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hammf.cn/gtidmhoori.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gtusljdjzu.html

val (a, b) = Pair(1, 2)
来源：http://hz.ehwqpu.com/gterpvkwyz.html

[T13] Kotlin：只读 Map
来源：http://hz.jlsjyb.cn/gtboyjlbyj.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtpqxadxrz.html

[T14] Kotlin：循环
来源：http://hz.tanke756.top/gtenkvwgnh.html

for (i in 1..10) println(i)
来源：http://hz.0kj1m.cn/gtdpdlyvnj.html

[T15] Kotlin：接口
来源：http://hz.jinqigufen.top/gtnfsuryyz.html

interface Shape { fun area(): Double }
来源：http://hz.ydzc1.top/gtiuwpalgw.html

[T16] Swift：Hello World
来源：http://hz.yonumen.top/gteelgjbab.html

print("Hello")
来源：http://hz.chenzaomai.com/gthkoobjjl.html

[T17] Swift：变量与常量
来源：http://hz.jianghu66.top/gtiasbrxqo.html

var a = 1;  let b = 2
来源：http://hz.gaohongyu789.top/gtzhvlrkhz.html

[T18] Swift：字符串插值
来源：http://hz.andypj.xyz/gtydjeobjb.html

"值: \(b)"
来源：http://hz.ybcxt.top/gtimxnkukh.html

[T19] Swift：可选绑定
来源：http://hz.vqdsnc.cn/gtnqsdatha.html

if let n = opt { print(n) }
来源：http://hz.yangfankeji.com/gtvtgzsqqh.html

[T20] Swift：数组操作
来源：http://hz.ppjwa.cn/gtoldahtjh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenzaomai.com/gtfbsgrurs.html

[T21] Swift：遍历
来源：http://hz.jiagoushi.top/gthhncbbkh.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtlmxkfdbw.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gterxggiof.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gteeknvkue.html

[T23] Swift：函数
来源：http://hz.chenlongwang.top/gtxrxmeqyc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.meibo888.top/gtytdcvfcc.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gtfcqevfks.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtzmbjiqfp.html

[T25] Swift：结构体
来源：http://hz.daria6918.cn/gtuwvwaazx.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtqcgqzluo.html

[T26] Swift：类与重写
来源：http://hz.hammf.cn/gtjtvshhhx.html

class A: Base { override func f() {} }
来源：http://hz.c1oappe.top/gtnzgtehjo.html

[T27] Swift：错误处理
来源：http://hz.bjfxy.top/gtchmrypqq.html

do { try f() } catch { print(error) }
来源：http://hz.svipenyu.cn/gtynensbrc.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtyvgcthai.html

enum Color { case red, green }
来源：http://hz.316326.xyz/gtqgmrqcjf.html

[T29] Swift：guard 提前返回
来源：http://hz.zhixingplan.top/gtynrkjgfd.html

guard let x = opt else { return }
来源：http://hz.cheryme.top/gtghlasrtb.html

[T30] Swift：协议
来源：http://hz.pycfn.com/gtvoqhcwdi.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtaiyleuid.html

[T31] Lua：Hello World
来源：http://hz.zhiwuduotai.top/gthrabxpcf.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtgsjghafq.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtmomvyaay.html

local a = 1
来源：http://hz.hnxiangtu.top/gtapvhlitl.html

[T33] Lua：表（数组）
来源：http://hz.nwbrower.top/gtcsqacvra.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhiwuduotai.top/gtrzucqkae.html

[T34] Lua：遍历表
来源：http://hz.fzhhl.top/gtlirohpre.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yonumen.top/gtfqxsskgz.html

[T35] Lua：字典表
来源：http://hz.yj20258888.top/gtsbupxgzb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhiwuduotai.top/gtbuhrvjte.html

[T36] Lua：函数
来源：http://hz.hywenlv.cn/gtoliwehwz.html

function add(a, b) return a + b end
来源：http://hz.xuanzx.com/gtcriankvm.html

[T37] Lua：字符串拼接
来源：http://hz.wangshuangyany.cn/gticfzgacz.html

"a" .. "b"
来源：http://hz.shangyingyoupin.top/gtohmlncku.html

[T38] Lua：条件
来源：http://hz.redwolf501.top/gtyclqldar.html

if x > 0 then print("正") end
来源：http://hz.chenjidiqi.icu/gtivkdxiwd.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtrujfhvmo.html

string.find(s, "%d+")
来源：http://hz.nanxuanxn.top/gtdxsarrmy.html

[T40] Lua：元表
来源：http://hz.pycfn.com/gtyzvxyjmp.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigfzy.top/gtazvismzy.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gtqxlsoxyk.html

print "Hello\n";
来源：http://hz.kuanghao11.cn/gtvsqqjdse.html

[T42] Perl：变量类型
来源：http://hz.dashuyun.cn/gtjppuvzfr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hnqzz.top/gttnuvsqzb.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtpeerokzp.html

"值: $a"
来源：http://hz.zhengqikj.top/gtjxcbdlth.html

[T44] Perl：条件
来源：http://hz.xuanzx.com/gthgadhlfu.html

if ($a > 0) { print "正"; }
来源：http://hz.yueranfly.top/gtxgqtlfif.html

[T45] Perl：数组遍历
来源：http://hz.ydzc1.top/gtbrijxedq.html

for my $x (@arr) { print $x; }
来源：http://hz.aizwys.cn/gtbkoqezhm.html

[T46] Perl：哈希操作
来源：http://hz.shanyushiyangtech.top/gtmhfdzqsm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cucudq.cn/gtugbnxjeu.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtmqqmbcjd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.quarkkingdee.top/gtgjoyfhbu.html

[T48] Perl：正则替换
来源：http://hz.nanxinkj.top/gtkwxmrsjo.html

$s =~ s/old/new/g;
来源：http://hz.yuanzhike.top/gttitgpmzw.html

[T49] Perl：函数
来源：http://hz.wangdashe.top/gtnxwbecxw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.bjfxy.top/gttaurxymu.html

[T50] Perl：逐行读文件
来源：http://hz.guowangkeji.top/gtcssshoqk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yonumen.top/gtsngtbvot.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tianlin.xyz/gtktiocrjz.html

[T51] Scala：Hello World
来源：http://hz.yongpay.top/gtrnlxqtgt.html

println("Hello")
来源：http://hz.tianlin.xyz/gtadyzdhwp.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gtfghyozhr.html

val a = 1;  var b = 2
来源：http://hz.smart0.xyz/gtfgmkuapv.html

[T53] Scala：字符串插值
来源：http://hz.jinqigufen.top/gtueiowyzc.html

s"值: $b"
来源：http://hz.birdmap.top/gtepefvjpu.html

[T54] Scala：集合映射
来源：http://hz.kuanghao11.cn/gtnlwayebc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gaohongyu789.top/gtmkcicknz.html

[T55] Scala：集合过滤
来源：http://hz.0kj1m.cn/gtbqgcfnfo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258888.top/gtmzofwlwf.html

[T56] Scala：样例类
来源：http://hz.zhiwuduotai.top/gtngdafoal.html

case class User(name: String, age: Int)
来源：http://hz.nanxuanxn.top/gtgobomzmt.html

[T57] Scala：模式匹配
来源：http://hz.birdmap.top/gtqyuerrox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daxiang520.top/gtuktjyvyz.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtfirxcevg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aibaodan.cn/gtjygfmdjr.html

[T59] Scala：循环
来源：http://hz.gotoacloud.top/gtdvfakwkv.html

for (i <- 1 to 10) println(i)
来源：http://hz.jlsjyb.cn/gtsgydfpkf.html

[T60] Scala：折叠
来源：http://hz.nanxuanxn.top/gtlqrmxkjp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnxiangtu.top/gtntiseidn.html

================================================================================
来源：http://hz.jinqigufen.top/gtcjbhxhfo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gtmbfoajbz.html

================================================================================
来源：http://hz.sweek.top/gtavqyurcw.html

[U01] Py：创建虚拟环境
来源：http://hz.havefunace.top/gtthlnqxjo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zdqjudy.top/gtjbaahueo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tianlin.xyz/gtktvvlvxa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yangfankeji.com/gtrozjoyoa.html

[U03] Py：加载 .env 配置
来源：http://hz.nanxinkj.top/gtxgtwfois.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nanxuanxn.top/gtckwyvniz.html

[U04] Py：变量调试打印
来源：http://hz.yonumen.top/gtlbdnbsyx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nwbrower.top/gtrgdouwot.html

[U05] Py：列表去重且保序
来源：http://hz.nanxinkj.top/gtxpopnouh.html

list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtrmagxkeo.html

[U06] Py：合并两个字典
来源：http://hz.vqdsnc.cn/gtbiqzewzm.html

{**a, **b}
来源：http://hz.hnqzz.top/gtojlmhovy.html

[U07] Py：反转字典键值
来源：http://hz.gzhubu.top/gtkexfxsvr.html

{v: k for k, v in d.items()}
来源：http://hz.jinyuanbaomall.cn/gtcbloljmu.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtarneiqlm.html

[y for x in nested for y in x]
来源：http://hz.zhixingplan.top/gtfexnqbgm.html

[U09] Py：字典取最大值的键
来源：http://hz.yuxming.cn/gtjzuopwec.html

max(d, key=d.get)
来源：http://hz.shanyushiyangtech.top/gtpgwuxbfy.html

[U10] Py：按值排序字典
来源：http://hz.zhaomingkeji.xyz/gtthrucfgn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gtyrrwevuo.html

[U11] Py：生成器表达式
来源：http://hz.feifeiyinyue.top/gtamgsqawu.html

(x * 2 for x in arr)
来源：http://hz.jlsjyb.cn/gtvlafaujq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtafrralad.html

Counter(arr).most_common(3)
来源：http://hz.wangshuangyany.cn/gtbtmqgjgl.html

[U13] Py：固定长度队列
来源：http://hz.chenzaomai.com/gtkajkgmso.html

deque(maxlen=10)
来源：http://hz.zhoulong.xyz/gtnnsqnefu.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtjyqkwxja.html

defaultdict(list)
来源：http://hz.shanyushiyangkeji.top/gtpdiehamq.html

[U15] Py：高精度计时
来源：http://hz.tianlin.xyz/gtnjrnmjxj.html

t = time.perf_counter()
来源：http://hz.snrcjt.cn/gtltswqsix.html

[U16] Py：命令行参数解析
来源：http://hz.zhaomingkeji.xyz/gtrtdxlwwz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gotoacloud.top/gtivdhsdip.html

[U17] Py：初始化日志
来源：http://hz.cucudq.cn/gtrqfswtis.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jlsjyb.cn/gtvibikrxk.html

[U18] Py：预编译正则
来源：http://hz.hammf.cn/gtwajdrzas.html

pat = re.compile(r"\d+")
来源：http://hz.yj202588.top/gtnaxoxuvr.html

[U19] Py：正则替换带回调
来源：http://hz.aibaodan.cn/gtocmzwpfr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtjpcwbeaf.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigfzy.top/gtvzqsmckr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenlongwang.top/gtclbqrrii.html

[U21] Py：自定义上下文管理器
来源：http://hz.sufxvd.cn/gtnqytwgnx.html

@contextlib.contextmanager
来源：http://hz.shzxlz.cn/gtprozthuo.html

[U22] Py：矩阵转置
来源：http://hz.jinqigufen.top/gtznjlcyzr.html

list(zip(*m))
来源：http://hz.iojbl.cn/gtjyvqaslo.html

[U23] Py：分块读取大文件
来源：http://hz.shangyingyoupin.top/gtepyoucyp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guannengcc.top/gthuuikvxp.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangkeji.top/gtcdpviisz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtygmeyzhe.html

[U25] Py：CSV 按字典读
来源：http://hz.hywenlv.cn/gtmuradxan.html

csv.DictReader(f)
来源：http://hz.cqqwz.cn/gtifktalwq.html

[U26] Py：并发下载
来源：http://hz.yongpay.top/gtodqtqvmw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cqqwz.cn/gtehduiwmc.html

[U27] Py：异步 HTTP
来源：http://hz.zycfv.cn/gtxzjgnppg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.mhx1999.top/gtasyicigj.html

[U28] Py：类型别名
来源：http://hz.zhongyouzk.top/gtwlgulgtx.html

UserId = int
来源：http://hz.c1oappe.top/gtqlktgbvc.html


<!-- 参考信息 -->