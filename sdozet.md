代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.kuanghao11.cn/gtcybsvcgo.html

[R72] 等待端口就绪
来源：http://hz.daxiang520.top/gtkcdokcva.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtggwupvqv.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gtuzgvhtbz.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtxfwhqpck.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gthalheivu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtzoavtngc.html

[R75] 导出环境变量
来源：http://hz.xuanzx.com/gtegekzcqd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pycfn.com/gtlhxjkmhc.html

[R76] 使用临时文件
来源：http://hz.meibo888.top/gtiqnnixvj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtwziyjaxq.html

[R77] 读取用户输入
来源：http://hz.vqdsnc.cn/gtsgvoockn.html

read -rp "请输入: " ans
来源：http://hz.hfpthk.cn/gthlyplubv.html

[R78] 交互式菜单
来源：http://hz.sxryk.cn/gtdqkngyes.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cqqwz.cn/gttiilcjop.html

[R79] 解析命令行选项
来源：http://hz.yvedp.cn/gtsnbdgtgm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtyvkztwtl.html

[R80] 查看脚本执行耗时
来源：http://hz.ydzc1.top/gtoluuifco.html

time ./run.sh
来源：http://hz.daxiang520.top/gtygkufuzp.html

================================================================================
来源：http://hz.ivvv.top/gtbuuctldi.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtfinmanyd.html

================================================================================
来源：http://hz.yuanzhike.top/gtdlnvuymf.html

[S01] C：Hello World
来源：http://hz.xinyue.icu/gtlrznziqc.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtoqqyizat.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhoulong.xyz/gtwgvxihgh.html

[S02] C：变量与格式化输出
来源：http://hz.ywan-chungtsiang.top/gtlnzyhqsw.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gtqrxaalhv.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gtvmpcnulk.html

int x; scanf("%d", &x);
来源：http://hz.fengsongda.top/gtpfeozhwz.html

[S04] C：字符串复制
来源：http://hz.jinqigufen.top/gtkbsvofch.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenzaomai.com/gtohwrwtgm.html

[S05] C：字符串长度
来源：http://hz.kuanghao11.cn/gthtirssam.html

strlen(s)
来源：http://hz.shzxlz.cn/gtyzxtlboh.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangtech.top/gtnwxpeiwi.html

strcmp(a, b) == 0
来源：http://hz.zdqjudy.top/gtmyidudaz.html

[S07] C：数组遍历求和
来源：http://hz.sweek.top/gtwuujufum.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pengpengdd.cyou/gtjfujfemc.html

[S08] C：动态内存分配与释放
来源：http://hz.yj202588.top/gtsmxnbpag.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtsehxjerx.html

[S09] C：结构体定义与初始化
来源：http://hz.havefunace.top/gtgrmziufe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gogol.net.cn/gtnnwxtpaf.html

[S10] C：指针与解引用
来源：http://hz.yonumen.top/gtylzpgels.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtzvnuaxtx.html

[S11] C：逐行读文件
来源：http://hz.ppjwa.cn/gtkpwoatrf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydjk.org.cn/gtcrbxvgmc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gtdrsrgbxm.html

fclose(f);
来源：http://hz.ivvv.top/gtuuyxfoep.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtbokqvvqa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtvrfaxycy.html

[S13] C：宏定义
来源：http://hz.xuetiantiany.cn/gtiedtosov.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sysykeji.top/gtwzlsxdll.html

[S14] C：枚举
来源：http://hz.yonumen.top/gtphamkijd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gthbkmmoso.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtqbcdxyii.html

(double) a / b
来源：http://hz.havefunace.top/gtzrraetyx.html

[S16] C：位操作置位
来源：http://hz.jiagoushi.top/gtufdltuqw.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtmijcnlrn.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtqdkplnde.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daria6918.cn/gttyfuerlh.html

[S18] C：命令行参数
来源：http://hz.aizwys.cn/gtegcllnzf.html

int main(int argc, char **argv)
来源：http://hz.chenjidiqi.icu/gtyssndbjt.html

[S19] C：快速排序
来源：http://hz.jqgufenzy.top/gtqemzllop.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtibvmwxbi.html

