代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtiuiklchb.html

[S02] C：变量与格式化输出
来源：http://hz.birdmap.top/gtbnuexrrd.html

int a = 10; printf("%d\n", a);
来源：http://hz.yvedp.cn/gtoqgzshji.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gtrhgnozkf.html

int x; scanf("%d", &x);
来源：http://hz.shuidangran.top/gtkfaekujl.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gtngpjufaf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtoqlwvgmo.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtmxsbotss.html

strlen(s)
来源：http://hz.yangfankeji.com/gtxwxekiev.html

[S06] C：字符串比较
来源：http://hz.yuanzhike.top/gtykqnmhkr.html

strcmp(a, b) == 0
来源：http://hz.fzhhl.top/gtnqlfwvxq.html

[S07] C：数组遍历求和
来源：http://hz.wangdashe.top/gtwtwrsrnd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtusumggpa.html

[S08] C：动态内存分配与释放
来源：http://hz.gogol.net.cn/gtniqdcxjc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.svipenyu.cn/gtmoxbzdiw.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtjnocrcvq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigfzy.top/gtsnexdtvg.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gtqwlgwqng.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtkyhezcfg.html

[S11] C：逐行读文件
来源：http://hz.cheryme.top/gtgqnsdpme.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtzghsttfo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cheryme.top/gttlfaqmpv.html

fclose(f);
来源：http://hz.yj202588.top/gteoawbtlr.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gttyybfvnv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yongpay.top/gtvypvrfgs.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gtlrehwdtz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.haohaochexian.top/gtfeebqbit.html

[S14] C：枚举
来源：http://hz.shuidangran.top/gtxmuyroty.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.meibo888.top/gtasyjsuqz.html

[S15] C：类型转换
来源：http://hz.hnxiangtu.top/gtukzqesro.html

(double) a / b
来源：http://hz.jianghu66.top/gtqecyfzzs.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gthhlilynx.html

x |= (1 << 3);
来源：http://hz.daxiang520.top/gtlbotnnvp.html

[S17] C：安全拼接字符串
来源：http://hz.jianghu66.top/gtgasrcfiv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cucudq.cn/gtmhajirtb.html

[S18] C：命令行参数
来源：http://hz.xziqi.cn/gtgbbbcwkg.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gtolcrgxce.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtzyrxsujc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtrgwunupc.html

[S20] C：二分查找
来源：http://hz.hongshengwenyu.top/gtuvkjfurk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sysykeji.top/gtelmnculx.html

[S21] C：字符类别判断
来源：http://hz.gaohongyu789.top/gtkixiouqb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gthwjobhlp.html

[S22] C：字符串转数字
来源：http://hz.yj20258.top/gtaoratjbi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hysaishi.cn/gtdddpbkac.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtlndfnkcc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gtuibuxemq.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gtlujpgsdv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtymottqgw.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtbrodiuzz.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtzekniwer.html

[S26] C：内存清零
来源：http://hz.chenjidiqi.icu/gtgodbnyvs.html

memset(a, 0, sizeof a);
来源：http://hz.zhixingplan.top/gtulzfwphd.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtzlyebqtp.html

const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtxqtrkxjb.html

[S28] C：静态变量
来源：http://hz.chenjidiqi.icu/gtfkhqsttd.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtxmksilgx.html

[S29] C：变参函数
来源：http://hz.snrcjt.cn/gtieubhxkg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtddvfzguk.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtgregliyg.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtgegxcdyw.html

#define X_H
来源：http://hz.hysaishi.cn/gtzprxccun.html

#endif
来源：http://hz.cheryme.top/gtdkaxenae.html

[S31] C++：Hello World
来源：http://hz.dianchejie.cn/gtxmpzboiw.html

#include <iostream>
来源：http://hz.yj202588.top/gtstnxjjgm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.birdmap.top/gtojjfdtzj.html

[S32] C++：字符串
来源：http://hz.shanyushiyangtech.top/gtqsxvgzjs.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtuzslymsw.html

[S33] C++：vector 增删
来源：http://hz.ybcxt.top/gtnhspmqtq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shzxlz.cn/gtstycpeyk.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtxecuwlpc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sysykeji.top/gtthnwkuwa.html

