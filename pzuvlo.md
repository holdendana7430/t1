代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.9152youxi.cn/gtsmlvpget.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtjqqfecdm.html

int *p = &a;  *p = 5;
来源：http://hz.hnqzz.top/gtmwmkdhob.html

[S11] C：逐行读文件
来源：http://hz.ivvv.top/gthbevoxoh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj202588.top/gtspoesigc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtfofxqada.html

fclose(f);
来源：http://hz.yangfankeji.com/gtmbjdcsrx.html

[S12] C：写文件
来源：http://hz.jlsjyb.cn/gtssiuwpsp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtapnmmjpp.html

[S13] C：宏定义
来源：http://hz.ybcxt.top/gtagppqytm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnxiangtu.top/gtktjvuubm.html

[S14] C：枚举
来源：http://hz.316326.xyz/gtirmjvozr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtbpxixmyh.html

[S15] C：类型转换
来源：http://hz.sufxvd.cn/gtykogdnjf.html

(double) a / b
来源：http://hz.fzhhl.top/gthwzcsahi.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gtwisrgwzo.html

x |= (1 << 3);
来源：http://hz.yuanzhike.top/gttuvpltdf.html

[S17] C：安全拼接字符串
来源：http://hz.shuidangran.top/gtaepqunfn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.havefunace.top/gtakqfonhh.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtlfvnsctw.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtakhigvan.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gtfnfvhrqu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtsiahglxw.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtxcsjvktf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtrzmzskjf.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtknkbmfrc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gzhubu.top/gtradeyyun.html

[S22] C：字符串转数字
来源：http://hz.quarkkingdee.top/gtcuybikey.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtfsejgbde.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtdfvvlgbn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydzc1.top/gtzmaocuru.html

[S24] C：获取本地时间
来源：http://hz.chenzaomai.com/gtxeckquqt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ybcxt.top/gtwohyucsc.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtpuuitbig.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtwfyypzee.html

[S26] C：内存清零
来源：http://hz.jiagoushi.top/gtdcpkrhwp.html

memset(a, 0, sizeof a);
来源：http://hz.hfpthk.cn/gtmihwtpki.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gthxolhbbz.html

const double PI = 3.14159;
来源：http://hz.gogol.net.cn/gtvzxjmfwo.html

[S28] C：静态变量
来源：http://hz.yueranfly.top/gtepitbebe.html

static int counter = 0;
来源：http://hz.kuanghao11.cn/gtzfeeaeer.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtvscdkitr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtazpizfcp.html

[S30] C：头文件保护
来源：http://hz.feifeiyinyue.top/gtrprcsbpv.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtgmksnuji.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gtiedpdwny.html

#endif
来源：http://hz.shangyingyoupin.top/gttgefuxzt.html

[S31] C++：Hello World
来源：http://hz.yuanzhike.top/gtwcqiyxiz.html

#include <iostream>
来源：http://hz.aizwys.cn/gtyzgqrqed.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gogol.net.cn/gtfwgiswix.html

[S32] C++：字符串
来源：http://hz.vqdsnc.cn/gtzuwebgkt.html

std::string s = "hi";  s += "!";
来源：http://hz.jyoumei.cn/gtglpaoxff.html

[S33] C++：vector 增删
来源：http://hz.tian-w.cn/gtbqecfzfu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtgkxxtjlq.html

[S34] C++：遍历 vector
来源：http://hz.gzhubu.top/gtonudybsp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hysaishi.cn/gtuiaiexco.html

[S35] C++：map
来源：http://hz.jqgufenzy.top/gtbzwxukfn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtazwxmgkn.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtlaxcfkqu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtiibbhwsx.html

[S37] C++：set
来源：http://hz.xylfe.cn/gtqlufgdhh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fzhhl.top/gtlxxrjcet.html

[S38] C++：排序
来源：http://hz.jinyuanbaomall.cn/gtkivfapvp.html

std::sort(v.begin(), v.end());
来源：http://hz.hywenlv.cn/gtifikmpmt.html

[S39] C++：自定义比较器排序
来源：http://hz.iojbl.cn/gtwnykvapd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.kuanghao11.cn/gtmvlswqir.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gtdwuckzpa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhongyouzk.top/gtxfztcddc.html

[S41] C++：类与构造函数
来源：http://hz.gotoacloud.top/gtxncukjdb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yonumen.top/gtgehwxykg.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtctehcbgb.html