[S20] C：二分查找
来源：http://hz.ehwqpu.com/gtdnrfjbhw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gttzvnnglv.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangtech.top/gtulirzbdk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aibaodan.cn/gtwzdainfm.html

[S22] C：字符串转数字
来源：http://hz.ybcxt.top/gtktgunpps.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gthosvzpvp.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtamsasspq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtcpwojuyj.html

[S24] C：获取本地时间
来源：http://hz.sufxvd.cn/gtrgfwdmud.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gtzoxybrnc.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gtetgshsbv.html

memcpy(dst, src, n);
来源：http://hz.vqdsnc.cn/gtslznluqs.html

[S26] C：内存清零
来源：http://hz.havefunace.top/gtcvvykdmz.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtcxnyogjv.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtzhpzudxy.html

const double PI = 3.14159;
来源：http://hz.hammf.cn/gtyurwefly.html

[S28] C：静态变量
来源：http://hz.tanke756.top/gtxsrfdpyc.html

static int counter = 0;
来源：http://hz.yuxming.cn/gtppwkiydc.html

[S29] C：变参函数
来源：http://hz.xingfuxueyuan.xyz/gtbskelbci.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.meibo888.top/gtxglouflz.html

[S30] C：头文件保护
来源：http://hz.xziqi.cn/gtcqdsrsef.html

#ifndef X_H
来源：http://hz.sweek.top/gtktqkkomt.html

#define X_H
来源：http://hz.cucudq.cn/gtpjyidztc.html

#endif
来源：http://hz.pycfn.com/gtfnbfaqlm.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtgmfwkdrn.html

#include <iostream>
来源：http://hz.guannengcc.top/gtlrqbmtyn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ivvv.top/gtsuhwghbf.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtopqjhhtp.html

std::string s = "hi";  s += "!";
来源：http://hz.smart0.xyz/gtegjrvtyq.html

[S33] C++：vector 增删
来源：http://hz.kuanghao11.cn/gtzvlqpjbl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yueranfly.top/gtlfpajhoh.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gttoqtvnzf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtlqcxmxyt.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtvyahmswr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtihkdahqg.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtigashjpk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtqzrrspno.html

[S37] C++：set
来源：http://hz.fengsongda.top/gtyihxvivd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sweek.top/gtmqepwxxy.html

[S38] C++：排序
来源：http://hz.ydzc1.top/gtveiyktsx.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtdrickhyz.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtrhsjqogo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aibaodan.cn/gtxbhmhnwc.html

[S40] C++：查找元素
来源：http://hz.snrcjt.cn/gtqwlqtiae.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangkeji.top/gtgdlaspcf.html

[S41] C++：类与构造函数
来源：http://hz.ybcxt.top/gthjxujuzr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yvedp.cn/gtunntuzfp.html

[S42] C++：继承与虚函数
来源：http://hz.guannengcc.top/gtfhppzzbj.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtxohkgdlu.html

[S43] C++：智能指针
来源：http://hz.cheryme.top/gtietrgihq.html

auto p = std::make_unique<int>(5);
来源：http://hz.mhx1999.top/gtoxatkrbo.html

[S44] C++：引用传参
来源：http://hz.cqqwz.cn/gtgkqbjgxi.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtfgiblyxj.html

[S45] C++：lambda
来源：http://hz.gotoacloud.top/gtggkmcyzz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xingfuxueyuan.xyz/gtcxuyduom.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtgfszweat.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ivvv.top/gtphayxwcr.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhixingplan.top/gtmnklhduf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtcnempsrw.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gttpesapum.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhengqikj.top/gtqojymaia.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangkeji.top/gtedsyfjqc.html

[S49] C++：写文件
来源：http://hz.meibo888.top/gtuzneqinl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.redwolf501.top/gtedqdwuvy.html

[S50] C++：格式化数字
来源：http://hz.aibaodan.cn/gtglsfqrjr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gtlomsnsuk.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtzmwwwjqc.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtwtmelfsf.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gtacqtitcw.html

int size() const noexcept { return n_; }
来源：http://hz.zdqjudy.top/gtdyahlqsi.html

[S53] C++：移动语义
来源：http://hz.ppjwa.cn/gtbbjcvpoi.html