[S35] C++：map
来源：http://hz.shanyushiyangtech.top/gtwwzwlmqk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtbmtdmtbt.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtjyvwruwz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtwjkffezq.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtmfphjagi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtfqvzbegv.html

[S38] C++：排序
来源：http://hz.jlsjyb.cn/gtqmvefbpc.html

std::sort(v.begin(), v.end());
来源：http://hz.yongpay.top/gtizroaiiz.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtbtfvxilx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtjrgwbxjz.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtfqbqjdjf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gtozvhalfy.html

[S41] C++：类与构造函数
来源：http://hz.jiagoushi.top/gtnfmarpyj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtqfpsavwa.html

[S42] C++：继承与虚函数
来源：http://hz.havefunace.top/gtqxvjpbrk.html

class B : public Base { public: void f() override {} };
来源：http://hz.shzxlz.cn/gtbeurtbky.html

[S43] C++：智能指针
来源：http://hz.9152youxi.cn/gtwljprhxg.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtdzzfzuuy.html

[S44] C++：引用传参
来源：http://hz.ppjwa.cn/gtvhhujibr.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtvnivtxny.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtkdifgxvm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtztusnsuh.html

[S46] C++：函数模板
来源：http://hz.yuanzhike.top/gtkcdrxnei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tianlin.xyz/gtodidnuga.html

[S47] C++：结构化绑定遍历
来源：http://hz.hongshengwenyu.top/gtdtfqdtur.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gogol.net.cn/gtsoslvjon.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtatfexlzq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cashguo.top/gtrlclqcwc.html

while (std::getline(in, line)) { }
来源：http://hz.hnxiangtu.top/gtcxixhiov.html

[S49] C++：写文件
来源：http://hz.tianlin.xyz/gtikscmlqo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtblxtnipw.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtlljupqag.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.quarkkingdee.top/gtslbtsuax.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtpxrjdvsg.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gtfcwjmbmv.html

[S52] C++：const 与 noexcept
来源：http://hz.aizwys.cn/gtockxtnxu.html

int size() const noexcept { return n_; }
来源：http://hz.xingfuxueyuan.xyz/gtdnrvkqcr.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtfogdfike.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtowqdxpwu.html

[S54] C++：异常处理
来源：http://hz.nanxinkj.top/gtlhprogum.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtgpbaxnqx.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gtwxvrzrpb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xinyue.icu/gtqrbbgojz.html

[S56] C++：optional
来源：http://hz.tianlin.xyz/gtiyutvzfk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shangyingyoupin.top/gtvhybqutr.html

[S57] C++：编译期常量
来源：http://hz.pengpengdd.cyou/gtuiethqtz.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gthfgmyvat.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtyekcxvyf.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gtuqayacsy.html

[S59] C++：静态断言
来源：http://hz.zhongyouzk.top/gtmsvzasny.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.vqdsnc.cn/gtlrqbvzei.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gtvllrjnme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sweek.top/gtlbxaxivn.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyxfiuggo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtjqccxykk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgsmcycna.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtwqzgpfvc.html

println("Hello")
来源：http://hz.jinqigufen.top/gtswqxltdx.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtdsrigrih.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinyuanbaomall.cn/gthqxlwuis.html

[T03] Kotlin：字符串模板
来源：http://hz.yangfankeji.com/gtyvnmeiyg.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gtvsuccyzz.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtmdkzoess.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtrokwjrra.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gtbgzhpvjo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zdqjudy.top/gtacitvfgl.html

[T06] Kotlin：集合映射
来源：http://hz.yanxiufei.cn/gtoenfozgf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gtwazwdaoc.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtwkzjigqj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zdqjudy.top/gtvvglmktk.html

[T08] Kotlin：数据类
来源：http://hz.dashuyun.cn/gtjaiwjzrq.html

data class User(val name: String, val age: Int)
来源：http://hz.xingfuxueyuan.xyz/gtleysqtzt.html

[T09] Kotlin：扩展函数
来源：http://hz.0kj1m.cn/gtmdrweczo.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtviihhicd.html

