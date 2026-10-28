代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ehwqpu.com/gtslgkpjtu.html

[S02] C：变量与格式化输出
来源：http://hz.ivvv.top/gttrviwamq.html

int a = 10; printf("%d\n", a);
来源：http://hz.fengsongda.top/gtairzfxpp.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtdrbjzlfp.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gthmjljxjt.html

[S04] C：字符串复制
来源：http://hz.jqgfzy.top/gtymciymfk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtojgxsfks.html

[S05] C：字符串长度
来源：http://hz.cdnleiting.top/gtbxntwhpn.html

strlen(s)
来源：http://hz.daxiang520.top/gtyhtsylis.html

[S06] C：字符串比较
来源：http://hz.daxiang520.top/gtiquxczov.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gtuvpqbstw.html

[S07] C：数组遍历求和
来源：http://hz.jinyuanbaomall.cn/gtvwbtuooo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhoulong.xyz/gtbsifhpxb.html

[S08] C：动态内存分配与释放
来源：http://hz.havefunace.top/gteaablgrv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jlsjyb.cn/gtyflvgqpk.html

[S09] C：结构体定义与初始化
来源：http://hz.havefunace.top/gtfhuuppgt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hammf.cn/gtowrfwwgx.html

[S10] C：指针与解引用
来源：http://hz.sysykeji.top/gtfeemysqn.html

int *p = &a;  *p = 5;
来源：http://hz.wangshuangyany.cn/gtzwsoetsp.html

[S11] C：逐行读文件
来源：http://hz.ybcxt.top/gtikrsyuup.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gttlybqeed.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cucudq.cn/gtlondvomw.html

fclose(f);
来源：http://hz.gaohongyu789.top/gtuzoczeyc.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gtkrncdnjf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnqzz.top/gtuestfvgg.html

[S13] C：宏定义
来源：http://hz.redwolf501.top/gtqzfbfeyd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtpyptqilm.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gtckfjjyou.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tianlin.xyz/gtefhwlqgp.html

[S15] C：类型转换
来源：http://hz.gaohongyu789.top/gtsrmtarzt.html

(double) a / b
来源：http://hz.yuanzhike.top/gtihogftnp.html

[S16] C：位操作置位
来源：http://hz.yj20258.top/gtbtyvonxx.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gtwihetpaj.html

[S17] C：安全拼接字符串
来源：http://hz.chenjidiqi.icu/gttbtihxaj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtaxahovmx.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtinvwbywr.html

int main(int argc, char **argv)
来源：http://hz.zhaomingkeji.xyz/gtddakvnmr.html

[S19] C：快速排序
来源：http://hz.ydzc1.top/gtoeemhidp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtcqxxnnxt.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtpbnqoyaa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtxkjgmurr.html

[S21] C：字符类别判断
来源：http://hz.dashuyun.cn/gtlhlaxauz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtypwztkpy.html

[S22] C：字符串转数字
来源：http://hz.andypj.xyz/gtcbxajyfd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtooawvpna.html

[S23] C：随机数
来源：http://hz.dashuyun.cn/gttnggiera.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtqnkqbpnl.html

[S24] C：获取本地时间
来源：http://hz.cdnleiting.top/gtyhfgwkni.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtllwqhgcx.html

[S25] C：内存拷贝
来源：http://hz.cdnleiting.top/gtgqkrknni.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtqrnokrkt.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtisitmzfh.html

memset(a, 0, sizeof a);
来源：http://hz.zhengqikj.top/gtwmtrgtjk.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtllqldgsc.html

const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtgawlpcvf.html

[S28] C：静态变量
来源：http://hz.yj20258888.top/gtlwkqxofr.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtuntirbdt.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gtudoqdfxo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtkxdmdtih.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtbzydluoe.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gtzkohnazn.html

#define X_H
来源：http://hz.daria6918.cn/gtrzqaqvab.html

#endif
来源：http://hz.sysykeji.top/gtyutrcaoo.html

[S31] C++：Hello World
来源：http://hz.wangshuangyany.cn/gtkcankdwm.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtdwelsgbf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.andypj.xyz/gtypnkvffs.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gttpmvcaly.html

