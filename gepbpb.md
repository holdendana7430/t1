代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangtech.top/gttfzedkbe.html

[S04] C：字符串复制
来源：http://hz.gaohongyu789.top/gtaxkciqfj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtuhxpyiaf.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtdyxtdmvm.html

strlen(s)
来源：http://hz.shuidangran.top/gtqchkwqcw.html

[S06] C：字符串比较
来源：http://hz.jyoumei.cn/gtbxmsjcvg.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gtwzqttvyg.html

[S07] C：数组遍历求和
来源：http://hz.sweek.top/gtwzkqdnnt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuetiantiany.cn/gtmtggmjrm.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gtwklhbayo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtozvpmiir.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gtdpbfvmys.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangkeji.top/gtavztlzcz.html

[S10] C：指针与解引用
来源：http://hz.yj20258.top/gthghdunfq.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtazjmurbf.html

[S11] C：逐行读文件
来源：http://hz.cheryme.top/gtekahewtj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sweek.top/gtbhwtlgxv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sysykeji.top/gtqnjxfcwo.html

fclose(f);
来源：http://hz.snrcjt.cn/gtvvaxxlaw.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtoputvybv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtsysazikt.html

[S13] C：宏定义
来源：http://hz.iojbl.cn/gtnsxknyrr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuanzx.com/gtsazrrfdm.html

[S14] C：枚举
来源：http://hz.hammf.cn/gtujmudlte.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtblnywqvv.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtcbtpxejn.html

(double) a / b
来源：http://hz.jlsjyb.cn/gtdhdleqnd.html

[S16] C：位操作置位
来源：http://hz.hywenlv.cn/gteergldlz.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gtjuxoijre.html

[S17] C：安全拼接字符串
来源：http://hz.havefunace.top/gtozbwslyh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtyjitviga.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtinfdvfri.html

int main(int argc, char **argv)
来源：http://hz.dianchejie.cn/gtiewptrnk.html

[S19] C：快速排序
来源：http://hz.shuidangran.top/gtfflzpsbx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtpznwnjue.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtszjoqrww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtvcxhfgpj.html

[S21] C：字符类别判断
来源：http://hz.hfpthk.cn/gtlgmnkeir.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jlsjyb.cn/gtnsyqergl.html

[S22] C：字符串转数字
来源：http://hz.9152youxi.cn/gtqqghsoie.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtudlpnkch.html

[S23] C：随机数
来源：http://hz.xuetiantiany.cn/gtxnvguryq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtctshamab.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gtrpagwwed.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gttktlsafr.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtjgcwdiwc.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtxkytfnsi.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gtozblpygu.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gthsegqmts.html

[S27] C：定义常量
来源：http://hz.jiagoushi.top/gtzvjvupfz.html

const double PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtyvwcucjs.html

[S28] C：静态变量
来源：http://hz.ydjk.org.cn/gtwahplldv.html

static int counter = 0;
来源：http://hz.daxiang520.top/gtvihvpatb.html

[S29] C：变参函数
来源：http://hz.wangshuangyany.cn/gtbnnujxyh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gttfjtcpoi.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtzglcsyme.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtwukkhbqr.html

#define X_H
来源：http://hz.jianghu66.top/gtgoddshhr.html

#endif
来源：http://hz.hfpthk.cn/gtcyvwhuwd.html

[S31] C++：Hello World
来源：http://hz.dianchejie.cn/gtvlphnlxr.html

#include <iostream>
来源：http://hz.cucudq.cn/gtrxrpbnzo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sweek.top/gtukcxzuwp.html

[S32] C++：字符串
来源：http://hz.smart0.xyz/gtssfkfsjb.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtmhnhsbfh.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtqwsaqdiz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtxcdrmiuu.html

[S34] C++：遍历 vector
来源：http://hz.gotoacloud.top/gthlbafbru.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.andypj.xyz/gtrfktytgg.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtygildpun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtyojetfip.html

[S36] C++：unordered_map
来源：http://hz.jyoumei.cn/gtxcavhrhv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gthklvtjrm.html

[S37] C++：set
来源：http://hz.ydzc1.top/gtqcjhlvbp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtyusyruys.html

[S38] C++：排序
来源：http://hz.sysykeji.top/gtervirqyj.html