[T10] Kotlin：默认参数
来源：http://hz.0kj1m.cn/gtccuxxjfe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtlrgdnuqe.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtwyyfhhkb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtcynvuzaj.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258.top/gtesmtajdu.html

val (a, b) = Pair(1, 2)
来源：http://hz.havefunace.top/gtmhnccxen.html

[T13] Kotlin：只读 Map
来源：http://hz.ivvv.top/gthgkvltdp.html

val m = mapOf("a" to 1)
来源：http://hz.cheryme.top/gtldttckgq.html

[T14] Kotlin：循环
来源：http://hz.sweek.top/gtxzgfdefb.html

for (i in 1..10) println(i)
来源：http://hz.svipenyu.cn/gtfjiyaump.html

[T15] Kotlin：接口
来源：http://hz.yj20258.top/gtzpoepopo.html

interface Shape { fun area(): Double }
来源：http://hz.jlsjyb.cn/gtoyiofawh.html

[T16] Swift：Hello World
来源：http://hz.c1oappe.top/gtklczirje.html

print("Hello")
来源：http://hz.fzhhl.top/gtqwyhsmvd.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangkeji.top/gtxhuunhoj.html

var a = 1;  let b = 2
来源：http://hz.zhijiandao.cn/gtuulqvffr.html

[T18] Swift：字符串插值
来源：http://hz.zhixingplan.top/gtgiecundp.html

"值: \(b)"
来源：http://hz.ybcxt.top/gtrebcioqb.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtmmibkjjh.html

if let n = opt { print(n) }
来源：http://hz.cheryme.top/gtjzqanpug.html

[T20] Swift：数组操作
来源：http://hz.jyoumei.cn/gtmmqyxwqh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shuidangran.top/gtnfzkzxbm.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gtkgfjrdfh.html

for x in a { print(x) }
来源：http://hz.sxryk.cn/gtjlmiziwp.html

[T22] Swift：字典
来源：http://hz.cheryme.top/gtkbzrabgk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tian-w.cn/gtkfmwctzr.html

[T23] Swift：函数
来源：http://hz.jinghuilouyu.cn/gtayqlhkvy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuanzx.com/gtqvygmwqu.html

[T24] Swift：闭包
来源：http://hz.yonumen.top/gtzortahyz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj202588.top/gtmwpyaaeu.html

[T25] Swift：结构体
来源：http://hz.zhongyouzk.top/gtrkemvoru.html

struct P { var x: Int }
来源：http://hz.hysaishi.cn/gtasjtqhsd.html

[T26] Swift：类与重写
来源：http://hz.c1oappe.top/gtpgsogtys.html

class A: Base { override func f() {} }
来源：http://hz.xingfuxueyuan.xyz/gtyfslsyzk.html

[T27] Swift：错误处理
来源：http://hz.cqqwz.cn/gtzchxnztu.html

do { try f() } catch { print(error) }
来源：http://hz.fengsongda.top/gtzkcmvqoa.html

[T28] Swift：枚举
来源：http://hz.zycfv.cn/gtfixxhkwo.html

enum Color { case red, green }
来源：http://hz.cashguo.top/gtwzbryuud.html

[T29] Swift：guard 提前返回
来源：http://hz.cqqwz.cn/gtuggnrmms.html

guard let x = opt else { return }
来源：http://hz.zhaomingkeji.xyz/gtmshamjhz.html

[T30] Swift：协议
来源：http://hz.yvedp.cn/gthqbttdsw.html

protocol Shape { func area() -> Double }
来源：http://hz.yj20258888.top/gtzhocnddq.html

[T31] Lua：Hello World
来源：http://hz.guowangkeji.top/gtkmxztbkw.html

print("Hello")
来源：http://hz.meibo888.top/gtzdsczavp.html

[T32] Lua：局部变量
来源：http://hz.hammf.cn/gtzzkalule.html

local a = 1
来源：http://hz.cqqwz.cn/gtppmyevxp.html

[T33] Lua：表（数组）
来源：http://hz.chenjidiqi.icu/gtbaqzvhie.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cdnleiting.top/gthbwraihr.html

[T34] Lua：遍历表
来源：http://hz.zhongyouzk.top/gtvoebfian.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgufenzy.top/gtovitzshc.html