std::string s = "hi";  s += "!";
来源：http://hz.ybcxt.top/gtmskvcqmm.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtkkudapbc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtlsmsrjdo.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtqsgkmhul.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.mhx1999.top/gtilcmzvve.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtdiuseuyu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtfukvansl.html

[S36] C++：unordered_map
来源：http://hz.ydjk.org.cn/gtyrvrksoi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtwtzqlxrn.html

[S37] C++：set
来源：http://hz.nwbrower.top/gttzdjcwrp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gotoacloud.top/gtfkmpbtzd.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtqhsbztyj.html

std::sort(v.begin(), v.end());
来源：http://hz.fengsongda.top/gtzootzobo.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtptsbeteq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.quarkkingdee.top/gthenolzcm.html

[S40] C++：查找元素
来源：http://hz.xziqi.cn/gtngmadqmh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtccavlfiz.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtczjgxhty.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gtjbqnfuwn.html

[S42] C++：继承与虚函数
来源：http://hz.tanke756.top/gtqmyroolc.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnxiangtu.top/gthutprhsl.html

[S43] C++：智能指针
来源：http://hz.yuxming.cn/gtnwgfvquq.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtvkgfuzoc.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtvowofvdv.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gtkasdjmoy.html

[S45] C++：lambda
来源：http://hz.shzxlz.cn/gtzbffzlmr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtfnbedkzz.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gtllujpjex.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.snrcjt.cn/gtjzldlldl.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtleqgghad.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aibaodan.cn/gtwvsrczul.html

[S48] C++：逐行读文件
来源：http://hz.zycfv.cn/gtafbyidcr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtkiputyyc.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gtggpzptcw.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gtuttewavr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gtcbqttgvo.html

[S50] C++：格式化数字
来源：http://hz.yvedp.cn/gtqtligrcq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gtxwgehyaa.html

[S51] C++：显式类型转换
来源：http://hz.redwolf501.top/gtzoxypgjs.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gttubxjulg.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxinkj.top/gtlastjtdv.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtzeblpfrt.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtnsjijton.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtyvmbgavq.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtjzehyopq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtsnhbkysu.html

[S55] C++：结构化绑定
来源：http://hz.redwolf501.top/gtnpvhybcy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.redwolf501.top/gtwvnvlstb.html

[S56] C++：optional
来源：http://hz.hfpthk.cn/gtjvyckpqm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258888.top/gtxwnvoirb.html

[S57] C++：编译期常量
来源：http://hz.xinyue.icu/gtxuibfblk.html

constexpr int N = 10;
来源：http://hz.9152youxi.cn/gtvfsuxxig.html

[S58] C++：命名空间
来源：http://hz.0kj1m.cn/gttematdhg.html

namespace ns { int f() { return 1; } }
来源：http://hz.birdmap.top/gtslkatnln.html

[S59] C++：静态断言
来源：http://hz.ywan-chungtsiang.top/gtyftztigs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenlongwang.top/gtdlonspij.html

[S60] C++：遍历并删除元素
来源：http://hz.yangfankeji.com/gtmehszaqe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.smart0.xyz/gtpfnzdwtz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtuyvocect.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtqffjrboj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtuhtjhkwd.html

[T01] Kotlin：Hello World
来源：http://hz.guannengcc.top/gttbsnqneq.html

println("Hello")
来源：http://hz.hnqzz.top/gtygocrjbh.html

[T02] Kotlin：变量
来源：http://hz.c1oappe.top/gtxzzumisn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.iojbl.cn/gtlayupszn.html

[T03] Kotlin：字符串模板
来源：http://hz.vqdsnc.cn/gtouqobkub.html

"值: $b"
来源：http://hz.xinyue.icu/gtnsywsgrp.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gtxaqrunpe.html

val n: String? = null;  n?.length
来源：http://hz.hfpthk.cn/gtzpnyngtq.html

[T05] Kotlin：when 表达式
来源：http://hz.kuanghao11.cn/gtxuspzqil.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hammf.cn/gtmjjtktqd.html

[T06] Kotlin：集合映射
来源：http://hz.tianlin.xyz/gtukqnhvcv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ivvv.top/gttdpnvyit.html

[T07] Kotlin：集合过滤
来源：http://hz.gaohongyu789.top/gtdtitwzzl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.dianchejie.cn/gtfwgzlanf.html

