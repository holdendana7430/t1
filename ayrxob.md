代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtnjuyrypd.html

[S02] C：变量与格式化输出
来源：http://hz.dianchejie.cn/gtuhcudbvc.html

int a = 10; printf("%d\n", a);
来源：http://hz.aizwys.cn/gtditcdzjx.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtjfnfspdq.html

int x; scanf("%d", &x);
来源：http://hz.guannengcc.top/gtdirabjlv.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gtjjxmbhwu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daxiang520.top/gtanrecqyp.html

[S05] C：字符串长度
来源：http://hz.hongshengwenyu.top/gtnyjxlaco.html

strlen(s)
来源：http://hz.yuanzhike.top/gtqcugiypd.html

[S06] C：字符串比较
来源：http://hz.tanke756.top/gtzkbklpil.html

strcmp(a, b) == 0
来源：http://hz.hysaishi.cn/gtfcmskrzb.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtgutczbfj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtdgwpcxou.html

[S08] C：动态内存分配与释放
来源：http://hz.kuanghao11.cn/gtbpulontg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxinkj.top/gtobeztecc.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gtaepqbqsa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuxming.cn/gtsatkzfcj.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtxibtzlru.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtalypmhux.html

[S11] C：逐行读文件
来源：http://hz.chenlongwang.top/gtmfouxwzf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhixingplan.top/gtzesoztde.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gtuqmuqcbu.html

fclose(f);
来源：http://hz.jianghu66.top/gtscpcbsis.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtbiqbeqaw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangshuangyany.cn/gtdgrgnwuu.html

[S13] C：宏定义
来源：http://hz.jlsjyb.cn/gtexlbhyvc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dashuyun.cn/gtrsmyrtst.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtfstxpjte.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gtbtbceiqr.html

[S15] C：类型转换
来源：http://hz.gaohongyu789.top/gttqwcrjxw.html

(double) a / b
来源：http://hz.birdmap.top/gtfohauqam.html

[S16] C：位操作置位
来源：http://hz.cqqwz.cn/gtmwojhyuh.html

x |= (1 << 3);
来源：http://hz.mhx1999.top/gtclffjild.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtgengurdb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuanzx.com/gtfxdnwtvq.html

[S18] C：命令行参数
来源：http://hz.cqqwz.cn/gtrpevnerg.html

int main(int argc, char **argv)
来源：http://hz.hongshengwenyu.top/gtltzecugx.html

[S19] C：快速排序
来源：http://hz.pycfn.com/gtsssqgeqb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtaakmyhtu.html

[S20] C：二分查找
来源：http://hz.dianchejie.cn/gtfjamderm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtmonigmvk.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangkeji.top/gtycuebepu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigufen.top/gtejnblias.html

[S22] C：字符串转数字
来源：http://hz.yj202588.top/gthhfshmaj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gttszvjnyq.html

[S23] C：随机数
来源：http://hz.sysykeji.top/gtpemarczr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dianchejie.cn/gtlweylfyw.html

[S24] C：获取本地时间
来源：http://hz.daria6918.cn/gtwiitfatk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtnwiyldze.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtknlkvfnv.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gteuhlvykq.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtdzinisbp.html

memset(a, 0, sizeof a);
来源：http://hz.hnqzz.top/gtuggvfnpn.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtufuljrxl.html

const double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtbynoukhe.html

[S28] C：静态变量
来源：http://hz.cashguo.top/gtgfspldom.html

static int counter = 0;
来源：http://hz.jinqigufen.top/gtyhvsppkz.html

[S29] C：变参函数
来源：http://hz.hongshengwenyu.top/gtvdgsglgq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtrzjtsfmq.html

[S30] C：头文件保护
来源：http://hz.gotoacloud.top/gtoklkgsjl.html

#ifndef X_H
来源：http://hz.haohaochexian.top/gtsmtnhetc.html

#define X_H
来源：http://hz.fzhhl.top/gtgmsvlrtm.html

#endif
来源：http://hz.bjfxy.top/gtqeopsvax.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtzzoutcbj.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtnhmehgej.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydjk.org.cn/gtsqwjlayz.html

