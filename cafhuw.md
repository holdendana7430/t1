代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aizwys.cn/gtnsmbvprd.html

[S02] C：变量与格式化输出
来源：http://hz.c1oappe.top/gtjwqdcuhy.html

int a = 10; printf("%d\n", a);
来源：http://hz.cashguo.top/gtcbumzugk.html

[S03] C：读入整数
来源：http://hz.chenzaomai.com/gtmivsuaim.html

int x; scanf("%d", &x);
来源：http://hz.tian-w.cn/gtrsysyjeu.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtpigmvows.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.316326.xyz/gteuguwyue.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtkovurbvt.html

strlen(s)
来源：http://hz.0kj1m.cn/gtfhnxevoc.html

[S06] C：字符串比较
来源：http://hz.ppjwa.cn/gtqwdhluot.html

strcmp(a, b) == 0
来源：http://hz.ywan-chungtsiang.top/gtonpilttu.html

[S07] C：数组遍历求和
来源：http://hz.kuanghao11.cn/gtaqnyvkui.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.9152youxi.cn/gtflwxkksn.html

[S08] C：动态内存分配与释放
来源：http://hz.snrcjt.cn/gtlcmanbqy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gtrljeyvtw.html

[S09] C：结构体定义与初始化
来源：http://hz.hnxiangtu.top/gtbxhdhnho.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtepchdntg.html

[S10] C：指针与解引用
来源：http://hz.ivvv.top/gtaqusxtbz.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtklohtrck.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtykuxfztn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenlongwang.top/gtdswnfzli.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ywan-chungtsiang.top/gtdalrraen.html

fclose(f);
来源：http://hz.jianghu66.top/gtsrhpnmiz.html

[S12] C：写文件
来源：http://hz.9152youxi.cn/gtlkzgsbts.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gotoacloud.top/gtrgjxcfck.html

[S13] C：宏定义
来源：http://hz.tian-w.cn/gtlfnkrwka.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtomqjafqb.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gtausbjnxr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.snrcjt.cn/gtvksojrcj.html

[S15] C：类型转换
来源：http://hz.jyoumei.cn/gtgeofwnex.html

(double) a / b
来源：http://hz.iojbl.cn/gtqxnhnhgs.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gtzaelaklv.html

x |= (1 << 3);
来源：http://hz.dianchejie.cn/gtaxzuzlzt.html

[S17] C：安全拼接字符串
来源：http://hz.zhengqikj.top/gtgfnlcbrv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gtddfbyguz.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtcovomsqg.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtqdjkfpdu.html

[S19] C：快速排序
来源：http://hz.shanyushiyangkeji.top/gtkyyulyvy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtuivscjcq.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gttxyurylt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtmrxpaimr.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtqhhfllsa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.fengsongda.top/gtvkocsngw.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtnngnofpc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtrlqyajuk.html

[S23] C：随机数
来源：http://hz.cqqwz.cn/gtmfnejoaz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jiagoushi.top/gtxukylmmk.html

[S24] C：获取本地时间
来源：http://hz.yj202588.top/gtkbrfyowy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xylfe.cn/gtdsszagsq.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gttlrqojyn.html

memcpy(dst, src, n);
来源：http://hz.nwbrower.top/gtvnozjqke.html

[S26] C：内存清零
来源：http://hz.yonumen.top/gtszileeqo.html

memset(a, 0, sizeof a);
来源：http://hz.jinghuilouyu.cn/gthaujohqm.html

[S27] C：定义常量
来源：http://hz.shuidangran.top/gtaqmivnhy.html

const double PI = 3.14159;
来源：http://hz.haohaochexian.top/gtxwzdienm.html

[S28] C：静态变量
来源：http://hz.sysykeji.top/gtnaqwjkxb.html

static int counter = 0;
来源：http://hz.zdqjudy.top/gtrzzxgpyl.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gttltorfxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigfzy.top/gtuymtkhei.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtqvzlqwhy.html

#ifndef X_H
来源：http://hz.ivvv.top/gtiuuzyjme.html

#define X_H
来源：http://hz.shuidangran.top/gtpdmfvnrs.html

#endif
来源：http://hz.ybcxt.top/gtouffitxs.html

[S31] C++：Hello World
来源：http://hz.jiagoushi.top/gtpjpviczk.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtendncuue.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yanxiufei.cn/gtestuidbd.html

