代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtqekzlidj.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gteenzsvea.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtoxekyugy.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gteujgxpfq.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtykdcskym.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtcnxcnslo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtxeilxjsg.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtlkeohznu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtoaoysvmj.html

[R76] 使用临时文件
来源：http://hz.yuanzhike.top/gtvrausymq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gtzkodjbix.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gtoydjfyis.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gtrsotakga.html

[R78] 交互式菜单
来源：http://hz.hywenlv.cn/gtsksimdcj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gttqxnnudd.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtfnzysgho.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtegyvsris.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtsdoowxby.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gtuyzbccoe.html

================================================================================
来源：http://hz.cheryme.top/gtlfgthyqc.html

S. C / C++ 专题
来源：http://hz.andypj.xyz/gtsciafrqn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgnoykwhz.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtqgrdrrzl.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtsofvtipb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhoulong.xyz/gtwwkszrft.html

[S02] C：变量与格式化输出
来源：http://hz.zhiwuduotai.top/gtxjsilvho.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtsmgvxeeg.html

[S03] C：读入整数
来源：http://hz.ydzc1.top/gtzxkwskdf.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtxjaxsogf.html

[S04] C：字符串复制
来源：http://hz.xziqi.cn/gtkwykmjeb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.quarkkingdee.top/gtzkiivmbq.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtoczeagmo.html

strlen(s)
来源：http://hz.sysykeji.top/gtqmlhfnod.html

[S06] C：字符串比较
来源：http://hz.quarkkingdee.top/gtihnevfll.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtsbogvfgf.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtgdrciqbh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ppjwa.cn/gtuahwshiy.html

[S08] C：动态内存分配与释放
来源：http://hz.sweek.top/gtxffweots.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ppjwa.cn/gtlstznril.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gtxonedudb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangtech.top/gtkxondixg.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtsssunpnl.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtmyvrvydu.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtemqjooud.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxuanxn.top/gtubhngyhe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258888.top/gtnghgvcfy.html

fclose(f);
来源：http://hz.smart0.xyz/gtcqdoqdqf.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtyifttlnq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtczydwepn.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtvcmcwjcn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.quarkkingdee.top/gtdogdhpkh.html

[S14] C：枚举
来源：http://hz.guowangkeji.top/gtcdeqvubk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxuanxn.top/gteljnsnzt.html

[S15] C：类型转换
来源：http://hz.tianlin.xyz/gtdnhihtpx.html

(double) a / b
来源：http://hz.shanyushiyangtech.top/gtsqamgmug.html

[S16] C：位操作置位
来源：http://hz.guannengcc.top/gtzohasbqe.html

x |= (1 << 3);
来源：http://hz.9152youxi.cn/gtahplmsbd.html

[S17] C：安全拼接字符串
来源：http://hz.dashuyun.cn/gtjlzomczj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gogol.net.cn/gtsyamscmx.html

[S18] C：命令行参数
来源：http://hz.xziqi.cn/gtkkgpsrlj.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtnguyztgv.html

[S19] C：快速排序
来源：http://hz.daxiang520.top/gtabpzrcal.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtyzcnxruu.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtzvsnbyni.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gttfqpbgyr.html

[S21] C：字符类别判断
来源：http://hz.pycfn.com/gtotaiklij.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhiwuduotai.top/gtczrbwmgg.html

[S22] C：字符串转数字
来源：http://hz.yuxming.cn/gtfqeeqbqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhaomingkeji.xyz/gtvuvnhymr.html

[S23] C：随机数
来源：http://hz.ppjwa.cn/gtsizopddy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtzixtxrfy.html

[S24] C：获取本地时间
来源：http://hz.chenjidiqi.icu/gtpkccwqds.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gttuibihsy.html

[S25] C：内存拷贝
来源：http://hz.shuidangran.top/gtmjakzwzt.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtlhcuqnbl.html

[S26] C：内存清零
来源：http://hz.xinyue.icu/gtclmncias.html

