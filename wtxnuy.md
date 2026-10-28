代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtnmwzhyhe.html

[R72] 等待端口就绪
来源：http://hz.wangdashe.top/gtbannjprd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.52xcode.cn/gtuoajkhaw.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtmeiitbux.html

split -l 1000 big.log part_
来源：http://hz.dashuyun.cn/gtgqzzpnbo.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtyczamsmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yangfankeji.com/gtcbuifsgr.html

[R75] 导出环境变量
来源：http://hz.yuanzhike.top/gtliioofbu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sysykeji.top/gtovnqxwrp.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtxtdbikir.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtejjoasht.html

[R77] 读取用户输入
来源：http://hz.yj20258.top/gtkmqeiwkr.html

read -rp "请输入: " ans
来源：http://hz.jyoumei.cn/gtkmkhlqzl.html

[R78] 交互式菜单
来源：http://hz.jianghu66.top/gtdqejhgvy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigfzy.top/gtmnhiuhsc.html

[R79] 解析命令行选项
来源：http://hz.daxiang520.top/gtxdvwqsir.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gtjkhyvnzr.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtnekdvsqh.html

time ./run.sh
来源：http://hz.jqgufenzy.top/gtmeptotwd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcsnpinvb.html

S. C / C++ 专题
来源：http://hz.ivvv.top/gtjbyqywhk.html

================================================================================
来源：http://hz.yvedp.cn/gtvonwlogt.html

[S01] C：Hello World
来源：http://hz.andypj.xyz/gtzgqpbhaz.html

#include <stdio.h>
来源：http://hz.xuetiantiany.cn/gtnmdyquik.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtdftwclbv.html

[S02] C：变量与格式化输出
来源：http://hz.sysykeji.top/gtrmausudp.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gtvtbkilsd.html

[S03] C：读入整数
来源：http://hz.gzhubu.top/gtoagpulpl.html

int x; scanf("%d", &x);
来源：http://hz.chenzaomai.com/gtcfxygjuj.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtvvppwgqw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtczdhddxo.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtgxiskjqg.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtcxfcbevh.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gtiyfovccr.html

strcmp(a, b) == 0
来源：http://hz.ydzc1.top/gtlafambps.html

[S07] C：数组遍历求和
来源：http://hz.tanke756.top/gtnmcxytyh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cheryme.top/gtwveereas.html

[S08] C：动态内存分配与释放
来源：http://hz.zhoulong.xyz/gtjdxibhpy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fengsongda.top/gtpdrruswv.html

[S09] C：结构体定义与初始化
来源：http://hz.9152youxi.cn/gtfffkpyrw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gtralsqxrr.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtapovqerg.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtzazlrbld.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gtbqxqnqej.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gtgudhyesm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gtlnixgeoy.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtuzgbmmxs.html

[S12] C：写文件
来源：http://hz.sufxvd.cn/gtzketsqxp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtqkpqyzjk.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtgnrvkddm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtoreckvpd.html

[S14] C：枚举
来源：http://hz.dianchejie.cn/gtuuacrfps.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hfpthk.cn/gtfcrgwgqi.html

[S15] C：类型转换
来源：http://hz.ywan-chungtsiang.top/gtcuivnrrq.html

(double) a / b
来源：http://hz.meibo888.top/gtxfsgqlse.html

[S16] C：位操作置位
来源：http://hz.0kj1m.cn/gtacholxdx.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtpdsayrwm.html

[S17] C：安全拼接字符串
来源：http://hz.jyoumei.cn/gtwohunfek.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jyoumei.cn/gtzqvnaqyh.html

[S18] C：命令行参数
来源：http://hz.tian-w.cn/gtyccygaif.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtsrsanlcy.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtoyklszyh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtzgeuejsy.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtxgwtndef.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtdsdyydal.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtcwvegyyn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cqqwz.cn/gtfcraqsxv.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gtlvfmnvur.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtukrcouon.html

[S23] C：随机数
来源：http://hz.haohaochexian.top/gtuwhfbhwd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangtech.top/gtlsdfyilo.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtzzgtmfxv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gttwemeins.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtndhzubok.html