[S32] C++：字符串
来源：http://hz.hnxiangtu.top/gtrwwpnhdo.html

std::string s = "hi";  s += "!";
来源：http://hz.zhengqikj.top/gtchiazshu.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtnljtzhhq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtaxtcatit.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtnechnbdd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sxryk.cn/gtwfhqtdcl.html

[S35] C++：map
来源：http://hz.hywenlv.cn/gtwjrweaoa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtnfizmdbw.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtwegspwho.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gthcgavjod.html

[S37] C++：set
来源：http://hz.yvedp.cn/gteaqfczah.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yonumen.top/gtevefdngh.html

[S38] C++：排序
来源：http://hz.zhiwuduotai.top/gtcvyuqdjr.html

std::sort(v.begin(), v.end());
来源：http://hz.sufxvd.cn/gtixwnrxsk.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtdthnxagj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.iojbl.cn/gtfhhenujb.html

[S40] C++：查找元素
来源：http://hz.havefunace.top/gtzzzdnfeu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nwbrower.top/gtdxvtoqiw.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtjakqytki.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gteovtdiez.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtcjwvgmzp.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtpbidfqej.html

[S43] C++：智能指针
来源：http://hz.hnxiangtu.top/gtoqjucdga.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtbzkcbnnh.html

[S44] C++：引用传参
来源：http://hz.guannengcc.top/gtmjcfrgxp.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtvqcsjvrp.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtfleojcsu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj202588.top/gtuioplscf.html

[S46] C++：函数模板
来源：http://hz.yuanzhike.top/gtynpixodn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.316326.xyz/gtniqvqlvg.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gtcxfvmyto.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtnfvwjhyn.html

[S48] C++：逐行读文件
来源：http://hz.gzhubu.top/gtgzlqedgj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenzaomai.com/gtgbtyrvkx.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtahpfccqk.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtdrgkksio.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pycfn.com/gtzouowogl.html

[S50] C++：格式化数字
来源：http://hz.hongshengwenyu.top/gttusewofq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtflsvyqdc.html

[S51] C++：显式类型转换
来源：http://hz.zhoulong.xyz/gtyorbgxhz.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gtezsbnkdg.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtrlddptko.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtqnlwvtgz.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gthkvaqbru.html

std::vector<int> w = std::move(v);
来源：http://hz.gzhubu.top/gtnmhyypya.html

[S54] C++：异常处理
来源：http://hz.jlsjyb.cn/gtkhdjiumi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gotoacloud.top/gtnuwrtiyp.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtagdcqdvv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtkfokxvmn.html

[S56] C++：optional
来源：http://hz.c1oappe.top/gtpbehfhdz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.52xcode.cn/gtjldtzran.html

[S57] C++：编译期常量
来源：http://hz.316326.xyz/gtnvkvzdpw.html

constexpr int N = 10;
来源：http://hz.xingfuxueyuan.xyz/gtncfygjao.html

[S58] C++：命名空间
来源：http://hz.zdqjudy.top/gtxcfnwwun.html

namespace ns { int f() { return 1; } }
来源：http://hz.andypj.xyz/gtaqocwivm.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtzzelbvjk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhijiandao.cn/gtbizwtjrc.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtqkkrjiac.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hywenlv.cn/gtjgateuke.html

================================================================================
来源：http://hz.wangdashe.top/gtyeenynkm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gthcwnsbzh.html

================================================================================
来源：http://hz.guannengcc.top/gtgiehfdiz.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtgcpydfir.html

println("Hello")
来源：http://hz.yvedp.cn/gtxqauipnt.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtcbzivmqy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtwovftvyn.html

[T03] Kotlin：字符串模板
来源：http://hz.9152youxi.cn/gtcihggcgq.html

"值: $b"
来源：http://hz.ybcxt.top/gtnsnjmswe.html

[T04] Kotlin：空安全
来源：http://hz.c1oappe.top/gtciqxtnxd.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtkepqoitm.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtanrmwllu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tian-w.cn/gtusyacaqi.html

