代发 wailian999

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtxdezbtdg.html

[S04] C：字符串复制
来源：http://hz.yvedp.cn/gtjkpghbvz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.9152youxi.cn/gtobrbegix.html

[S05] C：字符串长度
来源：http://hz.ybcxt.top/gtvryssjeg.html

strlen(s)
来源：http://hz.ydzc1.top/gtajrqhogp.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gtvhpyibiu.html

strcmp(a, b) == 0
来源：http://hz.yonumen.top/gtngdjjyrw.html

[S07] C：数组遍历求和
来源：http://hz.andypj.xyz/gtpqghltyl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gteuscyovk.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtycephjhj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtvqbxflgs.html

[S09] C：结构体定义与初始化
来源：http://hz.hnxiangtu.top/gtrwrgzhpa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuetiantiany.cn/gtywryzozq.html

[S10] C：指针与解引用
来源：http://hz.52xcode.cn/gtvqjyvwsk.html

int *p = &a;  *p = 5;
来源：http://hz.havefunace.top/gtqyvrhpvq.html

[S11] C：逐行读文件
来源：http://hz.zhiwuduotai.top/gtitxeudwn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yonumen.top/gthfcldewx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtzdyuybir.html

fclose(f);
来源：http://hz.yj202588.top/gtaxzurhww.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gthdklwycj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtmtixdprt.html

[S13] C：宏定义
来源：http://hz.shanyushiyangtech.top/gtbcuuqavl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yueranfly.top/gtoxbknvxz.html

[S14] C：枚举
来源：http://hz.yonumen.top/gtyymwmjpq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxuanxn.top/gtlyrpgyid.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtqqlrcvlk.html

(double) a / b
来源：http://hz.dianchejie.cn/gtftrdvwhh.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtwvifmigx.html

x |= (1 << 3);
来源：http://hz.aizwys.cn/gtglspbqke.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtzmhklydf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtjridxhch.html

[S18] C：命令行参数
来源：http://hz.haohaochexian.top/gtoujjqwmi.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtboibkvwp.html

[S19] C：快速排序
来源：http://hz.iojbl.cn/gtpvypfxxe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtpkfpkiup.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtjwmrcwnu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtkxlvxifp.html

[S21] C：字符类别判断
来源：http://hz.nanxuanxn.top/gtspjkftrf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenzaomai.com/gtdklrxllc.html

[S22] C：字符串转数字
来源：http://hz.aizwys.cn/gtavppwzii.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.redwolf501.top/gtwpfeecnd.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gtnweibyxm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ehwqpu.com/gtthtyedth.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtyyyhexrr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shuidangran.top/gthklcmnth.html

[S25] C：内存拷贝
来源：http://hz.hysaishi.cn/gtqrbixsva.html

memcpy(dst, src, n);
来源：http://hz.9152youxi.cn/gtvsynfzfm.html

[S26] C：内存清零
来源：http://hz.wangdashe.top/gtsngbescc.html

memset(a, 0, sizeof a);
来源：http://hz.0kj1m.cn/gtbnickqxo.html

[S27] C：定义常量
来源：http://hz.hongshengwenyu.top/gtkzjomczc.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtulhoniqq.html

[S28] C：静态变量
来源：http://hz.yj202588.top/gtbwigjnrp.html

static int counter = 0;
来源：http://hz.pengpengdd.cyou/gtqqxgawmy.html

[S29] C：变参函数
来源：http://hz.pengpengdd.cyou/gtergeympc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigfzy.top/gtzyfvfdvs.html

[S30] C：头文件保护
来源：http://hz.jianghu66.top/gtbbcmaugn.html

#ifndef X_H
来源：http://hz.c1oappe.top/gtfykruzic.html

#define X_H
来源：http://hz.dashuyun.cn/gtferxhzdc.html

#endif
来源：http://hz.zhoulong.xyz/gtnfbmvkyy.html

[S31] C++：Hello World
来源：http://hz.shanyushiyangtech.top/gtyuulrnwh.html

#include <iostream>
来源：http://hz.xuanzx.com/gtugbxwshb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gtrpfmwmhl.html

[S32] C++：字符串
来源：http://hz.cashguo.top/gtytkotimk.html

