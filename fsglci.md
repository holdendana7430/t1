代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.jyoumei.cn/gtsfvwklnf.html

[S04] C：字符串复制
来源：http://hz.cdnleiting.top/gticvvlovy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dashuyun.cn/gtykdmaceu.html

[S05] C：字符串长度
来源：http://hz.nanxinkj.top/gtkwbxonrc.html

strlen(s)
来源：http://hz.gaohongyu789.top/gtnjieaxdx.html

[S06] C：字符串比较
来源：http://hz.zhoulong.xyz/gtebznnewl.html

strcmp(a, b) == 0
来源：http://hz.jinyuanbaomall.cn/gtkfboqluq.html

[S07] C：数组遍历求和
来源：http://hz.daxiang520.top/gtqyyfdzuv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sxryk.cn/gtqovkwyxe.html

[S08] C：动态内存分配与释放
来源：http://hz.yvedp.cn/gtpvufsurc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sufxvd.cn/gtxfllmtci.html

[S09] C：结构体定义与初始化
来源：http://hz.daria6918.cn/gtghdzppbw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.9152youxi.cn/gtnimlyyuc.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtklwxhgwt.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtseqjpwez.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gtvnqtnoth.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigfzy.top/gtseoukusq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtsktpjphp.html

fclose(f);
来源：http://hz.ivvv.top/gtuenuctsy.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtoyhvlbxj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sysykeji.top/gtahqpygpg.html

[S13] C：宏定义
来源：http://hz.pengpengdd.cyou/gtwdyqpabu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtauszkaff.html

[S14] C：枚举
来源：http://hz.9152youxi.cn/gtqazgdbru.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.c1oappe.top/gtmjyhglgd.html

[S15] C：类型转换
来源：http://hz.fzhhl.top/gtnythvikv.html

(double) a / b
来源：http://hz.guannengcc.top/gtshduceih.html

[S16] C：位操作置位
来源：http://hz.yj20258888.top/gtkgjyqivv.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtmcpevkxj.html

[S17] C：安全拼接字符串
来源：http://hz.xziqi.cn/gtfkwryagk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtrcnhktif.html

[S18] C：命令行参数
来源：http://hz.tianlin.xyz/gtwocdyizr.html

int main(int argc, char **argv)
来源：http://hz.kuanghao11.cn/gtcmqskhhl.html

[S19] C：快速排序
来源：http://hz.tianlin.xyz/gtezuiwhyp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtfgmqbcrt.html

[S20] C：二分查找
来源：http://hz.xylfe.cn/gttwthaqxc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtlmlpqeae.html

[S21] C：字符类别判断
来源：http://hz.jqgufenzy.top/gtylczuptk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtsllwsskp.html

[S22] C：字符串转数字
来源：http://hz.9152youxi.cn/gtflfwgput.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gogol.net.cn/gtxcyjipiz.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtyfkanywa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangkeji.top/gtaxqtmfie.html

[S24] C：获取本地时间
来源：http://hz.tian-w.cn/gtudkyzirg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gaohongyu789.top/gtzjmkgysh.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtbedplhqc.html

memcpy(dst, src, n);
来源：http://hz.wangshuangyany.cn/gtmmtfvxii.html

[S26] C：内存清零
来源：http://hz.gzhubu.top/gtofudgurc.html

memset(a, 0, sizeof a);
来源：http://hz.jiagoushi.top/gtshlkilaf.html

[S27] C：定义常量
来源：http://hz.sxryk.cn/gtmcpkasco.html

const double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gthqtrbzfe.html

[S28] C：静态变量
来源：http://hz.jinqigufen.top/gtjgiwllpn.html

static int counter = 0;
来源：http://hz.pycfn.com/gthbmttviq.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtswowpxre.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtswdpcqrr.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtmbwqebft.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtfxdlmxdm.html

#define X_H
来源：http://hz.chenlongwang.top/gtaofyyyki.html

#endif
来源：http://hz.snrcjt.cn/gthixpbjjv.html

[S31] C++：Hello World
来源：http://hz.aibaodan.cn/gtfvltikrk.html