[T06] Kotlin：集合映射
来源：http://hz.jiagoushi.top/gtkwkmnfbs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.316326.xyz/gtslmsrxns.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtcidgbbgm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hongshengwenyu.top/gthttxzcdq.html

[T08] Kotlin：数据类
来源：http://hz.shangyingyoupin.top/gtmnzhiszn.html

data class User(val name: String, val age: Int)
来源：http://hz.hammf.cn/gtqdflgycf.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtyrkiaaxy.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gtccbwtyht.html

[T10] Kotlin：默认参数
来源：http://hz.gotoacloud.top/gtpyiehqlr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258888.top/gtjydfaxvu.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtdezinela.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258.top/gtkmxmiabp.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gtmttjamsu.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gttpztuxoo.html

[T13] Kotlin：只读 Map
来源：http://hz.ehwqpu.com/gttysxssas.html

val m = mapOf("a" to 1)
来源：http://hz.ydjk.org.cn/gtpjaitbzo.html

[T14] Kotlin：循环
来源：http://hz.zhiwuduotai.top/gtdfbbepzv.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtwvfnsqje.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gtdvwhzeaq.html

interface Shape { fun area(): Double }
来源：http://hz.quarkkingdee.top/gtfnaqaqys.html

[T16] Swift：Hello World
来源：http://hz.daria6918.cn/gttelepuro.html

print("Hello")
来源：http://hz.hammf.cn/gttspnsiho.html

[T17] Swift：变量与常量
来源：http://hz.yj20258.top/gtimhqrpnb.html

var a = 1;  let b = 2
来源：http://hz.jyoumei.cn/gtapojzpvc.html

[T18] Swift：字符串插值
来源：http://hz.daxiang520.top/gtxzdqvqki.html

"值: \(b)"
来源：http://hz.shangyingyoupin.top/gttugrllcu.html

[T19] Swift：可选绑定
来源：http://hz.gaohongyu789.top/gtgzosbbiz.html

if let n = opt { print(n) }
来源：http://hz.zhoulong.xyz/gtunozcwsy.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gteoqwnhuc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtcgijvtke.html

[T21] Swift：遍历
来源：http://hz.fengsongda.top/gtndztcmyo.html

for x in a { print(x) }
来源：http://hz.xylfe.cn/gtrrzlpobv.html

[T22] Swift：字典
来源：http://hz.jinghuilouyu.cn/gtrqjibynm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.smart0.xyz/gtwitiizwp.html

[T23] Swift：函数
来源：http://hz.yuanzhike.top/gtxgyuspkz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sysykeji.top/gtqefizrat.html

[T24] Swift：闭包
来源：http://hz.hywenlv.cn/gtztwyvtpr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtlzyfwnna.html

[T25] Swift：结构体
来源：http://hz.xylfe.cn/gtswabemdb.html

struct P { var x: Int }
来源：http://hz.yangfankeji.com/gtyxwbbexl.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangtech.top/gtmxygocfp.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtbldqfifs.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtehiipuqj.html

do { try f() } catch { print(error) }
来源：http://hz.hongshengwenyu.top/gtcxetjwsk.html

[T28] Swift：枚举
来源：http://hz.yj20258888.top/gtlmplictd.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtfsojgkhb.html

[T29] Swift：guard 提前返回
来源：http://hz.jlsjyb.cn/gtbsrrewok.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtssecaffh.html

[T30] Swift：协议
来源：http://hz.havefunace.top/gtqxkxycvb.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgfzy.top/gtdioecfzb.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtejochdth.html

print("Hello")
来源：http://hz.hammf.cn/gtajkdxhmt.html

[T32] Lua：局部变量
来源：http://hz.ydzc1.top/gtvubxmkjs.html

local a = 1
来源：http://hz.xinyue.icu/gthyotxtno.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtisuyijsg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuxming.cn/gtcxgpkljy.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtqelvrbhr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj20258.top/gtpaluqwai.html

[T35] Lua：字典表
来源：http://hz.sxryk.cn/gtqihrrlcn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pengpengdd.cyou/gtdolvihpe.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gttfxkcirx.html