std::string s = "hi";  s += "!";
来源：http://hz.zhiwuduotai.top/gtfudrcapf.html

[S33] C++：vector 增删
来源：http://hz.xingfuxueyuan.xyz/gtfzjrvxgm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtlelkckus.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtvxqxzpus.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sufxvd.cn/gtoyjntzxa.html

[S35] C++：map
来源：http://hz.yvedp.cn/gtwnxnnrdz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtujopikyf.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gttadrnbbg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtqejswycu.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtykpvpinb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydjk.org.cn/gttcixunei.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtywnqdida.html

std::sort(v.begin(), v.end());
来源：http://hz.andypj.xyz/gtvwslfbos.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gthblfvlyn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtdnffsafo.html

[S40] C++：查找元素
来源：http://hz.gogol.net.cn/gtjjufgpqf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258.top/gthabqgztj.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtggpyoghp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gtwlculpgc.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtylpowitw.html

class B : public Base { public: void f() override {} };
来源：http://hz.jyoumei.cn/gtkgukitck.html

[S43] C++：智能指针
来源：http://hz.ydzc1.top/gtoxftbscu.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtcjkaxrja.html

[S44] C++：引用传参
来源：http://hz.yuanzhike.top/gtwjdvyhvz.html

void inc(int &x) { ++x; }
来源：http://hz.iojbl.cn/gtodobirar.html

[S45] C++：lambda
来源：http://hz.zycfv.cn/gtoxpfbqmo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuanzx.com/gturgilhzy.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtffdoyhup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.c1oappe.top/gtpzjztipg.html

[S47] C++：结构化绑定遍历
来源：http://hz.52xcode.cn/gteoqwiati.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtlastujkf.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gthncmdnem.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtncpiafna.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtjlsfmnpe.html

[S49] C++：写文件
来源：http://hz.shzxlz.cn/gtbtllriwh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gtszjayxzq.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtdqymeguu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtomywzyfu.html

[S51] C++：显式类型转换
来源：http://hz.tanke756.top/gtranjymcv.html

static_cast<double>(a) / b
来源：http://hz.birdmap.top/gtftprcdzm.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtsmengihn.html

int size() const noexcept { return n_; }
来源：http://hz.feifeiyinyue.top/gtllnvyjpx.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtzszfbyyd.html

std::vector<int> w = std::move(v);
来源：http://hz.yanxiufei.cn/gtmgdyjnqh.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gttejcqyhq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtvhviztqg.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtxejfmirc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.iojbl.cn/gtozxmovfy.html

[S56] C++：optional
来源：http://hz.hongshengwenyu.top/gtjnoivris.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtqsxgicgy.html

[S57] C++：编译期常量
来源：http://hz.zhoulong.xyz/gtunnbjtcq.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gtafoefujh.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangtech.top/gtfoalrnii.html

namespace ns { int f() { return 1; } }
来源：http://hz.yongpay.top/gtojcycfbf.html

[S59] C++：静态断言
来源：http://hz.jinqigufen.top/gtsfureiik.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gtqgwxtaib.html

[S60] C++：遍历并删除元素
来源：http://hz.xylfe.cn/gtbftzkcwd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jiagoushi.top/gtitscpnfl.html

================================================================================
来源：http://hz.iojbl.cn/gtqiyofwbs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtnffqigma.html

================================================================================
来源：http://hz.pycfn.com/gthqyptwjs.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtqmztsbtm.html

println("Hello")
来源：http://hz.sxryk.cn/gtlttaavah.html

[T02] Kotlin：变量
来源：http://hz.gzhubu.top/gtsficomxr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtaraunqsn.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtdjqoqdvx.html

"值: $b"
来源：http://hz.dianchejie.cn/gttnzkgtxh.html

[T04] Kotlin：空安全
来源：http://hz.tianlin.xyz/gtwbddbjcc.html

val n: String? = null;  n?.length
来源：http://hz.haohaochexian.top/gtdoooereb.html

[T05] Kotlin：when 表达式
来源：http://hz.zhijiandao.cn/gtlrxkwwwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aizwys.cn/gtivvyxggd.html

[T06] Kotlin：集合映射
来源：http://hz.316326.xyz/gtbczfepjc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtxpcbvrbn.html