std::vector<int> w = std::move(v);
来源：http://hz.kuanghao11.cn/gtazeiohnd.html

[S54] C++：异常处理
来源：http://hz.zhaomingkeji.xyz/gtesigqgow.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydjk.org.cn/gtulzvutvl.html

[S55] C++：结构化绑定
来源：http://hz.dashuyun.cn/gtzmdgxoic.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtsoqgivxe.html

[S56] C++：optional
来源：http://hz.jianghu66.top/gtlspkpvmg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtxredyizj.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtwovkahdz.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtwlubjhos.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtjujniuet.html

namespace ns { int f() { return 1; } }
来源：http://hz.smart0.xyz/gtogkvgrzw.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtdiogecdp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pengpengdd.cyou/gtxlpbkmaj.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtjgcdwaxz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gtjnmgolib.html

================================================================================
来源：http://hz.hywenlv.cn/gttcasjfvk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtkaxbavuo.html

================================================================================
来源：http://hz.meibo888.top/gtnbotstbu.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtvnebptrc.html

println("Hello")
来源：http://hz.ybcxt.top/gtxmqkowij.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtbiolwumv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daria6918.cn/gtcohxizkz.html

[T03] Kotlin：字符串模板
来源：http://hz.yueranfly.top/gtonfnhrnp.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gtiancnfaa.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtttoekabi.html

val n: String? = null;  n?.length
来源：http://hz.xingfuxueyuan.xyz/gtimbubtcj.html

[T05] Kotlin：when 表达式
来源：http://hz.yuanzhike.top/gtnhmprqhz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtlyleyibx.html

[T06] Kotlin：集合映射
来源：http://hz.xuetiantiany.cn/gthariyifz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.svipenyu.cn/gtfhkrclnk.html

[T07] Kotlin：集合过滤
来源：http://hz.yanxiufei.cn/gtrzgztrof.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shuidangran.top/gtbxvwovft.html

[T08] Kotlin：数据类
来源：http://hz.jqgufenzy.top/gtdqzeawwr.html

data class User(val name: String, val age: Int)
来源：http://hz.sweek.top/gtjbjokoyy.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtrkiledud.html

fun String.exclaim() = this + "!"
来源：http://hz.ppjwa.cn/gtobkptktp.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258888.top/gtjqjdjlrs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tianlin.xyz/gtrjwbmfmd.html

[T11] Kotlin：协程
来源：http://hz.zhongyouzk.top/gtyabhlfox.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gtblmzjxeq.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gtktivaogq.html

val (a, b) = Pair(1, 2)
来源：http://hz.gotoacloud.top/gtjvabyuyz.html

[T13] Kotlin：只读 Map
来源：http://hz.sxryk.cn/gtirgojnge.html

val m = mapOf("a" to 1)
来源：http://hz.mhx1999.top/gtyoislmtx.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtrftoeerr.html

for (i in 1..10) println(i)
来源：http://hz.meibo888.top/gtfdujcclf.html

[T15] Kotlin：接口
来源：http://hz.cdnleiting.top/gtexogkahn.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtomfvzhrb.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gtsbsymyrl.html

print("Hello")
来源：http://hz.ehwqpu.com/gtabsuyfkg.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtouzmqqgi.html

var a = 1;  let b = 2
来源：http://hz.jinyuanbaomall.cn/gtziesxshi.html

[T18] Swift：字符串插值
来源：http://hz.ivvv.top/gtfencfyuo.html

"值: \(b)"
来源：http://hz.mhx1999.top/gtmuhwgiyl.html

[T19] Swift：可选绑定
来源：http://hz.wangshuangyany.cn/gtmnxcgpvi.html

if let n = opt { print(n) }
来源：http://hz.aibaodan.cn/gtizjggqsr.html

[T20] Swift：数组操作
来源：http://hz.dashuyun.cn/gtqzyunufh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xziqi.cn/gtodtptnff.html

[T21] Swift：遍历
来源：http://hz.sxryk.cn/gtjvxhlrgv.html

for x in a { print(x) }
来源：http://hz.wangshuangyany.cn/gtuipmamfj.html

