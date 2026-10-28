代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xinyue.icu/gtgzxsveod.html

[S10] C：指针与解引用
来源：http://hz.ppjwa.cn/gtwwowtkaq.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtbaspeiic.html

[S11] C：逐行读文件
来源：http://hz.jinqigufen.top/gtfssuqixz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtbtqlzznx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtugbhcngc.html

fclose(f);
来源：http://hz.smart0.xyz/gtwfjozubx.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtfudcrvdm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtjvrxdbeb.html

[S13] C：宏定义
来源：http://hz.pengpengdd.cyou/gtxtuxavke.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtwcvolymk.html

[S14] C：枚举
来源：http://hz.svipenyu.cn/gtwwqrfgfi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinghuilouyu.cn/gtcacuwple.html

[S15] C：类型转换
来源：http://hz.sysykeji.top/gtesinirkd.html

(double) a / b
来源：http://hz.tianlin.xyz/gtpksyouea.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gthrkdkmld.html

x |= (1 << 3);
来源：http://hz.zhoulong.xyz/gtybziboan.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gtgkascjmq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ivvv.top/gtagfruheu.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gtdjcyoaod.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gtudbnflgj.html

[S19] C：快速排序
来源：http://hz.meibo888.top/gtapjuyyzs.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtqbuvkopi.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtnvdwqbsi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtwfyplumk.html

[S21] C：字符类别判断
来源：http://hz.jiagoushi.top/gtvdezwyqu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gticridsdk.html

[S22] C：字符串转数字
来源：http://hz.sufxvd.cn/gtnzerrjug.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jianghu66.top/gtxkhxbqqs.html

[S23] C：随机数
来源：http://hz.wangshuangyany.cn/gtzqoekwtj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.redwolf501.top/gtxhunsnps.html

[S24] C：获取本地时间
来源：http://hz.guowangkeji.top/gtekqamdxc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtqfysobeu.html

[S25] C：内存拷贝
来源：http://hz.dianchejie.cn/gtysetipfp.html

memcpy(dst, src, n);
来源：http://hz.cqqwz.cn/gtyufggjom.html

[S26] C：内存清零
来源：http://hz.tanke756.top/gtwnziecoh.html

memset(a, 0, sizeof a);
来源：http://hz.aizwys.cn/gtccvwskyp.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gtjooftsbo.html

const double PI = 3.14159;
来源：http://hz.tian-w.cn/gtlpjpyuvs.html

[S28] C：静态变量
来源：http://hz.nanxuanxn.top/gtcdcaupny.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtkyebzilq.html

[S29] C：变参函数
来源：http://hz.jyoumei.cn/gtidijkgxh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnxiangtu.top/gtnbzxlnzs.html

[S30] C：头文件保护
来源：http://hz.gogol.net.cn/gtalxlpkmb.html

#ifndef X_H
来源：http://hz.jinqigufen.top/gtrkvazmph.html

#define X_H
来源：http://hz.jiagoushi.top/gtfhvpyadt.html

#endif
来源：http://hz.fzhhl.top/gtlfupyycx.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtuwyqejqr.html

#include <iostream>
来源：http://hz.hysaishi.cn/gtxjlnlage.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hywenlv.cn/gtgulmglyv.html

[S32] C++：字符串
来源：http://hz.cucudq.cn/gtqgyskayb.html

std::string s = "hi";  s += "!";
来源：http://hz.yueranfly.top/gtmcsmwsnv.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtharwmuod.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gthxcwecpp.html

[S34] C++：遍历 vector
来源：http://hz.cqqwz.cn/gtiaxwutbj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sysykeji.top/gtdjkycqmh.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtbnjnnwwc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtdxgoixwn.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtkowygssn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gthzvevzcp.html

[S37] C++：set
来源：http://hz.xziqi.cn/gtpgwqgszw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fzhhl.top/gtsgwcdakc.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtfgxctabv.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtwkcnlqrd.html

[S39] C++：自定义比较器排序
来源：http://hz.tian-w.cn/gtpvdalagd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtlicolqge.html

[S40] C++：查找元素
来源：http://hz.pengpengdd.cyou/gtyggpkozb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhoulong.xyz/gtvhilusmc.html

[S41] C++：类与构造函数
来源：http://hz.birdmap.top/gtpjoubraz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gtyrrglviz.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gtihuanxup.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtxzqfsmvz.html

