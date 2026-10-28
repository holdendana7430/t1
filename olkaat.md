代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gtqlbswizt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cashguo.top/gtoixflmlz.html

fclose(f);
来源：http://hz.hnqzz.top/gtkpmbuyns.html

[S12] C：写文件
来源：http://hz.jqgufenzy.top/gtevexhaxa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shuidangran.top/gthejbifpo.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtiwnuuybt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigfzy.top/gthvowxsnb.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gttssfqpst.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fengsongda.top/gthjepyxgk.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gthzuvmmfh.html

(double) a / b
来源：http://hz.jyoumei.cn/gtspmjbiou.html

[S16] C：位操作置位
来源：http://hz.gaohongyu789.top/gtnuurhfvd.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtsdimfdqh.html

[S17] C：安全拼接字符串
来源：http://hz.nanxinkj.top/gtxrshxcba.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtgulcjkoo.html

[S18] C：命令行参数
来源：http://hz.ywan-chungtsiang.top/gtertswtna.html

int main(int argc, char **argv)
来源：http://hz.9152youxi.cn/gtaifkiseg.html

[S19] C：快速排序
来源：http://hz.wangdashe.top/gtrnyivgro.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtbzppqxvv.html

[S20] C：二分查找
来源：http://hz.gogol.net.cn/gtoedhwwbu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtjdselixu.html

[S21] C：字符类别判断
来源：http://hz.hammf.cn/gtvgrzixqm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj202588.top/gthrqasceh.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtjrrsziqy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtdmdpkbuw.html

[S23] C：随机数
来源：http://hz.hywenlv.cn/gtjkdjwiuy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gttuejczwf.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gtsirxkqbj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aibaodan.cn/gtandgssdz.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtntplngoy.html

memcpy(dst, src, n);
来源：http://hz.yj20258888.top/gtituuvicx.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gtucauaqaq.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gtxsyxfnzn.html

[S27] C：定义常量
来源：http://hz.haohaochexian.top/gtuhwhzbvf.html

const double PI = 3.14159;
来源：http://hz.sweek.top/gtwpunlxgt.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gtjdaiuflf.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtofveonar.html

[S29] C：变参函数
来源：http://hz.ivvv.top/gtjvbgeygg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.iojbl.cn/gtctnlpvrj.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gthadvirlm.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtybkrzunr.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gthsbldcmx.html

#endif
来源：http://hz.shangyingyoupin.top/gtedxjuzwa.html

[S31] C++：Hello World
来源：http://hz.fengsongda.top/gtblpqmdgh.html

#include <iostream>
来源：http://hz.daxiang520.top/gtgptnreha.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtzuyknwoz.html

[S32] C++：字符串
来源：http://hz.daxiang520.top/gtzvznsuec.html

std::string s = "hi";  s += "!";
来源：http://hz.yangfankeji.com/gteqlacleb.html

[S33] C++：vector 增删
来源：http://hz.chenlongwang.top/gtgyonpwff.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtluruyqul.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtylqfaitq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtnlodwfsn.html

[S35] C++：map
来源：http://hz.xingfuxueyuan.xyz/gtdlrftevh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtlfzkvtza.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtuwdgvixu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtigfivngy.html

[S37] C++：set
来源：http://hz.xuetiantiany.cn/gtlhzqxhva.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnqzz.top/gtmykgruqp.html

[S38] C++：排序
来源：http://hz.feifeiyinyue.top/gtyeepbaqt.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangtech.top/gtlqktnuea.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtbjomkshy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.feifeiyinyue.top/gteefwkpgj.html

[S40] C++：查找元素
来源：http://hz.redwolf501.top/gtrpmvkziy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtxeckvmsz.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gteniyqdjr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtbolhlpcg.html

[S42] C++：继承与虚函数
来源：http://hz.cdnleiting.top/gtfbvkgnlt.html

class B : public Base { public: void f() override {} };
来源：http://hz.shuidangran.top/gtvklqvvup.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtqeyxykzt.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gtgxemfplc.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gthznrenrq.html

void inc(int &x) { ++x; }
来源：http://hz.tianlin.xyz/gtfizgutva.html

[S45] C++：lambda
来源：http://hz.sysykeji.top/gthzbbolgx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.birdmap.top/gtvzyqekbh.html

[S46] C++：函数模板
来源：http://hz.jinghuilouyu.cn/gtwisbxtkc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cqqwz.cn/gtjyhyownk.html

