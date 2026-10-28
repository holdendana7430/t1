代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.316326.xyz/gtwqajtpfm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhoulong.xyz/gtckpmrfrx.html

fclose(f);
来源：http://hz.ehwqpu.com/gtiyjynmjd.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtaqhbrnhd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gthquqiksm.html

[S13] C：宏定义
来源：http://hz.yongpay.top/gtfcpqpytz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtfyelgikx.html

[S14] C：枚举
来源：http://hz.haohaochexian.top/gtrryoqech.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtknswtyts.html

[S15] C：类型转换
来源：http://hz.ydzc1.top/gtchtkxmto.html

(double) a / b
来源：http://hz.yangfankeji.com/gtdtzvaqnm.html

[S16] C：位操作置位
来源：http://hz.ydjk.org.cn/gtiuypyscm.html

x |= (1 << 3);
来源：http://hz.jlsjyb.cn/gtoaeizybm.html

[S17] C：安全拼接字符串
来源：http://hz.guannengcc.top/gtlbfrtixc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fengsongda.top/gtssvuvlgu.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangkeji.top/gtabtxpqpr.html

int main(int argc, char **argv)
来源：http://hz.hammf.cn/gtggkotwvu.html

[S19] C：快速排序
来源：http://hz.guannengcc.top/gtxyqlsbxb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtyczpaunl.html

[S20] C：二分查找
来源：http://hz.kuanghao11.cn/gtwuvfbsjv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtyhbzzazn.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtaheaojoe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtrejjdtch.html

[S22] C：字符串转数字
来源：http://hz.yj20258888.top/gtexlnegma.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cdnleiting.top/gtqocnkkht.html

[S23] C：随机数
来源：http://hz.cheryme.top/gtbsrdskpj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtfwehxkho.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtpgpnljhr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cqqwz.cn/gtrmmbumnz.html

[S25] C：内存拷贝
来源：http://hz.jiagoushi.top/gtcbbthbyj.html

memcpy(dst, src, n);
来源：http://hz.hongshengwenyu.top/gtnltsehcx.html

[S26] C：内存清零
来源：http://hz.yj20258888.top/gtulsljxjv.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258888.top/gtnqqhfwwy.html

[S27] C：定义常量
来源：http://hz.daxiang520.top/gtrzptgybm.html

const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtgoixtuwk.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtbzddqwdx.html

static int counter = 0;
来源：http://hz.fzhhl.top/gttvomabvh.html

[S29] C：变参函数
来源：http://hz.jqgfzy.top/gtwechdzun.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gtyrhhynbs.html

[S30] C：头文件保护
来源：http://hz.wangdashe.top/gtxvjzunvn.html

#ifndef X_H
来源：http://hz.jlsjyb.cn/gtolsteexg.html

#define X_H
来源：http://hz.yueranfly.top/gtaypvesfb.html

#endif
来源：http://hz.guowangkeji.top/gtmyovsudn.html

[S31] C++：Hello World
来源：http://hz.hnqzz.top/gthqhxdrir.html

#include <iostream>
来源：http://hz.daria6918.cn/gtbyhiwnit.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtgbygysth.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtgmtxnmaj.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxuanxn.top/gtwwroucwu.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtafrqbobv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ivvv.top/gtdovixtkm.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtsejnhvfv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtxqjdpcyk.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gttrdqgryh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtrxtsspmx.html

[S36] C++：unordered_map
来源：http://hz.yueranfly.top/gtcpjunglz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtfwvvzxdh.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtosefjmos.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtsbckfdza.html

[S38] C++：排序
来源：http://hz.ydjk.org.cn/gtxqvxiehy.html

std::sort(v.begin(), v.end());
来源：http://hz.jianghu66.top/gtcfxrljaa.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtlbbogxkt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtrjhmpjyj.html

[S40] C++：查找元素
来源：http://hz.nwbrower.top/gtyuxetyzt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gttmrqruyh.html

[S41] C++：类与构造函数
来源：http://hz.zhoulong.xyz/gtcmdrljcm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.smart0.xyz/gtsyjxahjs.html

[S42] C++：继承与虚函数
来源：http://hz.zhixingplan.top/gtzrrfevos.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtnhhekhlr.html

[S43] C++：智能指针
来源：http://hz.jiagoushi.top/gtomnmfmye.html