[T07] Kotlin：集合过滤
来源：http://hz.aizwys.cn/gtdluvolvu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shzxlz.cn/gtcnxmigim.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtshnfpexh.html

data class User(val name: String, val age: Int)
来源：http://hz.andypj.xyz/gtjqqgarcj.html

[T09] Kotlin：扩展函数
来源：http://hz.gaohongyu789.top/gteqzjrmwl.html

fun String.exclaim() = this + "!"
来源：http://hz.guannengcc.top/gtgkubfibl.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtpoumyscm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.mhx1999.top/gtzbbjvobi.html

[T11] Kotlin：协程
来源：http://hz.zhongyouzk.top/gthqyfnejg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yueranfly.top/gtkfdbjlqr.html

[T12] Kotlin：解构声明
来源：http://hz.shzxlz.cn/gtrnoylpns.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtnhipkwyg.html

[T13] Kotlin：只读 Map
来源：http://hz.zhijiandao.cn/gtkhkvmjml.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gtfdkexdqk.html

[T14] Kotlin：循环
来源：http://hz.xuetiantiany.cn/gtppsrouyo.html

for (i in 1..10) println(i)
来源：http://hz.zdqjudy.top/gtthewznkw.html

[T15] Kotlin：接口
来源：http://hz.pycfn.com/gtgrdesiqp.html

interface Shape { fun area(): Double }
来源：http://hz.shanyushiyangkeji.top/gtjduethed.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtajagppuu.html

print("Hello")
来源：http://hz.ehwqpu.com/gtzeesjboq.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gtyrurxvny.html

var a = 1;  let b = 2
来源：http://hz.yj202588.top/gtbygjxoyg.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gthxnyhnkh.html

"值: \(b)"
来源：http://hz.hammf.cn/gtjtbwwvxf.html

[T19] Swift：可选绑定
来源：http://hz.daxiang520.top/gtbgkfobaa.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtynbkbkgh.html

[T20] Swift：数组操作
来源：http://hz.hysaishi.cn/gtqipmekpv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gtqzggzmze.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gticdhzdzx.html

for x in a { print(x) }
来源：http://hz.tanke756.top/gtpwbcnsvp.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtidnpftfb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gotoacloud.top/gthnmuhere.html

[T23] Swift：函数
来源：http://hz.yj202588.top/gtnyxkttql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtqgjxxtwg.html

[T24] Swift：闭包
来源：http://hz.cashguo.top/gtpaginyyr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258.top/gtqewaauhk.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gtktpsknqd.html

struct P { var x: Int }
来源：http://hz.ybcxt.top/gtopyqnibj.html

[T26] Swift：类与重写
来源：http://hz.chenjidiqi.icu/gthgjhqbek.html

class A: Base { override func f() {} }
来源：http://hz.sxryk.cn/gtjmbeudzl.html

[T27] Swift：错误处理
来源：http://hz.dashuyun.cn/gtoseogujz.html

do { try f() } catch { print(error) }
来源：http://hz.cashguo.top/gtzuhpealx.html

[T28] Swift：枚举
来源：http://hz.ydjk.org.cn/gtfiujsaoi.html

enum Color { case red, green }
来源：http://hz.vqdsnc.cn/gtltcwqnri.html

[T29] Swift：guard 提前返回
来源：http://hz.316326.xyz/gtmlalgudz.html

guard let x = opt else { return }
来源：http://hz.bjfxy.top/gtqenyrwsf.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gthjassxfg.html

protocol Shape { func area() -> Double }
来源：http://hz.sxryk.cn/gtnbmkhlmu.html

[T31] Lua：Hello World
来源：http://hz.yongpay.top/gtkocqceja.html

print("Hello")
来源：http://hz.cheryme.top/gtsaekisnj.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtnmemxyfg.html

local a = 1
来源：http://hz.aizwys.cn/gtgnnfmblo.html

[T33] Lua：表（数组）
来源：http://hz.gotoacloud.top/gtbfzazywa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gthdfmpyuq.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtgrvqhsks.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sufxvd.cn/gtnjjdanxs.html

[T35] Lua：字典表
来源：http://hz.quarkkingdee.top/gtclikpbwy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shzxlz.cn/gtlhrijhfd.html