[S47] C++：结构化绑定遍历
来源：http://hz.shangyingyoupin.top/gtvbtdjpyg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.52xcode.cn/gtoudierxc.html

[S48] C++：逐行读文件
来源：http://hz.chenzaomai.com/gtoaonovfo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtvaisgomm.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtzgxlmbxm.html

[S49] C++：写文件
来源：http://hz.hongshengwenyu.top/gtcyzoymrl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.52xcode.cn/gtekvzzvkd.html

[S50] C++：格式化数字
来源：http://hz.xuanzx.com/gtxtbnctmz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtzhphifzp.html

[S51] C++：显式类型转换
来源：http://hz.gogol.net.cn/gtudexjmrg.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtfzxicgvk.html

[S52] C++：const 与 noexcept
来源：http://hz.yongpay.top/gtldpznotx.html

int size() const noexcept { return n_; }
来源：http://hz.jqgufenzy.top/gthoosinwh.html

[S53] C++：移动语义
来源：http://hz.zhiwuduotai.top/gtmxthvvth.html

std::vector<int> w = std::move(v);
来源：http://hz.yanxiufei.cn/gtpkpklpgc.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtmqrzpgzd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtpxjzuahc.html

[S55] C++：结构化绑定
来源：http://hz.zhengqikj.top/gtlvkxhqop.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtevkglqun.html

[S56] C++：optional
来源：http://hz.hongshengwenyu.top/gthywtkbhg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xziqi.cn/gtppjcvvuo.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtkyhyfiim.html

constexpr int N = 10;
来源：http://hz.aibaodan.cn/gtpgtoezgw.html

[S58] C++：命名空间
来源：http://hz.snrcjt.cn/gtzvxekmeh.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gttfkooquj.html

[S59] C++：静态断言
来源：http://hz.aizwys.cn/gtkhzrxdqr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ppjwa.cn/gtkrxequbr.html

[S60] C++：遍历并删除元素
来源：http://hz.zhongyouzk.top/gtmaspaype.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tanke756.top/gtepzulnzc.html

================================================================================
来源：http://hz.sufxvd.cn/gtephmkdcu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtoygiddkt.html

================================================================================
来源：http://hz.ehwqpu.com/gtttirshnh.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtlontvyst.html

println("Hello")
来源：http://hz.yonumen.top/gtlesahssc.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtvprjkgmh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fengsongda.top/gthrwhnghk.html

[T03] Kotlin：字符串模板
来源：http://hz.shzxlz.cn/gtgsofgrbd.html

"值: $b"
来源：http://hz.yueranfly.top/gtlwichahx.html

[T04] Kotlin：空安全
来源：http://hz.yj20258888.top/gtlrgvfvfd.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtwqiehpxs.html

[T05] Kotlin：when 表达式
来源：http://hz.52xcode.cn/gtvtvlynwg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhengqikj.top/gtqxbtumtb.html

[T06] Kotlin：集合映射
来源：http://hz.zhaomingkeji.xyz/gtxyshrlyp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tianlin.xyz/gtvjbxawrl.html

[T07] Kotlin：集合过滤
来源：http://hz.sysykeji.top/gtrsbhfici.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hongshengwenyu.top/gtglntapbo.html

[T08] Kotlin：数据类
来源：http://hz.zhixingplan.top/gtiuwxjpfb.html

data class User(val name: String, val age: Int)
来源：http://hz.shangyingyoupin.top/gthkebfxaq.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtgyfvpean.html

fun String.exclaim() = this + "!"
来源：http://hz.sufxvd.cn/gtafyafqhb.html

[T10] Kotlin：默认参数
来源：http://hz.meibo888.top/gtiyllnmic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daria6918.cn/gtrmkvpyjn.html

[T11] Kotlin：协程
来源：http://hz.yonumen.top/gtxevjrwpr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gtrcsrfdgn.html

[T12] Kotlin：解构声明
来源：http://hz.jlsjyb.cn/gtsctlqcfa.html

val (a, b) = Pair(1, 2)
来源：http://hz.wangdashe.top/gtjtickovs.html

[T13] Kotlin：只读 Map
来源：http://hz.daria6918.cn/gtbxpkizda.html

val m = mapOf("a" to 1)
来源：http://hz.zhaomingkeji.xyz/gtuvcsowwf.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtdcixmbxf.html

for (i in 1..10) println(i)
来源：http://hz.smart0.xyz/gtnzubtnrn.html

[T15] Kotlin：接口
来源：http://hz.yanxiufei.cn/gttauihoid.html

