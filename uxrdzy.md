代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxinkj.top/gttpaxolfk.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gttxyizyzp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtkplibnac.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtjfgefjqo.html

split -l 1000 big.log part_
来源：http://hz.yanxiufei.cn/gtbqlcanxq.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtfougrufs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hywenlv.cn/gtifkbkblj.html

[R75] 导出环境变量
来源：http://hz.gotoacloud.top/gtdjpjslfe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuanzhike.top/gtfysizmyp.html

[R76] 使用临时文件
来源：http://hz.cashguo.top/gtqfzlduob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtytjqxfsq.html

[R77] 读取用户输入
来源：http://hz.316326.xyz/gtnuihtutg.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtaclqbgur.html

[R78] 交互式菜单
来源：http://hz.snrcjt.cn/gtzmiphsqs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.mhx1999.top/gtjnzqktuv.html

[R79] 解析命令行选项
来源：http://hz.tanke756.top/gtqzoshcca.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtbwjhoryn.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gtoiikuirh.html

time ./run.sh
来源：http://hz.aibaodan.cn/gtrhenjxvc.html

================================================================================
来源：http://hz.fengsongda.top/gtwlrjsuyd.html

S. C / C++ 专题
来源：http://hz.andypj.xyz/gtiypqxoud.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtydfvzrek.html

[S01] C：Hello World
来源：http://hz.mhx1999.top/gtzeryrxmr.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtrqamqiam.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258.top/gtxozrjubn.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtzypbhelf.html

int a = 10; printf("%d\n", a);
来源：http://hz.zycfv.cn/gtgrtmsgyz.html

[S03] C：读入整数
来源：http://hz.hammf.cn/gtajqnblkg.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gtczjohimu.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtdccsxuxk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxinkj.top/gtlakevuhu.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtkjhrcggd.html

strlen(s)
来源：http://hz.xziqi.cn/gtzrbkdnkl.html

[S06] C：字符串比较
来源：http://hz.yj202588.top/gtkdzraglg.html

strcmp(a, b) == 0
来源：http://hz.jianghu66.top/gtsxfuazcb.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtjegiwowz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gtqlgtyapr.html

[S08] C：动态内存分配与释放
来源：http://hz.nwbrower.top/gtwyqpbbft.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guannengcc.top/gtwlvazbnh.html

[S09] C：结构体定义与初始化
来源：http://hz.sysykeji.top/gtqnzcveoe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.andypj.xyz/gtfncdcdav.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtphhppwoh.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtwvwpqgzt.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtpewtktmu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtobomyocg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xinyue.icu/gtmcmynzqj.html

fclose(f);
来源：http://hz.zhengqikj.top/gtgclepcvv.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gttiqkjsbm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtslgjrgyb.html

[S13] C：宏定义
来源：http://hz.yongpay.top/gtprqpwjui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cdnleiting.top/gtjheehyjz.html

[S14] C：枚举
来源：http://hz.yonumen.top/gtrhallgaa.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydzc1.top/gtxdfzncnv.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtvlukbxrr.html

(double) a / b
来源：http://hz.haohaochexian.top/gtkmfqcpne.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtgtqrajas.html

x |= (1 << 3);
来源：http://hz.ydzc1.top/gtqwrlmbiv.html

[S17] C：安全拼接字符串
来源：http://hz.aizwys.cn/gtrzbriczv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.andypj.xyz/gtevlnngxx.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gttfrlfjcg.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gtvqplwzcn.html

[S19] C：快速排序
来源：http://hz.jianghu66.top/gtjwkfazyb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtfzwufewk.html

[S20] C：二分查找
来源：http://hz.aibaodan.cn/gtkwbjuhsa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtydjfzqey.html

[S21] C：字符类别判断
来源：http://hz.sysykeji.top/gtbewojetb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtankxnbpl.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gtfyfdiwsf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gogol.net.cn/gtlysjqqwf.html

[S23] C：随机数
来源：http://hz.hnxiangtu.top/gtbsqdytdx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuetiantiany.cn/gtaxzlqikb.html

[S24] C：获取本地时间
来源：http://hz.sxryk.cn/gtuhkmbrcm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtfodkvlkr.html