#include <iostream>
来源：http://hz.quarkkingdee.top/gtgwyxdrza.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gttgzvkvmq.html

[S32] C++：字符串
来源：http://hz.daria6918.cn/gtbvfsbspj.html

std::string s = "hi";  s += "!";
来源：http://hz.yanxiufei.cn/gtqgwfwafn.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtjntblqmp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258888.top/gthlxvsvte.html

[S34] C++：遍历 vector
来源：http://hz.iojbl.cn/gteumktiqx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jlsjyb.cn/gtcoicdycu.html

[S35] C++：map
来源：http://hz.dashuyun.cn/gttgcjxery.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtmlkyrfon.html

[S36] C++：unordered_map
来源：http://hz.nanxinkj.top/gtyyoigozu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtrhjhtnin.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtgkizvpob.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtdyzadces.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gtsgccanab.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtmdmkxmvw.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtuqtouxli.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigufen.top/gtmoeimkmm.html

[S40] C++：查找元素
来源：http://hz.daxiang520.top/gtptegceht.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.pycfn.com/gtuepdaeud.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gtjlmueowt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtynpuxsga.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258.top/gtzmlflpcy.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinqigfzy.top/gtzafsihzh.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtulwcyezw.html

auto p = std::make_unique<int>(5);
来源：http://hz.tianlin.xyz/gtukphmocs.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gtcknrlgnr.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtsmcyuyxw.html

[S45] C++：lambda
来源：http://hz.jyoumei.cn/gtmaqdmsfl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtfemirfij.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gtokquzyet.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gotoacloud.top/gtpdaganxo.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhaomingkeji.xyz/gtsyqbhbmo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtnkvrgvwt.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gtryjepyhc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtwmfpsefm.html

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtjypegjau.html

[S49] C++：写文件
来源：http://hz.jiagoushi.top/gthxmdslyp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtadmzkvph.html

[S50] C++：格式化数字
来源：http://hz.kuanghao11.cn/gtsheydhro.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sweek.top/gtkmuajtao.html

[S51] C++：显式类型转换
来源：http://hz.sysykeji.top/gtiraanwli.html

static_cast<double>(a) / b
来源：http://hz.ppjwa.cn/gtkzdpdtfk.html

[S52] C++：const 与 noexcept
来源：http://hz.zhiwuduotai.top/gtyxqnemaj.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gtvytoevgi.html

[S53] C++：移动语义
来源：http://hz.zhaomingkeji.xyz/gtnqynjeng.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtxgeleiix.html

[S54] C++：异常处理
来源：http://hz.yueranfly.top/gtgwssfrcg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtltfvgriq.html

[S55] C++：结构化绑定
来源：http://hz.andypj.xyz/gtloygcnsq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigfzy.top/gtenotdqsi.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtkecsiqoj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gtmlbqsvre.html

[S57] C++：编译期常量
来源：http://hz.hfpthk.cn/gticonlwkh.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtfvosqzrp.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtagjsiqyo.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gtbfglicvq.html

[S59] C++：静态断言
来源：http://hz.316326.xyz/gtqmfnhgnp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.c1oappe.top/gtvlyzczpb.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxuanxn.top/gtmxlzawsv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nwbrower.top/gtmrxesvgt.html

================================================================================
来源：http://hz.bjfxy.top/gtlorxnwtk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gtjiucisuy.html

================================================================================
来源：http://hz.sxryk.cn/gtcfkadpxy.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtgpcdjwcj.html

println("Hello")
来源：http://hz.ehwqpu.com/gtludnvddz.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtzauqpqsq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ivvv.top/gtuvnxmyzk.html

[T03] Kotlin：字符串模板
来源：http://hz.tanke756.top/gtoharpnze.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtdbgxevkv.html

[T04] Kotlin：空安全
来源：http://hz.yanxiufei.cn/gtupdecftq.html

val n: String? = null;  n?.length
来源：http://hz.yj202588.top/gtuazmswgr.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigufen.top/gtqhygfesb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtegmunaki.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gtlvqckudy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shangyingyoupin.top/gtpqdtyqds.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtqjaczmaj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtyhqpjwic.html