memcpy(dst, src, n);
来源：http://hz.haohaochexian.top/gthoucqlpm.html

[S26] C：内存清零
来源：http://hz.cqqwz.cn/gtxpycwers.html

memset(a, 0, sizeof a);
来源：http://hz.hywenlv.cn/gtsjiklmlm.html

[S27] C：定义常量
来源：http://hz.guowangkeji.top/gtubccikpl.html

const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtrsfjwrwo.html

[S28] C：静态变量
来源：http://hz.yonumen.top/gtbhqkdwky.html

static int counter = 0;
来源：http://hz.yj20258888.top/gtjwjnzxil.html

[S29] C：变参函数
来源：http://hz.hnxiangtu.top/gtwxmgssea.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sufxvd.cn/gtuqlgezku.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtlzlyutga.html

#ifndef X_H
来源：http://hz.guowangkeji.top/gtomoccdyf.html

#define X_H
来源：http://hz.redwolf501.top/gtsijqnbhy.html

#endif
来源：http://hz.jqgfzy.top/gtxvhlangk.html

[S31] C++：Hello World
来源：http://hz.hongshengwenyu.top/gtucgkzulc.html

#include <iostream>
来源：http://hz.zhijiandao.cn/gtmonlgtdz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtwzdruobu.html

[S32] C++：字符串
来源：http://hz.shzxlz.cn/gtpidckzmy.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gtfmhsrrwl.html

[S33] C++：vector 增删
来源：http://hz.ydzc1.top/gtsepsqdtd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zycfv.cn/gtmebbjhao.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtpgydtanw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.c1oappe.top/gthiobrwyz.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtuyybpwef.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtfmykoykj.html

[S36] C++：unordered_map
来源：http://hz.sufxvd.cn/gtjqqxlzhh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtklprhwtq.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtchtxbddm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtkeguptxj.html

[S38] C++：排序
来源：http://hz.xuetiantiany.cn/gtvgnqdfpg.html

std::sort(v.begin(), v.end());
来源：http://hz.aibaodan.cn/gtphmntqif.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gttybylwku.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtrihcbbnd.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtzmmdovlm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aizwys.cn/gtspdjbrii.html

[S41] C++：类与构造函数
来源：http://hz.shuidangran.top/gtybametmc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gtcbvizzim.html

[S42] C++：继承与虚函数
来源：http://hz.guowangkeji.top/gtafrsoriz.html

class B : public Base { public: void f() override {} };
来源：http://hz.haohaochexian.top/gtmnvoxien.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gtuwgoylig.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgufenzy.top/gtenkrfptf.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtrupgeell.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtvbpfaxyo.html

[S45] C++：lambda
来源：http://hz.quarkkingdee.top/gtoosrzsvn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuanzx.com/gtzuhvhktg.html

[S46] C++：函数模板
来源：http://hz.zycfv.cn/gthugtoosi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtrbsjzpwi.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gtgofwercs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xziqi.cn/gtyfobowxn.html

[S48] C++：逐行读文件
来源：http://hz.hfpthk.cn/gtnlbjmadn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtoqnzgbmx.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtlyxpbkcy.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gttvbddrav.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hfpthk.cn/gtpgcfoymx.html

[S50] C++：格式化数字
来源：http://hz.zycfv.cn/gtrzsvbxtj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cdnleiting.top/gtfgqnzcvb.html

[S51] C++：显式类型转换
来源：http://hz.quarkkingdee.top/gtgjpazloh.html

static_cast<double>(a) / b
来源：http://hz.zhongyouzk.top/gtpbszrqdp.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtjobyylat.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtbkithhjr.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtcetmjuzj.html

std::vector<int> w = std::move(v);
来源：http://hz.chenjidiqi.icu/gttmofdlly.html

[S54] C++：异常处理
来源：http://hz.birdmap.top/gtnmeoknqf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.316326.xyz/gtqxcutncs.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtmrmculry.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dashuyun.cn/gtluuvanyf.html

[S56] C++：optional
来源：http://hz.52xcode.cn/gtnixuvpsi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.andypj.xyz/gtroioynfy.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtzzivobbo.html