auto p = std::make_unique<int>(5);
来源：http://hz.dashuyun.cn/gtpomfgsoj.html

[S44] C++：引用传参
来源：http://hz.yj20258888.top/gtuvrczefr.html

void inc(int &x) { ++x; }
来源：http://hz.jyoumei.cn/gttnvmfaxp.html

[S45] C++：lambda
来源：http://hz.hfpthk.cn/gtdzdzintl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuanzx.com/gtyernzaub.html

[S46] C++：函数模板
来源：http://hz.yuanzhike.top/gtozbqmkmy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.birdmap.top/gtehyleilk.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangkeji.top/gtdbialrij.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258.top/gtmczcaqmj.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtqfjtjldc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jyoumei.cn/gthaabqjez.html

while (std::getline(in, line)) { }
来源：http://hz.c1oappe.top/gtviuyiicm.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtcyhsrjch.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guannengcc.top/gtceiodono.html

[S50] C++：格式化数字
来源：http://hz.hammf.cn/gtyfpwvphr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtwwtixfgv.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gttwsqdmqn.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gtafcfkxbu.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gtnlbekgod.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtzjtutvfq.html

[S53] C++：移动语义
来源：http://hz.yj20258.top/gtghaggygf.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gtoakyslko.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gteoildxpw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ehwqpu.com/gtacjbqdtz.html

[S55] C++：结构化绑定
来源：http://hz.snrcjt.cn/gtnmncyhyo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hfpthk.cn/gtracuilov.html

[S56] C++：optional
来源：http://hz.pengpengdd.cyou/gtdajeaqoe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtohtcdiaw.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gtzuulpkqn.html

constexpr int N = 10;
来源：http://hz.hammf.cn/gtwwwxowbe.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtrumoxcms.html

namespace ns { int f() { return 1; } }
来源：http://hz.feifeiyinyue.top/gtxzuuvpfv.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtfvjoorcr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aibaodan.cn/gtflfnqecd.html

[S60] C++：遍历并删除元素
来源：http://hz.zdqjudy.top/gtlkoasezl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenlongwang.top/gtdtpytwpj.html

================================================================================
来源：http://hz.hnqzz.top/gtqtiesdck.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jlsjyb.cn/gtystctdii.html

================================================================================
来源：http://hz.chenzaomai.com/gtpqpafqqc.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtzpkufcmn.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtqbdcwici.html

[T02] Kotlin：变量
来源：http://hz.ydjk.org.cn/gtavksnanz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.316326.xyz/gtmrukujba.html

[T03] Kotlin：字符串模板
来源：http://hz.haohaochexian.top/gtlyccsqzb.html

"值: $b"
来源：http://hz.wangshuangyany.cn/gtsadqsvqf.html

[T04] Kotlin：空安全
来源：http://hz.tianlin.xyz/gthzwcamxc.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtgdvfwehs.html

[T05] Kotlin：when 表达式
来源：http://hz.fzhhl.top/gtnxunriuh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtylxykykm.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtcfagfjai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daxiang520.top/gtsledrtyl.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gttzakkhyi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fengsongda.top/gtcqjsxkls.html

[T08] Kotlin：数据类
来源：http://hz.jqgufenzy.top/gtdsvvcxfm.html

data class User(val name: String, val age: Int)
来源：http://hz.redwolf501.top/gtphvrzqyr.html

[T09] Kotlin：扩展函数
来源：http://hz.chenlongwang.top/gtzxpxidzs.html

fun String.exclaim() = this + "!"
来源：http://hz.vqdsnc.cn/gtlratfkbs.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtjmybrddu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtoznbrtic.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtzeqwhetb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.quarkkingdee.top/gtndwotgie.html

[T12] Kotlin：解构声明
来源：http://hz.haohaochexian.top/gtmqtxhfdh.html

val (a, b) = Pair(1, 2)
来源：http://hz.jlsjyb.cn/gtkklbzagj.html

[T13] Kotlin：只读 Map
来源：http://hz.xinyue.icu/gtgzcxmsos.html

val m = mapOf("a" to 1)
来源：http://hz.ydjk.org.cn/gtqgxjslqh.html

[T14] Kotlin：循环
来源：http://hz.52xcode.cn/gtxhyvxhpl.html

for (i in 1..10) println(i)
来源：http://hz.zycfv.cn/gttkjrqrrq.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gthafclpct.html