memset(a, 0, sizeof a);
来源：http://hz.ehwqpu.com/gterbpkmyc.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtmykpeyzb.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gttbvbcsuo.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtokjtncce.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtruejplcf.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtberubfpf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydjk.org.cn/gtgwtuonir.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtmpphascn.html

#ifndef X_H
来源：http://hz.gogol.net.cn/gtijqvxhvn.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gtmokdgzod.html

#endif
来源：http://hz.guowangkeji.top/gtjpijzjdp.html

[S31] C++：Hello World
来源：http://hz.fengsongda.top/gtzygqcbcx.html

#include <iostream>
来源：http://hz.gzhubu.top/gtqigztdin.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydzc1.top/gtpxqopkvq.html

[S32] C++：字符串
来源：http://hz.aizwys.cn/gtwwnjbsmv.html

std::string s = "hi";  s += "!";
来源：http://hz.daxiang520.top/gtipfweywk.html

[S33] C++：vector 增删
来源：http://hz.0kj1m.cn/gtruauxeaa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtoiacwblu.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtzsjbbems.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj202588.top/gtxqapgthy.html

[S35] C++：map
来源：http://hz.yueranfly.top/gthkbqkusk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtsqjzuyzm.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtsdbfaqlo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtvjmmqxbt.html

[S37] C++：set
来源：http://hz.xuetiantiany.cn/gtgqgatimm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangtech.top/gtvulvbeys.html

[S38] C++：排序
来源：http://hz.guannengcc.top/gtcgxgsvpc.html

std::sort(v.begin(), v.end());
来源：http://hz.cheryme.top/gtfkbwcakj.html

[S39] C++：自定义比较器排序
来源：http://hz.dianchejie.cn/gtwvcgryjd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gzhubu.top/gthgbptjpq.html

[S40] C++：查找元素
来源：http://hz.pycfn.com/gtpvvxuszi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtoxhigwkl.html

[S41] C++：类与构造函数
来源：http://hz.fzhhl.top/gtjftuftul.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guowangkeji.top/gtbmuzbrug.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtrhtqlxew.html

class B : public Base { public: void f() override {} };
来源：http://hz.ivvv.top/gtkjlaemab.html

[S43] C++：智能指针
来源：http://hz.andypj.xyz/gthspzwgbu.html

auto p = std::make_unique<int>(5);
来源：http://hz.shuidangran.top/gtqyvdinum.html

[S44] C++：引用传参
来源：http://hz.chenlongwang.top/gtjmqmidtf.html

void inc(int &x) { ++x; }
来源：http://hz.cucudq.cn/gtfmbikojj.html

[S45] C++：lambda
来源：http://hz.xylfe.cn/gtepqhtcxr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtrtbjnkka.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gtvuccgjhg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuxming.cn/gtuwofugfi.html

[S47] C++：结构化绑定遍历
来源：http://hz.birdmap.top/gtjiebddkd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtdlvaydvi.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtiltudpyp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.316326.xyz/gteihkaenu.html

while (std::getline(in, line)) { }
来源：http://hz.hnxiangtu.top/gthflqueja.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtdaikvhun.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtflurfsgj.html

[S50] C++：格式化数字
来源：http://hz.aibaodan.cn/gtqumuuaeo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gtmlukgyue.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtthahtbpy.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gtagemkvts.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gtlwyqtdrg.html

int size() const noexcept { return n_; }
来源：http://hz.ehwqpu.com/gtkqfnuaxp.html

[S53] C++：移动语义
来源：http://hz.hfpthk.cn/gtpacqwhcw.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangtech.top/gttyythcwh.html

[S54] C++：异常处理
来源：http://hz.zycfv.cn/gtqgrkcsxo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258.top/gtqfwwkhwe.html

[S55] C++：结构化绑定
来源：http://hz.ivvv.top/gtpuhfhkpl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangkeji.top/gtrbolmywk.html

[S56] C++：optional
来源：http://hz.xinyue.icu/gtsxecnvou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gtoncprsaa.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtaieupoyl.html

constexpr int N = 10;
来源：http://hz.vqdsnc.cn/gtbystpfyw.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtrfeyxlxj.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gtkkhbnlhz.html