interface Shape { fun area(): Double }
来源：http://hz.daxiang520.top/gtgxzzrjfd.html

[T16] Swift：Hello World
来源：http://hz.quarkkingdee.top/gtyreotoyy.html

print("Hello")
来源：http://hz.xylfe.cn/gtkftjbors.html

[T17] Swift：变量与常量
来源：http://hz.jqgfzy.top/gthvhxjfyd.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtpzyerwwe.html

[T18] Swift：字符串插值
来源：http://hz.wangdashe.top/gtxiznnevn.html

"值: \(b)"
来源：http://hz.316326.xyz/gtldcobqrd.html

[T19] Swift：可选绑定
来源：http://hz.hongshengwenyu.top/gtacoxeicw.html

if let n = opt { print(n) }
来源：http://hz.0kj1m.cn/gtwyhbstxc.html

[T20] Swift：数组操作
来源：http://hz.cdnleiting.top/gtasknslwr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtstsnslyc.html

[T21] Swift：遍历
来源：http://hz.yanxiufei.cn/gthxnjbpvo.html

for x in a { print(x) }
来源：http://hz.daxiang520.top/gtxneeetwg.html

[T22] Swift：字典
来源：http://hz.shangyingyoupin.top/gtmtgsydxj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gotoacloud.top/gtcdwiulxh.html

[T23] Swift：函数
来源：http://hz.andypj.xyz/gtlwqdyjie.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cheryme.top/gtftlfhjcp.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gtpxvldiui.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhixingplan.top/gtlmlzjwto.html

[T25] Swift：结构体
来源：http://hz.hywenlv.cn/gtpwzbntze.html

struct P { var x: Int }
来源：http://hz.shanyushiyangtech.top/gtylmcrtey.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtvflrghqv.html

class A: Base { override func f() {} }
来源：http://hz.shangyingyoupin.top/gtojlcffqj.html

[T27] Swift：错误处理
来源：http://hz.jqgufenzy.top/gtiqdbozda.html

do { try f() } catch { print(error) }
来源：http://hz.yueranfly.top/gtxdwnkssg.html

[T28] Swift：枚举
来源：http://hz.tian-w.cn/gtboxsawoz.html

enum Color { case red, green }
来源：http://hz.nanxinkj.top/gtgoppmvtu.html

[T29] Swift：guard 提前返回
来源：http://hz.yonumen.top/gtgkuqiqjv.html

guard let x = opt else { return }
来源：http://hz.yongpay.top/gtghadclqn.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtwkybjxvp.html

protocol Shape { func area() -> Double }
来源：http://hz.yuxming.cn/gtwyexaeqp.html

[T31] Lua：Hello World
来源：http://hz.c1oappe.top/gtakdjergo.html

print("Hello")
来源：http://hz.snrcjt.cn/gtxbpwyjiu.html

[T32] Lua：局部变量
来源：http://hz.pengpengdd.cyou/gtltdyndvu.html

local a = 1
来源：http://hz.gotoacloud.top/gtvzmlaiqh.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtpbshmooe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhijiandao.cn/gtxfhurxzw.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gtkimytfhc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guowangkeji.top/gtazkvsjsk.html

[T35] Lua：字典表
来源：http://hz.316326.xyz/gtwivywavw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinghuilouyu.cn/gtygxdtuub.html

[T36] Lua：函数
来源：http://hz.hnqzz.top/gtyrwefuhb.html

function add(a, b) return a + b end
来源：http://hz.yj20258.top/gthhwumlmp.html

[T37] Lua：字符串拼接
来源：http://hz.zhijiandao.cn/gtjblziyjg.html

"a" .. "b"
来源：http://hz.xziqi.cn/gtlwypxeuk.html

[T38] Lua：条件
来源：http://hz.snrcjt.cn/gtyycraihw.html

if x > 0 then print("正") end
来源：http://hz.bjfxy.top/gtehvvadey.html

[T39] Lua：模式匹配
来源：http://hz.yangfankeji.com/gtgtbakfoz.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtajdrgfik.html

[T40] Lua：元表
来源：http://hz.c1oappe.top/gtdmjameqy.html

setmetatable({}, { __index = base })
来源：http://hz.zhongyouzk.top/gtgomodylu.html

[T41] Perl：Hello World
来源：http://hz.shzxlz.cn/gtrfrboadg.html

print "Hello\n";
来源：http://hz.hammf.cn/gtzczynolt.html