[S32] C++：字符串
来源：http://hz.xziqi.cn/gtnavblggo.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtpunkmizs.html

[S33] C++：vector 增删
来源：http://hz.pengpengdd.cyou/gtcndlghnx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.0kj1m.cn/gtfratleli.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtrfvkgegh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.vqdsnc.cn/gtzducrzdl.html

[S35] C++：map
来源：http://hz.ehwqpu.com/gtuahsbwam.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuxming.cn/gtgwdjpyqy.html

[S36] C++：unordered_map
来源：http://hz.xuetiantiany.cn/gtpfpgjejw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtkdlwkwcr.html

[S37] C++：set
来源：http://hz.hfpthk.cn/gtljaybuff.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gtesrusrth.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtduspxswh.html

std::sort(v.begin(), v.end());
来源：http://hz.zhongyouzk.top/gtzkvddfyl.html

[S39] C++：自定义比较器排序
来源：http://hz.jiagoushi.top/gtwdmvuxbf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuanzhike.top/gtijechnhs.html

[S40] C++：查找元素
来源：http://hz.hongshengwenyu.top/gtvshufozx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yueranfly.top/gtpwuobsbl.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gtuwbbmwwq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gtzwymhsbu.html

[S42] C++：继承与虚函数
来源：http://hz.zhongyouzk.top/gthiwbyukp.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtaewnppor.html

[S43] C++：智能指针
来源：http://hz.mhx1999.top/gtgoepwput.html

auto p = std::make_unique<int>(5);
来源：http://hz.jiagoushi.top/gtmrncigor.html

[S44] C++：引用传参
来源：http://hz.yuxming.cn/gtzphbtvqw.html

void inc(int &x) { ++x; }
来源：http://hz.redwolf501.top/gtrimfdthw.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gtufmszbjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pengpengdd.cyou/gtocgjgezf.html

[S46] C++：函数模板
来源：http://hz.xylfe.cn/gtghwrbpcl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cucudq.cn/gthziijuvz.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtlwvvtuib.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gteoibrlxz.html

[S48] C++：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtgoeulqzz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tianlin.xyz/gthlcbzwmb.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gteamkmbhi.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtyhztvupv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.havefunace.top/gtrzvvphqy.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtnixwmxey.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtdujmhlmg.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gtjhaulxke.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtpyffinoi.html

[S52] C++：const 与 noexcept
来源：http://hz.pycfn.com/gtkqgmzgmh.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtfzkqcsah.html

[S53] C++：移动语义
来源：http://hz.sxryk.cn/gtwlrnozcz.html

std::vector<int> w = std::move(v);
来源：http://hz.fzhhl.top/gtlifvusat.html

[S54] C++：异常处理
来源：http://hz.ivvv.top/gtfzdozbwt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cashguo.top/gtxgkpmjbo.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gttzebqapw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gtlrjnqtpy.html

[S56] C++：optional
来源：http://hz.c1oappe.top/gtxvmzrhpj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.0kj1m.cn/gtgwqjsbrl.html

[S57] C++：编译期常量
来源：http://hz.dianchejie.cn/gtwfxmvyhb.html

constexpr int N = 10;
来源：http://hz.tanke756.top/gttcwldyrz.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gtwhjnhtrx.html

namespace ns { int f() { return 1; } }
来源：http://hz.tanke756.top/gtawxrumlg.html

[S59] C++：静态断言
来源：http://hz.fzhhl.top/gtrlnllkxv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtftfnapcc.html

[S60] C++：遍历并删除元素
来源：http://hz.nwbrower.top/gtjgptgmmz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zdqjudy.top/gtswbwkgix.html

================================================================================
来源：http://hz.cheryme.top/gtlwxnrmyd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydjk.org.cn/gtzblshzds.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyyjpkost.html

[T01] Kotlin：Hello World
来源：http://hz.fengsongda.top/gtncurgnsg.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtvuvyaggu.html

[T02] Kotlin：变量
来源：http://hz.cdnleiting.top/gtcxmcegdh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hongshengwenyu.top/gtnodvpbso.html

[T03] Kotlin：字符串模板
来源：http://hz.svipenyu.cn/gtnngrdkzb.html

"值: $b"
来源：http://hz.yj202588.top/gtwcuxcejk.html

[T04] Kotlin：空安全
来源：http://hz.yj20258.top/gtvvyfvqeh.html