class B : public Base { public: void f() override {} };
来源：http://hz.jianghu66.top/gthalrpinq.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtqrhagtmb.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gtfcskvkac.html

[S44] C++：引用传参
来源：http://hz.yueranfly.top/gtckfnwrbc.html

void inc(int &x) { ++x; }
来源：http://hz.zhixingplan.top/gtjtglxqrm.html

[S45] C++：lambda
来源：http://hz.sufxvd.cn/gtmxucwcis.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sweek.top/gtwilbhczv.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtyjmsuixo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtyjrqdyaj.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gtwvapmwlv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hnqzz.top/gtjaxphgec.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gtnmuhzqih.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.svipenyu.cn/gtucdcjqfj.html

while (std::getline(in, line)) { }
来源：http://hz.shzxlz.cn/gtqnzpvsgu.html

[S49] C++：写文件
来源：http://hz.mhx1999.top/gttknohktu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtkzndcwki.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtxjgjngjb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cheryme.top/gtkdqcvmtn.html

[S51] C++：显式类型转换
来源：http://hz.shangyingyoupin.top/gtrryfcjln.html

static_cast<double>(a) / b
来源：http://hz.iojbl.cn/gtksbrrswp.html

[S52] C++：const 与 noexcept
来源：http://hz.yongpay.top/gtfghhzgou.html

int size() const noexcept { return n_; }
来源：http://hz.dianchejie.cn/gtibcgwogg.html

[S53] C++：移动语义
来源：http://hz.jiagoushi.top/gtagioumzn.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtkfgorhht.html

[S54] C++：异常处理
来源：http://hz.shzxlz.cn/gtttsanfkf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtdvfalmmb.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtziysrbbx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtbjzhnnci.html

[S56] C++：optional
来源：http://hz.xinyue.icu/gtfyiigcuz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cashguo.top/gtibitzsxo.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtoqngzwvo.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtnuxryglq.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtfhzhpqmv.html

namespace ns { int f() { return 1; } }
来源：http://hz.guannengcc.top/gtaujxoapu.html

[S59] C++：静态断言
来源：http://hz.chenlongwang.top/gthxqfmgxv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.smart0.xyz/gtcjuodcak.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gtoohctyes.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangkeji.top/gtlpwhvhsb.html

================================================================================
来源：http://hz.nwbrower.top/gtmcxldwmn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtzwfentnk.html

================================================================================
来源：http://hz.jyoumei.cn/gtogyoqouu.html

[T01] Kotlin：Hello World
来源：http://hz.zhoulong.xyz/gthqzsfpfd.html

println("Hello")
来源：http://hz.9152youxi.cn/gtabailaia.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtjqiyuszp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtshaxmznm.html

[T03] Kotlin：字符串模板
来源：http://hz.bjfxy.top/gtgqmvwjnk.html

"值: $b"
来源：http://hz.andypj.xyz/gtoyljoxhg.html

[T04] Kotlin：空安全
来源：http://hz.xinyue.icu/gtoevwneel.html

val n: String? = null;  n?.length
来源：http://hz.smart0.xyz/gtcvwwyjzm.html

[T05] Kotlin：when 表达式
来源：http://hz.tian-w.cn/gtlzvqriat.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yangfankeji.com/gtxdhccnjh.html

[T06] Kotlin：集合映射
来源：http://hz.zhiwuduotai.top/gtmexillnk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gthfjtnfzn.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigufen.top/gtiqumbqqb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtikhbqeak.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangtech.top/gtbdbcryry.html

data class User(val name: String, val age: Int)
来源：http://hz.ydjk.org.cn/gttovseijv.html

[T09] Kotlin：扩展函数
来源：http://hz.hnxiangtu.top/gtevtfsxsf.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxinkj.top/gtllwccqkz.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtnkukpith.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.smart0.xyz/gtmqtnczhv.html

[T11] Kotlin：协程
来源：http://hz.shzxlz.cn/gtvkjqhgki.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtouyuqyzh.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtzjtwndsx.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gthxovkuda.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigfzy.top/gtolgthyiw.html

val m = mapOf("a" to 1)
来源：http://hz.feifeiyinyue.top/gtytxwvcst.html

[T14] Kotlin：循环
来源：http://hz.jqgfzy.top/gtwrwgagaf.html

for (i in 1..10) println(i)
来源：http://hz.jiagoushi.top/gtsybifjtq.html

[T15] Kotlin：接口
来源：http://hz.xingfuxueyuan.xyz/gtofneaelm.html

interface Shape { fun area(): Double }
来源：http://hz.yj202588.top/gtiqcfrhzg.html

