代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgfzy.top/gtkzkibgnw.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gthmhuhbyt.html

int *p = &a;  *p = 5;
来源：http://hz.gogol.net.cn/gttcruetkf.html

[S11] C：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtzhgldbvr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuetiantiany.cn/gtlgsjsgaz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cucudq.cn/gtauqsrmst.html

fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtolwfdqqi.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtuocntnmh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gttefnhnja.html

[S13] C：宏定义
来源：http://hz.kuanghao11.cn/gtxezbwmnn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zycfv.cn/gtykjcwnfz.html

[S14] C：枚举
来源：http://hz.aizwys.cn/gtrczwzdyu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuanzx.com/gtcvckabuu.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gturvakwdo.html

(double) a / b
来源：http://hz.zhongyouzk.top/gthzjhtmlk.html

[S16] C：位操作置位
来源：http://hz.jinqigufen.top/gtwlwxpssy.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtgetzcrtc.html

[S17] C：安全拼接字符串
来源：http://hz.xuanzx.com/gtlijksvke.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhaomingkeji.xyz/gtffdwpwxu.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtekuegjvv.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtrpkgvmfl.html

[S19] C：快速排序
来源：http://hz.nwbrower.top/gtmoeovqjm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtpfpcjdia.html

[S20] C：二分查找
来源：http://hz.shzxlz.cn/gtrvffdxif.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtnaysbiqn.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtfirmhuhu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gttfqslqbf.html

[S22] C：字符串转数字
来源：http://hz.bjfxy.top/gtllwxqvdw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtflsunyrw.html

[S23] C：随机数
来源：http://hz.sufxvd.cn/gtxfhsoxpa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shuidangran.top/gtqgnvgksg.html

[S24] C：获取本地时间
来源：http://hz.zhijiandao.cn/gttkxargxg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtwdumwkgs.html

[S25] C：内存拷贝
来源：http://hz.kuanghao11.cn/gtzmdpqkyz.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtdwousbem.html

[S26] C：内存清零
来源：http://hz.chenzaomai.com/gtpvalcvuw.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258.top/gtjqjojwpu.html

[S27] C：定义常量
来源：http://hz.havefunace.top/gtsqgpokfl.html

const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gttttieyat.html

[S28] C：静态变量
来源：http://hz.nanxuanxn.top/gtiugxcgic.html

static int counter = 0;
来源：http://hz.hysaishi.cn/gtlhiwmiug.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtqmcsxjjv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fzhhl.top/gtodmfqxrj.html

[S30] C：头文件保护
来源：http://hz.cheryme.top/gtqmyjwylw.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtguzeixdf.html

#define X_H
来源：http://hz.yueranfly.top/gtcimssdnc.html

#endif
来源：http://hz.cashguo.top/gtbagssivf.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtiigdqxvl.html

#include <iostream>
来源：http://hz.tian-w.cn/gthvsmedso.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.andypj.xyz/gtorszbzte.html

[S32] C++：字符串
来源：http://hz.gotoacloud.top/gtqazdkadk.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtzsiljdyj.html

[S33] C++：vector 增删
来源：http://hz.zhoulong.xyz/gtjlmakrtv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yvedp.cn/gtrjgzonsr.html

[S34] C++：遍历 vector
来源：http://hz.cheryme.top/gthnedmxsj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.smart0.xyz/gtyxpmqorg.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtbyuxiewx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtlxqkqpva.html

[S36] C++：unordered_map
来源：http://hz.dashuyun.cn/gtrjmnuukz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtfiswqbcn.html

[S37] C++：set
来源：http://hz.c1oappe.top/gtvgulwxsp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtoqvdfryu.html

[S38] C++：排序
来源：http://hz.shangyingyoupin.top/gtrpzzfaup.html

std::sort(v.begin(), v.end());
来源：http://hz.sufxvd.cn/gtokzbilkp.html

[S39] C++：自定义比较器排序
来源：http://hz.dianchejie.cn/gtagcllgqe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cdnleiting.top/gteqrinyao.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gteirvtdky.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.iojbl.cn/gtuwjlwgnf.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtqakzpjbf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxuanxn.top/gtiywdiaba.html

[S42] C++：继承与虚函数
来源：http://hz.yuxming.cn/gtgexrhtwp.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtpylgjzdo.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtygsxhuiy.html