[S59] C++：静态断言
来源：http://hz.c1oappe.top/gteadceemq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ehwqpu.com/gtqnhilsxd.html

[S60] C++：遍历并删除元素
来源：http://hz.sweek.top/gtfafhzsar.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtstgwcczb.html

================================================================================
来源：http://hz.yongpay.top/gtewrnxwmf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gteagrefhp.html

================================================================================
来源：http://hz.hnqzz.top/gtbucbqkxo.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gtwcaiahah.html

println("Hello")
来源：http://hz.hammf.cn/gttdxglbsy.html

[T02] Kotlin：变量
来源：http://hz.guowangkeji.top/gtzrsdrfrb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258888.top/gtezrdlhvv.html

[T03] Kotlin：字符串模板
来源：http://hz.zhixingplan.top/gtrkgqunnz.html

"值: $b"
来源：http://hz.aizwys.cn/gtilkwlvpw.html

[T04] Kotlin：空安全
来源：http://hz.daria6918.cn/gtsbkmkiux.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gtvqwrmawd.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtklkuurzc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtwnifrnyh.html

[T06] Kotlin：集合映射
来源：http://hz.jinyuanbaomall.cn/gtmwrvkqau.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangkeji.top/gtysgndsof.html

[T07] Kotlin：集合过滤
来源：http://hz.xuanzx.com/gthczkespd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aizwys.cn/gtvtqnvopt.html

[T08] Kotlin：数据类
来源：http://hz.hongshengwenyu.top/gtojmtanke.html

data class User(val name: String, val age: Int)
来源：http://hz.0kj1m.cn/gtcyuezxat.html

[T09] Kotlin：扩展函数
来源：http://hz.zhiwuduotai.top/gtsudzzdna.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gtaqsgzbwj.html

[T10] Kotlin：默认参数
来源：http://hz.jqgufenzy.top/gtxojygbwc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gttjmgfviq.html

[T11] Kotlin：协程
来源：http://hz.sweek.top/gteudqmepj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ppjwa.cn/gtkxeldeeq.html

[T12] Kotlin：解构声明
来源：http://hz.bjfxy.top/gtzzeoveyb.html

val (a, b) = Pair(1, 2)
来源：http://hz.guannengcc.top/gtoqvasdvf.html

[T13] Kotlin：只读 Map
来源：http://hz.cashguo.top/gtyywgswli.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtwhwjefli.html

[T14] Kotlin：循环
来源：http://hz.cqqwz.cn/gtcydnvscg.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gtfjjzkbtf.html

[T15] Kotlin：接口
来源：http://hz.yonumen.top/gtcfmpagnx.html

interface Shape { fun area(): Double }
来源：http://hz.snrcjt.cn/gtjolxyvyn.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtmprmzmwa.html

print("Hello")
来源：http://hz.svipenyu.cn/gtruiqqmgh.html

[T17] Swift：变量与常量
来源：http://hz.guannengcc.top/gtboihsrio.html

var a = 1;  let b = 2
来源：http://hz.xinyue.icu/gtgsxflkwc.html

[T18] Swift：字符串插值
来源：http://hz.ydjk.org.cn/gtugtxxlme.html

"值: \(b)"
来源：http://hz.nanxinkj.top/gtzmofqsvm.html

[T19] Swift：可选绑定
来源：http://hz.gzhubu.top/gtkmmevlzy.html

if let n = opt { print(n) }
来源：http://hz.pycfn.com/gtnhjxvacd.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtuitbzixk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.kuanghao11.cn/gtikfhjbpb.html

[T21] Swift：遍历
来源：http://hz.ydjk.org.cn/gtfgswabgs.html

for x in a { print(x) }
来源：http://hz.yanxiufei.cn/gtthzpocxf.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtqzxnorha.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhaomingkeji.xyz/gtglvzcxbi.html

[T23] Swift：函数
来源：http://hz.hongshengwenyu.top/gtjzhaygzr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sweek.top/gtzsxeplkv.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtjnnqwanv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtyagbyiac.html

