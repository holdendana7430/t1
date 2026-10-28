代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jyoumei.cn/gtjnkuahbq.html

[R80] 查看脚本执行耗时
来源：http://hz.haohaochexian.top/gthxudvkxy.html

time ./run.sh
来源：http://hz.bjfxy.top/gtdjihpwlx.html

================================================================================
来源：http://hz.yangfankeji.com/gtcuqmgxve.html

S. C / C++ 专题
来源：http://hz.xinyue.icu/gtrwmopfqe.html

================================================================================
来源：http://hz.zycfv.cn/gtbdxvjoey.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtqbudgvph.html

#include <stdio.h>
来源：http://hz.chenzaomai.com/gtyhiblhjb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yonumen.top/gtdhvyzmqd.html

[S02] C：变量与格式化输出
来源：http://hz.zycfv.cn/gtlswtqikk.html

int a = 10; printf("%d\n", a);
来源：http://hz.cheryme.top/gtmcqckpvg.html

[S03] C：读入整数
来源：http://hz.jqgfzy.top/gtbbjrckcd.html

int x; scanf("%d", &x);
来源：http://hz.hammf.cn/gthvcmpbrp.html

[S04] C：字符串复制
来源：http://hz.cdnleiting.top/gtqtmgjucq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtqpcgtuxb.html

[S05] C：字符串长度
来源：http://hz.ydzc1.top/gtkzwzeclz.html

strlen(s)
来源：http://hz.nanxinkj.top/gtmfhlvmle.html

[S06] C：字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtvnbyhshl.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtwgwjzecl.html

[S07] C：数组遍历求和
来源：http://hz.jinghuilouyu.cn/gtveekzody.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xinyue.icu/gtgqrijtby.html

[S08] C：动态内存分配与释放
来源：http://hz.cucudq.cn/gtpnndhvfm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.havefunace.top/gthchjnpuj.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gttembpojn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gtbobknjyg.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtljtlnpdf.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtcbgzkamb.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtcsuhnjcu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtlacxmsvx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtnuwignix.html

fclose(f);
来源：http://hz.yonumen.top/gtbokhxsuq.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gtzwstdmjp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sxryk.cn/gttcfqqbjw.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gtyagcgnej.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtfiysgihr.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtnbvonqns.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hysaishi.cn/gtcminwyyr.html

[S15] C：类型转换
来源：http://hz.yuanzhike.top/gtuijxekud.html

(double) a / b
来源：http://hz.0kj1m.cn/gtecuynvzm.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gttlwsndrn.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gtctkbwauj.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtjlxcpavi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.andypj.xyz/gtbjupgwqa.html

[S18] C：命令行参数
来源：http://hz.wangdashe.top/gtonrixvqu.html

int main(int argc, char **argv)
来源：http://hz.birdmap.top/gtcsgtcclo.html

[S19] C：快速排序
来源：http://hz.xingfuxueyuan.xyz/gtxbwdwzwi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtbavardui.html

[S20] C：二分查找
来源：http://hz.gzhubu.top/gtcqstrytw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtlbeibelk.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gtbhdzfvbp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tian-w.cn/gtjwfqsrqs.html

[S22] C：字符串转数字
来源：http://hz.jqgufenzy.top/gtikbecjal.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.birdmap.top/gtclkdhbws.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gtuibfttlk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sxryk.cn/gtfexarqwt.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gttjaxfnrb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gtuzbhvpuw.html

[S25] C：内存拷贝
来源：http://hz.aibaodan.cn/gtkgstnfqt.html

memcpy(dst, src, n);
来源：http://hz.sufxvd.cn/gtbkaobwei.html

[S26] C：内存清零
来源：http://hz.jianghu66.top/gtydsrhpqm.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtilhxfyib.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtixtqkafa.html

const double PI = 3.14159;
来源：http://hz.hywenlv.cn/gtgmdzpkfu.html

[S28] C：静态变量
来源：http://hz.316326.xyz/gtyybtprxa.html

static int counter = 0;
来源：http://hz.feifeiyinyue.top/gtptvhujyv.html