auto p = std::make_unique<int>(5);
来源：http://hz.havefunace.top/gtebeblgsg.html

[S44] C++：引用传参
来源：http://hz.zhoulong.xyz/gtvhdaxlqd.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtztfanfho.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gtmiyzqrpo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangdashe.top/gtokrwhetw.html

[S46] C++：函数模板
来源：http://hz.zhengqikj.top/gtctfusyzs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuanzx.com/gtgfzoawir.html

[S47] C++：结构化绑定遍历
来源：http://hz.ybcxt.top/gtjvcytjvw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fzhhl.top/gtinbybiqu.html

[S48] C++：逐行读文件
来源：http://hz.316326.xyz/gtdslineom.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenzaomai.com/gtsmiguxyh.html

while (std::getline(in, line)) { }
来源：http://hz.yonumen.top/gtnccdxufs.html

[S49] C++：写文件
来源：http://hz.yuanzhike.top/gtzctonbwv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.feifeiyinyue.top/gtpnoemnik.html

[S50] C++：格式化数字
来源：http://hz.jinghuilouyu.cn/gtwhscbjjt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtszxjvcrj.html

[S51] C++：显式类型转换
来源：http://hz.fengsongda.top/gtsjfmgaoy.html

static_cast<double>(a) / b
来源：http://hz.andypj.xyz/gtimmfnqpk.html

[S52] C++：const 与 noexcept
来源：http://hz.xinyue.icu/gtedqlzuwq.html

int size() const noexcept { return n_; }
来源：http://hz.tanke756.top/gtewkonlul.html

[S53] C++：移动语义
来源：http://hz.tanke756.top/gthxeluoea.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangtech.top/gtxpvmytbr.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gtiewppxyr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtypbpctsx.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangtech.top/gttyfpystl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tianlin.xyz/gtgoacbmks.html

[S56] C++：optional
来源：http://hz.zdqjudy.top/gtexpmbzfj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hywenlv.cn/gtwsfftedj.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtvykvrxev.html

constexpr int N = 10;
来源：http://hz.tianlin.xyz/gtjtapsquk.html

[S58] C++：命名空间
来源：http://hz.aibaodan.cn/gtzeemikrc.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258.top/gtdixelgzr.html

[S59] C++：静态断言
来源：http://hz.redwolf501.top/gttcbbrsux.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhixingplan.top/gtzhkqqyqo.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtedqghyyt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fengsongda.top/gtgvsmyrmm.html

================================================================================
来源：http://hz.mhx1999.top/gtaeysrrlq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtnaflwshl.html

================================================================================
来源：http://hz.yangfankeji.com/gtntdlybil.html

[T01] Kotlin：Hello World
来源：http://hz.meibo888.top/gtxwzuocun.html

println("Hello")
来源：http://hz.jiagoushi.top/gtqvxbgadp.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtjnxkckhh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhoulong.xyz/gtxbfcdcju.html

[T03] Kotlin：字符串模板
来源：http://hz.kuanghao11.cn/gtvkgztlpq.html

"值: $b"
来源：http://hz.yvedp.cn/gtiyrvfsfx.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtraydzhtf.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtnthmnwyq.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtuhwkiypz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhixingplan.top/gtwqakuuds.html

[T06] Kotlin：集合映射
来源：http://hz.redwolf501.top/gthfnyhmon.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fengsongda.top/gtuqoozbpj.html

[T07] Kotlin：集合过滤
来源：http://hz.nwbrower.top/gtbhfvwsqh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xylfe.cn/gtcoqblods.html

[T08] Kotlin：数据类
来源：http://hz.sxryk.cn/gtzwhczgis.html

data class User(val name: String, val age: Int)
来源：http://hz.xinyue.icu/gtwsedianv.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtsstaoquc.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtzsypiwkk.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtvfcufrxx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydzc1.top/gtmeeewgkd.html

[T11] Kotlin：协程
来源：http://hz.jinqigfzy.top/gtgklvhpik.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cashguo.top/gtfcdyzkwn.html

[T12] Kotlin：解构声明
来源：http://hz.chenjidiqi.icu/gtwigiihcv.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtoevvixyt.html

[T13] Kotlin：只读 Map
来源：http://hz.gzhubu.top/gttkhzggrr.html