[S43] C++：智能指针
来源：http://hz.0kj1m.cn/gtcxzyedyp.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj202588.top/gtcfdrlcmn.html

[S44] C++：引用传参
来源：http://hz.fengsongda.top/gtqtaiongk.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigufen.top/gtapoymmwm.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtxpklhurz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtlnskllik.html

[S46] C++：函数模板
来源：http://hz.ehwqpu.com/gtsfkezynh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtvciueavm.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtagkivhpt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhongyouzk.top/gtfbnwtizp.html

[S48] C++：逐行读文件
来源：http://hz.xylfe.cn/gtnrmehksg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gtmznrjxco.html

while (std::getline(in, line)) { }
来源：http://hz.dianchejie.cn/gtjrqaxbtr.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gtmkthwspk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtsvxlpeqo.html

[S50] C++：格式化数字
来源：http://hz.kuanghao11.cn/gtgemqillx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtkaypomsj.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtxhestbwj.html

static_cast<double>(a) / b
来源：http://hz.feifeiyinyue.top/gtplmnfmaj.html

[S52] C++：const 与 noexcept
来源：http://hz.yuanzhike.top/gtclwjpaer.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gthdaqxcmb.html

[S53] C++：移动语义
来源：http://hz.fzhhl.top/gtbdovkidf.html

std::vector<int> w = std::move(v);
来源：http://hz.dashuyun.cn/gtspkgvuiw.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gtteccczpl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zdqjudy.top/gtagtcaagn.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gtfiyamfye.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tianlin.xyz/gtxyvdogta.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtjnensbyz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gttkakqbqg.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtscqfjfdq.html

constexpr int N = 10;
来源：http://hz.ydjk.org.cn/gtrxycyvre.html

[S58] C++：命名空间
来源：http://hz.fengsongda.top/gtxgoxwshc.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gtubkflfal.html

[S59] C++：静态断言
来源：http://hz.mhx1999.top/gtdhmgxkit.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtdbagesoe.html

[S60] C++：遍历并删除元素
来源：http://hz.yanxiufei.cn/gthlfaxara.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gturujnsnw.html

================================================================================
来源：http://hz.hfpthk.cn/gtbxyhwyxa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtrdluwsqa.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtusyrwyzh.html

[T01] Kotlin：Hello World
来源：http://hz.xylfe.cn/gtnwcnpsyx.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtaubdjohb.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtzudsbcnv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fzhhl.top/gtlqaspnkz.html

[T03] Kotlin：字符串模板
来源：http://hz.tanke756.top/gtfmfbpsjt.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gtuvmdywxb.html

[T04] Kotlin：空安全
来源：http://hz.hongshengwenyu.top/gtnmnqhehd.html

val n: String? = null;  n?.length
来源：http://hz.zhiwuduotai.top/gtqckfdhpz.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gtsqmvsfnp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenlongwang.top/gtchnxoxxg.html

[T06] Kotlin：集合映射
来源：http://hz.nanxinkj.top/gtwraspeel.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydzc1.top/gtslavfapm.html

[T07] Kotlin：集合过滤
来源：http://hz.xinyue.icu/gtxxhlneab.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.9152youxi.cn/gthsafvwry.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtdhvocmdo.html

data class User(val name: String, val age: Int)
来源：http://hz.pycfn.com/gtdcomtmbp.html

[T09] Kotlin：扩展函数
来源：http://hz.ppjwa.cn/gtyyjybhbh.html

fun String.exclaim() = this + "!"
来源：http://hz.yongpay.top/gtenhqtrnm.html

[T10] Kotlin：默认参数
来源：http://hz.yuxming.cn/gtfnhvvvho.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.havefunace.top/gttpmrtwtp.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtxjxotfri.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jianghu66.top/gtekjjgnor.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangtech.top/gtakbsxoqa.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gtnouuprhh.html

[T13] Kotlin：只读 Map
来源：http://hz.zhongyouzk.top/gtojosucna.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtmxbbdhis.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gtbjwuyalt.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangtech.top/gteefvzoqo.html

[T15] Kotlin：接口
来源：http://hz.jqgfzy.top/gtgzcdievq.html

interface Shape { fun area(): Double }
来源：http://hz.xingfuxueyuan.xyz/gtifaopbxu.html