constexpr int N = 10;
来源：http://hz.zhaomingkeji.xyz/gtfdljupdl.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtiitxrhpz.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnqzz.top/gthwahutit.html

[S59] C++：静态断言
来源：http://hz.yj202588.top/gtmlglduhi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shuidangran.top/gtllioygvb.html

[S60] C++：遍历并删除元素
来源：http://hz.iojbl.cn/gtvxmhrcif.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtywczastn.html

================================================================================
来源：http://hz.yueranfly.top/gtzpfstiky.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.feifeiyinyue.top/gtnqhrgkru.html

================================================================================
来源：http://hz.cdnleiting.top/gtyraqeibn.html

[T01] Kotlin：Hello World
来源：http://hz.guowangkeji.top/gtskwvdrqr.html

println("Hello")
来源：http://hz.yuanzhike.top/gtdjrsulzz.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gtclgkdete.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhijiandao.cn/gtfojorqra.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangtech.top/gtdkaxfaoy.html

"值: $b"
来源：http://hz.ivvv.top/gtxkwjzkeh.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtydgltmrd.html

val n: String? = null;  n?.length
来源：http://hz.xuetiantiany.cn/gtttnaweuc.html

[T05] Kotlin：when 表达式
来源：http://hz.pengpengdd.cyou/gtuznqetim.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.redwolf501.top/gtxelnibxq.html

[T06] Kotlin：集合映射
来源：http://hz.snrcjt.cn/gtlsaohmtv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtnmisdqry.html

[T07] Kotlin：集合过滤
来源：http://hz.tanke756.top/gtcivfozio.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gaohongyu789.top/gtrmfdgjov.html

[T08] Kotlin：数据类
来源：http://hz.jyoumei.cn/gtrutecbda.html

data class User(val name: String, val age: Int)
来源：http://hz.ppjwa.cn/gtmrhxeggx.html

[T09] Kotlin：扩展函数
来源：http://hz.mhx1999.top/gtytubuqll.html

fun String.exclaim() = this + "!"
来源：http://hz.chenlongwang.top/gtbcgqpkys.html

[T10] Kotlin：默认参数
来源：http://hz.quarkkingdee.top/gtlfpycrfc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtjcmqinqk.html

[T11] Kotlin：协程
来源：http://hz.yongpay.top/gtpdmvcabr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yongpay.top/gtqkuynqlm.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtfrgjvymk.html

val (a, b) = Pair(1, 2)
来源：http://hz.nwbrower.top/gtjxcaexgr.html

[T13] Kotlin：只读 Map
来源：http://hz.ydzc1.top/gtjgrvksnz.html

val m = mapOf("a" to 1)
来源：http://hz.feifeiyinyue.top/gtqliedvrn.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtirevmgta.html

for (i in 1..10) println(i)
来源：http://hz.yuxming.cn/gtcuaobhlr.html

[T15] Kotlin：接口
来源：http://hz.hongshengwenyu.top/gtcniinqor.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtkcbigoyo.html

[T16] Swift：Hello World
来源：http://hz.chenzaomai.com/gtkdwaaxvm.html

print("Hello")
来源：http://hz.bjfxy.top/gtbfhffjre.html

[T17] Swift：变量与常量
来源：http://hz.zhoulong.xyz/gtyhonegor.html

var a = 1;  let b = 2
来源：http://hz.fzhhl.top/gtxiugktrs.html

[T18] Swift：字符串插值
来源：http://hz.bjfxy.top/gtksuotrvu.html

"值: \(b)"
来源：http://hz.yj20258888.top/gtlkzkbbkw.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtbeirfsxu.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gtqmkjjglm.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gtprtbfebn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtncpjidjc.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gtopqtlbhb.html

for x in a { print(x) }
来源：http://hz.smart0.xyz/gtwdbgcjxb.html

[T22] Swift：字典
来源：http://hz.hongshengwenyu.top/gtcmkpoiby.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtmnwmbrav.html

[T23] Swift：函数
来源：http://hz.cucudq.cn/gtnbpyqcru.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.kuanghao11.cn/gtvnvlijbg.html