[T35] Lua：字典表
来源：http://hz.zhijiandao.cn/gtzgydiajl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cdnleiting.top/gtlziebkls.html

[T36] Lua：函数
来源：http://hz.sysykeji.top/gthvoagqdu.html

function add(a, b) return a + b end
来源：http://hz.yueranfly.top/gtzxakwgaj.html

[T37] Lua：字符串拼接
来源：http://hz.yuanzhike.top/gtlyojwrxf.html

"a" .. "b"
来源：http://hz.wangdashe.top/gtrxjkuraa.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtzvtwtbej.html

if x > 0 then print("正") end
来源：http://hz.haohaochexian.top/gtxqmkmxhv.html

[T39] Lua：模式匹配
来源：http://hz.sysykeji.top/gtzkpmehkx.html

string.find(s, "%d+")
来源：http://hz.jqgfzy.top/gttoxfoacy.html

[T40] Lua：元表
来源：http://hz.shanyushiyangkeji.top/gtqtbvhpza.html

setmetatable({}, { __index = base })
来源：http://hz.jlsjyb.cn/gtrnqidspx.html

[T41] Perl：Hello World
来源：http://hz.jiagoushi.top/gtcpdubakc.html

print "Hello\n";
来源：http://hz.wangshuangyany.cn/gtpjwtfsag.html

[T42] Perl：变量类型
来源：http://hz.9152youxi.cn/gtwsplfejt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.c1oappe.top/gtflqhtaqv.html

[T43] Perl：字符串插值
来源：http://hz.zhixingplan.top/gtbpgxyjqv.html

"值: $a"
来源：http://hz.gogol.net.cn/gthzrxcncv.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gtewggzoit.html

if ($a > 0) { print "正"; }
来源：http://hz.ywan-chungtsiang.top/gtfjwciucv.html

[T45] Perl：数组遍历
来源：http://hz.hywenlv.cn/gtjvfxgbxp.html

for my $x (@arr) { print $x; }
来源：http://hz.tanke756.top/gtbtpjavop.html

[T46] Perl：哈希操作
来源：http://hz.feifeiyinyue.top/gtwnjmqlus.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jlsjyb.cn/gtyxvnjuys.html

[T47] Perl：正则捕获
来源：http://hz.redwolf501.top/gtrvgurirl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shzxlz.cn/gtffmpaphh.html

[T48] Perl：正则替换
来源：http://hz.yj20258888.top/gtjfchqihy.html

$s =~ s/old/new/g;
来源：http://hz.chenjidiqi.icu/gtiuxrglgj.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtqbisrzbw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cdnleiting.top/gtbtosfkpg.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtfghoygkg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuanzhike.top/gtckzuihou.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhixingplan.top/gtguirvsxg.html

[T51] Scala：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtednvgcey.html

println("Hello")
来源：http://hz.fengsongda.top/gtkiizaltd.html

[T52] Scala：变量
来源：http://hz.iojbl.cn/gtwkedhoyk.html

val a = 1;  var b = 2
来源：http://hz.yanxiufei.cn/gtvrgmvlxr.html

[T53] Scala：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtvfsxpndc.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtqohhhmgk.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangkeji.top/gtmmwpfdyx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydjk.org.cn/gtvikbvdew.html

[T55] Scala：集合过滤
来源：http://hz.daxiang520.top/gtqkzboyza.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yonumen.top/gtoscdvbty.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gthcaxvlqe.html

case class User(name: String, age: Int)
来源：http://hz.xuetiantiany.cn/gtruolbuen.html

[T57] Scala：模式匹配
来源：http://hz.yongpay.top/gtcgnzzljl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cqqwz.cn/gtguufejib.html

[T58] Scala：函数定义
来源：http://hz.jlsjyb.cn/gtwcujecoo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtiibmjdeh.html

[T59] Scala：循环
来源：http://hz.aibaodan.cn/gtmoayttsr.html

for (i <- 1 to 10) println(i)
来源：http://hz.nanxuanxn.top/gtpzrvjbfg.html

[T60] Scala：折叠
来源：http://hz.dianchejie.cn/gttwqvpjil.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yangfankeji.com/gtveskzzga.html