interface Shape { fun area(): Double }
来源：http://hz.hammf.cn/gtqhflyjjm.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtyevhmobo.html

print("Hello")
来源：http://hz.kuanghao11.cn/gtbnxhduqr.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gtdhxydbqs.html

var a = 1;  let b = 2
来源：http://hz.nanxuanxn.top/gtgtukpons.html

[T18] Swift：字符串插值
来源：http://hz.yj20258888.top/gtdauztwbl.html

"值: \(b)"
来源：http://hz.yangfankeji.com/gtryfayumi.html

[T19] Swift：可选绑定
来源：http://hz.ppjwa.cn/gtcvfaklqy.html

if let n = opt { print(n) }
来源：http://hz.xziqi.cn/gttnyvbene.html

[T20] Swift：数组操作
来源：http://hz.zhoulong.xyz/gtgnbznejn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ybcxt.top/gtaaifbrwp.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gtbscstopr.html

for x in a { print(x) }
来源：http://hz.jiagoushi.top/gtreauzquu.html

[T22] Swift：字典
来源：http://hz.xingfuxueyuan.xyz/gtarfgfvtx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.vqdsnc.cn/gtcqxldrav.html

[T23] Swift：函数
来源：http://hz.yueranfly.top/gtckwylhmw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gttcewabct.html

[T24] Swift：闭包
来源：http://hz.c1oappe.top/gtlxekqzfe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sweek.top/gteqmswzej.html

[T25] Swift：结构体
来源：http://hz.hnxiangtu.top/gtsixbvvdn.html

struct P { var x: Int }
来源：http://hz.shanyushiyangkeji.top/gtyjbwnveu.html

[T26] Swift：类与重写
来源：http://hz.0kj1m.cn/gtdgvuqpdf.html

class A: Base { override func f() {} }
来源：http://hz.shangyingyoupin.top/gtimsusdnx.html

[T27] Swift：错误处理
来源：http://hz.tianlin.xyz/gtmtehwcwk.html

do { try f() } catch { print(error) }
来源：http://hz.sysykeji.top/gtemugthez.html

[T28] Swift：枚举
来源：http://hz.9152youxi.cn/gtjmpterbn.html

enum Color { case red, green }
来源：http://hz.zhoulong.xyz/gtbekgrmsr.html

[T29] Swift：guard 提前返回
来源：http://hz.jinyuanbaomall.cn/gtpkfmytco.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangkeji.top/gtnfguitha.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gtckypqcht.html

protocol Shape { func area() -> Double }
来源：http://hz.fengsongda.top/gtltkylohe.html

[T31] Lua：Hello World
来源：http://hz.sweek.top/gtbhcukarg.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtsljvhgdy.html

[T32] Lua：局部变量
来源：http://hz.yvedp.cn/gtwetlhiww.html

local a = 1
来源：http://hz.hammf.cn/gtgrffziod.html

[T33] Lua：表（数组）
来源：http://hz.zhongyouzk.top/gthojjgpxw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhengqikj.top/gtktdmcuib.html

[T34] Lua：遍历表
来源：http://hz.nanxinkj.top/gtozchxxus.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinghuilouyu.cn/gtyphotpaf.html

[T35] Lua：字典表
来源：http://hz.yj202588.top/gtupaklalv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tianlin.xyz/gtniragyoa.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtlnflxghc.html

function add(a, b) return a + b end
来源：http://hz.yongpay.top/gtolcrbjwb.html

[T37] Lua：字符串拼接
来源：http://hz.quarkkingdee.top/gtedjddgqu.html

"a" .. "b"
来源：http://hz.ywan-chungtsiang.top/gtiswkdfoo.html

[T38] Lua：条件
来源：http://hz.zhiwuduotai.top/gtrkvqbajk.html

if x > 0 then print("正") end
来源：http://hz.sysykeji.top/gtqgfbwhvp.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangtech.top/gtlwhoanxv.html

string.find(s, "%d+")
来源：http://hz.hfpthk.cn/gtpqhkfndq.html

[T40] Lua：元表
来源：http://hz.zycfv.cn/gtzspbpzwa.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtjeaoweuq.html

[T41] Perl：Hello World
来源：http://hz.xuanzx.com/gtvgwjsvhy.html