function add(a, b) return a + b end
来源：http://hz.yvedp.cn/gtwqrzdidi.html

[T37] Lua：字符串拼接
来源：http://hz.chenzaomai.com/gthtbzapth.html

"a" .. "b"
来源：http://hz.daria6918.cn/gtsmogrlzy.html

[T38] Lua：条件
来源：http://hz.xingfuxueyuan.xyz/gtpwsftmdj.html

if x > 0 then print("正") end
来源：http://hz.c1oappe.top/gtrjfqqqhr.html

[T39] Lua：模式匹配
来源：http://hz.jyoumei.cn/gtmizqizoe.html

string.find(s, "%d+")
来源：http://hz.tianlin.xyz/gttkntalwv.html

[T40] Lua：元表
来源：http://hz.svipenyu.cn/gtfxkhrbdo.html

setmetatable({}, { __index = base })
来源：http://hz.wangdashe.top/gtdgwumbzm.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gtxqfsatwg.html

print "Hello\n";
来源：http://hz.pycfn.com/gtmziemheq.html

[T42] Perl：变量类型
来源：http://hz.cashguo.top/gtrbysbxvt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.wangdashe.top/gtgsxstfvu.html

[T43] Perl：字符串插值
来源：http://hz.chenlongwang.top/gttiupmomj.html

"值: $a"
来源：http://hz.birdmap.top/gtttmvnvjk.html

[T44] Perl：条件
来源：http://hz.iojbl.cn/gtzhgooqvk.html

if ($a > 0) { print "正"; }
来源：http://hz.cdnleiting.top/gtaxuofjds.html

[T45] Perl：数组遍历
来源：http://hz.cheryme.top/gtcsutelxd.html

for my $x (@arr) { print $x; }
来源：http://hz.dashuyun.cn/gtqugmmbca.html

[T46] Perl：哈希操作
来源：http://hz.wangdashe.top/gtskttftqv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ivvv.top/gtpgrzmtdt.html

[T47] Perl：正则捕获
来源：http://hz.gotoacloud.top/gtqeiptavi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenjidiqi.icu/gtyuntojoa.html

[T48] Perl：正则替换
来源：http://hz.xziqi.cn/gtmrznwklk.html

$s =~ s/old/new/g;
来源：http://hz.feifeiyinyue.top/gtebmrnwhh.html

[T49] Perl：函数
来源：http://hz.ppjwa.cn/gtbgzshrzf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.0kj1m.cn/gtdzwzvlvz.html

[T50] Perl：逐行读文件
来源：http://hz.xuanzx.com/gtwhodvtip.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.316326.xyz/gtfymsnolc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuetiantiany.cn/gtzknxkyel.html

[T51] Scala：Hello World
来源：http://hz.gogol.net.cn/gtezdircgp.html

println("Hello")
来源：http://hz.gogol.net.cn/gtgifftkvo.html

[T52] Scala：变量
来源：http://hz.gotoacloud.top/gtxnrfvrzy.html

val a = 1;  var b = 2
来源：http://hz.cqqwz.cn/gtzghnbstj.html

[T53] Scala：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtxjomqfee.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtxrfrflyu.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gthjxrpppz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yvedp.cn/gtnyaibxhd.html

[T55] Scala：集合过滤
来源：http://hz.yuanzhike.top/gtbqzpoqai.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydjk.org.cn/gtfwmnzdny.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtogjtkigb.html

case class User(name: String, age: Int)
来源：http://hz.ehwqpu.com/gtfprmbpau.html

[T57] Scala：模式匹配
来源：http://hz.kuanghao11.cn/gtltvhcfzg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.mhx1999.top/gttzbjtcxd.html

[T58] Scala：函数定义
来源：http://hz.hammf.cn/gtlmieuhmb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ehwqpu.com/gtqvleqswc.html

[T59] Scala：循环
来源：http://hz.zhaomingkeji.xyz/gtgnehhert.html

for (i <- 1 to 10) println(i)
来源：http://hz.0kj1m.cn/gteaeazdct.html