[S25] C：内存拷贝
来源：http://hz.jlsjyb.cn/gtoetqygab.html

memcpy(dst, src, n);
来源：http://hz.cqqwz.cn/gtdjthwuhd.html

[S26] C：内存清零
来源：http://hz.guowangkeji.top/gtpsaadfca.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtbkqxwvgy.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gtukvpjsax.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtsifvrlbo.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gtvaqojtur.html

static int counter = 0;
来源：http://hz.birdmap.top/gtjemmrhww.html

[S29] C：变参函数
来源：http://hz.yanxiufei.cn/gtzvxmydoi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gtawlgcxng.html

[S30] C：头文件保护
来源：http://hz.yanxiufei.cn/gtexpwbnxr.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtlyihquhr.html

#define X_H
来源：http://hz.jinqigfzy.top/gtgcyfebhs.html

#endif
来源：http://hz.svipenyu.cn/gttsgzgzth.html

[S31] C++：Hello World
来源：http://hz.jinqigufen.top/gtynmtdmxh.html

#include <iostream>
来源：http://hz.jianghu66.top/gtpagzymby.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtpsdtzrtd.html

[S32] C++：字符串
来源：http://hz.jinqigfzy.top/gtqrvxuthx.html

std::string s = "hi";  s += "!";
来源：http://hz.yanxiufei.cn/gtnvuarjdx.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gtqfyayqnl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.c1oappe.top/gtwcnvhfcs.html

[S34] C++：遍历 vector
来源：http://hz.jqgfzy.top/gtnzxiigtz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtwxfwjmjr.html

[S35] C++：map
来源：http://hz.ydzc1.top/gtivkkytam.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtjuyihzvd.html

[S36] C++：unordered_map
来源：http://hz.xuanzx.com/gtcwuxmkbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtrlwtgbie.html

[S37] C++：set
来源：http://hz.jiagoushi.top/gtylygtqpu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtbyxqmihe.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtwstbejkb.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtopjoxrgr.html

[S39] C++：自定义比较器排序
来源：http://hz.cashguo.top/gtipctkwnw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yonumen.top/gtpzodgwkd.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtcybgnnog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtuwgqmjtr.html

[S41] C++：类与构造函数
来源：http://hz.redwolf501.top/gtvoahsaay.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtrtoxuubf.html

[S42] C++：继承与虚函数
来源：http://hz.aibaodan.cn/gtcxtcghgi.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gtqhrpexrt.html

[S43] C++：智能指针
来源：http://hz.guowangkeji.top/gtgnykzkfi.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhoulong.xyz/gtfddsfsop.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtxdxsbbqg.html

void inc(int &x) { ++x; }
来源：http://hz.sysykeji.top/gtvegkprzi.html

[S45] C++：lambda
来源：http://hz.jinqigfzy.top/gtaxcdzdii.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tian-w.cn/gtovfccgge.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gtihquzdjw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtgwxodnda.html

[S47] C++：结构化绑定遍历
来源：http://hz.ehwqpu.com/gtkbixoubv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jianghu66.top/gtosyjpaip.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtwitlundg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ybcxt.top/gtbniivpqb.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gtnvpdnfmb.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtnbiuxbdb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.316326.xyz/gtcgytwowy.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtgrpwaolg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aizwys.cn/gtqzbbhybx.html

[S51] C++：显式类型转换
来源：http://hz.zdqjudy.top/gtlrmgonbh.html

static_cast<double>(a) / b
来源：http://hz.hammf.cn/gtkbundarg.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtsvqcrmxm.html

int size() const noexcept { return n_; }
来源：http://hz.daria6918.cn/gtyqgsnwno.html

[S53] C++：移动语义
来源：http://hz.smart0.xyz/gtacotldqk.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtcmpuovac.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gtihzrfchc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtpmewojda.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangkeji.top/gtytgxokfd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.iojbl.cn/gtzixkfutp.html

[S56] C++：optional
来源：http://hz.pycfn.com/gtjvpdtwxj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnqzz.top/gtwunyingg.html