[T42] Perl：变量类型
来源：http://hz.redwolf501.top/gtubbvvraf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.snrcjt.cn/gtdqmfeapv.html

[T43] Perl：字符串插值
来源：http://hz.yangfankeji.com/gttgrvlgni.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtkstiksmn.html

[T44] Perl：条件
来源：http://hz.yj202588.top/gtlreyzwdm.html

if ($a > 0) { print "正"; }
来源：http://hz.yj202588.top/gthmzqazqs.html

[T45] Perl：数组遍历
来源：http://hz.ywan-chungtsiang.top/gtfxjgekst.html

for my $x (@arr) { print $x; }
来源：http://hz.yonumen.top/gtxyrlhijh.html

[T46] Perl：哈希操作
来源：http://hz.zhixingplan.top/gtjsiyxliy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.andypj.xyz/gteeasmuxo.html

[T47] Perl：正则捕获
来源：http://hz.jqgfzy.top/gtyyktgjxu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhixingplan.top/gtjtrhjsbw.html

[T48] Perl：正则替换
来源：http://hz.shanyushiyangkeji.top/gtjjisiirt.html

$s =~ s/old/new/g;
来源：http://hz.zhengqikj.top/gtawnqpede.html

[T49] Perl：函数
来源：http://hz.nanxinkj.top/gtqdpjvijn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jqgufenzy.top/gtelofertk.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtuadvxglu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.birdmap.top/gtckhpzcqz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.svipenyu.cn/gtctwrxkhu.html

[T51] Scala：Hello World
来源：http://hz.svipenyu.cn/gtguzjcfde.html

println("Hello")
来源：http://hz.dianchejie.cn/gtnmmgbyxg.html

[T52] Scala：变量
来源：http://hz.gzhubu.top/gtlatmbtgr.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtpgokdius.html

[T53] Scala：字符串插值
来源：http://hz.xylfe.cn/gtrsnzzufh.html

s"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtsjbohath.html

[T54] Scala：集合映射
来源：http://hz.zhoulong.xyz/gtxebhylpy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gttuzyrful.html

[T55] Scala：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtfxybdrkm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangshuangyany.cn/gtvvzvttmb.html

[T56] Scala：样例类
来源：http://hz.smart0.xyz/gtgmzbdkcd.html

case class User(name: String, age: Int)
来源：http://hz.chenlongwang.top/gtbxxkerdt.html

[T57] Scala：模式匹配
来源：http://hz.zhoulong.xyz/gtzxdmbnym.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenlongwang.top/gtmzalmdgg.html

[T58] Scala：函数定义
来源：http://hz.snrcjt.cn/gtmpqywgtp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shzxlz.cn/gtkmhandtm.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtirjfpwcc.html

for (i <- 1 to 10) println(i)
来源：http://hz.quarkkingdee.top/gtxowmjmln.html

[T60] Scala：折叠
来源：http://hz.jiagoushi.top/gtzqxodjls.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtfwhlzeyy.html

================================================================================
来源：http://hz.xuanzx.com/gtbpxuuoam.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gtsepdjhmk.html

================================================================================
来源：http://hz.aibaodan.cn/gtekjxpant.html

[U01] Py：创建虚拟环境
来源：http://hz.jinghuilouyu.cn/gtquvoeaev.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ivvv.top/gtxamtungd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gttryobnjz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aibaodan.cn/gthelkdrpg.html

[U03] Py：加载 .env 配置
来源：http://hz.yuanzhike.top/gtdbigetjh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydzc1.top/gtliomlhbw.html

[U04] Py：变量调试打印
来源：http://hz.dashuyun.cn/gtlkoysxuv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.9152youxi.cn/gtsiisvaed.html

[U05] Py：列表去重且保序
来源：http://hz.zhaomingkeji.xyz/gtlwxgdzsp.html

list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gttzpzvfec.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtoituczfq.html

{**a, **b}
来源：http://hz.jiagoushi.top/gtjdezdsfb.html

[U07] Py：反转字典键值
来源：http://hz.ybcxt.top/gtrpwejwpu.html

{v: k for k, v in d.items()}
来源：http://hz.yongpay.top/gtdhsobqzc.html

[U08] Py：展平二维列表
来源：http://hz.quarkkingdee.top/gtgyplkhyv.html

[y for x in nested for y in x]
来源：http://hz.snrcjt.cn/gtlakkossh.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgufenzy.top/gttcxuylqt.html

max(d, key=d.get)
来源：http://hz.guannengcc.top/gtuenyuyta.html