[T08] Kotlin：数据类
来源：http://hz.wangdashe.top/gtibjdftwj.html

data class User(val name: String, val age: Int)
来源：http://hz.daxiang520.top/gtiqoiaijr.html

[T09] Kotlin：扩展函数
来源：http://hz.9152youxi.cn/gtrsugdrpe.html

fun String.exclaim() = this + "!"
来源：http://hz.zhaomingkeji.xyz/gtamwcarhi.html

[T10] Kotlin：默认参数
来源：http://hz.ybcxt.top/gteytqryph.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jlsjyb.cn/gtdungzgsu.html

[T11] Kotlin：协程
来源：http://hz.wangdashe.top/gtclcmrjjd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gtowfgqtyc.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangtech.top/gtssqxxrmd.html

val (a, b) = Pair(1, 2)
来源：http://hz.meibo888.top/gtmeibwemi.html

[T13] Kotlin：只读 Map
来源：http://hz.xuanzx.com/gttwfbhzvw.html

val m = mapOf("a" to 1)
来源：http://hz.yj202588.top/gtfvsubfca.html

[T14] Kotlin：循环
来源：http://hz.bjfxy.top/gtajoymgkz.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtjqhzuhmy.html

[T15] Kotlin：接口
来源：http://hz.chenzaomai.com/gtlnqhwgjc.html

interface Shape { fun area(): Double }
来源：http://hz.nwbrower.top/gthashjtmt.html

[T16] Swift：Hello World
来源：http://hz.ppjwa.cn/gtjjwijvnh.html

print("Hello")
来源：http://hz.guowangkeji.top/gtzdfhglvt.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtskzjlrkb.html

var a = 1;  let b = 2
来源：http://hz.cqqwz.cn/gtgddruiaj.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtgrsedpco.html

"值: \(b)"
来源：http://hz.nanxuanxn.top/gtbfmijube.html

[T19] Swift：可选绑定
来源：http://hz.jyoumei.cn/gtmwgabztx.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtnjrhgres.html

[T20] Swift：数组操作
来源：http://hz.fzhhl.top/gtqbgaitgw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gtogahxkha.html

[T21] Swift：遍历
来源：http://hz.nanxinkj.top/gtidilronb.html

for x in a { print(x) }
来源：http://hz.chenjidiqi.icu/gtcgyfezly.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtodwmkrgz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangtech.top/gtjbcjlibk.html

[T23] Swift：函数
来源：http://hz.0kj1m.cn/gteteapulg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.52xcode.cn/gtpyxegzyc.html

[T24] Swift：闭包
来源：http://hz.dashuyun.cn/gtavgkuvyj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gthpytjazp.html

[T25] Swift：结构体
来源：http://hz.ywan-chungtsiang.top/gtttearrya.html

struct P { var x: Int }
来源：http://hz.pengpengdd.cyou/gtummzlrhy.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gtarectsuy.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gtxyzfxrjs.html

[T27] Swift：错误处理
来源：http://hz.yj20258888.top/gtxyqemnbn.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangtech.top/gtztizxhlb.html

[T28] Swift：枚举
来源：http://hz.gotoacloud.top/gtywmhsrtk.html

enum Color { case red, green }
来源：http://hz.yonumen.top/gtfnbonurm.html

[T29] Swift：guard 提前返回
来源：http://hz.bjfxy.top/gtpadxzexd.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtchfxslvl.html

[T30] Swift：协议
来源：http://hz.ivvv.top/gtsanuukvn.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtfkirkdcw.html

[T31] Lua：Hello World
来源：http://hz.mhx1999.top/gtnmjbflpy.html

print("Hello")
来源：http://hz.cashguo.top/gtymgprrio.html

[T32] Lua：局部变量
来源：http://hz.jqgfzy.top/gthojecplp.html

local a = 1
来源：http://hz.hfpthk.cn/gtjgjfuqqw.html

[T33] Lua：表（数组）
来源：http://hz.xinyue.icu/gtetdiqhiq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtzsugwgji.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtcvcogykz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nwbrower.top/gtrtjkbvng.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gttxuhhanh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtcdwrzxrd.html