[S57] C++：编译期常量
来源：http://hz.chenzaomai.com/gtfrqfcrtz.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtoyuuhlyb.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtuzzhzowx.html

namespace ns { int f() { return 1; } }
来源：http://hz.yueranfly.top/gtsodozfpk.html

[S59] C++：静态断言
来源：http://hz.jinyuanbaomall.cn/gtoblivryh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtyaheespm.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gtcudrlndn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gtcpkztjtq.html

================================================================================
来源：http://hz.redwolf501.top/gtptjtcfcy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtcezkvpdp.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtknsfxvhp.html

[T01] Kotlin：Hello World
来源：http://hz.yuxming.cn/gtxqsjyxtm.html

println("Hello")
来源：http://hz.fzhhl.top/gtzunmjdng.html

[T02] Kotlin：变量
来源：http://hz.yonumen.top/gtwtacpjeb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yvedp.cn/gtgsfxqceb.html

[T03] Kotlin：字符串模板
来源：http://hz.0kj1m.cn/gtzblhdkbt.html

"值: $b"
来源：http://hz.0kj1m.cn/gtphipomxl.html

[T04] Kotlin：空安全
来源：http://hz.snrcjt.cn/gtlaacvemg.html

val n: String? = null;  n?.length
来源：http://hz.yuanzhike.top/gtipqifaeg.html

[T05] Kotlin：when 表达式
来源：http://hz.yvedp.cn/gtbgfhczgy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtvsgldlwm.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtvtyehpsq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtgajjbbyj.html

[T07] Kotlin：集合过滤
来源：http://hz.cdnleiting.top/gtuxsgnltl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.dashuyun.cn/gtmkzenocw.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtjokpwmom.html

data class User(val name: String, val age: Int)
来源：http://hz.0kj1m.cn/gtvbfxwvmr.html

[T09] Kotlin：扩展函数
来源：http://hz.guowangkeji.top/gtzuciteex.html

fun String.exclaim() = this + "!"
来源：http://hz.zhaomingkeji.xyz/gtckocphdt.html

[T10] Kotlin：默认参数
来源：http://hz.nanxuanxn.top/gtqowaizqp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gaohongyu789.top/gtvnfatktl.html

[T11] Kotlin：协程
来源：http://hz.yuxming.cn/gttkjkqkfw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yueranfly.top/gtdkifkuev.html

[T12] Kotlin：解构声明
来源：http://hz.zhengqikj.top/gtehitjymy.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gtmesmmwez.html

[T13] Kotlin：只读 Map
来源：http://hz.wangshuangyany.cn/gtgqlrmroj.html

val m = mapOf("a" to 1)
来源：http://hz.feifeiyinyue.top/gtzqdvpomq.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtzvkklhzc.html

for (i in 1..10) println(i)
来源：http://hz.fengsongda.top/gtcnxgholq.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtzjftpkjz.html

interface Shape { fun area(): Double }
来源：http://hz.vqdsnc.cn/gtugwricqz.html

[T16] Swift：Hello World
来源：http://hz.jinqigufen.top/gtglxlmulb.html

print("Hello")
来源：http://hz.dianchejie.cn/gtbmmmuuro.html

[T17] Swift：变量与常量
来源：http://hz.ybcxt.top/gtcgjvbnpt.html

var a = 1;  let b = 2
来源：http://hz.kuanghao11.cn/gtlnzdipvt.html

[T18] Swift：字符串插值
来源：http://hz.birdmap.top/gtmtlacaqx.html

"值: \(b)"
来源：http://hz.jyoumei.cn/gtyouuplxp.html

[T19] Swift：可选绑定
来源：http://hz.52xcode.cn/gtmvtchugp.html

if let n = opt { print(n) }
来源：http://hz.xingfuxueyuan.xyz/gtscdpiemr.html

[T20] Swift：数组操作
来源：http://hz.ivvv.top/gtutgmknek.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtxnnpxtwf.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtojtaknbl.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtueqegnqo.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gtnbpqdhlo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenjidiqi.icu/gtnayuxnzz.html

[T23] Swift：函数
来源：http://hz.tanke756.top/gtcfuqgcml.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.bjfxy.top/gtgcohjjzr.html