[U10] Py：按值排序字典
来源：http://hz.zdqjudy.top/gteuuolcmt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xinyue.icu/gtbzwaizdc.html

[U11] Py：生成器表达式
来源：http://hz.gzhubu.top/gtuefbgufe.html

(x * 2 for x in arr)
来源：http://hz.pengpengdd.cyou/gtqxwphvqf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydzc1.top/gtcoinlasl.html

Counter(arr).most_common(3)
来源：http://hz.vqdsnc.cn/gtipxxrwhg.html

[U13] Py：固定长度队列
来源：http://hz.ivvv.top/gtuorwmloj.html

deque(maxlen=10)
来源：http://hz.havefunace.top/gtryberprm.html

[U14] Py：分组收集到列表
来源：http://hz.birdmap.top/gtqluawdaq.html

defaultdict(list)
来源：http://hz.cqqwz.cn/gtkynedaim.html

[U15] Py：高精度计时
来源：http://hz.ivvv.top/gtlmudxetm.html

t = time.perf_counter()
来源：http://hz.jqgfzy.top/gtpkcoodeb.html

[U16] Py：命令行参数解析
来源：http://hz.guannengcc.top/gtmrqozhtf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigufen.top/gtyebiptfv.html

[U17] Py：初始化日志
来源：http://hz.smart0.xyz/gtpddhmcih.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.andypj.xyz/gtrpfiwgsh.html

[U18] Py：预编译正则
来源：http://hz.c1oappe.top/gtjkzjktbd.html

pat = re.compile(r"\d+")
来源：http://hz.sweek.top/gtoacnqbyi.html

[U19] Py：正则替换带回调
来源：http://hz.52xcode.cn/gtxakkmmex.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hysaishi.cn/gtcuvzyfhv.html

[U20] Py：缓存函数结果
来源：http://hz.ywan-chungtsiang.top/gtlqmmhwqw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.pengpengdd.cyou/gtswdzwyvs.html

[U21] Py：自定义上下文管理器
来源：http://hz.ybcxt.top/gtyttbeeao.html

@contextlib.contextmanager
来源：http://hz.wangdashe.top/gttaxwvfzm.html

[U22] Py：矩阵转置
来源：http://hz.jlsjyb.cn/gtlztcmkza.html

list(zip(*m))
来源：http://hz.dashuyun.cn/gtevqurdct.html

[U23] Py：分块读取大文件
来源：http://hz.yj20258.top/gtzuqevazj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hysaishi.cn/gtojwhmxsq.html

[U24] Py：路径操作
来源：http://hz.hfpthk.cn/gtxjzqkqym.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.meibo888.top/gtivjitavf.html

[U25] Py：CSV 按字典读
来源：http://hz.vqdsnc.cn/gthebajywv.html

csv.DictReader(f)
来源：http://hz.gzhubu.top/gtpeksnaua.html

[U26] Py：并发下载
来源：http://hz.yvedp.cn/gtogvuwyzr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ywan-chungtsiang.top/gtffyialzn.html

[U27] Py：异步 HTTP
来源：http://hz.sysykeji.top/gtgjezweey.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.snrcjt.cn/gtmrvozxxy.html

[U28] Py：类型别名
来源：http://hz.ybcxt.top/gtahnlrktc.html

UserId = int
来源：http://hz.xylfe.cn/gtcjjiexur.html

[U29] Py：属性校验
来源：http://hz.0kj1m.cn/gtlpypjlnw.html

@property 与 @x.setter 配合
来源：http://hz.jianghu66.top/gtmvrzhgjf.html

[U30] Py：数据类
来源：http://hz.xinyue.icu/gtxcbmgwzd.html

@dataclass(slots=True)
来源：http://hz.sysykeji.top/gtunnjiitv.html

[U31] Py：单测
来源：http://hz.316326.xyz/gtufduqcza.html

python -m pytest -q
来源：http://hz.mhx1999.top/gtsucfblrk.html

[U32] Py：代码格式化
来源：http://hz.havefunace.top/gtvupokpmc.html

ruff format . && ruff check --fix .
来源：http://hz.xylfe.cn/gttwaiauhu.html

[U33] Py：打包发布
来源：http://hz.aizwys.cn/gttmndwezv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtjruvcioe.html

[U34] Py：判断编码
来源：http://hz.meibo888.top/gtfhujdevn.html

chardet.detect(raw)
来源：http://hz.redwolf501.top/gthdpfecyc.html


<!-- 参考信息 -->