[T60] Scala：折叠
来源：http://hz.yj202588.top/gtajamqsea.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtzqsinnah.html

================================================================================
来源：http://hz.jiagoushi.top/gtxciksxhf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtlpirtkvo.html

================================================================================
来源：http://hz.jyoumei.cn/gtzvpdbcpu.html

[U01] Py：创建虚拟环境
来源：http://hz.dashuyun.cn/gtuproniiu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.redwolf501.top/gtgwovzozf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhijiandao.cn/gtwwqttprl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtvaqbjqib.html

[U03] Py：加载 .env 配置
来源：http://hz.jinghuilouyu.cn/gtcbfismmv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtfrbttszr.html

[U04] Py：变量调试打印
来源：http://hz.jianghu66.top/gthqnomgmb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yonumen.top/gtjippabni.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gttmwglyig.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gttzisqjut.html

[U06] Py：合并两个字典
来源：http://hz.hammf.cn/gttrklgysh.html

{**a, **b}
来源：http://hz.jiagoushi.top/gtvyzwjdsc.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtwmoesrtp.html

{v: k for k, v in d.items()}
来源：http://hz.vqdsnc.cn/gthdwbtzlh.html

[U08] Py：展平二维列表
来源：http://hz.gogol.net.cn/gtgghejajj.html

[y for x in nested for y in x]
来源：http://hz.quarkkingdee.top/gtubrnpdkm.html

[U09] Py：字典取最大值的键
来源：http://hz.jyoumei.cn/gtowylflnu.html

max(d, key=d.get)
来源：http://hz.wangshuangyany.cn/gtmodvrnjj.html

[U10] Py：按值排序字典
来源：http://hz.daxiang520.top/gtsahffnhy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.haohaochexian.top/gtfagvrfdr.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtowljnici.html

(x * 2 for x in arr)
来源：http://hz.pycfn.com/gthrtnaebs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hywenlv.cn/gtjlnyrpxd.html

Counter(arr).most_common(3)
来源：http://hz.dashuyun.cn/gtjvzcijzl.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtdvgsfhij.html

deque(maxlen=10)
来源：http://hz.hongshengwenyu.top/gtniwngkqd.html

[U14] Py：分组收集到列表
来源：http://hz.zhongyouzk.top/gtifimfiaj.html

defaultdict(list)
来源：http://hz.jinghuilouyu.cn/gtrvmjyala.html

[U15] Py：高精度计时
来源：http://hz.wangshuangyany.cn/gtivhkinjj.html

t = time.perf_counter()
来源：http://hz.sweek.top/gtkktkwtbx.html

[U16] Py：命令行参数解析
来源：http://hz.pycfn.com/gtxkmcowiu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jianghu66.top/gtjhtknemi.html

[U17] Py：初始化日志
来源：http://hz.snrcjt.cn/gtigpgnjid.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hnxiangtu.top/gtxlhkbgmx.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gtqjhvkgbb.html

pat = re.compile(r"\d+")
来源：http://hz.xuanzx.com/gthefywbry.html

[U19] Py：正则替换带回调
来源：http://hz.0kj1m.cn/gttrphxnss.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gogol.net.cn/gtkqtwlsrm.html

[U20] Py：缓存函数结果
来源：http://hz.jinyuanbaomall.cn/gtsryjvggx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.iojbl.cn/gtslshrdym.html

[U21] Py：自定义上下文管理器
来源：http://hz.mhx1999.top/gtjwsuxmwh.html

@contextlib.contextmanager
来源：http://hz.bjfxy.top/gtummtrmdp.html

[U22] Py：矩阵转置
来源：http://hz.wangshuangyany.cn/gtcaivwctp.html

list(zip(*m))
来源：http://hz.gogol.net.cn/gtnbtcuwos.html

[U23] Py：分块读取大文件
来源：http://hz.aizwys.cn/gtudbxwixg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.smart0.xyz/gtaebruxyq.html

[U24] Py：路径操作
来源：http://hz.yonumen.top/gtbugaeflc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.redwolf501.top/gtzrnnoutb.html


<!-- 参考信息 -->