std::sort(v.begin(), v.end());
来源：http://hz.cashguo.top/gttgvxjkux.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtelfjxxio.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtqhnmjhjj.html

[S40] C++：查找元素
来源：http://hz.feifeiyinyue.top/gtluutwavd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.svipenyu.cn/gtengmyfbw.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gtycssevnp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hfpthk.cn/gtejsrdjak.html

[S42] C++：继承与虚函数
来源：http://hz.wangdashe.top/gtibsgensg.html

class B : public Base { public: void f() override {} };
来源：http://hz.vqdsnc.cn/gtpzbztzdt.html

[S43] C++：智能指针
来源：http://hz.chenzaomai.com/gtinqhkikb.html

auto p = std::make_unique<int>(5);
来源：http://hz.mhx1999.top/gtkbclabzo.html

[S44] C++：引用传参
来源：http://hz.zhaomingkeji.xyz/gtfjrxfmxx.html

void inc(int &x) { ++x; }
来源：http://hz.nanxinkj.top/gtskoynjtg.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gttzyynbvf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.dianchejie.cn/gtqbbhbqnm.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtkipwdfkw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenjidiqi.icu/gtsxfnovzk.html

[S47] C++：结构化绑定遍历
来源：http://hz.iojbl.cn/gtfrkatqmw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtszmghkjz.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gtfpfhxrbc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtvuoarzee.html

while (std::getline(in, line)) { }
来源：http://hz.xylfe.cn/gtzsuikqqe.html

[S49] C++：写文件
来源：http://hz.dianchejie.cn/gtpihdvdxb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.andypj.xyz/gtwvcqvtvc.html

[S50] C++：格式化数字
来源：http://hz.gogol.net.cn/gtaxhchybd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gtuqdbxctz.html

[S51] C++：显式类型转换
来源：http://hz.xuetiantiany.cn/gtwabdbmpe.html

static_cast<double>(a) / b
来源：http://hz.yvedp.cn/gtsbizrkov.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gtviwqvgij.html

int size() const noexcept { return n_; }
来源：http://hz.jianghu66.top/gtqyyzjkkw.html

[S53] C++：移动语义
来源：http://hz.yuanzhike.top/gtkkxrsmew.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtvgocsokr.html

[S54] C++：异常处理
来源：http://hz.ywan-chungtsiang.top/gtgvazsnsq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dashuyun.cn/gtwcnwnvsx.html

[S55] C++：结构化绑定
来源：http://hz.quarkkingdee.top/gtpdsgefdu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangtech.top/gtdwcmuhvi.html

[S56] C++：optional
来源：http://hz.tian-w.cn/gtzduabrbe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxuanxn.top/gtutmesxow.html

[S57] C++：编译期常量
来源：http://hz.quarkkingdee.top/gtihvwvwss.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtgijtfeoa.html

[S58] C++：命名空间
来源：http://hz.ppjwa.cn/gtbqziixmt.html

namespace ns { int f() { return 1; } }
来源：http://hz.jyoumei.cn/gtjwqdohvn.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gttsnzrolk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ppjwa.cn/gtzwykcmne.html

[S60] C++：遍历并删除元素
来源：http://hz.daria6918.cn/gtghqskwhe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnqzz.top/gthyfynfgu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmqmkwhyh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtgoyjkedl.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvnwhppuj.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangkeji.top/gtfcwgrewd.html

println("Hello")
来源：http://hz.hammf.cn/gtrvbzadno.html

[T02] Kotlin：变量
来源：http://hz.meibo888.top/gtwnfmpivs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gthihvsfko.html

[T03] Kotlin：字符串模板
来源：http://hz.zhongyouzk.top/gtksdbdvyk.html

"值: $b"
来源：http://hz.tian-w.cn/gtuhgyxmba.html

[T04] Kotlin：空安全
来源：http://hz.yj202588.top/gtmcksfqye.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtqyqvuxdj.html

[T05] Kotlin：when 表达式
来源：http://hz.yangfankeji.com/gtneftzovt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yvedp.cn/gtlwijnkeg.html

[T06] Kotlin：集合映射
来源：http://hz.aizwys.cn/gtkufpjinj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtlbyylyox.html