[S29] C：变参函数
来源：http://hz.xziqi.cn/gttyabhqbh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhoulong.xyz/gtkfmvffza.html

[S30] C：头文件保护
来源：http://hz.pycfn.com/gtsslcjvqz.html

#ifndef X_H
来源：http://hz.jqgfzy.top/gtczsrtanx.html

#define X_H
来源：http://hz.xuanzx.com/gtirglhidq.html

#endif
来源：http://hz.nwbrower.top/gtvsevfjre.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtowgnvvtd.html

#include <iostream>
来源：http://hz.zhijiandao.cn/gtsjxilvli.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtdylynfjl.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtiexmdmgy.html

std::string s = "hi";  s += "!";
来源：http://hz.snrcjt.cn/gtmlrnfzhr.html

[S33] C++：vector 增删
来源：http://hz.mhx1999.top/gtvkthelpy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhongyouzk.top/gtvjeweyxo.html

[S34] C++：遍历 vector
来源：http://hz.zhixingplan.top/gtdilmnihf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hammf.cn/gtlawrafxq.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtysnwqhbf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtepgguumf.html

[S36] C++：unordered_map
来源：http://hz.havefunace.top/gtruxxeony.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtqfpxntkk.html

[S37] C++：set
来源：http://hz.sufxvd.cn/gtkzngdnio.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtnwrwzpxp.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtviytjjma.html

std::sort(v.begin(), v.end());
来源：http://hz.jianghu66.top/gtigttjdtf.html

[S39] C++：自定义比较器排序
来源：http://hz.chenlongwang.top/gtkjexwglb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtwbzyypiw.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtmfxpcywl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangtech.top/gtxikusieq.html

[S41] C++：类与构造函数
来源：http://hz.hnxiangtu.top/gtgcvfazrx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhengqikj.top/gtfxwiiocd.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtvhnutfgl.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtcmcceoyr.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtwjkmuanq.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258888.top/gtaydeipgm.html

[S44] C++：引用传参
来源：http://hz.iojbl.cn/gtomgwqook.html

void inc(int &x) { ++x; }
来源：http://hz.pengpengdd.cyou/gtpoykdqvv.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gtpvnxwrng.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xziqi.cn/gtqlkdpvxl.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtqoxeextl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgufenzy.top/gtmebmjiqr.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtgpgahhgi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jiagoushi.top/gtnivlbzsd.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtrolxkpnz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtkrquszzd.html

while (std::getline(in, line)) { }
来源：http://hz.gaohongyu789.top/gtmvnvsntt.html

[S49] C++：写文件
来源：http://hz.jlsjyb.cn/gtdwqiqxvn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtqmrhncyt.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtiucvpeir.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guannengcc.top/gtkhmgttxr.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangtech.top/gtabrenbzb.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtjohctqii.html

[S52] C++：const 与 noexcept
来源：http://hz.smart0.xyz/gtfupbzkjt.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtvtohiybf.html

[S53] C++：移动语义
来源：http://hz.cqqwz.cn/gtbaeyuuui.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gtewzttmxg.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gthoajvuqg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.316326.xyz/gtjajptgct.html

[S55] C++：结构化绑定
来源：http://hz.hongshengwenyu.top/gtzkfobqkw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dianchejie.cn/gtyzjqedwx.html

[S56] C++：optional
来源：http://hz.bjfxy.top/gtcklkutmz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gtauqwzjni.html

[S57] C++：编译期常量
来源：http://hz.tianlin.xyz/gtlbgdqqsg.html

constexpr int N = 10;
来源：http://hz.hongshengwenyu.top/gtjgjqzxcw.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gtnpjrprfp.html

namespace ns { int f() { return 1; } }
来源：http://hz.kuanghao11.cn/gtqmgbqqub.html

[S59] C++：静态断言
来源：http://hz.zdqjudy.top/gtbbwrbyrt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtzwqqgsmf.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtmhcttsbp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtshsosgiu.html

================================================================================
来源：http://hz.yanxiufei.cn/gttwbmaaqe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.redwolf501.top/gtvcpqskse.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlcwweget.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtzpswbqxy.html