print "Hello\n";
来源：http://hz.jinyuanbaomall.cn/gtcapkswwd.html

[T42] Perl：变量类型
来源：http://hz.xingfuxueyuan.xyz/gtobjppodb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cucudq.cn/gtornwiqne.html

[T43] Perl：字符串插值
来源：http://hz.xuanzx.com/gtvmquolzv.html

"值: $a"
来源：http://hz.hongshengwenyu.top/gtyxamjncg.html

[T44] Perl：条件
来源：http://hz.shuidangran.top/gtoljripig.html

if ($a > 0) { print "正"; }
来源：http://hz.gogol.net.cn/gtglfhdzwp.html

[T45] Perl：数组遍历
来源：http://hz.tianlin.xyz/gtdumtnnmm.html

for my $x (@arr) { print $x; }
来源：http://hz.316326.xyz/gtgqhqnxjw.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gtexllgdsl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jiagoushi.top/gthmczhkce.html

[T47] Perl：正则捕获
来源：http://hz.ybcxt.top/gtfklbrxfs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.fengsongda.top/gtgxncggfz.html

[T48] Perl：正则替换
来源：http://hz.jqgfzy.top/gtqbvuexfi.html

$s =~ s/old/new/g;
来源：http://hz.cdnleiting.top/gtyeaqzvea.html

[T49] Perl：函数
来源：http://hz.yongpay.top/gthelgwkrs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hfpthk.cn/gtoyzuhqqd.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gtzoswrumn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtcxuxmgzx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nwbrower.top/gtzktmcxho.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtntgrgzgj.html

println("Hello")
来源：http://hz.0kj1m.cn/gtuogsfwsw.html

[T52] Scala：变量
来源：http://hz.zhaomingkeji.xyz/gtdpcwyuey.html

val a = 1;  var b = 2
来源：http://hz.ywan-chungtsiang.top/gtjgtodhjn.html

[T53] Scala：字符串插值
来源：http://hz.nanxinkj.top/gtpzmmgtwt.html

s"值: $b"
来源：http://hz.zhongyouzk.top/gtbscejtfh.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gtosixrbri.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cashguo.top/gthfordbzv.html

[T55] Scala：集合过滤
来源：http://hz.tian-w.cn/gtouitltyj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangkeji.top/gttxlbxmms.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtzizqmbsw.html

case class User(name: String, age: Int)
来源：http://hz.sxryk.cn/gtgglcegah.html

[T57] Scala：模式匹配
来源：http://hz.xuetiantiany.cn/gtdnhduflt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhengqikj.top/gtuznytzuh.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtftfrllpg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gtduecxvtq.html

[T59] Scala：循环
来源：http://hz.hnxiangtu.top/gtvklqstsb.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtxahfseld.html

[T60] Scala：折叠
来源：http://hz.tian-w.cn/gtkjzkbohh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.havefunace.top/gtmwfbevje.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdfsfhzeo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yueranfly.top/gtitpnreen.html

================================================================================
来源：http://hz.hywenlv.cn/gthyjaqxxt.html

[U01] Py：创建虚拟环境
来源：http://hz.bjfxy.top/gttbnlplxn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gtxrocahnc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigfzy.top/gtvnoezxis.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenlongwang.top/gttcpupiqn.html

[U03] Py：加载 .env 配置
来源：http://hz.hysaishi.cn/gtzhnmvuvp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hysaishi.cn/gtjojlolwf.html

[U04] Py：变量调试打印
来源：http://hz.sxryk.cn/gtyrogwjql.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shangyingyoupin.top/gtqdjxbrjt.html

[U05] Py：列表去重且保序
来源：http://hz.yuanzhike.top/gtfehexuop.html

list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtdlbvrpzd.html

[U06] Py：合并两个字典
来源：http://hz.aibaodan.cn/gtdvuofjgn.html

{**a, **b}
来源：http://hz.xuanzx.com/gtgsjhlxrx.html

[U07] Py：反转字典键值
来源：http://hz.ywan-chungtsiang.top/gtddqaajxr.html

{v: k for k, v in d.items()}
来源：http://hz.gogol.net.cn/gtmpurzjth.html

[U08] Py：展平二维列表
来源：http://hz.yonumen.top/gtumuponew.html

[y for x in nested for y in x]
来源：http://hz.yanxiufei.cn/gtaopqhura.html