[T22] Swift：字典
来源：http://hz.vqdsnc.cn/gttsepeubm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtzaxlybje.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtixjdhqho.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ybcxt.top/gtlmdgpggc.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gteggbthnu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnxiangtu.top/gtxpbfuwhz.html

[T25] Swift：结构体
来源：http://hz.shangyingyoupin.top/gtftermleb.html

struct P { var x: Int }
来源：http://hz.0kj1m.cn/gtumjjvvtz.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtccgtguka.html

class A: Base { override func f() {} }
来源：http://hz.xylfe.cn/gtttcgobby.html

[T27] Swift：错误处理
来源：http://hz.tian-w.cn/gtqhlwdshp.html

do { try f() } catch { print(error) }
来源：http://hz.chenlongwang.top/gtmhadcmrm.html

[T28] Swift：枚举
来源：http://hz.zhixingplan.top/gtovtkotuo.html

enum Color { case red, green }
来源：http://hz.ppjwa.cn/gtmeksecyn.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtfhmbdeut.html

guard let x = opt else { return }
来源：http://hz.dianchejie.cn/gtgikgdqzo.html

[T30] Swift：协议
来源：http://hz.ehwqpu.com/gtijnfwaeh.html

protocol Shape { func area() -> Double }
来源：http://hz.aibaodan.cn/gtbnzqzogx.html

[T31] Lua：Hello World
来源：http://hz.cucudq.cn/gtdxjqqlwy.html

print("Hello")
来源：http://hz.ydzc1.top/gtgyepaygu.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtslhgfakh.html

local a = 1
来源：http://hz.wangshuangyany.cn/gtozyfpimr.html

[T33] Lua：表（数组）
来源：http://hz.sysykeji.top/gtoitnuzhd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinghuilouyu.cn/gtoyiqxyfn.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtfnuabyvm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shzxlz.cn/gtiiwdnxyb.html

[T35] Lua：字典表
来源：http://hz.zdqjudy.top/gtfrbswppp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pycfn.com/gtfuuhpuge.html

[T36] Lua：函数
来源：http://hz.xziqi.cn/gttcnfsdjk.html

function add(a, b) return a + b end
来源：http://hz.hammf.cn/gthuezfumr.html

[T37] Lua：字符串拼接
来源：http://hz.sufxvd.cn/gtszmkgohe.html

"a" .. "b"
来源：http://hz.cdnleiting.top/gtbaetbgou.html

[T38] Lua：条件
来源：http://hz.redwolf501.top/gtdcxzrzph.html

if x > 0 then print("正") end
来源：http://hz.xinyue.icu/gtgwpadnpe.html

[T39] Lua：模式匹配
来源：http://hz.hnqzz.top/gtrndsnqmg.html

string.find(s, "%d+")
来源：http://hz.sweek.top/gtbdddrgiy.html

[T40] Lua：元表
来源：http://hz.jqgfzy.top/gtelqiqlei.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtfomujvef.html

[T41] Perl：Hello World
来源：http://hz.ydzc1.top/gtlnxrogzs.html

print "Hello\n";
来源：http://hz.yuanzhike.top/gtrzvzaiwd.html

[T42] Perl：变量类型
来源：http://hz.ehwqpu.com/gtcxrrbghs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zycfv.cn/gtthxsawll.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gthhhdrajb.html

"值: $a"
来源：http://hz.52xcode.cn/gtddfllgdw.html

[T44] Perl：条件
来源：http://hz.chenlongwang.top/gtxckzqejy.html

if ($a > 0) { print "正"; }
来源：http://hz.havefunace.top/gthgzhqtzz.html

[T45] Perl：数组遍历
来源：http://hz.zhixingplan.top/gtmriqcpas.html

for my $x (@arr) { print $x; }
来源：http://hz.haohaochexian.top/gtzaofdtmh.html

[T46] Perl：哈希操作
来源：http://hz.dianchejie.cn/gtfwjqynhg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zycfv.cn/gtwjurnfic.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gthwfdojqx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sweek.top/gtzarotpss.html

[T48] Perl：正则替换
来源：http://hz.tanke756.top/gtffyausxj.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gthevoboob.html

[T49] Perl：函数
来源：http://hz.chenjidiqi.icu/gtkjwscbxb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.wangdashe.top/gtzeuvupam.html