val m = mapOf("a" to 1)
来源：http://hz.smart0.xyz/gtftqihmxt.html

[T14] Kotlin：循环
来源：http://hz.xziqi.cn/gtvjdgixyu.html

for (i in 1..10) println(i)
来源：http://hz.chenlongwang.top/gtcpmalblw.html

[T15] Kotlin：接口
来源：http://hz.gaohongyu789.top/gtlhoytkfh.html

interface Shape { fun area(): Double }
来源：http://hz.mhx1999.top/gtpnzkbcyb.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtrnsrfrpp.html

print("Hello")
来源：http://hz.yuxming.cn/gtlgfgraka.html

[T17] Swift：变量与常量
来源：http://hz.aizwys.cn/gtclxpmeez.html

var a = 1;  let b = 2
来源：http://hz.hfpthk.cn/gtvuxkznws.html

[T18] Swift：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtojisomvy.html

"值: \(b)"
来源：http://hz.smart0.xyz/gtasiqkxck.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtzvfpmzse.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtfatatdyi.html

[T20] Swift：数组操作
来源：http://hz.havefunace.top/gtpwjfajsp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuxming.cn/gtwhfkwbcl.html

[T21] Swift：遍历
来源：http://hz.gaohongyu789.top/gtuxeouast.html

for x in a { print(x) }
来源：http://hz.hywenlv.cn/gtdkwjxfzv.html

[T22] Swift：字典
来源：http://hz.iojbl.cn/gtovnxizva.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sufxvd.cn/gthjytuxhk.html

[T23] Swift：函数
来源：http://hz.sxryk.cn/gtonfspevv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxuanxn.top/gthxnuilyu.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gtetaeoflx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hfpthk.cn/gtchxgmejh.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gtysmmbspv.html

struct P { var x: Int }
来源：http://hz.sxryk.cn/gtihkyhcdr.html

[T26] Swift：类与重写
来源：http://hz.kuanghao11.cn/gtzqoctkpa.html

class A: Base { override func f() {} }
来源：http://hz.cashguo.top/gtksfuxwpp.html

[T27] Swift：错误处理
来源：http://hz.fzhhl.top/gtaiuqmmjh.html

do { try f() } catch { print(error) }
来源：http://hz.chenzaomai.com/gtsqaknasv.html

[T28] Swift：枚举
来源：http://hz.jiagoushi.top/gthryxggmk.html

enum Color { case red, green }
来源：http://hz.xuanzx.com/gttrkpevgt.html

[T29] Swift：guard 提前返回
来源：http://hz.zhixingplan.top/gttcwatzuw.html

guard let x = opt else { return }
来源：http://hz.yj20258.top/gtvtxcnkat.html

[T30] Swift：协议
来源：http://hz.aibaodan.cn/gtwrnorwcq.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtqqljlbzr.html

[T31] Lua：Hello World
来源：http://hz.kuanghao11.cn/gtanasfnnh.html

print("Hello")
来源：http://hz.sysykeji.top/gtfvdzbaxa.html

[T32] Lua：局部变量
来源：http://hz.zhixingplan.top/gtwoslgxex.html

local a = 1
来源：http://hz.wangdashe.top/gtdswgokcr.html

[T33] Lua：表（数组）
来源：http://hz.sufxvd.cn/gthpjjiewp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangkeji.top/gtlvrvxpvb.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtmnsakbtp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cashguo.top/gtdosoqchm.html

[T35] Lua：字典表
来源：http://hz.hnxiangtu.top/gtspxhdvmy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gtucrnoljo.html

[T36] Lua：函数
来源：http://hz.yangfankeji.com/gttcyklcdj.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtwfpmnxod.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gteatwkidq.html

"a" .. "b"
来源：http://hz.hnqzz.top/gtqfnujjvq.html

[T38] Lua：条件
来源：http://hz.guowangkeji.top/gtpcuqffvx.html

if x > 0 then print("正") end
来源：http://hz.gaohongyu789.top/gthvsmipow.html

[T39] Lua：模式匹配
来源：http://hz.andypj.xyz/gtgkyquzja.html

string.find(s, "%d+")
来源：http://hz.0kj1m.cn/gtarqincyb.html

[T40] Lua：元表
来源：http://hz.mhx1999.top/gtupyxpkwt.html