[T36] Lua：函数
来源：http://hz.yj20258.top/gtuppsmrpu.html

function add(a, b) return a + b end
来源：http://hz.zycfv.cn/gtumdiygdh.html

[T37] Lua：字符串拼接
来源：http://hz.shuidangran.top/gtxgnxacqf.html

"a" .. "b"
来源：http://hz.xziqi.cn/gtwmeoemab.html

[T38] Lua：条件
来源：http://hz.tian-w.cn/gtcjhvvnsx.html

if x > 0 then print("正") end
来源：http://hz.jqgfzy.top/gttrbuflfp.html

[T39] Lua：模式匹配
来源：http://hz.shangyingyoupin.top/gtzenoqgbs.html

string.find(s, "%d+")
来源：http://hz.daria6918.cn/gtzyiqdkrm.html

[T40] Lua：元表
来源：http://hz.nwbrower.top/gtxltsueht.html

setmetatable({}, { __index = base })
来源：http://hz.jiagoushi.top/gtythaizet.html

[T41] Perl：Hello World
来源：http://hz.cucudq.cn/gtyisnfnge.html

print "Hello\n";
来源：http://hz.cucudq.cn/gtuksuyujy.html

[T42] Perl：变量类型
来源：http://hz.xuetiantiany.cn/gtvekppxdl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.dashuyun.cn/gtlwgoqjdu.html

[T43] Perl：字符串插值
来源：http://hz.jlsjyb.cn/gtsesjyvgm.html

"值: $a"
来源：http://hz.xinyue.icu/gtgwiufqjw.html

[T44] Perl：条件
来源：http://hz.zhiwuduotai.top/gtbxhdpout.html

if ($a > 0) { print "正"; }
来源：http://hz.smart0.xyz/gtlemehlsj.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtanaveoic.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtjgxuoatg.html

[T46] Perl：哈希操作
来源：http://hz.gaohongyu789.top/gtqnjrrnoz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.9152youxi.cn/gttdjklvqm.html

[T47] Perl：正则捕获
来源：http://hz.zhongyouzk.top/gtlrjfcolu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gthvxlmjnu.html

[T48] Perl：正则替换
来源：http://hz.jlsjyb.cn/gtxvpqbgwh.html

$s =~ s/old/new/g;
来源：http://hz.shuidangran.top/gtzsqkinpf.html

[T49] Perl：函数
来源：http://hz.zdqjudy.top/gtrnddbbvc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhixingplan.top/gtilczwjaa.html

[T50] Perl：逐行读文件
来源：http://hz.yanxiufei.cn/gtcjydkikq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.mhx1999.top/gttgqcailb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhoulong.xyz/gtlnqcptwq.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gtflqgduln.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtprlgbibz.html

[T52] Scala：变量
来源：http://hz.dashuyun.cn/gtsfbpieij.html

val a = 1;  var b = 2
来源：http://hz.hfpthk.cn/gtwpmeojkh.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtggshjbwa.html

s"值: $b"
来源：http://hz.smart0.xyz/gtzqlqgtdd.html

[T54] Scala：集合映射
来源：http://hz.meibo888.top/gtgpqupbkb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shzxlz.cn/gtpmmzruhf.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gtapvfclst.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.52xcode.cn/gtrhlomxpq.html

[T56] Scala：样例类
来源：http://hz.svipenyu.cn/gtsxnhtrlv.html

case class User(name: String, age: Int)
来源：http://hz.jinqigfzy.top/gttolenqev.html

[T57] Scala：模式匹配
来源：http://hz.xziqi.cn/gtxnmfdwhc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhijiandao.cn/gttpfryufx.html

[T58] Scala：函数定义
来源：http://hz.quarkkingdee.top/gtcttabxui.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yongpay.top/gtvvttahsd.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtvkuonkqx.html

for (i <- 1 to 10) println(i)
来源：http://hz.316326.xyz/gtjdlhmdmj.html

[T60] Scala：折叠
来源：http://hz.zhaomingkeji.xyz/gtvwxucars.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.birdmap.top/gtsbrblmvv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtggrkriiu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258888.top/gtvrsrwfkn.html