[T36] Lua：函数
来源：http://hz.yangfankeji.com/gtnuxgtmbb.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtyacqlude.html

[T37] Lua：字符串拼接
来源：http://hz.sufxvd.cn/gtrrmifhmo.html

"a" .. "b"
来源：http://hz.ivvv.top/gtzadxwpyv.html

[T38] Lua：条件
来源：http://hz.yj20258.top/gtcgcrzruo.html

if x > 0 then print("正") end
来源：http://hz.jqgfzy.top/gtjntvjvhm.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtjgjnqmyz.html

string.find(s, "%d+")
来源：http://hz.cqqwz.cn/gtmyztkatg.html

[T40] Lua：元表
来源：http://hz.quarkkingdee.top/gtbkxqkurn.html

setmetatable({}, { __index = base })
来源：http://hz.jqgufenzy.top/gtghtumykm.html

[T41] Perl：Hello World
来源：http://hz.0kj1m.cn/gtolnpwvxm.html

print "Hello\n";
来源：http://hz.guannengcc.top/gttuhiylgh.html

[T42] Perl：变量类型
来源：http://hz.hysaishi.cn/gtfniirdnx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.vqdsnc.cn/gtozadonee.html

[T43] Perl：字符串插值
来源：http://hz.zhijiandao.cn/gtamjcnogk.html

"值: $a"
来源：http://hz.tianlin.xyz/gtbuoluglq.html

[T44] Perl：条件
来源：http://hz.cdnleiting.top/gtqmovtfix.html

if ($a > 0) { print "正"; }
来源：http://hz.hammf.cn/gtvsuzothp.html

[T45] Perl：数组遍历
来源：http://hz.yuanzhike.top/gthpetwtiq.html

for my $x (@arr) { print $x; }
来源：http://hz.chenlongwang.top/gtehebyvtl.html

[T46] Perl：哈希操作
来源：http://hz.yuanzhike.top/gthiqsodah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtezlcdsou.html

[T47] Perl：正则捕获
来源：http://hz.hongshengwenyu.top/gtceaywxco.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtvhtkclht.html

[T48] Perl：正则替换
来源：http://hz.guowangkeji.top/gtaqybbsvc.html

$s =~ s/old/new/g;
来源：http://hz.jinyuanbaomall.cn/gtvqwyhnio.html

[T49] Perl：函数
来源：http://hz.jianghu66.top/gtfncsdafe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.pycfn.com/gtgjzygbxc.html

[T50] Perl：逐行读文件
来源：http://hz.shzxlz.cn/gtzsovnhig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xingfuxueyuan.xyz/gtoovlxbic.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daxiang520.top/gtywsaxsuo.html

[T51] Scala：Hello World
来源：http://hz.svipenyu.cn/gtqjmscfae.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtavdgqjbm.html

[T52] Scala：变量
来源：http://hz.jinyuanbaomall.cn/gtxmscqbky.html

val a = 1;  var b = 2
来源：http://hz.guowangkeji.top/gtttpwbidw.html

[T53] Scala：字符串插值
来源：http://hz.fengsongda.top/gtisziovwm.html

s"值: $b"
来源：http://hz.andypj.xyz/gtqrdbxeuz.html

[T54] Scala：集合映射
来源：http://hz.hongshengwenyu.top/gtcewusojh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhaomingkeji.xyz/gtqkrxikir.html

[T55] Scala：集合过滤
来源：http://hz.nanxuanxn.top/gtuqixlqzw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ppjwa.cn/gtjumsdoxj.html

[T56] Scala：样例类
来源：http://hz.kuanghao11.cn/gtftyolmwq.html

case class User(name: String, age: Int)
来源：http://hz.tianlin.xyz/gtmrgcfhfs.html

[T57] Scala：模式匹配
来源：http://hz.pycfn.com/gtpicckljw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cqqwz.cn/gtptscdinp.html

[T58] Scala：函数定义
来源：http://hz.dashuyun.cn/gtuwgqtpzh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zdqjudy.top/gtttrhlphb.html

[T59] Scala：循环
来源：http://hz.ppjwa.cn/gtqbhbbcmk.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtbrtdtpqg.html