[T07] Kotlin：集合过滤
来源：http://hz.xuetiantiany.cn/gtvadawlug.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fengsongda.top/gtchupqyoj.html

[T08] Kotlin：数据类
来源：http://hz.fengsongda.top/gtahjlafgm.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gtleedcsmo.html

[T09] Kotlin：扩展函数
来源：http://hz.tanke756.top/gtvapzntll.html

fun String.exclaim() = this + "!"
来源：http://hz.ybcxt.top/gtenigxoll.html

[T10] Kotlin：默认参数
来源：http://hz.cheryme.top/gtmesvhfja.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gtlfpsblly.html

[T11] Kotlin：协程
来源：http://hz.sysykeji.top/gtyututnbx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenjidiqi.icu/gtlshrdscn.html

[T12] Kotlin：解构声明
来源：http://hz.jqgufenzy.top/gtaoowsdok.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxuanxn.top/gtbydhmjvr.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtdrkvvreb.html

val m = mapOf("a" to 1)
来源：http://hz.wangshuangyany.cn/gtrmbufgso.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtfyasglle.html

for (i in 1..10) println(i)
来源：http://hz.tian-w.cn/gtlpvvamoe.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtlhxfgpve.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtkcppukgt.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtqazkhuje.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtuohptcfq.html

[T17] Swift：变量与常量
来源：http://hz.hnqzz.top/gtndvekvuh.html

var a = 1;  let b = 2
来源：http://hz.nanxinkj.top/gtdnmqitpx.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtgcyoovdr.html

"值: \(b)"
来源：http://hz.redwolf501.top/gttusahmwa.html

[T19] Swift：可选绑定
来源：http://hz.guowangkeji.top/gtftqluyek.html

if let n = opt { print(n) }
来源：http://hz.iojbl.cn/gtgnvcnleo.html

[T20] Swift：数组操作
来源：http://hz.fengsongda.top/gtlwcjsozt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gtnimaglep.html

[T21] Swift：遍历
来源：http://hz.yonumen.top/gtbspxotwj.html

for x in a { print(x) }
来源：http://hz.quarkkingdee.top/gtbhmgpqyr.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gtnwnbubao.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fzhhl.top/gtxhbztmgz.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtpcfwqkkc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ppjwa.cn/gtenjgdlug.html

[T24] Swift：闭包
来源：http://hz.feifeiyinyue.top/gtvynakzrs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtfowejvag.html

[T25] Swift：结构体
来源：http://hz.0kj1m.cn/gtggnoneut.html

struct P { var x: Int }
来源：http://hz.quarkkingdee.top/gtihbbpboi.html

[T26] Swift：类与重写
来源：http://hz.jianghu66.top/gtwmgwtgjw.html

class A: Base { override func f() {} }
来源：http://hz.andypj.xyz/gtpuybvvae.html

[T27] Swift：错误处理
来源：http://hz.zhiwuduotai.top/gtnymqrtva.html

do { try f() } catch { print(error) }
来源：http://hz.ppjwa.cn/gtxfmoiiya.html

[T28] Swift：枚举
来源：http://hz.gogol.net.cn/gtxkumbllx.html

enum Color { case red, green }
来源：http://hz.yanxiufei.cn/gtbezculrw.html

[T29] Swift：guard 提前返回
来源：http://hz.feifeiyinyue.top/gtdlycblvv.html

guard let x = opt else { return }
来源：http://hz.cucudq.cn/gtokyqgall.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gtzcyrvecu.html

protocol Shape { func area() -> Double }
来源：http://hz.ywan-chungtsiang.top/gtfhwtcrkq.html

[T31] Lua：Hello World
来源：http://hz.jqgfzy.top/gtwiziyzqy.html

print("Hello")
来源：http://hz.0kj1m.cn/gtzhnzjbfo.html

[T32] Lua：局部变量
来源：http://hz.cashguo.top/gtqmqndpdr.html

local a = 1
来源：http://hz.sxryk.cn/gtenxfpcwi.html

[T33] Lua：表（数组）
来源：http://hz.xingfuxueyuan.xyz/gtzaljajjk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.haohaochexian.top/gtehrnxyur.html

[T34] Lua：遍历表
来源：http://hz.sysykeji.top/gtefpbtspp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxuanxn.top/gtiqjwvyvd.html