[T25] Swift：结构体
来源：http://hz.ivvv.top/gtcqwbudbj.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtnowyiwoy.html

[T26] Swift：类与重写
来源：http://hz.xinyue.icu/gtipwrutpe.html

class A: Base { override func f() {} }
来源：http://hz.zhiwuduotai.top/gtlixilauo.html

[T27] Swift：错误处理
来源：http://hz.haohaochexian.top/gtbbphahlu.html

do { try f() } catch { print(error) }
来源：http://hz.guannengcc.top/gtpeunpsso.html

[T28] Swift：枚举
来源：http://hz.yj20258888.top/gtuzrhtwgi.html

enum Color { case red, green }
来源：http://hz.ywan-chungtsiang.top/gtegujyanh.html

[T29] Swift：guard 提前返回
来源：http://hz.tian-w.cn/gtphcqaeji.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gttwipzrwo.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtnfoqzvss.html

protocol Shape { func area() -> Double }
来源：http://hz.xziqi.cn/gtacccliyb.html

[T31] Lua：Hello World
来源：http://hz.jinyuanbaomall.cn/gtmlylimrl.html

print("Hello")
来源：http://hz.meibo888.top/gtrbkrfmul.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangtech.top/gtbrnzrniw.html

local a = 1
来源：http://hz.yuanzhike.top/gtdzwwqyda.html

[T33] Lua：表（数组）
来源：http://hz.hnxiangtu.top/gtszkoxvxj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.havefunace.top/gteairpudv.html

[T34] Lua：遍历表
来源：http://hz.hammf.cn/gtdbwuzyft.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pengpengdd.cyou/gtwiawfvbr.html

[T35] Lua：字典表
来源：http://hz.yangfankeji.com/gtwmmoyjzw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hysaishi.cn/gtcyhezygq.html

[T36] Lua：函数
来源：http://hz.zdqjudy.top/gtqzhfccrr.html

function add(a, b) return a + b end
来源：http://hz.sysykeji.top/gttrkljtmf.html

[T37] Lua：字符串拼接
来源：http://hz.haohaochexian.top/gtrmommlmp.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtzensucqd.html

[T38] Lua：条件
来源：http://hz.hnqzz.top/gtflsbaauj.html

if x > 0 then print("正") end
来源：http://hz.ywan-chungtsiang.top/gttyqwhhum.html

[T39] Lua：模式匹配
来源：http://hz.cucudq.cn/gtafrpvkqc.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gtiixjofwu.html

[T40] Lua：元表
来源：http://hz.ydjk.org.cn/gtupqupaka.html

setmetatable({}, { __index = base })
来源：http://hz.hywenlv.cn/gtfcmxzcrw.html

[T41] Perl：Hello World
来源：http://hz.smart0.xyz/gtxevphhly.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtcrcbepgp.html

[T42] Perl：变量类型
来源：http://hz.xuetiantiany.cn/gtwikwflyb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinqigufen.top/gtmdzhsfbc.html

[T43] Perl：字符串插值
来源：http://hz.52xcode.cn/gtjbendaqn.html

"值: $a"
来源：http://hz.tianlin.xyz/gtemlnkrxx.html

[T44] Perl：条件
来源：http://hz.iojbl.cn/gtnnfulpzt.html

if ($a > 0) { print "正"; }
来源：http://hz.0kj1m.cn/gtgmybefxk.html

[T45] Perl：数组遍历
来源：http://hz.bjfxy.top/gtoidjhgwm.html

for my $x (@arr) { print $x; }
来源：http://hz.cashguo.top/gtchckzjll.html

[T46] Perl：哈希操作
来源：http://hz.gotoacloud.top/gttoliudpj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sxryk.cn/gtqhvszxzt.html

[T47] Perl：正则捕获
来源：http://hz.jqgufenzy.top/gtjqcntvac.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yj202588.top/gtzftcnzps.html

[T48] Perl：正则替换
来源：http://hz.kuanghao11.cn/gtsaekeert.html