[T16] Swift：Hello World
来源：http://hz.redwolf501.top/gtyjnxanyd.html

print("Hello")
来源：http://hz.hnxiangtu.top/gtcazawvsd.html

[T17] Swift：变量与常量
来源：http://hz.hywenlv.cn/gthniphmxh.html

var a = 1;  let b = 2
来源：http://hz.shzxlz.cn/gttdoayllk.html

[T18] Swift：字符串插值
来源：http://hz.cqqwz.cn/gtrnexbxrf.html

"值: \(b)"
来源：http://hz.zhijiandao.cn/gttdhuowuz.html

[T19] Swift：可选绑定
来源：http://hz.yj20258.top/gtpjtejbzt.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gteeqlkeal.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtewgvehdn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ydzc1.top/gttfcymijd.html

[T21] Swift：遍历
来源：http://hz.chenzaomai.com/gtrtulpgis.html

for x in a { print(x) }
来源：http://hz.jiagoushi.top/gtrdfxzmfv.html

[T22] Swift：字典
来源：http://hz.daxiang520.top/gtzdefmhcj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gtxuqzygbw.html

[T23] Swift：函数
来源：http://hz.jqgufenzy.top/gtdegfnwhu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gtbwqvjctw.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtohugkgrc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.vqdsnc.cn/gtkdnbhjnz.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gtbbudffdf.html

struct P { var x: Int }
来源：http://hz.kuanghao11.cn/gtjobtszzx.html

[T26] Swift：类与重写
来源：http://hz.daria6918.cn/gtvzarkhry.html

class A: Base { override func f() {} }
来源：http://hz.jinqigfzy.top/gtfjntkjgp.html

[T27] Swift：错误处理
来源：http://hz.xinyue.icu/gtrcenmoid.html

do { try f() } catch { print(error) }
来源：http://hz.yuanzhike.top/gtvxkjglpi.html

[T28] Swift：枚举
来源：http://hz.nanxinkj.top/gtzpgkncym.html

enum Color { case red, green }
来源：http://hz.hnqzz.top/gtywotbhwj.html

[T29] Swift：guard 提前返回
来源：http://hz.jyoumei.cn/gtbkpyycou.html

guard let x = opt else { return }
来源：http://hz.havefunace.top/gttbpxzfql.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gthyplsmkm.html

protocol Shape { func area() -> Double }
来源：http://hz.yuxming.cn/gtzoirhjit.html

[T31] Lua：Hello World
来源：http://hz.fzhhl.top/gtkjhjvxss.html

print("Hello")
来源：http://hz.aibaodan.cn/gtonnknrzh.html

[T32] Lua：局部变量
来源：http://hz.guowangkeji.top/gtlfftbolo.html

local a = 1
来源：http://hz.birdmap.top/gtkrxyqnal.html

[T33] Lua：表（数组）
来源：http://hz.quarkkingdee.top/gtkfjbdmlq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hongshengwenyu.top/gtywxpwhoi.html

[T34] Lua：遍历表
来源：http://hz.jinqigfzy.top/gtrwetvfzb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sxryk.cn/gtjyiglecw.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtqwhmryjo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtjvuyekbv.html

[T36] Lua：函数
来源：http://hz.jlsjyb.cn/gtgleltxbp.html

function add(a, b) return a + b end
来源：http://hz.wangdashe.top/gtxnnkblzb.html

[T37] Lua：字符串拼接
来源：http://hz.jianghu66.top/gtobzzaztd.html

"a" .. "b"
来源：http://hz.jlsjyb.cn/gtfxxknlqo.html

[T38] Lua：条件
来源：http://hz.jinghuilouyu.cn/gttrsnubma.html

if x > 0 then print("正") end
来源：http://hz.haohaochexian.top/gtphozihtm.html

[T39] Lua：模式匹配
来源：http://hz.yuxming.cn/gtpjaqmsav.html

string.find(s, "%d+")
来源：http://hz.ybcxt.top/gtbygsjbli.html

[T40] Lua：元表
来源：http://hz.cdnleiting.top/gtccskrvpi.html

setmetatable({}, { __index = base })
来源：http://hz.gotoacloud.top/gtimmfqrqc.html

[T41] Perl：Hello World
来源：http://hz.xuanzx.com/gtgcvothec.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtfswhslnm.html

[T42] Perl：变量类型
来源：http://hz.yueranfly.top/gtiislcvts.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.andypj.xyz/gtokyjhzje.html