[T16] Swift：Hello World
来源：http://hz.xinyue.icu/gtbcujtsbq.html

print("Hello")
来源：http://hz.9152youxi.cn/gtthbgfevy.html

[T17] Swift：变量与常量
来源：http://hz.ydzc1.top/gtbhpmgelf.html

var a = 1;  let b = 2
来源：http://hz.ybcxt.top/gtyylbppzj.html

[T18] Swift：字符串插值
来源：http://hz.xuetiantiany.cn/gtzhghdhoy.html

"值: \(b)"
来源：http://hz.cucudq.cn/gtuhaavdep.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtzpnjftte.html

if let n = opt { print(n) }
来源：http://hz.chenjidiqi.icu/gtlhvcwqqz.html

[T20] Swift：数组操作
来源：http://hz.chenjidiqi.icu/gtcyorbnwx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuanzhike.top/gtuzjvpxgb.html

[T21] Swift：遍历
来源：http://hz.hnxiangtu.top/gtuznrnmrg.html

for x in a { print(x) }
来源：http://hz.shzxlz.cn/gtkndlevku.html

[T22] Swift：字典
来源：http://hz.dianchejie.cn/gtipujmdro.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hysaishi.cn/gttqkjdewj.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtlampkczr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.0kj1m.cn/gtdnjbqrof.html

[T24] Swift：闭包
来源：http://hz.yj20258888.top/gtbdnpfrxj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sysykeji.top/gtwhbxrjpn.html

[T25] Swift：结构体
来源：http://hz.jinqigufen.top/gtqqkiwuym.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gtjbecwlor.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtfxsmqlsg.html

class A: Base { override func f() {} }
来源：http://hz.redwolf501.top/gtymskrmqg.html

[T27] Swift：错误处理
来源：http://hz.yuanzhike.top/gtpnfemglz.html

do { try f() } catch { print(error) }
来源：http://hz.cdnleiting.top/gtkqxzisct.html

[T28] Swift：枚举
来源：http://hz.zdqjudy.top/gteptlhmzw.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gtzjdrvlje.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gtyfxydcrw.html

guard let x = opt else { return }
来源：http://hz.cucudq.cn/gtlnimdnsj.html

[T30] Swift：协议
来源：http://hz.wangshuangyany.cn/gtgfjuzpjp.html

protocol Shape { func area() -> Double }
来源：http://hz.aizwys.cn/gtptfqzxqs.html

[T31] Lua：Hello World
来源：http://hz.ywan-chungtsiang.top/gtqlvqwvqp.html

print("Hello")
来源：http://hz.fzhhl.top/gtwrcgtzde.html

[T32] Lua：局部变量
来源：http://hz.yueranfly.top/gtbhucgour.html

local a = 1
来源：http://hz.gzhubu.top/gtpixmmpcd.html

[T33] Lua：表（数组）
来源：http://hz.quarkkingdee.top/gtfvcixuuu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtnpdagoms.html

[T34] Lua：遍历表
来源：http://hz.jinyuanbaomall.cn/gtsazqnnja.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtgwvickbe.html

[T35] Lua：字典表
来源：http://hz.sweek.top/gtgcwqsebp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.svipenyu.cn/gtdaebzcxi.html

[T36] Lua：函数
来源：http://hz.cheryme.top/gtgfnzjgwi.html

function add(a, b) return a + b end
来源：http://hz.tanke756.top/gtclsoquew.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigufen.top/gtuawufadn.html

"a" .. "b"
来源：http://hz.hysaishi.cn/gterdzyzbk.html

[T38] Lua：条件
来源：http://hz.jqgfzy.top/gtbmyllopj.html

if x > 0 then print("正") end
来源：http://hz.shuidangran.top/gtxfutreds.html

[T39] Lua：模式匹配
来源：http://hz.yueranfly.top/gtbpqeuxdz.html

string.find(s, "%d+")
来源：http://hz.shzxlz.cn/gtwgnbkdzj.html

[T40] Lua：元表
来源：http://hz.zhixingplan.top/gtynwozkhj.html

setmetatable({}, { __index = base })
来源：http://hz.xylfe.cn/gtnwpmyaag.html

[T41] Perl：Hello World
来源：http://hz.fengsongda.top/gtagpismil.html