[T08] Kotlin：数据类
来源：http://hz.smart0.xyz/gtqifcyyww.html

data class User(val name: String, val age: Int)
来源：http://hz.zhiwuduotai.top/gthdycvmqt.html

[T09] Kotlin：扩展函数
来源：http://hz.gaohongyu789.top/gtnnbzqrdv.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gtchbcalnl.html

[T10] Kotlin：默认参数
来源：http://hz.yj202588.top/gtrvnknoci.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ppjwa.cn/gtnoyqakro.html

[T11] Kotlin：协程
来源：http://hz.jinghuilouyu.cn/gtszvedcwz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtkrajprwx.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtjskyrclr.html

val (a, b) = Pair(1, 2)
来源：http://hz.jlsjyb.cn/gtyxodugww.html

[T13] Kotlin：只读 Map
来源：http://hz.ywan-chungtsiang.top/gtbylekjsm.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtrxlxpeus.html

[T14] Kotlin：循环
来源：http://hz.dianchejie.cn/gtnjwsbdek.html

for (i in 1..10) println(i)
来源：http://hz.yj20258.top/gthluaptdv.html

[T15] Kotlin：接口
来源：http://hz.tanke756.top/gtcodpcqlq.html

interface Shape { fun area(): Double }
来源：http://hz.yonumen.top/gtulpovijb.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gttkuwmwtn.html

print("Hello")
来源：http://hz.xylfe.cn/gtkcnlrcdx.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtlqtszulk.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtbfarsetp.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtmvxptbnh.html

"值: \(b)"
来源：http://hz.yuxming.cn/gtthycjith.html

[T19] Swift：可选绑定
来源：http://hz.sxryk.cn/gtxoaqrzht.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtzobhgahb.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtwoozefji.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xingfuxueyuan.xyz/gtufjkyzlr.html

[T21] Swift：遍历
来源：http://hz.ivvv.top/gtewdennwc.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtwmcvipeh.html

[T22] Swift：字典
来源：http://hz.shangyingyoupin.top/gtenxxcxyz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hysaishi.cn/gteytykznh.html

[T23] Swift：函数
来源：http://hz.bjfxy.top/gtgoifbumr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gzhubu.top/gtgxltsrhi.html

[T24] Swift：闭包
来源：http://hz.aibaodan.cn/gtlalysnvo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtmgdxamec.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gtazdmojgt.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtddpaxgdd.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtgxhvzuca.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gteqjfdsbh.html

[T27] Swift：错误处理
来源：http://hz.jianghu66.top/gtrlbmmcam.html

do { try f() } catch { print(error) }
来源：http://hz.wangdashe.top/gtdjjdiwgm.html

[T28] Swift：枚举
来源：http://hz.yuanzhike.top/gtoegboswr.html

enum Color { case red, green }
来源：http://hz.jqgufenzy.top/gtktkjopat.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangtech.top/gtojboukwd.html

guard let x = opt else { return }
来源：http://hz.kuanghao11.cn/gtrfskfuoc.html

[T30] Swift：协议
来源：http://hz.chenjidiqi.icu/gtxairdmrd.html

protocol Shape { func area() -> Double }
来源：http://hz.hnxiangtu.top/gtqzpgialv.html

[T31] Lua：Hello World
来源：http://hz.zhengqikj.top/gtvkcvukvr.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtmaapwqvs.html

[T32] Lua：局部变量
来源：http://hz.tian-w.cn/gtdxneaors.html

local a = 1
来源：http://hz.ydzc1.top/gtcmkcbach.html

[T33] Lua：表（数组）
来源：http://hz.chenlongwang.top/gtzvkqtbff.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cashguo.top/gtegvjepom.html

[T34] Lua：遍历表
来源：http://hz.fengsongda.top/gtndzduhxy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgufenzy.top/gtkescviuw.html

[T35] Lua：字典表
来源：http://hz.ehwqpu.com/gtnsroqrjk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gotoacloud.top/gtbkppulcr.html

[T36] Lua：函数
来源：http://hz.wangshuangyany.cn/gtlleldqsm.html