val n: String? = null;  n?.length
来源：http://hz.nwbrower.top/gtvzuowxum.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gtlkbvwbrb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtxoemniuq.html

[T06] Kotlin：集合映射
来源：http://hz.quarkkingdee.top/gtiyiiyayd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.redwolf501.top/gtjzaqoywr.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gtwkukziat.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgufenzy.top/gtfgvkjrrs.html

[T08] Kotlin：数据类
来源：http://hz.zhaomingkeji.xyz/gtvzbgokbf.html

data class User(val name: String, val age: Int)
来源：http://hz.yuanzhike.top/gtlutnqbms.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gttlqghyun.html

fun String.exclaim() = this + "!"
来源：http://hz.svipenyu.cn/gtlqwuvuby.html

[T10] Kotlin：默认参数
来源：http://hz.hysaishi.cn/gtmlsylmcl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtljocvefw.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtqgddkdtv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuetiantiany.cn/gtbstofpvz.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtsglmvauy.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtvmbbhsbs.html

[T13] Kotlin：只读 Map
来源：http://hz.chenzaomai.com/gtbeqvshlf.html

val m = mapOf("a" to 1)
来源：http://hz.iojbl.cn/gtxvxgluky.html

[T14] Kotlin：循环
来源：http://hz.xingfuxueyuan.xyz/gtkylfboeh.html

for (i in 1..10) println(i)
来源：http://hz.pengpengdd.cyou/gtfhuvkbzi.html

[T15] Kotlin：接口
来源：http://hz.xylfe.cn/gteurnchqa.html

interface Shape { fun area(): Double }
来源：http://hz.cheryme.top/gtojjtuyiw.html

[T16] Swift：Hello World
来源：http://hz.yuxming.cn/gtqaapvzuy.html

print("Hello")
来源：http://hz.tian-w.cn/gtszjgdrgb.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtftcjmvfj.html

var a = 1;  let b = 2
来源：http://hz.sysykeji.top/gtmlvjryck.html

[T18] Swift：字符串插值
来源：http://hz.gzhubu.top/gtllshmdny.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtzjjscbnc.html

[T19] Swift：可选绑定
来源：http://hz.yj202588.top/gtsbkftlta.html

if let n = opt { print(n) }
来源：http://hz.jinqigfzy.top/gtbrnuevkv.html

[T20] Swift：数组操作
来源：http://hz.redwolf501.top/gtzgicchjn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgfzy.top/gtfpqqvwem.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gtggronciy.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtatvbbycg.html

[T22] Swift：字典
来源：http://hz.daxiang520.top/gtktsckgiu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gotoacloud.top/gtgwkemkjc.html

[T23] Swift：函数
来源：http://hz.xuanzx.com/gtqfgjrajo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnxiangtu.top/gtmtouemtb.html

[T24] Swift：闭包
来源：http://hz.ehwqpu.com/gtxatyoeao.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cdnleiting.top/gtvznpqpwt.html

[T25] Swift：结构体
来源：http://hz.52xcode.cn/gtfaseutmi.html

struct P { var x: Int }
来源：http://hz.jqgufenzy.top/gtstbkggrk.html

[T26] Swift：类与重写
来源：http://hz.9152youxi.cn/gtwkdnqtro.html

class A: Base { override func f() {} }
来源：http://hz.sxryk.cn/gtdunxbjit.html

[T27] Swift：错误处理
来源：http://hz.jqgufenzy.top/gtpnqpvbvd.html

do { try f() } catch { print(error) }
来源：http://hz.dashuyun.cn/gthmiguvwc.html

[T28] Swift：枚举
来源：http://hz.daxiang520.top/gttxetvbfz.html

enum Color { case red, green }
来源：http://hz.ywan-chungtsiang.top/gtbcbmljla.html

[T29] Swift：guard 提前返回
来源：http://hz.nanxuanxn.top/gtkhptrrkw.html

guard let x = opt else { return }
来源：http://hz.52xcode.cn/gtfevddhfh.html

[T30] Swift：协议
来源：http://hz.yj20258.top/gtgvsvhptn.html

protocol Shape { func area() -> Double }
来源：http://hz.hywenlv.cn/gtroavkqim.html

[T31] Lua：Hello World
来源：http://hz.tanke756.top/gtmpnhoxnf.html