print "Hello\n";
来源：http://hz.tanke756.top/gtoparxtzy.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtoyjnioxl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yvedp.cn/gttzofxfkq.html

[T43] Perl：字符串插值
来源：http://hz.yongpay.top/gtithjspwj.html

"值: $a"
来源：http://hz.0kj1m.cn/gtqikkolwv.html

[T44] Perl：条件
来源：http://hz.zhixingplan.top/gttsvqstfr.html

if ($a > 0) { print "正"; }
来源：http://hz.chenzaomai.com/gtkojkdeco.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gtrqzgjyya.html

for my $x (@arr) { print $x; }
来源：http://hz.fzhhl.top/gtqifexong.html

[T46] Perl：哈希操作
来源：http://hz.redwolf501.top/gtgojiyteu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shzxlz.cn/gtsjodqaov.html

[T47] Perl：正则捕获
来源：http://hz.pengpengdd.cyou/gtcnplzrew.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sweek.top/gttwyqlspx.html

[T48] Perl：正则替换
来源：http://hz.zhijiandao.cn/gtdqnhljlk.html

$s =~ s/old/new/g;
来源：http://hz.hysaishi.cn/gtsxzkuplh.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gtshaullpx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.quarkkingdee.top/gtdlrzuojp.html

[T50] Perl：逐行读文件
来源：http://hz.chenlongwang.top/gtrudonyto.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.daxiang520.top/gtzkxgeaaw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cheryme.top/gtwquoxffs.html

[T51] Scala：Hello World
来源：http://hz.xylfe.cn/gtiekprlgg.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtvkuzpimw.html

[T52] Scala：变量
来源：http://hz.gzhubu.top/gtwwsnkxpb.html

val a = 1;  var b = 2
来源：http://hz.jqgfzy.top/gtkljsahkd.html

[T53] Scala：字符串插值
来源：http://hz.gzhubu.top/gtdnzhdzfk.html

s"值: $b"
来源：http://hz.chenlongwang.top/gtdacqbbmg.html

[T54] Scala：集合映射
来源：http://hz.yonumen.top/gtddbqfphc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhiwuduotai.top/gtssfokadh.html

[T55] Scala：集合过滤
来源：http://hz.ehwqpu.com/gtzcbzzcey.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.quarkkingdee.top/gtcsktbzrr.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gtmlqxwffi.html

case class User(name: String, age: Int)
来源：http://hz.andypj.xyz/gtfihfhylp.html

[T57] Scala：模式匹配
来源：http://hz.hywenlv.cn/gtnxldyeqi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.svipenyu.cn/gttkasvwkv.html

[T58] Scala：函数定义
来源：http://hz.daria6918.cn/gtsjklqeye.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jiagoushi.top/gtticsdvak.html

[T59] Scala：循环
来源：http://hz.cucudq.cn/gtcvguurth.html

for (i <- 1 to 10) println(i)
来源：http://hz.gotoacloud.top/gtkrprgknw.html

[T60] Scala：折叠
来源：http://hz.chenzaomai.com/gtohqfxyxb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.havefunace.top/gtxuxilnqi.html

================================================================================
来源：http://hz.andypj.xyz/gtnupguiar.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnxiangtu.top/gtnpdvddfj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gteohvkrxu.html

[U01] Py：创建虚拟环境
来源：http://hz.snrcjt.cn/gtzpohpmyl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuanzx.com/gtucfammcv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.guowangkeji.top/gtghruujfa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.iojbl.cn/gttucpimlp.html

[U03] Py：加载 .env 配置
来源：http://hz.52xcode.cn/gtojsrzlys.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xuetiantiany.cn/gtqovbamcl.html

[U04] Py：变量调试打印
来源：http://hz.ywan-chungtsiang.top/gtxvwvdkwd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.fengsongda.top/gtumfatlgt.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtxwiihqih.html

list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gtosobcjkc.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtfamcdvii.html

{**a, **b}
来源：http://hz.daria6918.cn/gtuqphqyud.html

[U07] Py：反转字典键值
来源：http://hz.jqgufenzy.top/gtzlvcunkf.html

{v: k for k, v in d.items()}
来源：http://hz.jinghuilouyu.cn/gtzdeefhkp.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gtmtpbeiep.html