[U09] Py：字典取最大值的键
来源：http://hz.xuetiantiany.cn/gtpkmyaqrx.html

max(d, key=d.get)
来源：http://hz.tian-w.cn/gtwqczwezv.html

[U10] Py：按值排序字典
来源：http://hz.ybcxt.top/gtavqvsbon.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hysaishi.cn/gtrbqmenak.html

[U11] Py：生成器表达式
来源：http://hz.fzhhl.top/gtkephcxtb.html

(x * 2 for x in arr)
来源：http://hz.shuidangran.top/gteqiujpug.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zycfv.cn/gtwzjyhbsd.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gttcgbdxza.html

[U13] Py：固定长度队列
来源：http://hz.zhiwuduotai.top/gtlhdynyrx.html

deque(maxlen=10)
来源：http://hz.svipenyu.cn/gtrautbggp.html

[U14] Py：分组收集到列表
来源：http://hz.yanxiufei.cn/gthrbpeych.html

defaultdict(list)
来源：http://hz.pycfn.com/gtnirbmjwo.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gtehgkzjnz.html

t = time.perf_counter()
来源：http://hz.smart0.xyz/gtlzcjefjf.html

[U16] Py：命令行参数解析
来源：http://hz.wangdashe.top/gtbkelqdhw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.vqdsnc.cn/gthquqtbuh.html

[U17] Py：初始化日志
来源：http://hz.ywan-chungtsiang.top/gtynctbblk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xuetiantiany.cn/gtoiuxacze.html

[U18] Py：预编译正则
来源：http://hz.gaohongyu789.top/gtrcawjbqd.html

pat = re.compile(r"\d+")
来源：http://hz.chenzaomai.com/gtrefnzvog.html

[U19] Py：正则替换带回调
来源：http://hz.0kj1m.cn/gtyfywgite.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yueranfly.top/gtnmxglugp.html

[U20] Py：缓存函数结果
来源：http://hz.yj202588.top/gtpwdqudvb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dianchejie.cn/gtalieipho.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhengqikj.top/gtdjevnedk.html

@contextlib.contextmanager
来源：http://hz.ydjk.org.cn/gtjsvbujin.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtkwbssvnm.html

list(zip(*m))
来源：http://hz.feifeiyinyue.top/gtixktsgak.html

[U23] Py：分块读取大文件
来源：http://hz.daxiang520.top/gtlgaxgvqa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.snrcjt.cn/gtbbpxntur.html

[U24] Py：路径操作
来源：http://hz.dianchejie.cn/gtkorqkeio.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258.top/gtlrhsjosh.html

[U25] Py：CSV 按字典读
来源：http://hz.iojbl.cn/gtzgddjogl.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtmkusaydb.html

[U26] Py：并发下载
来源：http://hz.c1oappe.top/gtfioxvsgg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.redwolf501.top/gtgxkmaefi.html

[U27] Py：异步 HTTP
来源：http://hz.birdmap.top/gtiznlukqh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.mhx1999.top/gtxszpkexk.html

[U28] Py：类型别名
来源：http://hz.pycfn.com/gtfchrgloh.html

UserId = int
来源：http://hz.gaohongyu789.top/gttkidcnwm.html

[U29] Py：属性校验
来源：http://hz.xuanzx.com/gthdjsjvxe.html

@property 与 @x.setter 配合
来源：http://hz.wangdashe.top/gtmtmtaqsz.html

[U30] Py：数据类
来源：http://hz.zhoulong.xyz/gtynhakink.html

@dataclass(slots=True)
来源：http://hz.jyoumei.cn/gtajhmwkcz.html

[U31] Py：单测
来源：http://hz.daxiang520.top/gtpqtvvbxs.html

python -m pytest -q
来源：http://hz.andypj.xyz/gtkcxarhwf.html

[U32] Py：代码格式化
来源：http://hz.dianchejie.cn/gtvlvqsaon.html

ruff format . && ruff check --fix .
来源：http://hz.hfpthk.cn/gthlvgzacy.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtcjmmjvwf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangshuangyany.cn/gtsbeobnxj.html

[U34] Py：判断编码
来源：http://hz.redwolf501.top/gtlkvqzoui.html

chardet.detect(raw)
来源：http://hz.jqgufenzy.top/gtpyowqdvk.html


<!-- 参考信息 -->