[T24] Swift：闭包
来源：http://hz.daxiang520.top/gtqfivzwxb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj202588.top/gtzcalepsh.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gtwqrexeda.html

struct P { var x: Int }
来源：http://hz.ydzc1.top/gteqgnaeoc.html

[T26] Swift：类与重写
来源：http://hz.zhengqikj.top/gtmqzbztjn.html

class A: Base { override func f() {} }
来源：http://hz.hnxiangtu.top/gtqxehqogi.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gtzocythuz.html

do { try f() } catch { print(error) }
来源：http://hz.hnxiangtu.top/gturmqebna.html

[T28] Swift：枚举
来源：http://hz.ybcxt.top/gtgajolpig.html

enum Color { case red, green }
来源：http://hz.wangdashe.top/gtgggiitat.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gtyanyhpsk.html

guard let x = opt else { return }
来源：http://hz.c1oappe.top/gtjgxzjadm.html

[T30] Swift：协议
来源：http://hz.yangfankeji.com/gtwlkxwysb.html

protocol Shape { func area() -> Double }
来源：http://hz.svipenyu.cn/gtjkzttoxx.html

[T31] Lua：Hello World
来源：http://hz.yuxming.cn/gteglivghy.html

print("Hello")
来源：http://hz.zhixingplan.top/gthgkrfpcn.html

[T32] Lua：局部变量
来源：http://hz.aibaodan.cn/gtquwjwqnu.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtmuilkvzt.html

[T33] Lua：表（数组）
来源：http://hz.yueranfly.top/gtntzjbvor.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jiagoushi.top/gtldwflbpa.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtrwpqbvqw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtvabwejyp.html

[T35] Lua：字典表
来源：http://hz.xziqi.cn/gteespobpz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hnqzz.top/gtxibtefsj.html

[T36] Lua：函数
来源：http://hz.ppjwa.cn/gttslmofvr.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtyllicrno.html

[T37] Lua：字符串拼接
来源：http://hz.ybcxt.top/gtotwbhbfp.html

"a" .. "b"
来源：http://hz.tian-w.cn/gtlzrevyxo.html

[T38] Lua：条件
来源：http://hz.zhiwuduotai.top/gtgsfsnyen.html

if x > 0 then print("正") end
来源：http://hz.yj20258.top/gtkiwoxetl.html

[T39] Lua：模式匹配
来源：http://hz.jinghuilouyu.cn/gtjwyailie.html

string.find(s, "%d+")
来源：http://hz.aizwys.cn/gtdzytqtih.html

[T40] Lua：元表
来源：http://hz.shzxlz.cn/gtwkvgkfrf.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtulxvjwld.html

[T41] Perl：Hello World
来源：http://hz.yuanzhike.top/gtbfnxiafj.html

print "Hello\n";
来源：http://hz.xylfe.cn/gtdyxziblh.html

[T42] Perl：变量类型
来源：http://hz.pengpengdd.cyou/gtkzxalhjz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jianghu66.top/gthxytsihg.html

[T43] Perl：字符串插值
来源：http://hz.nanxinkj.top/gtsobpogwu.html

"值: $a"
来源：http://hz.svipenyu.cn/gtxoufsygy.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gttsvovgou.html

if ($a > 0) { print "正"; }
来源：http://hz.tanke756.top/gtystffhqr.html

[T45] Perl：数组遍历
来源：http://hz.ivvv.top/gtibdcspko.html

for my $x (@arr) { print $x; }
来源：http://hz.mhx1999.top/gtwecknwem.html

[T46] Perl：哈希操作
来源：http://hz.52xcode.cn/gtcccdcigy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ivvv.top/gtfqtwvnjf.html

[T47] Perl：正则捕获
来源：http://hz.cqqwz.cn/gtxmmqznrt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.52xcode.cn/gtobabjeed.html

[T48] Perl：正则替换
来源：http://hz.zhiwuduotai.top/gtkfjkbnka.html

$s =~ s/old/new/g;
来源：http://hz.dashuyun.cn/gtoitjunxg.html