function add(a, b) return a + b end
来源：http://hz.jinqigufen.top/gtarbjikkg.html

[T37] Lua：字符串拼接
来源：http://hz.cdnleiting.top/gtvgaafful.html

"a" .. "b"
来源：http://hz.jiagoushi.top/gttgfibsql.html

[T38] Lua：条件
来源：http://hz.andypj.xyz/gtzayrapcc.html

if x > 0 then print("正") end
来源：http://hz.chenzaomai.com/gtchuhsxei.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtawsolode.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangtech.top/gtikxhyorx.html

[T40] Lua：元表
来源：http://hz.jinyuanbaomall.cn/gtzsorotqi.html

setmetatable({}, { __index = base })
来源：http://hz.jyoumei.cn/gtrlbrkubb.html

[T41] Perl：Hello World
来源：http://hz.gzhubu.top/gtqrtgwjqi.html

print "Hello\n";
来源：http://hz.zhoulong.xyz/gtewpxsknv.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gtyccbtbwl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.feifeiyinyue.top/gtdnunndjc.html

[T43] Perl：字符串插值
来源：http://hz.iojbl.cn/gtneqwsruu.html

"值: $a"
来源：http://hz.kuanghao11.cn/gtiuzmehrq.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtqshyntjf.html

if ($a > 0) { print "正"; }
来源：http://hz.pengpengdd.cyou/gtoetwlugl.html

[T45] Perl：数组遍历
来源：http://hz.yonumen.top/gtybxzktfr.html

for my $x (@arr) { print $x; }
来源：http://hz.dashuyun.cn/gtidbvdopc.html

[T46] Perl：哈希操作
来源：http://hz.aibaodan.cn/gtrugqjkjz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258888.top/gtlasnwpsa.html

[T47] Perl：正则捕获
来源：http://hz.zhaomingkeji.xyz/gtgpldtdha.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ybcxt.top/gthvnkedvx.html

[T48] Perl：正则替换
来源：http://hz.hongshengwenyu.top/gtijctbpfz.html

$s =~ s/old/new/g;
来源：http://hz.feifeiyinyue.top/gtrrptkuno.html

[T49] Perl：函数
来源：http://hz.gotoacloud.top/gtntwhrrhr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ybcxt.top/gttqctexjt.html

[T50] Perl：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtyyxfppsh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinghuilouyu.cn/gtputshzfb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gtrdkjwvfj.html

[T51] Scala：Hello World
来源：http://hz.52xcode.cn/gtkuxozvla.html

println("Hello")
来源：http://hz.cashguo.top/gtwjsozfyv.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gttxqpyvoe.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gtnxnvqayc.html

[T53] Scala：字符串插值
来源：http://hz.tanke756.top/gtjadurqjx.html

s"值: $b"
来源：http://hz.hnqzz.top/gtaqbgutza.html

[T54] Scala：集合映射
来源：http://hz.meibo888.top/gtwrbvajav.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jqgfzy.top/gtahbcmhsl.html

[T55] Scala：集合过滤
来源：http://hz.yvedp.cn/gtzgbqmvgm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cqqwz.cn/gtqqqeorso.html

[T56] Scala：样例类
来源：http://hz.tanke756.top/gtdszmmgai.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gtdjhcnpsx.html

[T57] Scala：模式匹配
来源：http://hz.aibaodan.cn/gtrwbnkswm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yongpay.top/gtpfrtfwse.html

[T58] Scala：函数定义
来源：http://hz.jinyuanbaomall.cn/gtactamexx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.vqdsnc.cn/gtkzdwhsqv.html

[T59] Scala：循环
来源：http://hz.zhijiandao.cn/gtpxedswxh.html

for (i <- 1 to 10) println(i)
来源：http://hz.yongpay.top/gtqkrwebit.html

[T60] Scala：折叠
来源：http://hz.jyoumei.cn/gtlwheqhup.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nwbrower.top/gthtkoisbg.html

================================================================================
来源：http://hz.dashuyun.cn/gtbuegfcph.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtyzhzpblm.html