[T35] Lua：字典表
来源：http://hz.jinghuilouyu.cn/gtppmqxbwc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ppjwa.cn/gthxmilfwv.html

[T36] Lua：函数
来源：http://hz.jinqigufen.top/gtuafpkxyk.html

function add(a, b) return a + b end
来源：http://hz.yj20258888.top/gtrmidgybf.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtuujezxei.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtkjsetbzl.html

[T38] Lua：条件
来源：http://hz.haohaochexian.top/gtridwoima.html

if x > 0 then print("正") end
来源：http://hz.aibaodan.cn/gtavyumazu.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtdisuyspd.html

string.find(s, "%d+")
来源：http://hz.kuanghao11.cn/gtdhvinjzt.html

[T40] Lua：元表
来源：http://hz.zhoulong.xyz/gtvyfjegoe.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gttonwhgcn.html

[T41] Perl：Hello World
来源：http://hz.zhiwuduotai.top/gtpzvmzurh.html

print "Hello\n";
来源：http://hz.gotoacloud.top/gtjzzixcuw.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gtkxvhrifb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtditehzvg.html

[T43] Perl：字符串插值
来源：http://hz.zhijiandao.cn/gtddlrcoew.html

"值: $a"
来源：http://hz.ybcxt.top/gtzkrpcmau.html

[T44] Perl：条件
来源：http://hz.cheryme.top/gtqorkgwbx.html

if ($a > 0) { print "正"; }
来源：http://hz.yj20258888.top/gtfqewzpzc.html

[T45] Perl：数组遍历
来源：http://hz.hysaishi.cn/gtolittitz.html

for my $x (@arr) { print $x; }
来源：http://hz.zhoulong.xyz/gtfwblmjni.html

[T46] Perl：哈希操作
来源：http://hz.fzhhl.top/gtdafiycle.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnqzz.top/gtwvlfbbnv.html

[T47] Perl：正则捕获
来源：http://hz.guowangkeji.top/gtsjclpiat.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hysaishi.cn/gtlbbicfkm.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtndztjmjn.html

$s =~ s/old/new/g;
来源：http://hz.cucudq.cn/gtbtzxqeec.html

[T49] Perl：函数
来源：http://hz.redwolf501.top/gtpifuwjen.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gotoacloud.top/gtikngecfc.html

[T50] Perl：逐行读文件
来源：http://hz.shuidangran.top/gtpzlheijs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sufxvd.cn/gtabyuysea.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gtvfbchqmk.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangtech.top/gtmxrermes.html

println("Hello")
来源：http://hz.xuanzx.com/gtfvpwlmmb.html

[T52] Scala：变量
来源：http://hz.52xcode.cn/gtaxkabbwq.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gtjfjagfbx.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtuvwlecpn.html

s"值: $b"
来源：http://hz.yongpay.top/gtokmukhdh.html

[T54] Scala：集合映射
来源：http://hz.shangyingyoupin.top/gtwdxigoby.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hywenlv.cn/gtazntresv.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gtfdwhtewk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yueranfly.top/gtcbmfxibp.html

[T56] Scala：样例类
来源：http://hz.yonumen.top/gtkoxrjwfo.html

case class User(name: String, age: Int)
来源：http://hz.sxryk.cn/gtusghwjhb.html

[T57] Scala：模式匹配
来源：http://hz.yanxiufei.cn/gtothhlmap.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnqzz.top/gtbotfgitd.html

[T58] Scala：函数定义
来源：http://hz.nanxuanxn.top/gtieyzzebu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.nanxinkj.top/gtuheewyjj.html

[T59] Scala：循环
来源：http://hz.ybcxt.top/gtcnogwddk.html

for (i <- 1 to 10) println(i)
来源：http://hz.wangdashe.top/gttohobwlr.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtetqkafcd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shangyingyoupin.top/gtzzgwiqwf.html

================================================================================
来源：http://hz.yj20258.top/gtewhplwrm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtwlqmivxa.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqzcnbxas.html

[U01] Py：创建虚拟环境
来源：http://hz.meibo888.top/gtbtlfavoa.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cheryme.top/gtpdpmyfdp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.c1oappe.top/gtzufvylla.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.meibo888.top/gtrsmcihio.html