[T60] Scala：折叠
来源：http://hz.chenlongwang.top/gtimnabayu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.c1oappe.top/gthjaipgsw.html

================================================================================
来源：http://hz.gotoacloud.top/gtpfepvgla.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtgbqxhxtj.html

================================================================================
来源：http://hz.yangfankeji.com/gtlocqgaqt.html

[U01] Py：创建虚拟环境
来源：http://hz.yanxiufei.cn/gtcjstjqep.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtvqsnkpoa.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gtvswyvtlr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shuidangran.top/gtitgiilwh.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtlbriaqgf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.feifeiyinyue.top/gttkbhialh.html

[U04] Py：变量调试打印
来源：http://hz.zhixingplan.top/gtfexxctcz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.52xcode.cn/gtsyqtaavb.html

[U05] Py：列表去重且保序
来源：http://hz.sweek.top/gtdbjtquei.html

list(dict.fromkeys(arr))
来源：http://hz.pycfn.com/gtmnybyyku.html

[U06] Py：合并两个字典
来源：http://hz.shzxlz.cn/gtltzxhwyy.html

{**a, **b}
来源：http://hz.aibaodan.cn/gtrsfosmag.html

[U07] Py：反转字典键值
来源：http://hz.tian-w.cn/gtpfgeszrq.html

{v: k for k, v in d.items()}
来源：http://hz.wangdashe.top/gtycqchfgb.html

[U08] Py：展平二维列表
来源：http://hz.52xcode.cn/gtkdohhthu.html

[y for x in nested for y in x]
来源：http://hz.andypj.xyz/gtlrijnuum.html

[U09] Py：字典取最大值的键
来源：http://hz.birdmap.top/gtugdftsal.html

max(d, key=d.get)
来源：http://hz.tianlin.xyz/gtsnjucbmj.html

[U10] Py：按值排序字典
来源：http://hz.yueranfly.top/gtykehwuqk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gtgoeqhzcw.html

[U11] Py：生成器表达式
来源：http://hz.hongshengwenyu.top/gtstwbzcnt.html

(x * 2 for x in arr)
来源：http://hz.meibo888.top/gtqwjwqczq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gaohongyu789.top/gtjmmvoauw.html

Counter(arr).most_common(3)
来源：http://hz.c1oappe.top/gtkjnotnaz.html

[U13] Py：固定长度队列
来源：http://hz.sufxvd.cn/gteouzmsjt.html

deque(maxlen=10)
来源：http://hz.316326.xyz/gtdhjgcuph.html

[U14] Py：分组收集到列表
来源：http://hz.dianchejie.cn/gtvderdfhh.html

defaultdict(list)
来源：http://hz.xinyue.icu/gtpogikvkt.html

[U15] Py：高精度计时
来源：http://hz.cheryme.top/gtkgruhldp.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gtrcueouok.html

[U16] Py：命令行参数解析
来源：http://hz.jinqigufen.top/gtcvpcsiir.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigfzy.top/gtpzrlarej.html

[U17] Py：初始化日志
来源：http://hz.fengsongda.top/gtcsuqhnih.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinqigfzy.top/gtbxsvztse.html

[U18] Py：预编译正则
来源：http://hz.hnqzz.top/gtinczrklb.html

pat = re.compile(r"\d+")
来源：http://hz.tianlin.xyz/gtpfyvwjot.html

[U19] Py：正则替换带回调
来源：http://hz.cdnleiting.top/gttolwtcfl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.0kj1m.cn/gtuoazybad.html

[U20] Py：缓存函数结果
来源：http://hz.yuanzhike.top/gthipsqbfe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yueranfly.top/gtdyjxugkm.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gtgdccadsl.html

@contextlib.contextmanager
来源：http://hz.ivvv.top/gttciwadau.html

[U22] Py：矩阵转置
来源：http://hz.guowangkeji.top/gtbufwvfkp.html

list(zip(*m))
来源：http://hz.yangfankeji.com/gtgzgvvzgn.html

[U23] Py：分块读取大文件
来源：http://hz.hongshengwenyu.top/gtpinfckwo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangkeji.top/gtfqvcmkxr.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtwhzmxghc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sufxvd.cn/gttwrrjjub.html


<!-- 参考信息 -->