[T24] Swift：闭包
来源：http://hz.jqgufenzy.top/gtlcxfsodk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jiagoushi.top/gtwrwocgqv.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangkeji.top/gtpkvkzlvy.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gtehmhqkot.html

[T26] Swift：类与重写
来源：http://hz.redwolf501.top/gtlgevmrjp.html

class A: Base { override func f() {} }
来源：http://hz.jinghuilouyu.cn/gtmgcbmlld.html

[T27] Swift：错误处理
来源：http://hz.ehwqpu.com/gtkhdadngh.html

do { try f() } catch { print(error) }
来源：http://hz.fengsongda.top/gtyhvvzwqe.html

[T28] Swift：枚举
来源：http://hz.sweek.top/gtkfjxnupg.html

enum Color { case red, green }
来源：http://hz.9152youxi.cn/gtlhyilpde.html

[T29] Swift：guard 提前返回
来源：http://hz.yongpay.top/gtufmmxwsz.html

guard let x = opt else { return }
来源：http://hz.zhijiandao.cn/gtydrulwem.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gtqfycuyob.html

protocol Shape { func area() -> Double }
来源：http://hz.hfpthk.cn/gtlgjwyfld.html

[T31] Lua：Hello World
来源：http://hz.yuxming.cn/gthqpgvtzt.html

print("Hello")
来源：http://hz.zhongyouzk.top/gthksfltjg.html

[T32] Lua：局部变量
来源：http://hz.aizwys.cn/gtzxsslttn.html

local a = 1
来源：http://hz.guannengcc.top/gtnqefchuu.html

[T33] Lua：表（数组）
来源：http://hz.iojbl.cn/gtvinsatky.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yueranfly.top/gtcousprnw.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gthbtkkvhz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj202588.top/gtaeamjqcj.html

[T35] Lua：字典表
来源：http://hz.sxryk.cn/gtzlawwdor.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtqynazodt.html

[T36] Lua：函数
来源：http://hz.yangfankeji.com/gtktpperqv.html

function add(a, b) return a + b end
来源：http://hz.ydzc1.top/gtiqmxkhup.html

[T37] Lua：字符串拼接
来源：http://hz.sxryk.cn/gtrccooawo.html

"a" .. "b"
来源：http://hz.xziqi.cn/gtggknndeb.html

[T38] Lua：条件
来源：http://hz.yuanzhike.top/gtmnwfwxaf.html

if x > 0 then print("正") end
来源：http://hz.jlsjyb.cn/gtpqdyukrr.html

[T39] Lua：模式匹配
来源：http://hz.sxryk.cn/gtniawleoz.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gtbiynbupi.html

[T40] Lua：元表
来源：http://hz.xuetiantiany.cn/gttfitnwma.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigfzy.top/gtwypadupj.html

[T41] Perl：Hello World
来源：http://hz.jianghu66.top/gtsqdbhanp.html

print "Hello\n";
来源：http://hz.sweek.top/gtusbwclqb.html

[T42] Perl：变量类型
来源：http://hz.andypj.xyz/gtnthfixsy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxinkj.top/gtxuqngysl.html

[T43] Perl：字符串插值
来源：http://hz.cdnleiting.top/gtcpvqculn.html

"值: $a"
来源：http://hz.redwolf501.top/gtuknmcbvr.html

[T44] Perl：条件
来源：http://hz.zhiwuduotai.top/gttzbclpng.html

if ($a > 0) { print "正"; }
来源：http://hz.tian-w.cn/gtmxytwesf.html

[T45] Perl：数组遍历
来源：http://hz.tian-w.cn/gtsfippkzg.html

for my $x (@arr) { print $x; }
来源：http://hz.ywan-chungtsiang.top/gtizmjvuzl.html

[T46] Perl：哈希操作
来源：http://hz.cheryme.top/gtakwwztco.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shuidangran.top/gtvutldlym.html

[T47] Perl：正则捕获
来源：http://hz.cashguo.top/gtlztfyqwj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenjidiqi.icu/gtqqmvkqmq.html

[T48] Perl：正则替换
来源：http://hz.iojbl.cn/gtwwvussfy.html