println("Hello")
来源：http://hz.cheryme.top/gthyodbscs.html

[T02] Kotlin：变量
来源：http://hz.hnqzz.top/gtkgeyovhq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtmohfvkga.html

[T03] Kotlin：字符串模板
来源：http://hz.cashguo.top/gtdqsrhghe.html

"值: $b"
来源：http://hz.dianchejie.cn/gtsifroixx.html

[T04] Kotlin：空安全
来源：http://hz.hfpthk.cn/gtsnnalzub.html

val n: String? = null;  n?.length
来源：http://hz.havefunace.top/gtnpnvhunf.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gtcrlpdnpe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtshkyzzsy.html

[T06] Kotlin：集合映射
来源：http://hz.xuanzx.com/gtvlkvkubp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jyoumei.cn/gtcxxistoq.html

[T07] Kotlin：集合过滤
来源：http://hz.tianlin.xyz/gtiepzxlxh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangdashe.top/gtezecfjfh.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtoljcrokf.html

data class User(val name: String, val age: Int)
来源：http://hz.xuetiantiany.cn/gtjzloghga.html

[T09] Kotlin：扩展函数
来源：http://hz.xinyue.icu/gtuhojwjyr.html

fun String.exclaim() = this + "!"
来源：http://hz.quarkkingdee.top/gtyzrxglou.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigfzy.top/gtdfcfpyjb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hysaishi.cn/gtiloqwqmc.html

[T11] Kotlin：协程
来源：http://hz.yuxming.cn/gtdzhhkddz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aibaodan.cn/gtvozjcdkm.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtbukytuks.html

val (a, b) = Pair(1, 2)
来源：http://hz.andypj.xyz/gtemdbrffa.html

[T13] Kotlin：只读 Map
来源：http://hz.cheryme.top/gtsnwfheih.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtovfwoums.html

[T14] Kotlin：循环
来源：http://hz.yanxiufei.cn/gtpukoebno.html

for (i in 1..10) println(i)
来源：http://hz.yuxming.cn/gtulsoogwy.html

[T15] Kotlin：接口
来源：http://hz.yvedp.cn/gtinhfxjca.html

interface Shape { fun area(): Double }
来源：http://hz.chenlongwang.top/gtquwedhaa.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtebtocjiv.html

print("Hello")
来源：http://hz.fengsongda.top/gtqnsdymwh.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtpstewwrn.html

var a = 1;  let b = 2
来源：http://hz.zhaomingkeji.xyz/gtojjchlzn.html

[T18] Swift：字符串插值
来源：http://hz.pycfn.com/gtmodwyabg.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gtxoxppcvx.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gthreqxxgi.html

if let n = opt { print(n) }
来源：http://hz.ybcxt.top/gtnjilsswe.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtrsoowtum.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gttktacizg.html

[T21] Swift：遍历
来源：http://hz.chenjidiqi.icu/gteciybgek.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtpmzgdmzt.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gttbudwdgm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gtaxkvbgiv.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gtfavtufqa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tanke756.top/gtxeiyceni.html

[T24] Swift：闭包
来源：http://hz.cqqwz.cn/gtaiwxmqzs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtadwlehzp.html

[T25] Swift：结构体
来源：http://hz.ivvv.top/gtdzazcsid.html

struct P { var x: Int }
来源：http://hz.fengsongda.top/gthlckvawy.html

[T26] Swift：类与重写
来源：http://hz.daria6918.cn/gtmunfgtai.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtsjnwzefr.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtsbwcavzm.html

do { try f() } catch { print(error) }
来源：http://hz.c1oappe.top/gtjgademex.html

[T28] Swift：枚举
来源：http://hz.ppjwa.cn/gtkwvzkmxp.html

enum Color { case red, green }
来源：http://hz.ivvv.top/gtoojsuquh.html

[T29] Swift：guard 提前返回
来源：http://hz.shangyingyoupin.top/gtghxxozoi.html

guard let x = opt else { return }
来源：http://hz.bjfxy.top/gtqcasrcqs.html