[T43] Perl：字符串插值
来源：http://hz.sysykeji.top/gtbocuhzzg.html

"值: $a"
来源：http://hz.cheryme.top/gtcmmhmzuj.html

[T44] Perl：条件
来源：http://hz.shzxlz.cn/gtpworvjtm.html

if ($a > 0) { print "正"; }
来源：http://hz.mhx1999.top/gtdtkdlqow.html

[T45] Perl：数组遍历
来源：http://hz.cucudq.cn/gtzhucyxtd.html

for my $x (@arr) { print $x; }
来源：http://hz.yueranfly.top/gtdndmcyrw.html

[T46] Perl：哈希操作
来源：http://hz.ydzc1.top/gtwmsptikq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.316326.xyz/gtlvpazggg.html

[T47] Perl：正则捕获
来源：http://hz.tianlin.xyz/gtjgaxkbjx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.haohaochexian.top/gtfyvljror.html

[T48] Perl：正则替换
来源：http://hz.yongpay.top/gtakvkzrvp.html

$s =~ s/old/new/g;
来源：http://hz.wangdashe.top/gttmkscrjx.html

[T49] Perl：函数
来源：http://hz.shuidangran.top/gthbkebdfi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.redwolf501.top/gthasvqmrl.html

[T50] Perl：逐行读文件
来源：http://hz.quarkkingdee.top/gtaouyohux.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgufenzy.top/gtkxwhqgod.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangtech.top/gtskvtfbsb.html

[T51] Scala：Hello World
来源：http://hz.ywan-chungtsiang.top/gtirwfqygk.html

println("Hello")
来源：http://hz.hywenlv.cn/gtdfezenhv.html

[T52] Scala：变量
来源：http://hz.cucudq.cn/gtkxbpihkx.html

val a = 1;  var b = 2
来源：http://hz.jianghu66.top/gtefqhlkjj.html

[T53] Scala：字符串插值
来源：http://hz.haohaochexian.top/gtwsebvqry.html

s"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtgakqfqtx.html

[T54] Scala：集合映射
来源：http://hz.shangyingyoupin.top/gttpidttiy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.0kj1m.cn/gtwflerwyl.html

[T55] Scala：集合过滤
来源：http://hz.hfpthk.cn/gtupopxxcs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yuanzhike.top/gtplflzcys.html

[T56] Scala：样例类
来源：http://hz.xziqi.cn/gtuebvthga.html

case class User(name: String, age: Int)
来源：http://hz.wangdashe.top/gtrjzwmrxs.html

[T57] Scala：模式匹配
来源：http://hz.hysaishi.cn/gtepsvunzi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.birdmap.top/gtvjgsxixp.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gtoltssobq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258888.top/gtdaslccqp.html

[T59] Scala：循环
来源：http://hz.xylfe.cn/gtflydvsmr.html

for (i <- 1 to 10) println(i)
来源：http://hz.zdqjudy.top/gticyjhtjc.html

[T60] Scala：折叠
来源：http://hz.snrcjt.cn/gtftfqtytw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnqzz.top/gtjfntoqpr.html

================================================================================
来源：http://hz.yj20258888.top/gtiuxsduen.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jianghu66.top/gtubwglfya.html

================================================================================
来源：http://hz.xylfe.cn/gtqkryehnq.html

[U01] Py：创建虚拟环境
来源：http://hz.xuetiantiany.cn/gthyjykqla.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.dashuyun.cn/gtufqmpmot.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gzhubu.top/gtnlebykeb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sufxvd.cn/gtgftpdmrw.html

[U03] Py：加载 .env 配置
来源：http://hz.yj202588.top/gttehvkpkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydjk.org.cn/gtzjvoubcs.html

[U04] Py：变量调试打印
来源：http://hz.jiagoushi.top/gtlaantzdm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.chenzaomai.com/gtoiqkocgm.html

[U05] Py：列表去重且保序
来源：http://hz.yuxming.cn/gtsmnhdxvc.html

list(dict.fromkeys(arr))
来源：http://hz.yuxming.cn/gtdldplgdr.html

[U06] Py：合并两个字典
来源：http://hz.dianchejie.cn/gtgxwzceof.html

{**a, **b}
来源：http://hz.tanke756.top/gthfcxvgvu.html

[U07] Py：反转字典键值
来源：http://hz.zdqjudy.top/gtybpflzpq.html

{v: k for k, v in d.items()}
来源：http://hz.dashuyun.cn/gtikcjdtdq.html