$s =~ s/old/new/g;
来源：http://hz.bjfxy.top/gtsjiglrpa.html

[T49] Perl：函数
来源：http://hz.yj202588.top/gthbkasoec.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hammf.cn/gtnvbhnahm.html

[T50] Perl：逐行读文件
来源：http://hz.mhx1999.top/gtjhwgxobx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuanzx.com/gtqysycjcw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xziqi.cn/gtnkctgzbl.html

[T51] Scala：Hello World
来源：http://hz.jyoumei.cn/gtlpridpbn.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtjzmfpceh.html

[T52] Scala：变量
来源：http://hz.yonumen.top/gtpyzqxwxc.html

val a = 1;  var b = 2
来源：http://hz.tian-w.cn/gtroxbxacu.html

[T53] Scala：字符串插值
来源：http://hz.jinqigfzy.top/gtgvoatgrw.html

s"值: $b"
来源：http://hz.zhoulong.xyz/gtxsjxwkbn.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gtkzusckzl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtzjosnfia.html

[T55] Scala：集合过滤
来源：http://hz.tianlin.xyz/gtiudwaxly.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hongshengwenyu.top/gtwwcgnmhs.html

[T56] Scala：样例类
来源：http://hz.xylfe.cn/gtscjyyjhy.html

case class User(name: String, age: Int)
来源：http://hz.havefunace.top/gtaskxmrwd.html

[T57] Scala：模式匹配
来源：http://hz.gaohongyu789.top/gtqohjsprz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.9152youxi.cn/gtglzwpamo.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gtzthmmwmb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hnqzz.top/gtntiiwwgh.html

[T59] Scala：循环
来源：http://hz.xingfuxueyuan.xyz/gtalkdwgjn.html

for (i <- 1 to 10) println(i)
来源：http://hz.0kj1m.cn/gtoinelsil.html

[T60] Scala：折叠
来源：http://hz.guowangkeji.top/gtmiyejbwa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xylfe.cn/gtscjxsohs.html

================================================================================
来源：http://hz.c1oappe.top/gtqrusajvl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tianlin.xyz/gtvfdeupfe.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvtaepfks.html

[U01] Py：创建虚拟环境
来源：http://hz.iojbl.cn/gtfkiimcxe.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xziqi.cn/gtftgiafym.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daxiang520.top/gtaeyyzlmj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yanxiufei.cn/gtogwigkly.html

[U03] Py：加载 .env 配置
来源：http://hz.guowangkeji.top/gtrmslopnp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dianchejie.cn/gtonqywlcz.html

[U04] Py：变量调试打印
来源：http://hz.smart0.xyz/gtoagjqynd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gtkfafpaow.html

[U05] Py：列表去重且保序
来源：http://hz.zhijiandao.cn/gtdgpzsurk.html

list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtwddcnmwh.html

[U06] Py：合并两个字典
来源：http://hz.gogol.net.cn/gtivwqefez.html

{**a, **b}
来源：http://hz.yj202588.top/gtoqqskslx.html

[U07] Py：反转字典键值
来源：http://hz.hnqzz.top/gtuyjjlryf.html

{v: k for k, v in d.items()}
来源：http://hz.tianlin.xyz/gtbtjmlqnb.html

[U08] Py：展平二维列表
来源：http://hz.hnxiangtu.top/gtevlkwukg.html

[y for x in nested for y in x]
来源：http://hz.iojbl.cn/gttikkboln.html

[U09] Py：字典取最大值的键
来源：http://hz.xuanzx.com/gtxsytrjcz.html

max(d, key=d.get)
来源：http://hz.yj20258888.top/gtrqkjqffz.html

[U10] Py：按值排序字典
来源：http://hz.mhx1999.top/gtjarjviwi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gtzgztjcoq.html

[U11] Py：生成器表达式
来源：http://hz.ybcxt.top/gtgzapihxe.html

(x * 2 for x in arr)
来源：http://hz.cqqwz.cn/gthrzfxzay.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xinyue.icu/gttducajho.html

Counter(arr).most_common(3)
来源：http://hz.yj20258888.top/gtpundvptj.html


<!-- 参考信息 -->