print("Hello")
来源：http://hz.zhongyouzk.top/gttdudrtex.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtrieewfcv.html

local a = 1
来源：http://hz.shzxlz.cn/gtnwplenmv.html

[T33] Lua：表（数组）
来源：http://hz.jlsjyb.cn/gtbwshcamg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.fzhhl.top/gtzgrwqgqd.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtynpfhdas.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtzbvmccrw.html

[T35] Lua：字典表
来源：http://hz.birdmap.top/gtjtvkhfea.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtozczmeoc.html

[T36] Lua：函数
来源：http://hz.zhaomingkeji.xyz/gtmdemxirb.html

function add(a, b) return a + b end
来源：http://hz.snrcjt.cn/gtwqlaryzp.html

[T37] Lua：字符串拼接
来源：http://hz.mhx1999.top/gtzvytyqzv.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtqhswbpnn.html

[T38] Lua：条件
来源：http://hz.gotoacloud.top/gtonkdkgiy.html

if x > 0 then print("正") end
来源：http://hz.fengsongda.top/gtatfgqbhi.html

[T39] Lua：模式匹配
来源：http://hz.shuidangran.top/gtyntsshkk.html

string.find(s, "%d+")
来源：http://hz.hywenlv.cn/gtcjgcqyog.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtnwvomgvj.html

setmetatable({}, { __index = base })
来源：http://hz.hywenlv.cn/gthwpuruwh.html

[T41] Perl：Hello World
来源：http://hz.ywan-chungtsiang.top/gtejsvflto.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtszbptwqg.html

[T42] Perl：变量类型
来源：http://hz.0kj1m.cn/gthtdgngha.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xylfe.cn/gtoimzeytw.html

[T43] Perl：字符串插值
来源：http://hz.snrcjt.cn/gtmivhbxln.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtkgnuoqej.html

[T44] Perl：条件
来源：http://hz.cucudq.cn/gtnebagser.html

if ($a > 0) { print "正"; }
来源：http://hz.hysaishi.cn/gtckjwfdpp.html

[T45] Perl：数组遍历
来源：http://hz.wangshuangyany.cn/gtnofgpfsk.html

for my $x (@arr) { print $x; }
来源：http://hz.zhaomingkeji.xyz/gtyifbmjtx.html

[T46] Perl：哈希操作
来源：http://hz.jinqigfzy.top/gtvpnahucy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.daria6918.cn/gtqdwjxakd.html

[T47] Perl：正则捕获
来源：http://hz.yangfankeji.com/gtfieuutzq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuanzx.com/gtcgshhkpi.html

[T48] Perl：正则替换
来源：http://hz.aizwys.cn/gtomnvfsds.html

$s =~ s/old/new/g;
来源：http://hz.yonumen.top/gtqifqdbcz.html

[T49] Perl：函数
来源：http://hz.kuanghao11.cn/gtxhnbskjb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gaohongyu789.top/gtqejdflls.html

[T50] Perl：逐行读文件
来源：http://hz.sysykeji.top/gtzzdcuyip.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtyywwuvfw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ivvv.top/gtkypahsfa.html

[T51] Scala：Hello World
来源：http://hz.pycfn.com/gtatqmfbvg.html

println("Hello")
来源：http://hz.ppjwa.cn/gtseavpegp.html

[T52] Scala：变量
来源：http://hz.52xcode.cn/gtfugwfito.html

val a = 1;  var b = 2
来源：http://hz.haohaochexian.top/gtfyqxtzmm.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtxadfykiq.html

s"值: $b"
来源：http://hz.haohaochexian.top/gtnorzoqhf.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtbfwcqham.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinyuanbaomall.cn/gtazlpxjby.html

[T55] Scala：集合过滤
来源：http://hz.cashguo.top/gtrzjeixpn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hongshengwenyu.top/gtgufgqjre.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangtech.top/gthnapozxq.html

case class User(name: String, age: Int)
来源：http://hz.bjfxy.top/gttrmngxka.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtrpepzrbr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hammf.cn/gtlplarxca.html

[T58] Scala：函数定义
来源：http://hz.ywan-chungtsiang.top/gtnxvyvain.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.mhx1999.top/gtylzbkflc.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gtuyzastjd.html

for (i <- 1 to 10) println(i)
来源：http://hz.ehwqpu.com/gtqqiniopv.html