================================================================================
来源：http://hz.aibaodan.cn/gtxgqorsal.html

[U01] Py：创建虚拟环境
来源：http://hz.zycfv.cn/gtfiteinls.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zycfv.cn/gtkiigoehc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cdnleiting.top/gtekhfoqmr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cucudq.cn/gtfysybrnw.html

[U03] Py：加载 .env 配置
来源：http://hz.xziqi.cn/gtqbymkgfp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yonumen.top/gtfinwfcje.html

[U04] Py：变量调试打印
来源：http://hz.jiagoushi.top/gtvtkczupd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sysykeji.top/gtdjmwdcwd.html

[U05] Py：列表去重且保序
来源：http://hz.yuxming.cn/gtvsmdfotn.html

list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtuajcmgau.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtqdfpttuy.html

{**a, **b}
来源：http://hz.cucudq.cn/gtlrbzxqqh.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gtroplsvuh.html

{v: k for k, v in d.items()}
来源：http://hz.ivvv.top/gtbljcxuul.html

[U08] Py：展平二维列表
来源：http://hz.0kj1m.cn/gtaqidjcwt.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtzctininu.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgfzy.top/gtrqxzandi.html

max(d, key=d.get)
来源：http://hz.smart0.xyz/gtfgtbsjih.html

[U10] Py：按值排序字典
来源：http://hz.guannengcc.top/gttrrhtwmx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigufen.top/gtxmfljfwy.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtuujwqmji.html

(x * 2 for x in arr)
来源：http://hz.bjfxy.top/gtmcvkupiq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yanxiufei.cn/gthrxluwia.html

Counter(arr).most_common(3)
来源：http://hz.yuxming.cn/gtkzomjsbt.html

[U13] Py：固定长度队列
来源：http://hz.redwolf501.top/gtpycwyruw.html

deque(maxlen=10)
来源：http://hz.jinqigfzy.top/gtbpbhsirk.html

[U14] Py：分组收集到列表
来源：http://hz.haohaochexian.top/gtfpbqrehc.html

defaultdict(list)
来源：http://hz.xylfe.cn/gterppdilj.html

[U15] Py：高精度计时
来源：http://hz.guannengcc.top/gttsfxbbpq.html

t = time.perf_counter()
来源：http://hz.yangfankeji.com/gtwoizjfhg.html

[U16] Py：命令行参数解析
来源：http://hz.xylfe.cn/gtvgjhjths.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jyoumei.cn/gtiyjsluzy.html

[U17] Py：初始化日志
来源：http://hz.xziqi.cn/gtdoaqxkzs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hammf.cn/gtkkwbmqov.html

[U18] Py：预编译正则
来源：http://hz.52xcode.cn/gtjbjxjsuc.html

pat = re.compile(r"\d+")
来源：http://hz.wangdashe.top/gtlalmymhg.html

[U19] Py：正则替换带回调
来源：http://hz.316326.xyz/gtccpehoez.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangtech.top/gtscuvuidh.html

[U20] Py：缓存函数结果
来源：http://hz.ivvv.top/gtsxxsdtgt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.vqdsnc.cn/gtrcoinuiw.html

[U21] Py：自定义上下文管理器
来源：http://hz.hywenlv.cn/gtjndckxsc.html

@contextlib.contextmanager
来源：http://hz.zhiwuduotai.top/gtyrbpovmf.html

[U22] Py：矩阵转置
来源：http://hz.zycfv.cn/gtpzkwyiyl.html

list(zip(*m))
来源：http://hz.ivvv.top/gtiqvoqdoa.html

[U23] Py：分块读取大文件
来源：http://hz.wangdashe.top/gtxqoohiwm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gotoacloud.top/gtterxbafq.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtxvmdteps.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.316326.xyz/gtjhzwjshl.html

[U25] Py：CSV 按字典读
来源：http://hz.fengsongda.top/gtgmzahyzt.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtaeiwevrq.html

[U26] Py：并发下载
来源：http://hz.zhoulong.xyz/gtrzerdtfk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jianghu66.top/gtfljpykdl.html


<!-- 参考信息 -->