[U08] Py：展平二维列表
来源：http://hz.tanke756.top/gttqdrlqwr.html

[y for x in nested for y in x]
来源：http://hz.smart0.xyz/gtgzhiksgn.html

[U09] Py：字典取最大值的键
来源：http://hz.gotoacloud.top/gtuznnfoal.html

max(d, key=d.get)
来源：http://hz.shzxlz.cn/gtbuwospwo.html

[U10] Py：按值排序字典
来源：http://hz.fzhhl.top/gtbqqkgeww.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhongyouzk.top/gtgfeescmz.html

[U11] Py：生成器表达式
来源：http://hz.pengpengdd.cyou/gtwnmnoocd.html

(x * 2 for x in arr)
来源：http://hz.quarkkingdee.top/gtclinieor.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jyoumei.cn/gtimdpsers.html

Counter(arr).most_common(3)
来源：http://hz.wangdashe.top/gtrmovmhsv.html

[U13] Py：固定长度队列
来源：http://hz.sweek.top/gterlscplv.html

deque(maxlen=10)
来源：http://hz.hnxiangtu.top/gtcbghbelo.html

[U14] Py：分组收集到列表
来源：http://hz.shanyushiyangkeji.top/gtvosqpxtt.html

defaultdict(list)
来源：http://hz.dianchejie.cn/gtpeqrcrvz.html

[U15] Py：高精度计时
来源：http://hz.tian-w.cn/gtjejyyhii.html

t = time.perf_counter()
来源：http://hz.ehwqpu.com/gthxmcddaw.html

[U16] Py：命令行参数解析
来源：http://hz.haohaochexian.top/gtdgbgefbn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aizwys.cn/gtghhmytui.html

[U17] Py：初始化日志
来源：http://hz.chenlongwang.top/gtqboawtxr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sxryk.cn/gtxskowcjf.html

[U18] Py：预编译正则
来源：http://hz.zhengqikj.top/gtcrsrinkf.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtekpncyoo.html

[U19] Py：正则替换带回调
来源：http://hz.smart0.xyz/gtvenrtmir.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gtkgtcixna.html

[U20] Py：缓存函数结果
来源：http://hz.ybcxt.top/gtcpewdkqq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhiwuduotai.top/gtqbjskoom.html

[U21] Py：自定义上下文管理器
来源：http://hz.xuanzx.com/gtcenvmqeo.html

@contextlib.contextmanager
来源：http://hz.gogol.net.cn/gtwiuucfqt.html

[U22] Py：矩阵转置
来源：http://hz.jianghu66.top/gtxuxljjyz.html

list(zip(*m))
来源：http://hz.jqgufenzy.top/gtlweyktwl.html

[U23] Py：分块读取大文件
来源：http://hz.bjfxy.top/gtqdanlcxp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhongyouzk.top/gtmqyoxldc.html

[U24] Py：路径操作
来源：http://hz.vqdsnc.cn/gtyqebmqho.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.redwolf501.top/gtwtrjkpzh.html

[U25] Py：CSV 按字典读
来源：http://hz.jyoumei.cn/gtdseufpqg.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtrhuxrofo.html

[U26] Py：并发下载
来源：http://hz.cdnleiting.top/gtgokpmhio.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shzxlz.cn/gtsrwyexjd.html

[U27] Py：异步 HTTP
来源：http://hz.0kj1m.cn/gtcyloqpvp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.0kj1m.cn/gtakixsqim.html

[U28] Py：类型别名
来源：http://hz.aizwys.cn/gtlkxndjzs.html

UserId = int
来源：http://hz.jianghu66.top/gtfhnehnzf.html

[U29] Py：属性校验
来源：http://hz.bjfxy.top/gthifldgnd.html

@property 与 @x.setter 配合
来源：http://hz.0kj1m.cn/gttbnoftrf.html

[U30] Py：数据类
来源：http://hz.xylfe.cn/gtygzluota.html

@dataclass(slots=True)
来源：http://hz.aizwys.cn/gtnxyuizui.html

[U31] Py：单测
来源：http://hz.ehwqpu.com/gturuhtnyj.html

python -m pytest -q
来源：http://hz.yueranfly.top/gtzzpjfmvf.html

[U32] Py：代码格式化
来源：http://hz.ehwqpu.com/gtqeutnjqa.html

ruff format . && ruff check --fix .
来源：http://hz.ehwqpu.com/gtwvenfsej.html


<!-- 参考信息 -->