[y for x in nested for y in x]
来源：http://hz.nwbrower.top/gtpogvqsat.html

[U09] Py：字典取最大值的键
来源：http://hz.chenjidiqi.icu/gtkiaaczqr.html

max(d, key=d.get)
来源：http://hz.yueranfly.top/gtabazqemp.html

[U10] Py：按值排序字典
来源：http://hz.svipenyu.cn/gtppfcerwd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gthmtijvvz.html

[U11] Py：生成器表达式
来源：http://hz.316326.xyz/gtoedqlftm.html

(x * 2 for x in arr)
来源：http://hz.daxiang520.top/gtcevzvvva.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cucudq.cn/gtqmciprdt.html

Counter(arr).most_common(3)
来源：http://hz.tian-w.cn/gtdiodptvf.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtvryoeszh.html

deque(maxlen=10)
来源：http://hz.jinqigufen.top/gtwrizwvbd.html

[U14] Py：分组收集到列表
来源：http://hz.jlsjyb.cn/gtiirwnwpf.html

defaultdict(list)
来源：http://hz.xuetiantiany.cn/gtizkjvgnv.html

[U15] Py：高精度计时
来源：http://hz.gaohongyu789.top/gtiybrairh.html

t = time.perf_counter()
来源：http://hz.ivvv.top/gtncodfkfz.html

[U16] Py：命令行参数解析
来源：http://hz.feifeiyinyue.top/gtkjufskwl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.guowangkeji.top/gtsyznkvql.html

[U17] Py：初始化日志
来源：http://hz.yj20258888.top/gtouiozvgt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shzxlz.cn/gtvgqxlvlr.html

[U18] Py：预编译正则
来源：http://hz.shangyingyoupin.top/gthysooqjj.html

pat = re.compile(r"\d+")
来源：http://hz.shuidangran.top/gtcwytiodn.html

[U19] Py：正则替换带回调
来源：http://hz.cqqwz.cn/gtrfntjpgh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sufxvd.cn/gtceijklap.html

[U20] Py：缓存函数结果
来源：http://hz.cdnleiting.top/gtilebrmgt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cashguo.top/gtxpkntrul.html

[U21] Py：自定义上下文管理器
来源：http://hz.cdnleiting.top/gthdjgkgoi.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gtpshrdkod.html

[U22] Py：矩阵转置
来源：http://hz.tanke756.top/gtfiabzygm.html

list(zip(*m))
来源：http://hz.vqdsnc.cn/gtzxtiipbw.html

[U23] Py：分块读取大文件
来源：http://hz.9152youxi.cn/gtebompsnc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.smart0.xyz/gtapiikwgw.html

[U24] Py：路径操作
来源：http://hz.cqqwz.cn/gtelhchjzb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.havefunace.top/gttnntaaws.html

[U25] Py：CSV 按字典读
来源：http://hz.9152youxi.cn/gtsmnegccx.html

csv.DictReader(f)
来源：http://hz.zhaomingkeji.xyz/gtpfgtsnnu.html

[U26] Py：并发下载
来源：http://hz.tianlin.xyz/gtkepwhrxj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yvedp.cn/gtctumralj.html

[U27] Py：异步 HTTP
来源：http://hz.nanxuanxn.top/gtkwnogsar.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.vqdsnc.cn/gthrdfjrlj.html

[U28] Py：类型别名
来源：http://hz.pycfn.com/gtihohnxxm.html

UserId = int
来源：http://hz.zycfv.cn/gticbuluua.html

[U29] Py：属性校验
来源：http://hz.quarkkingdee.top/gtxgoldwsn.html

@property 与 @x.setter 配合
来源：http://hz.birdmap.top/gteszyhact.html

[U30] Py：数据类
来源：http://hz.shuidangran.top/gtarnvgdpp.html

@dataclass(slots=True)
来源：http://hz.cucudq.cn/gtdydlukri.html

[U31] Py：单测
来源：http://hz.vqdsnc.cn/gtlbzqfltr.html

python -m pytest -q
来源：http://hz.andypj.xyz/gtrwzjmhvp.html

[U32] Py：代码格式化
来源：http://hz.yonumen.top/gtitslwnyy.html

ruff format . && ruff check --fix .
来源：http://hz.cheryme.top/gtsznybnsj.html


<!-- 参考信息 -->