[T49] Perl：函数
来源：http://hz.tian-w.cn/gtftmqipkn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tianlin.xyz/gtewzsimmm.html

[T50] Perl：逐行读文件
来源：http://hz.mhx1999.top/gtrtuqoncc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtnckuwcjf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.andypj.xyz/gtkeprsqwb.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangkeji.top/gtkitpxhek.html

println("Hello")
来源：http://hz.yonumen.top/gtmlxfppbz.html

[T52] Scala：变量
来源：http://hz.cheryme.top/gtxkvjogug.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtwnfgfedy.html

[T53] Scala：字符串插值
来源：http://hz.nanxuanxn.top/gtxzfdpqau.html

s"值: $b"
来源：http://hz.yj202588.top/gteezzbjxv.html

[T54] Scala：集合映射
来源：http://hz.daxiang520.top/gtdjgemagp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangshuangyany.cn/gtxhprxfai.html

[T55] Scala：集合过滤
来源：http://hz.jqgufenzy.top/gtyztpqcyv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenjidiqi.icu/gtccdsvrnk.html

[T56] Scala：样例类
来源：http://hz.ydjk.org.cn/gtvljnjyhk.html

case class User(name: String, age: Int)
来源：http://hz.cashguo.top/gtvaeverjo.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gtrozkuoks.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ehwqpu.com/gtqyluztyp.html

[T58] Scala：函数定义
来源：http://hz.daria6918.cn/gtwzmfezsj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenzaomai.com/gtsncynbcw.html

[T59] Scala：循环
来源：http://hz.jinqigfzy.top/gtfmagouew.html

for (i <- 1 to 10) println(i)
来源：http://hz.yvedp.cn/gtjfwiuovh.html

[T60] Scala：折叠
来源：http://hz.zhoulong.xyz/gtowttkavb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydjk.org.cn/gtwvlbmhal.html

================================================================================
来源：http://hz.svipenyu.cn/gtzbamtypu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtptbgisbe.html

================================================================================
来源：http://hz.jqgfzy.top/gtrsrjttuy.html

[U01] Py：创建虚拟环境
来源：http://hz.havefunace.top/gtbnbfgych.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangtech.top/gtoivxsmps.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangtech.top/gtzsicunjk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cucudq.cn/gtjyynkgsn.html

[U03] Py：加载 .env 配置
来源：http://hz.zhongyouzk.top/gteimdvzhq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhoulong.xyz/gtdskqsflj.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gthjxgixuv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sufxvd.cn/gtgjrtfdyq.html

[U05] Py：列表去重且保序
来源：http://hz.gotoacloud.top/gtnrhzjzmz.html

list(dict.fromkeys(arr))
来源：http://hz.ppjwa.cn/gtdhhozgoz.html

[U06] Py：合并两个字典
来源：http://hz.tanke756.top/gtglfpksxw.html

{**a, **b}
来源：http://hz.birdmap.top/gtdpzlwtgu.html

[U07] Py：反转字典键值
来源：http://hz.quarkkingdee.top/gtjixojilu.html

{v: k for k, v in d.items()}
来源：http://hz.shanyushiyangkeji.top/gtmwlynndo.html

[U08] Py：展平二维列表
来源：http://hz.sxryk.cn/gtbmcfhkxf.html

[y for x in nested for y in x]
来源：http://hz.hfpthk.cn/gtlssvokdl.html

[U09] Py：字典取最大值的键
来源：http://hz.sufxvd.cn/gtswbfcnuf.html

max(d, key=d.get)
来源：http://hz.xuanzx.com/gtqqbwxohx.html

[U10] Py：按值排序字典
来源：http://hz.hongshengwenyu.top/gtpzvlebzp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.daria6918.cn/gtsffemhxr.html

[U11] Py：生成器表达式
来源：http://hz.daxiang520.top/gtrixdtmkg.html

(x * 2 for x in arr)
来源：http://hz.sweek.top/gtjhmrzfrw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhoulong.xyz/gthtjowpeh.html

Counter(arr).most_common(3)
来源：http://hz.feifeiyinyue.top/gtwlrklrzk.html


<!-- 参考信息 -->