[T50] Perl：逐行读文件
来源：http://hz.nanxuanxn.top/gtdhshzgdj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigfzy.top/gtqheycuwh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.kuanghao11.cn/gtvlagfdjb.html

[T51] Scala：Hello World
来源：http://hz.jlsjyb.cn/gtfigbrbrg.html

println("Hello")
来源：http://hz.zdqjudy.top/gtwrtodvdf.html

[T52] Scala：变量
来源：http://hz.yj20258.top/gtlkcoxshf.html

val a = 1;  var b = 2
来源：http://hz.hysaishi.cn/gtsunujcno.html

[T53] Scala：字符串插值
来源：http://hz.havefunace.top/gtqjavdlbz.html

s"值: $b"
来源：http://hz.yj202588.top/gtqsvpcrua.html

[T54] Scala：集合映射
来源：http://hz.nanxinkj.top/gtaowuhxxs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ppjwa.cn/gtipreopkt.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gthyyxbkaj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ivvv.top/gtzkgsojzm.html

[T56] Scala：样例类
来源：http://hz.iojbl.cn/gtxxrrboej.html

case class User(name: String, age: Int)
来源：http://hz.zhixingplan.top/gtzicsrdbs.html

[T57] Scala：模式匹配
来源：http://hz.wangshuangyany.cn/gtrqjlqxfc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.bjfxy.top/gtktezqlmx.html

[T58] Scala：函数定义
来源：http://hz.pengpengdd.cyou/gtdydxqugp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.9152youxi.cn/gtbrcdmwej.html

[T59] Scala：循环
来源：http://hz.hysaishi.cn/gtdwjdvuwy.html

for (i <- 1 to 10) println(i)
来源：http://hz.xylfe.cn/gtvzsjjiwz.html

[T60] Scala：折叠
来源：http://hz.jinyuanbaomall.cn/gtlkhjvrga.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hywenlv.cn/gtmzdutfud.html

================================================================================
来源：http://hz.sufxvd.cn/gtljxbswlj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhixingplan.top/gtijtmqzve.html

================================================================================
来源：http://hz.zhengqikj.top/gtmtlwnkpp.html

[U01] Py：创建虚拟环境
来源：http://hz.yuxming.cn/gttddmokhj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgfzy.top/gtcbucydsr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gtxqnvxirj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenlongwang.top/gtkzqoizti.html

[U03] Py：加载 .env 配置
来源：http://hz.chenlongwang.top/gtinvlvzbm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jlsjyb.cn/gtuabuyfik.html

[U04] Py：变量调试打印
来源：http://hz.xingfuxueyuan.xyz/gtqtkpathn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.c1oappe.top/gtmoxzyjyh.html

[U05] Py：列表去重且保序
来源：http://hz.meibo888.top/gtdtpejzna.html

list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtpcyjwqna.html

[U06] Py：合并两个字典
来源：http://hz.yvedp.cn/gtkjwimgwn.html

{**a, **b}
来源：http://hz.shanyushiyangkeji.top/gttbaisdhe.html

[U07] Py：反转字典键值
来源：http://hz.xinyue.icu/gtjkdlsxph.html

{v: k for k, v in d.items()}
来源：http://hz.nwbrower.top/gtyqpjfofx.html

[U08] Py：展平二维列表
来源：http://hz.ivvv.top/gtnjxpjcsy.html

[y for x in nested for y in x]
来源：http://hz.dianchejie.cn/gthtqjgban.html

[U09] Py：字典取最大值的键
来源：http://hz.andypj.xyz/gtvrohooxp.html

max(d, key=d.get)
来源：http://hz.bjfxy.top/gtsdlgvjyi.html

[U10] Py：按值排序字典
来源：http://hz.yanxiufei.cn/gtazdbwmnn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj20258888.top/gthghyojuk.html

[U11] Py：生成器表达式
来源：http://hz.iojbl.cn/gtzxycvzyz.html

(x * 2 for x in arr)
来源：http://hz.meibo888.top/gtucwmjrkb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258888.top/gtigraytfv.html

Counter(arr).most_common(3)
来源：http://hz.shanyushiyangkeji.top/gtfnliawgz.html


<!-- 参考信息 -->