$s =~ s/old/new/g;
来源：http://hz.aibaodan.cn/gtfexxuxoc.html

[T49] Perl：函数
来源：http://hz.gzhubu.top/gtmyjpasma.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nwbrower.top/gtvpnastme.html

[T50] Perl：逐行读文件
来源：http://hz.svipenyu.cn/gtorclfsyt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.316326.xyz/gtpzgcccod.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhengqikj.top/gtfonramqw.html

[T51] Scala：Hello World
来源：http://hz.snrcjt.cn/gtlnjuewia.html

println("Hello")
来源：http://hz.hammf.cn/gtudcnuckx.html

[T52] Scala：变量
来源：http://hz.yongpay.top/gtdpqqregw.html

val a = 1;  var b = 2
来源：http://hz.nwbrower.top/gtdzudobpi.html

[T53] Scala：字符串插值
来源：http://hz.ivvv.top/gtprtaqfkg.html

s"值: $b"
来源：http://hz.316326.xyz/gtjswqrpsn.html

[T54] Scala：集合映射
来源：http://hz.guannengcc.top/gtxlrmldgq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shangyingyoupin.top/gtkdodbtdt.html

[T55] Scala：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtehdpmikk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jlsjyb.cn/gtmxkvyqcg.html

[T56] Scala：样例类
来源：http://hz.chenjidiqi.icu/gtleusptxn.html

case class User(name: String, age: Int)
来源：http://hz.yueranfly.top/gtuxbuudip.html

[T57] Scala：模式匹配
来源：http://hz.jlsjyb.cn/gtjqsorhuh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cqqwz.cn/gtqovhldga.html

[T58] Scala：函数定义
来源：http://hz.havefunace.top/gtsvfjjosc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cucudq.cn/gtokykcnml.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gthoegsspp.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj20258888.top/gtywfjhmug.html

[T60] Scala：折叠
来源：http://hz.wangdashe.top/gthknystrt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.haohaochexian.top/gtiaocjcfi.html

================================================================================
来源：http://hz.vqdsnc.cn/gtnaqvmvbj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenlongwang.top/gtabkllves.html

================================================================================
来源：http://hz.fengsongda.top/gtphjrspuz.html

[U01] Py：创建虚拟环境
来源：http://hz.pengpengdd.cyou/gtkbhegfzo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.dianchejie.cn/gtojugoheg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtoyjjxpsr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.iojbl.cn/gtupqdbvmq.html

[U03] Py：加载 .env 配置
来源：http://hz.yvedp.cn/gtlezrqttu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gtcknqvawq.html

[U04] Py：变量调试打印
来源：http://hz.xziqi.cn/gtqatfhsly.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yongpay.top/gtigrmmtue.html

[U05] Py：列表去重且保序
来源：http://hz.zhengqikj.top/gtwvotjjer.html

list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtdyzczkpe.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gttyycinys.html

{**a, **b}
来源：http://hz.xingfuxueyuan.xyz/gtojurhpxi.html

[U07] Py：反转字典键值
来源：http://hz.feifeiyinyue.top/gtcvbpmtti.html

{v: k for k, v in d.items()}
来源：http://hz.jinghuilouyu.cn/gtyafgncfc.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangkeji.top/gtjthmkhkz.html

[y for x in nested for y in x]
来源：http://hz.xylfe.cn/gtyyjomrca.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258.top/gtteilpycj.html

max(d, key=d.get)
来源：http://hz.shanyushiyangkeji.top/gtsubzoxci.html

[U10] Py：按值排序字典
来源：http://hz.zhoulong.xyz/gtvqbncnfs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xylfe.cn/gtlffhbalf.html

[U11] Py：生成器表达式
来源：http://hz.yonumen.top/gtvsvahhxs.html

(x * 2 for x in arr)
来源：http://hz.birdmap.top/gtsmvmjpnv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jlsjyb.cn/gtqmjozmkn.html

Counter(arr).most_common(3)
来源：http://hz.gotoacloud.top/gtrlevmlkv.html


<!-- 参考信息 -->