================================================================================
来源：http://hz.fzhhl.top/gtowoeifbd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zycfv.cn/gtyuskrrin.html

================================================================================
来源：http://hz.snrcjt.cn/gtxzvnhfyx.html

[U01] Py：创建虚拟环境
来源：http://hz.hnqzz.top/gtpkwfygkz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gtgxgcckii.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cashguo.top/gtymfrjqvh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gtekgullvf.html

[U03] Py：加载 .env 配置
来源：http://hz.316326.xyz/gtgziiisgm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dianchejie.cn/gteplerlcr.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gtpqbvfavd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dashuyun.cn/gtjeniiuqc.html

[U05] Py：列表去重且保序
来源：http://hz.tanke756.top/gtubbhudih.html

list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtdfwtuysz.html

[U06] Py：合并两个字典
来源：http://hz.yueranfly.top/gtpoptpbeb.html

{**a, **b}
来源：http://hz.bjfxy.top/gtgnjenpju.html

[U07] Py：反转字典键值
来源：http://hz.jinqigfzy.top/gtgedkqpnk.html

{v: k for k, v in d.items()}
来源：http://hz.hywenlv.cn/gtbioqpgaz.html

[U08] Py：展平二维列表
来源：http://hz.cdnleiting.top/gtufyzosve.html

[y for x in nested for y in x]
来源：http://hz.wangshuangyany.cn/gtqfqxdwbf.html

[U09] Py：字典取最大值的键
来源：http://hz.jyoumei.cn/gthqqcbrud.html

max(d, key=d.get)
来源：http://hz.haohaochexian.top/gtbtqbhlrc.html

[U10] Py：按值排序字典
来源：http://hz.zhengqikj.top/gtyyikfagk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.haohaochexian.top/gtvbszjjcb.html

[U11] Py：生成器表达式
来源：http://hz.haohaochexian.top/gtewcskqvp.html

(x * 2 for x in arr)
来源：http://hz.kuanghao11.cn/gtqckxfabd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhaomingkeji.xyz/gtrquxmbfs.html

Counter(arr).most_common(3)
来源：http://hz.haohaochexian.top/gtsaohkfvh.html

[U13] Py：固定长度队列
来源：http://hz.smart0.xyz/gtxuwywwtr.html

deque(maxlen=10)
来源：http://hz.birdmap.top/gtycnbgdnd.html

[U14] Py：分组收集到列表
来源：http://hz.yuxming.cn/gtcwplpgbq.html

defaultdict(list)
来源：http://hz.zdqjudy.top/gthwqvnwag.html

[U15] Py：高精度计时
来源：http://hz.dianchejie.cn/gtzkgwscgv.html

t = time.perf_counter()
来源：http://hz.daria6918.cn/gtqvynkpog.html

[U16] Py：命令行参数解析
来源：http://hz.iojbl.cn/gtmznyggfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ppjwa.cn/gtnzvinroh.html

[U17] Py：初始化日志
来源：http://hz.jinqigufen.top/gtqjislafq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhengqikj.top/gtkrisycue.html

[U18] Py：预编译正则
来源：http://hz.jinqigfzy.top/gtaxjxsvss.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gthqjwedxt.html

[U19] Py：正则替换带回调
来源：http://hz.xuanzx.com/gtsjqxuums.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cqqwz.cn/gtdrxkvhoo.html

[U20] Py：缓存函数结果
来源：http://hz.nanxuanxn.top/gtitcahvna.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sufxvd.cn/gtcyvvdgll.html

[U21] Py：自定义上下文管理器
来源：http://hz.9152youxi.cn/gtojdgnmiq.html

@contextlib.contextmanager
来源：http://hz.tian-w.cn/gtquwqszfg.html

[U22] Py：矩阵转置
来源：http://hz.tianlin.xyz/gtocrocyza.html

list(zip(*m))
来源：http://hz.nanxuanxn.top/gtvtuqqonl.html

[U23] Py：分块读取大文件
来源：http://hz.hongshengwenyu.top/gteojiyqgj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhoulong.xyz/gtphrmvyiz.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtmkroxklh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yuxming.cn/gtaagbexgy.html


<!-- 参考信息 -->