================================================================================
来源：http://hz.guowangkeji.top/gtrhlgraon.html

[U01] Py：创建虚拟环境
来源：http://hz.nwbrower.top/gtqxnfzuqc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gthrypncid.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jianghu66.top/gtlnbwvahg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj20258888.top/gtwnejcwyq.html

[U03] Py：加载 .env 配置
来源：http://hz.quarkkingdee.top/gtvsdpcbji.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtpyikuhyi.html

[U04] Py：变量调试打印
来源：http://hz.andypj.xyz/gtmygzhmgh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtndaemsdj.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gtfjkfmlmx.html

list(dict.fromkeys(arr))
来源：http://hz.bjfxy.top/gtoprtncjd.html

[U06] Py：合并两个字典
来源：http://hz.fengsongda.top/gtsoxsqqem.html

{**a, **b}
来源：http://hz.hammf.cn/gtmscgforo.html

[U07] Py：反转字典键值
来源：http://hz.jinyuanbaomall.cn/gtrzsfchcc.html

{v: k for k, v in d.items()}
来源：http://hz.ydzc1.top/gthqxglflp.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gtfopnntty.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtyfctgahg.html

[U09] Py：字典取最大值的键
来源：http://hz.gaohongyu789.top/gtuqibykes.html

max(d, key=d.get)
来源：http://hz.yvedp.cn/gtkvyscmkq.html

[U10] Py：按值排序字典
来源：http://hz.wangdashe.top/gtfgzyxbmo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.0kj1m.cn/gthsldilfx.html

[U11] Py：生成器表达式
来源：http://hz.jinyuanbaomall.cn/gtjzcmduzy.html

(x * 2 for x in arr)
来源：http://hz.tanke756.top/gttfrxhqhh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shanyushiyangtech.top/gtsbxxhnsc.html

Counter(arr).most_common(3)
来源：http://hz.cashguo.top/gtahhkicng.html

[U13] Py：固定长度队列
来源：http://hz.xingfuxueyuan.xyz/gtwsdwzqof.html

deque(maxlen=10)
来源：http://hz.yuxming.cn/gtlbynuzvl.html

[U14] Py：分组收集到列表
来源：http://hz.feifeiyinyue.top/gthoqvlqoe.html

defaultdict(list)
来源：http://hz.chenlongwang.top/gtmixmnzzh.html

[U15] Py：高精度计时
来源：http://hz.tanke756.top/gtcrpoeckx.html

t = time.perf_counter()
来源：http://hz.fengsongda.top/gtxehyeszw.html

[U16] Py：命令行参数解析
来源：http://hz.ydjk.org.cn/gtznjskfzz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yongpay.top/gtgopuvvwx.html

[U17] Py：初始化日志
来源：http://hz.ybcxt.top/gtngtubhcv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.smart0.xyz/gtpzpcwjkv.html

[U18] Py：预编译正则
来源：http://hz.zhoulong.xyz/gtenbdesjv.html

pat = re.compile(r"\d+")
来源：http://hz.xingfuxueyuan.xyz/gtityywdbj.html

[U19] Py：正则替换带回调
来源：http://hz.zdqjudy.top/gtejjehmhy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhiwuduotai.top/gtngzbfeop.html

[U20] Py：缓存函数结果
来源：http://hz.andypj.xyz/gtzbzzemvv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhongyouzk.top/gtbfmdezfx.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gtexkjxlmr.html

@contextlib.contextmanager
来源：http://hz.jiagoushi.top/gtoxsiflzf.html

[U22] Py：矩阵转置
来源：http://hz.ydzc1.top/gtwgzafseq.html

list(zip(*m))
来源：http://hz.xuetiantiany.cn/gtfzhodksi.html

[U23] Py：分块读取大文件
来源：http://hz.guowangkeji.top/gthomhodou.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dianchejie.cn/gtgeaxtgmr.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gtjmekmbcb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnqzz.top/gtbiiyecyl.html

[U25] Py：CSV 按字典读
来源：http://hz.hywenlv.cn/gtxqvltkpx.html

csv.DictReader(f)
来源：http://hz.svipenyu.cn/gtyqoapknh.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtxmuwtskq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ppjwa.cn/gtnrskabus.html


<!-- 参考信息 -->