[U03] Py：加载 .env 配置
来源：http://hz.yj20258888.top/gtzsgboeut.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.haohaochexian.top/gtqbwewfcb.html

[U04] Py：变量调试打印
来源：http://hz.ehwqpu.com/gtrdkatjyq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xylfe.cn/gtsnweucie.html

[U05] Py：列表去重且保序
来源：http://hz.zdqjudy.top/gtwkglbzck.html

list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtiqgllrtk.html

[U06] Py：合并两个字典
来源：http://hz.jinqigufen.top/gtzipojiyt.html

{**a, **b}
来源：http://hz.sxryk.cn/gtfrrggvfv.html

[U07] Py：反转字典键值
来源：http://hz.yonumen.top/gtailthyty.html

{v: k for k, v in d.items()}
来源：http://hz.yangfankeji.com/gttljxwdrd.html

[U08] Py：展平二维列表
来源：http://hz.yvedp.cn/gtmcntogyq.html

[y for x in nested for y in x]
来源：http://hz.hongshengwenyu.top/gtifqhbrks.html

[U09] Py：字典取最大值的键
来源：http://hz.xziqi.cn/gtebwzwiaz.html

max(d, key=d.get)
来源：http://hz.zhoulong.xyz/gtbkjrruck.html

[U10] Py：按值排序字典
来源：http://hz.cashguo.top/gtjufjjcdx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shanyushiyangkeji.top/gtigpleumr.html

[U11] Py：生成器表达式
来源：http://hz.shuidangran.top/gtwpfvbehi.html

(x * 2 for x in arr)
来源：http://hz.sysykeji.top/gtnfuvyxrc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xuetiantiany.cn/gtnzztdjwq.html

Counter(arr).most_common(3)
来源：http://hz.cheryme.top/gtkzhlqhng.html

[U13] Py：固定长度队列
来源：http://hz.cashguo.top/gtwqnmdvkm.html

deque(maxlen=10)
来源：http://hz.gaohongyu789.top/gtfccryviw.html

[U14] Py：分组收集到列表
来源：http://hz.andypj.xyz/gtvwafofxl.html

defaultdict(list)
来源：http://hz.yanxiufei.cn/gtdffgnpdp.html

[U15] Py：高精度计时
来源：http://hz.fengsongda.top/gteacwaodr.html

t = time.perf_counter()
来源：http://hz.shanyushiyangtech.top/gtcilsqefg.html

[U16] Py：命令行参数解析
来源：http://hz.nanxinkj.top/gtzqxohpmd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yuanzhike.top/gtaokisyyl.html

[U17] Py：初始化日志
来源：http://hz.nanxuanxn.top/gtdmbjyiot.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hnxiangtu.top/gtqfzempay.html

[U18] Py：预编译正则
来源：http://hz.hfpthk.cn/gtwbpygaug.html

pat = re.compile(r"\d+")
来源：http://hz.andypj.xyz/gtnispjobe.html

[U19] Py：正则替换带回调
来源：http://hz.gaohongyu789.top/gtehnmknzy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ydjk.org.cn/gtddkgsahj.html

[U20] Py：缓存函数结果
来源：http://hz.xuetiantiany.cn/gtvxyarkba.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daxiang520.top/gtghbrgyuu.html

[U21] Py：自定义上下文管理器
来源：http://hz.jianghu66.top/gtoaieqmnh.html

@contextlib.contextmanager
来源：http://hz.xziqi.cn/gtzxxikjld.html

[U22] Py：矩阵转置
来源：http://hz.shzxlz.cn/gthzdzqsny.html

list(zip(*m))
来源：http://hz.tianlin.xyz/gtestgoopa.html

[U23] Py：分块读取大文件
来源：http://hz.gotoacloud.top/gtpoygopub.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gogol.net.cn/gtsuwcdalc.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gtfqxqrzxt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxuanxn.top/gtkktijxli.html

[U25] Py：CSV 按字典读
来源：http://hz.zhijiandao.cn/gtwdrszgqo.html

csv.DictReader(f)
来源：http://hz.hongshengwenyu.top/gtoebpewcv.html

[U26] Py：并发下载
来源：http://hz.xuetiantiany.cn/gtsopbtoqt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.haohaochexian.top/gtfbuastfq.html


<!-- 参考信息 -->