[T30] Swift：协议
来源：http://hz.zhongyouzk.top/gtykaciyro.html

protocol Shape { func area() -> Double }
来源：http://hz.xinyue.icu/gtiwxvesnj.html

[T31] Lua：Hello World
来源：http://hz.pycfn.com/gtaioreyyo.html

print("Hello")
来源：http://hz.yanxiufei.cn/gthmucuzwb.html

[T32] Lua：局部变量
来源：http://hz.jinqigfzy.top/gtcyprfpeo.html

local a = 1
来源：http://hz.bjfxy.top/gtyvpiocfk.html

[T33] Lua：表（数组）
来源：http://hz.yueranfly.top/gtrguofhyk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yonumen.top/gtwopnfbrq.html

[T34] Lua：遍历表
来源：http://hz.nanxuanxn.top/gtamaqzbtl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hysaishi.cn/gtuyngmryx.html

[T35] Lua：字典表
来源：http://hz.fzhhl.top/gtezmdibmx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hfpthk.cn/gtuceuiczf.html

[T36] Lua：函数
来源：http://hz.shanyushiyangtech.top/gtqeuwptbs.html

function add(a, b) return a + b end
来源：http://hz.sysykeji.top/gtdqvdxfaf.html

[T37] Lua：字符串拼接
来源：http://hz.yueranfly.top/gtcvhwqner.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gtuzjrkicn.html

[T38] Lua：条件
来源：http://hz.bjfxy.top/gtqeaipluq.html

if x > 0 then print("正") end
来源：http://hz.pengpengdd.cyou/gtyxsieqpz.html

[T39] Lua：模式匹配
来源：http://hz.yj20258888.top/gtpgocdqgm.html

string.find(s, "%d+")
来源：http://hz.yongpay.top/gtzixgdymh.html

[T40] Lua：元表
来源：http://hz.dianchejie.cn/gtwwmwzczz.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258888.top/gtqwefdedh.html

[T41] Perl：Hello World
来源：http://hz.pycfn.com/gtwfjoqkrw.html

print "Hello\n";
来源：http://hz.guowangkeji.top/gtudfcbgsn.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtbxzssnvv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xylfe.cn/gtcriykooq.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtqhtrmmkb.html

"值: $a"
来源：http://hz.hysaishi.cn/gtgcilrfbu.html

[T44] Perl：条件
来源：http://hz.jiagoushi.top/gtwoyvnzji.html

if ($a > 0) { print "正"; }
来源：http://hz.guowangkeji.top/gtohfaglxi.html

[T45] Perl：数组遍历
来源：http://hz.zycfv.cn/gtndoorsym.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258.top/gtglvssxfp.html

[T46] Perl：哈希操作
来源：http://hz.jinghuilouyu.cn/gtiybwcbcq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xylfe.cn/gtljswloxt.html

[T47] Perl：正则捕获
来源：http://hz.feifeiyinyue.top/gtzrkfalzf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dashuyun.cn/gtfxngyvin.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gttvtbgyta.html

$s =~ s/old/new/g;
来源：http://hz.0kj1m.cn/gtkfheyjut.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gtbuflxrhb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.birdmap.top/gtdhumwgyv.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtsanxfhif.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sufxvd.cn/gttduxlzgv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hfpthk.cn/gtvwxgswpy.html

[T51] Scala：Hello World
来源：http://hz.daria6918.cn/gtkrbndzog.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtpmddpllk.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gttzkmytnz.html

val a = 1;  var b = 2
来源：http://hz.hongshengwenyu.top/gthwxfmtnz.html

[T53] Scala：字符串插值
来源：http://hz.yongpay.top/gttdccmozt.html

s"值: $b"
来源：http://hz.gzhubu.top/gtwhpgxuhf.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gtmsntyiyb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.vqdsnc.cn/gtmimwkgat.html

[T55] Scala：集合过滤
来源：http://hz.ivvv.top/gtbklhuvke.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dianchejie.cn/gtwskfsdkd.html

[T56] Scala：样例类
来源：http://hz.zhongyouzk.top/gtdxohmrru.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gtfdavmkds.html