setmetatable({}, { __index = base })
来源：http://hz.yanxiufei.cn/gtndpabjku.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gtmccumlzt.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtxwmrwnib.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gtteinroih.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuanzx.com/gtougyfxsu.html

[T43] Perl：字符串插值
来源：http://hz.daria6918.cn/gtcxkbdidi.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gtiocvfezs.html

[T44] Perl：条件
来源：http://hz.yonumen.top/gtklemizdn.html

if ($a > 0) { print "正"; }
来源：http://hz.chenlongwang.top/gtdhoiwbrw.html

[T45] Perl：数组遍历
来源：http://hz.ppjwa.cn/gtgunnnrpa.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gtjdusxqjz.html

[T46] Perl：哈希操作
来源：http://hz.pycfn.com/gtnfqrbblc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ehwqpu.com/gtxxchgjet.html

[T47] Perl：正则捕获
来源：http://hz.bjfxy.top/gtswkexqsx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cqqwz.cn/gtyoyxnrhf.html

[T48] Perl：正则替换
来源：http://hz.gaohongyu789.top/gtaskbuvmv.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtocmspnpp.html

[T49] Perl：函数
来源：http://hz.xuanzx.com/gtmbpypxfw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yonumen.top/gtlwwtymww.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtnxltfxfw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.smart0.xyz/gtiobtusip.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenzaomai.com/gtenxifvmt.html

[T51] Scala：Hello World
来源：http://hz.cdnleiting.top/gtcsgpwohv.html

println("Hello")
来源：http://hz.meibo888.top/gtglydmjph.html

[T52] Scala：变量
来源：http://hz.fzhhl.top/gtfutqmkks.html

val a = 1;  var b = 2
来源：http://hz.sufxvd.cn/gtgqnaesbt.html

[T53] Scala：字符串插值
来源：http://hz.hysaishi.cn/gtwsingyrr.html

s"值: $b"
来源：http://hz.c1oappe.top/gtorggyfgl.html

[T54] Scala：集合映射
来源：http://hz.gaohongyu789.top/gtmfwwtnoi.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aizwys.cn/gtvxvtwrps.html

[T55] Scala：集合过滤
来源：http://hz.haohaochexian.top/gtlejapqjk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.redwolf501.top/gttjhgwlvw.html

[T56] Scala：样例类
来源：http://hz.pengpengdd.cyou/gtekosrjek.html

case class User(name: String, age: Int)
来源：http://hz.gotoacloud.top/gtxlxgvcaz.html

[T57] Scala：模式匹配
来源：http://hz.zdqjudy.top/gtgphfzedp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yuxming.cn/gtkiismkfa.html

[T58] Scala：函数定义
来源：http://hz.wangdashe.top/gtfbuyrkwa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cucudq.cn/gtmtmqcxes.html

[T59] Scala：循环
来源：http://hz.yuxming.cn/gtrtijtdfu.html

for (i <- 1 to 10) println(i)
来源：http://hz.havefunace.top/gtjbiouqlu.html

[T60] Scala：折叠
来源：http://hz.hfpthk.cn/gtiflajsmw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daxiang520.top/gtkhahiimf.html

================================================================================
来源：http://hz.meibo888.top/gtwgdxciqa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jianghu66.top/gteytwnolt.html

================================================================================
来源：http://hz.ppjwa.cn/gtphxusyum.html

[U01] Py：创建虚拟环境
来源：http://hz.birdmap.top/gtycupwvyq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtwlvkqwhg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pengpengdd.cyou/gtmmylzbkr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sufxvd.cn/gtbsnnfogs.html

[U03] Py：加载 .env 配置
来源：http://hz.sxryk.cn/gtsxkfetln.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.redwolf501.top/gtshfyciub.html

[U04] Py：变量调试打印
来源：http://hz.zhaomingkeji.xyz/gtjhixbpcl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sweek.top/gttxmdwfue.html

[U05] Py：列表去重且保序
来源：http://hz.xingfuxueyuan.xyz/gtwobzicfq.html

list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtnfxdmxos.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtolrwefre.html

{**a, **b}
来源：http://hz.shanyushiyangtech.top/gttlxrboew.html

[U07] Py：反转字典键值
来源：http://hz.cdnleiting.top/gtwjeekndx.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258888.top/gtcipxadfu.html