[T60] Scala：折叠
来源：http://hz.meibo888.top/gtjbwotqbf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gzhubu.top/gtdknbmhwf.html

================================================================================
来源：http://hz.daxiang520.top/gtbrmgpnay.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxinkj.top/gtnixnjnzo.html

================================================================================
来源：http://hz.daria6918.cn/gthvigpafb.html

[U01] Py：创建虚拟环境
来源：http://hz.meibo888.top/gtbkkjsxcd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shangyingyoupin.top/gtsizkkvso.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtgytkxqri.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.9152youxi.cn/gteyvpoztq.html

[U03] Py：加载 .env 配置
来源：http://hz.kuanghao11.cn/gtnywlhpne.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dashuyun.cn/gtnxcjtgjm.html

[U04] Py：变量调试打印
来源：http://hz.pycfn.com/gtsesroyza.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gogol.net.cn/gtawnmihlz.html

[U05] Py：列表去重且保序
来源：http://hz.svipenyu.cn/gtohpylwet.html

list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtcqvqvcnc.html

[U06] Py：合并两个字典
来源：http://hz.snrcjt.cn/gtuqjotyji.html

{**a, **b}
来源：http://hz.xingfuxueyuan.xyz/gtftkshidm.html

[U07] Py：反转字典键值
来源：http://hz.hammf.cn/gtpoyjwnsb.html

{v: k for k, v in d.items()}
来源：http://hz.aibaodan.cn/gtnsqmqtzf.html

[U08] Py：展平二维列表
来源：http://hz.birdmap.top/gtwvpaeaeq.html

[y for x in nested for y in x]
来源：http://hz.dianchejie.cn/gtijevylpf.html

[U09] Py：字典取最大值的键
来源：http://hz.feifeiyinyue.top/gtacymiari.html

max(d, key=d.get)
来源：http://hz.guowangkeji.top/gtegnfwoxr.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtscnkcoib.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.316326.xyz/gtqkjgceqt.html

[U11] Py：生成器表达式
来源：http://hz.meibo888.top/gtrquysodr.html

(x * 2 for x in arr)
来源：http://hz.chenlongwang.top/gtcvjeyqyc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hammf.cn/gtktwxgzya.html

Counter(arr).most_common(3)
来源：http://hz.0kj1m.cn/gtqanetwva.html

[U13] Py：固定长度队列
来源：http://hz.pycfn.com/gtqrxwiyvl.html

deque(maxlen=10)
来源：http://hz.wangdashe.top/gtrehnvsbv.html

[U14] Py：分组收集到列表
来源：http://hz.ppjwa.cn/gtdzcaeyma.html

defaultdict(list)
来源：http://hz.shuidangran.top/gtsngwqhfi.html

[U15] Py：高精度计时
来源：http://hz.nanxuanxn.top/gtierublxg.html

t = time.perf_counter()
来源：http://hz.gzhubu.top/gttebopchd.html

[U16] Py：命令行参数解析
来源：http://hz.0kj1m.cn/gtlldyvhwz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tianlin.xyz/gtekmwwznp.html

[U17] Py：初始化日志
来源：http://hz.iojbl.cn/gttmxmjofe.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gtmszbipkr.html

[U18] Py：预编译正则
来源：http://hz.ehwqpu.com/gtpjgphfsd.html

pat = re.compile(r"\d+")
来源：http://hz.pengpengdd.cyou/gtklcxpugm.html

[U19] Py：正则替换带回调
来源：http://hz.chenjidiqi.icu/gteuxjbkbm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinqigufen.top/gtxsuworct.html

[U20] Py：缓存函数结果
来源：http://hz.fzhhl.top/gthhbjymzm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sxryk.cn/gtmjszwkhr.html

[U21] Py：自定义上下文管理器
来源：http://hz.52xcode.cn/gtzvzjjkrr.html

@contextlib.contextmanager
来源：http://hz.guannengcc.top/gttggvpnhh.html

[U22] Py：矩阵转置
来源：http://hz.hammf.cn/gtjxfsjnny.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtbkxkqnti.html

[U23] Py：分块读取大文件
来源：http://hz.gogol.net.cn/gtlyfdxzgf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangkeji.top/gtzwowmtop.html

[U24] Py：路径操作
来源：http://hz.jinqigufen.top/gtqzmossfc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.bjfxy.top/gtnftlcijx.html


<!-- 参考信息 -->