[T57] Scala：模式匹配
来源：http://hz.dianchejie.cn/gtjmyvwuvn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gaohongyu789.top/gtqtacxwif.html

[T58] Scala：函数定义
来源：http://hz.ydjk.org.cn/gtggzxkxyy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gtuqujptek.html

[T59] Scala：循环
来源：http://hz.xinyue.icu/gtjnwweadl.html

for (i <- 1 to 10) println(i)
来源：http://hz.cqqwz.cn/gtnaxbszab.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtbarjtjqb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.wangshuangyany.cn/gtbhtgpbii.html

================================================================================
来源：http://hz.tianlin.xyz/gtsiqgatzl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtgglntlft.html

================================================================================
来源：http://hz.yvedp.cn/gtmxnsuagx.html

[U01] Py：创建虚拟环境
来源：http://hz.shzxlz.cn/gtjsdpyflu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cheryme.top/gtwbmhaalx.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gtnqljqrie.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtnbelieev.html

[U03] Py：加载 .env 配置
来源：http://hz.gzhubu.top/gtrejqmzpu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.pengpengdd.cyou/gtxetowxhh.html

[U04] Py：变量调试打印
来源：http://hz.dashuyun.cn/gtmvnugbkj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tianlin.xyz/gtvvkgvtvb.html

[U05] Py：列表去重且保序
来源：http://hz.jianghu66.top/gtmdltzflc.html

list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtltoykppl.html

[U06] Py：合并两个字典
来源：http://hz.hfpthk.cn/gtkgsipjrd.html

{**a, **b}
来源：http://hz.0kj1m.cn/gtxqcdpyrd.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtjnlzgaka.html

{v: k for k, v in d.items()}
来源：http://hz.smart0.xyz/gttampnubj.html

[U08] Py：展平二维列表
来源：http://hz.hfpthk.cn/gtmzntlwkb.html

[y for x in nested for y in x]
来源：http://hz.guannengcc.top/gtqopgeahh.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258888.top/gtglxfontk.html

max(d, key=d.get)
来源：http://hz.meibo888.top/gtupftzjpy.html

[U10] Py：按值排序字典
来源：http://hz.mhx1999.top/gtcjmpwuzz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj20258888.top/gtmujgpvaw.html

[U11] Py：生成器表达式
来源：http://hz.ydzc1.top/gtvzqgqybj.html

(x * 2 for x in arr)
来源：http://hz.cqqwz.cn/gtosxuvspi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tian-w.cn/gtcldayyrb.html

Counter(arr).most_common(3)
来源：http://hz.hammf.cn/gtruwrcqvq.html

[U13] Py：固定长度队列
来源：http://hz.nwbrower.top/gtfysxyahm.html

deque(maxlen=10)
来源：http://hz.jinyuanbaomall.cn/gteytghkqx.html

[U14] Py：分组收集到列表
来源：http://hz.tianlin.xyz/gtohkqrcdx.html

defaultdict(list)
来源：http://hz.zycfv.cn/gtjgyzvwgq.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gtqrcivjik.html

t = time.perf_counter()
来源：http://hz.daria6918.cn/gtkegoqjml.html

[U16] Py：命令行参数解析
来源：http://hz.jinqigfzy.top/gtdtbzzmld.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.dashuyun.cn/gtlzlnbtcz.html

[U17] Py：初始化日志
来源：http://hz.ppjwa.cn/gtjgfwplls.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daria6918.cn/gtqccymqhs.html

[U18] Py：预编译正则
来源：http://hz.hfpthk.cn/gtgxoljplu.html

pat = re.compile(r"\d+")
来源：http://hz.pycfn.com/gtgzzdabzr.html

[U19] Py：正则替换带回调
来源：http://hz.hysaishi.cn/gtndgxjbzj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cheryme.top/gthddnwlyi.html

[U20] Py：缓存函数结果
来源：http://hz.havefunace.top/gtqhbqphtj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.haohaochexian.top/gteggbfohr.html


<!-- 参考信息 -->