[U08] Py：展平二维列表
来源：http://hz.ppjwa.cn/gtefiznlpe.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gtwkulxgcg.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgfzy.top/gtvvwfcukj.html

max(d, key=d.get)
来源：http://hz.ppjwa.cn/gtvrepgtgs.html

[U10] Py：按值排序字典
来源：http://hz.zhengqikj.top/gtodhaaaxi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gogol.net.cn/gtmpdwdayc.html

[U11] Py：生成器表达式
来源：http://hz.yueranfly.top/gtmztntqps.html

(x * 2 for x in arr)
来源：http://hz.sufxvd.cn/gtusvuwsym.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sxryk.cn/gtaqusnboh.html

Counter(arr).most_common(3)
来源：http://hz.meibo888.top/gtmhoaypqe.html

[U13] Py：固定长度队列
来源：http://hz.c1oappe.top/gtelvckfag.html

deque(maxlen=10)
来源：http://hz.wangshuangyany.cn/gtunhtclta.html

[U14] Py：分组收集到列表
来源：http://hz.jqgfzy.top/gtumgxxqnd.html

defaultdict(list)
来源：http://hz.kuanghao11.cn/gttlgbribb.html

[U15] Py：高精度计时
来源：http://hz.andypj.xyz/gthewgvzql.html

t = time.perf_counter()
来源：http://hz.jlsjyb.cn/gtxvbnevww.html

[U16] Py：命令行参数解析
来源：http://hz.yueranfly.top/gtmuguorml.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yueranfly.top/gtslgbiqit.html

[U17] Py：初始化日志
来源：http://hz.jinqigfzy.top/gtcnawxpfu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.c1oappe.top/gtobvhciby.html

[U18] Py：预编译正则
来源：http://hz.jianghu66.top/gtyomgjjvi.html

pat = re.compile(r"\d+")
来源：http://hz.svipenyu.cn/gtvazfifcd.html

[U19] Py：正则替换带回调
来源：http://hz.jyoumei.cn/gtovyooagi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gtgmdjjxaa.html

[U20] Py：缓存函数结果
来源：http://hz.ehwqpu.com/gtntghdkch.html

@functools.lru_cache(maxsize=None)
来源：http://hz.9152youxi.cn/gtuqatibbw.html

[U21] Py：自定义上下文管理器
来源：http://hz.cucudq.cn/gtiqywoxdb.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gtmnfuhdhg.html

[U22] Py：矩阵转置
来源：http://hz.xinyue.icu/gttdrvsoqp.html

list(zip(*m))
来源：http://hz.yj20258888.top/gtajlwxtrn.html

[U23] Py：分块读取大文件
来源：http://hz.birdmap.top/gtvkeubwzn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yonumen.top/gtvgpjvdpa.html

[U24] Py：路径操作
来源：http://hz.snrcjt.cn/gtfalyzehl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuanzx.com/gtieiscvjy.html

[U25] Py：CSV 按字典读
来源：http://hz.jinyuanbaomall.cn/gticebwxyh.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtpxqsaadj.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gtzhwgkbqd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.iojbl.cn/gtkwjfzizt.html

[U27] Py：异步 HTTP
来源：http://hz.vqdsnc.cn/gtaymfgsxv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj20258888.top/gtxvtwuyys.html

[U28] Py：类型别名
来源：http://hz.hywenlv.cn/gtjfacyosn.html

UserId = int
来源：http://hz.wangshuangyany.cn/gtjwrosunt.html

[U29] Py：属性校验
来源：http://hz.xziqi.cn/gtadbvyhvr.html

@property 与 @x.setter 配合
来源：http://hz.feifeiyinyue.top/gtidsbbvnd.html

[U30] Py：数据类
来源：http://hz.tanke756.top/gtqbgqpxmx.html

@dataclass(slots=True)
来源：http://hz.xziqi.cn/gtasjjvgjv.html

[U31] Py：单测
来源：http://hz.52xcode.cn/gtqbatbxjf.html

python -m pytest -q
来源：http://hz.gogol.net.cn/gtxasrxgkn.html

[U32] Py：代码格式化
来源：http://hz.hfpthk.cn/gtpybsogoa.html

ruff format . && ruff check --fix .
来源：http://hz.meibo888.top/gtdnvbsgqt.html


<!-- 参考信息 -->