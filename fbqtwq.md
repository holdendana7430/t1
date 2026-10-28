代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ybcxt.top/gtyxwmissq.html

[R80] 查看脚本执行耗时
来源：http://hz.zycfv.cn/gtjhgqvfsk.html

time ./run.sh
来源：http://hz.chenjidiqi.icu/gtkqyvvbao.html

================================================================================
来源：http://hz.snrcjt.cn/gtogcvlqad.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gtvygaqbic.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzqrvblay.html

[S01] C：Hello World
来源：http://hz.birdmap.top/gtkyzpsuat.html

#include <stdio.h>
来源：http://hz.0kj1m.cn/gtdclkvctl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtzciyzjbx.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gtubqrljug.html

int a = 10; printf("%d\n", a);
来源：http://hz.quarkkingdee.top/gtfndjjhwy.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtvebjjzog.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtajjqezhe.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtzfivcxfd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gtrytjqzap.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtorwduwsr.html

strlen(s)
来源：http://hz.hammf.cn/gtbgopylxr.html

[S06] C：字符串比较
来源：http://hz.c1oappe.top/gtftruntsk.html

strcmp(a, b) == 0
来源：http://hz.zhijiandao.cn/gtuooiyoks.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangkeji.top/gtdcjylmpa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pycfn.com/gtvohddzbv.html

[S08] C：动态内存分配与释放
来源：http://hz.yanxiufei.cn/gtmisovwpi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgufenzy.top/gtwqzdjenx.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gtouxkaovb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cqqwz.cn/gtqdpbmppz.html

[S10] C：指针与解引用
来源：http://hz.yj20258888.top/gtxfucsdtt.html

int *p = &a;  *p = 5;
来源：http://hz.andypj.xyz/gtwncvsutn.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gtpwdtuxvl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gtikhltwnr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gtlwkguhsp.html

fclose(f);
来源：http://hz.hammf.cn/gtspuafdhd.html

[S12] C：写文件
来源：http://hz.hnxiangtu.top/gtbwdksxib.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ivvv.top/gttoajlmzz.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtvwcmrkjw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aibaodan.cn/gtjlqvpzid.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtfqdsuolb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gtagxoqpsv.html

[S15] C：类型转换
来源：http://hz.chenjidiqi.icu/gtloquizwd.html

(double) a / b
来源：http://hz.yongpay.top/gtieeuutrz.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gtdrlxrpvh.html

x |= (1 << 3);
来源：http://hz.zhiwuduotai.top/gtlwmicume.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtmgmajird.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cqqwz.cn/gttkskmmzh.html

[S18] C：命令行参数
来源：http://hz.aibaodan.cn/gtajbbraxr.html

int main(int argc, char **argv)
来源：http://hz.hfpthk.cn/gtkaozrqpt.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gtafwekahb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtpxbehbok.html

[S20] C：二分查找
来源：http://hz.aibaodan.cn/gtvpwowxea.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtpmzbnpii.html

[S21] C：字符类别判断
来源：http://hz.jinqigufen.top/gtkesoeylk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangdashe.top/gtasdbxkpz.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtpomqslrf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydjk.org.cn/gtowujumlz.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtbwtstbab.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangdashe.top/gtzvoegdqp.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtzrxxrsbr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigfzy.top/gtdjmkdfpr.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gtdeudnouf.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtvpcjcevr.html

[S26] C：内存清零
来源：http://hz.pengpengdd.cyou/gthpsmtrqg.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtiiormcxq.html

[S27] C：定义常量
来源：http://hz.jqgfzy.top/gtgpexnstk.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtvhygypfa.html

[S28] C：静态变量
来源：http://hz.tanke756.top/gtxkcnbdvb.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gtnfioqbuo.html

[S29] C：变参函数
来源：http://hz.52xcode.cn/gthgvkdkqx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhiwuduotai.top/gtpkxzpker.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtpsisjfot.html

#ifndef X_H
来源：http://hz.zycfv.cn/gtjyfskueq.html

#define X_H
来源：http://hz.c1oappe.top/gtzaqfziqx.html

#endif
来源：http://hz.gogol.net.cn/gtrawmkynm.html

[S31] C++：Hello World
来源：http://hz.yj202588.top/gtxqkdmolw.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gtkiywywld.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangtech.top/gtjtkqtkte.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gtchfikozs.html

std::string s = "hi";  s += "!";
来源：http://hz.xingfuxueyuan.xyz/gtcspjuqdv.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gttsnaopqu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cucudq.cn/gtcpyathuu.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtmqwsdcmp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hysaishi.cn/gtahyjmeya.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtbptaiwfs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtovscxwht.html

[S36] C++：unordered_map
来源：http://hz.chenzaomai.com/gtffyzuxdw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhengqikj.top/gtmxffvxhh.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtfpidwzhf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.52xcode.cn/gtjpwwipxz.html

[S38] C++：排序
来源：http://hz.mhx1999.top/gtbtbikyub.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gtxumttwyw.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtpwkhknuv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhoulong.xyz/gtqcwszkru.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtenweeurb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.kuanghao11.cn/gtxgarkyer.html

[S41] C++：类与构造函数
来源：http://hz.zhengqikj.top/gtrkdwshpd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jlsjyb.cn/gtglwlqcpv.html

[S42] C++：继承与虚函数
来源：http://hz.havefunace.top/gtbsgqoots.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuanzhike.top/gtddehrkly.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gtjvahwfwt.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxinkj.top/gtaeirqpxw.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtglgrjlif.html

void inc(int &x) { ++x; }
来源：http://hz.tianlin.xyz/gtlbjozfzb.html

[S45] C++：lambda
来源：http://hz.cqqwz.cn/gttrpcgzva.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtrobjllzb.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gtvmizkobw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtctzxvabm.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtknmzdgqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtirgmohzr.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtfjzmiaeg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhengqikj.top/gtamtctwpk.html

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtvvhdrncj.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtvdblivlk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hammf.cn/gtinrcewcv.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtcbexlxrh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtbrvvsima.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gtxgwtaxik.html

static_cast<double>(a) / b
来源：http://hz.gotoacloud.top/gtzhndpuvs.html

[S52] C++：const 与 noexcept
来源：http://hz.aizwys.cn/gtjvzsuulj.html

int size() const noexcept { return n_; }
来源：http://hz.andypj.xyz/gtwbpjsbyx.html

[S53] C++：移动语义
来源：http://hz.wangshuangyany.cn/gtpzblzwxk.html

std::vector<int> w = std::move(v);
来源：http://hz.xingfuxueyuan.xyz/gtuezmgwad.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtkijspkvo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtrufqeium.html

[S55] C++：结构化绑定
来源：http://hz.sufxvd.cn/gtzckpiijo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtestykuvd.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtxncepwtb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtcfqvtlqt.html

[S57] C++：编译期常量
来源：http://hz.yj202588.top/gtmlwzktdt.html

constexpr int N = 10;
来源：http://hz.jlsjyb.cn/gtzfctgtgz.html

[S58] C++：命名空间
来源：http://hz.yonumen.top/gtezdhxyic.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhongyouzk.top/gtfbhcptkt.html

[S59] C++：静态断言
来源：http://hz.sxryk.cn/gteqkjtncf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gthnnpqrfp.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxinkj.top/gtrqetavti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cqqwz.cn/gtwfkbeafr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvsylujhw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtjxojvadt.html

================================================================================
来源：http://hz.meibo888.top/gtnqziavnr.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtiuxorthj.html

println("Hello")
来源：http://hz.hfpthk.cn/gtmfdkypns.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gtwfgalypi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.meibo888.top/gtpecmgzbf.html

[T03] Kotlin：字符串模板
来源：http://hz.chenjidiqi.icu/gtnozsjlig.html

"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtvsryoege.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtolluwqpn.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtmepxmmin.html

[T05] Kotlin：when 表达式
来源：http://hz.yonumen.top/gtrgqqdvpz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtifpdrwnc.html

[T06] Kotlin：集合映射
来源：http://hz.yongpay.top/gtmjoijbit.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangdashe.top/gtetqdxsgc.html

[T07] Kotlin：集合过滤
来源：http://hz.gzhubu.top/gtpuvrikwt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtsulolrtu.html

[T08] Kotlin：数据类
来源：http://hz.jianghu66.top/gtsafjtnvi.html

data class User(val name: String, val age: Int)
来源：http://hz.shuidangran.top/gtryuoijsc.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtjybjdzmn.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtywligvdb.html

[T10] Kotlin：默认参数
来源：http://hz.quarkkingdee.top/gtxgwkscao.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zdqjudy.top/gtlkhqblha.html

[T11] Kotlin：协程
来源：http://hz.hysaishi.cn/gtzyzwlqkr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.vqdsnc.cn/gtfixrmusu.html

[T12] Kotlin：解构声明
来源：http://hz.hnxiangtu.top/gtpgokmzer.html

val (a, b) = Pair(1, 2)
来源：http://hz.yonumen.top/gtvmvzugdo.html

[T13] Kotlin：只读 Map
来源：http://hz.wangshuangyany.cn/gtgsxiifdn.html

val m = mapOf("a" to 1)
来源：http://hz.xuanzx.com/gtiaopxhgg.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gttmxtousl.html

for (i in 1..10) println(i)
来源：http://hz.xuetiantiany.cn/gtzsnevgiw.html

[T15] Kotlin：接口
来源：http://hz.52xcode.cn/gtsjshzyvz.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtvwusaosd.html

[T16] Swift：Hello World
来源：http://hz.meibo888.top/gtfrysjvsf.html

print("Hello")
来源：http://hz.aibaodan.cn/gtsljsycmo.html

[T17] Swift：变量与常量
来源：http://hz.316326.xyz/gtxgaxmwqh.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtabpkytnw.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtopjowdao.html

"值: \(b)"
来源：http://hz.sweek.top/gtwpmbnpqk.html

[T19] Swift：可选绑定
来源：http://hz.havefunace.top/gtoxgtlrcs.html

if let n = opt { print(n) }
来源：http://hz.birdmap.top/gtekwsfucp.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtveyjxncm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.feifeiyinyue.top/gtnuwujnja.html

[T21] Swift：遍历
来源：http://hz.fzhhl.top/gtjgueeyuo.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtqswgqxrk.html

[T22] Swift：字典
来源：http://hz.cdnleiting.top/gtqnisfpdj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.haohaochexian.top/gtmzpmcuxa.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtxjbkiodk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtzdkhtqkp.html

[T24] Swift：闭包
来源：http://hz.aizwys.cn/gtzgzepads.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtnibovwsd.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gtrqsrxujq.html

struct P { var x: Int }
来源：http://hz.sufxvd.cn/gtexgmsvce.html

[T26] Swift：类与重写
来源：http://hz.bjfxy.top/gtfezaavzn.html

class A: Base { override func f() {} }
来源：http://hz.nanxinkj.top/gtfbedqgzz.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtgfxllfbd.html

do { try f() } catch { print(error) }
来源：http://hz.andypj.xyz/gtqucoazwf.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangkeji.top/gtxwmwukja.html

enum Color { case red, green }
来源：http://hz.ehwqpu.com/gtyofrwwkt.html

[T29] Swift：guard 提前返回
来源：http://hz.wangdashe.top/gtykaitgfs.html

guard let x = opt else { return }
来源：http://hz.sxryk.cn/gtliverdeo.html

[T30] Swift：协议
来源：http://hz.shangyingyoupin.top/gtfosjujyu.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtyjxzalbj.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtjzgzqnte.html

print("Hello")
来源：http://hz.yj20258.top/gtcajjkqom.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtbcflmvwn.html

local a = 1
来源：http://hz.yangfankeji.com/gtqqjgtnua.html

[T33] Lua：表（数组）
来源：http://hz.jianghu66.top/gtazorkfqg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hammf.cn/gtmxntlnje.html

[T34] Lua：遍历表
来源：http://hz.tanke756.top/gtavqqvrlf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guannengcc.top/gtnnnmhiah.html

[T35] Lua：字典表
来源：http://hz.sufxvd.cn/gtzyipsklv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ivvv.top/gtckxdxaou.html

[T36] Lua：函数
来源：http://hz.hnqzz.top/gtazkilggj.html

function add(a, b) return a + b end
来源：http://hz.zycfv.cn/gtcczlhrpn.html

[T37] Lua：字符串拼接
来源：http://hz.guannengcc.top/gtueognjpo.html

"a" .. "b"
来源：http://hz.dashuyun.cn/gtzdrufesm.html

[T38] Lua：条件
来源：http://hz.quarkkingdee.top/gtdwrlsppf.html

if x > 0 then print("正") end
来源：http://hz.mhx1999.top/gtubhowmqb.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangkeji.top/gtgqahzeos.html

string.find(s, "%d+")
来源：http://hz.smart0.xyz/gtmfwvuekb.html

[T40] Lua：元表
来源：http://hz.sufxvd.cn/gtakhkladf.html

setmetatable({}, { __index = base })
来源：http://hz.yvedp.cn/gtrgmrcpdv.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtehzqwokn.html

print "Hello\n";
来源：http://hz.pycfn.com/gtpzeodmum.html

[T42] Perl：变量类型
来源：http://hz.zhaomingkeji.xyz/gtszounwpn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangtech.top/gtydnilnlv.html

[T43] Perl：字符串插值
来源：http://hz.hammf.cn/gtxoyfltds.html

"值: $a"
来源：http://hz.yanxiufei.cn/gtmjhtwgqk.html

[T44] Perl：条件
来源：http://hz.sxryk.cn/gteaarhswq.html

if ($a > 0) { print "正"; }
来源：http://hz.yvedp.cn/gtnxkeahun.html

[T45] Perl：数组遍历
来源：http://hz.iojbl.cn/gtyasfupsw.html

for my $x (@arr) { print $x; }
来源：http://hz.xziqi.cn/gthlmymbys.html

[T46] Perl：哈希操作
来源：http://hz.wangdashe.top/gtrqszqucs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258.top/gtdpywhgfw.html

[T47] Perl：正则捕获
来源：http://hz.smart0.xyz/gtdpqeeskd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.mhx1999.top/gtfsxazofr.html

[T48] Perl：正则替换
来源：http://hz.hysaishi.cn/gtvjyxdvry.html

$s =~ s/old/new/g;
来源：http://hz.xuetiantiany.cn/gtvybbmymd.html

[T49] Perl：函数
来源：http://hz.dianchejie.cn/gtnrwdjexf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnqzz.top/gtivifebnd.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtuislgtrt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhaomingkeji.xyz/gtlijykkcy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenjidiqi.icu/gtklwsvkay.html

[T51] Scala：Hello World
来源：http://hz.hnqzz.top/gtdutljeti.html

println("Hello")
来源：http://hz.yongpay.top/gtufjdvvta.html

[T52] Scala：变量
来源：http://hz.gaohongyu789.top/gteeaqdpgl.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtgimizwpa.html

[T53] Scala：字符串插值
来源：http://hz.yj20258888.top/gtfidcoxkj.html

s"值: $b"
来源：http://hz.jianghu66.top/gtpiweicto.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gteezdvipk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxuanxn.top/gtxkgnydaa.html

[T55] Scala：集合过滤
来源：http://hz.jinghuilouyu.cn/gtpziyaaho.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhongyouzk.top/gtcrvjauus.html

[T56] Scala：样例类
来源：http://hz.zhijiandao.cn/gtqwccviay.html

case class User(name: String, age: Int)
来源：http://hz.jiagoushi.top/gtwzzftyqv.html

[T57] Scala：模式匹配
来源：http://hz.hywenlv.cn/gtwmcppobm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxuanxn.top/gtonkdlzwz.html

[T58] Scala：函数定义
来源：http://hz.sxryk.cn/gtkwlxpkww.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yuxming.cn/gthrqcuwhl.html

[T59] Scala：循环
来源：http://hz.gogol.net.cn/gtmkhkeuqz.html

for (i <- 1 to 10) println(i)
来源：http://hz.0kj1m.cn/gtnmmnbsuu.html

[T60] Scala：折叠
来源：http://hz.xziqi.cn/gtfsldqwen.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtgqiulisj.html

================================================================================
来源：http://hz.shzxlz.cn/gtbeakbvcd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sufxvd.cn/gtbhxuknwl.html

================================================================================
来源：http://hz.daxiang520.top/gtwwertfnn.html

[U01] Py：创建虚拟环境
来源：http://hz.xziqi.cn/gtfvdyxtah.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuetiantiany.cn/gtegmiektg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgufenzy.top/gtopdghdfa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xinyue.icu/gtybvoboud.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gthlyodycv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangdashe.top/gtqnyujsch.html

[U04] Py：变量调试打印
来源：http://hz.hywenlv.cn/gtbxeadjyo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangshuangyany.cn/gtlqcvvdkh.html

[U05] Py：列表去重且保序
来源：http://hz.havefunace.top/gtdvevemsi.html

list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtvzghjlrx.html

[U06] Py：合并两个字典
来源：http://hz.ivvv.top/gtdunhmvsa.html

{**a, **b}
来源：http://hz.zhijiandao.cn/gtgxlcfykq.html

[U07] Py：反转字典键值
来源：http://hz.snrcjt.cn/gtirlnqfej.html

{v: k for k, v in d.items()}
来源：http://hz.wangshuangyany.cn/gtojehgost.html

[U08] Py：展平二维列表
来源：http://hz.yangfankeji.com/gtihtcpcam.html

[y for x in nested for y in x]
来源：http://hz.9152youxi.cn/gtbwrnjgvy.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258.top/gthbncrnpq.html

max(d, key=d.get)
来源：http://hz.cheryme.top/gtwpkbzjka.html

[U10] Py：按值排序字典
来源：http://hz.shzxlz.cn/gtnkdovdyr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj202588.top/gtnvmgeqgs.html

[U11] Py：生成器表达式
来源：http://hz.dashuyun.cn/gtcfewfyis.html

(x * 2 for x in arr)
来源：http://hz.quarkkingdee.top/gtdmlxnziu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.iojbl.cn/gtrzbzfxbr.html

Counter(arr).most_common(3)
来源：http://hz.xingfuxueyuan.xyz/gtbpfeqaem.html

[U13] Py：固定长度队列
来源：http://hz.jlsjyb.cn/gtqsndbnjy.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gtoraiqcee.html

[U14] Py：分组收集到列表
来源：http://hz.shanyushiyangkeji.top/gtqauxyjks.html

defaultdict(list)
来源：http://hz.316326.xyz/gtjyjjwbgb.html

[U15] Py：高精度计时
来源：http://hz.ydzc1.top/gtkjlysaeg.html

t = time.perf_counter()
来源：http://hz.dianchejie.cn/gtzebyliss.html

[U16] Py：命令行参数解析
来源：http://hz.tian-w.cn/gtfccjrvju.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nwbrower.top/gtbziflesd.html

[U17] Py：初始化日志
来源：http://hz.ybcxt.top/gtgyovchhk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gtouqettyj.html

[U18] Py：预编译正则
来源：http://hz.jlsjyb.cn/gtgsrfpvkr.html

pat = re.compile(r"\d+")
来源：http://hz.yongpay.top/gtwpwjjatz.html

[U19] Py：正则替换带回调
来源：http://hz.hammf.cn/gtetishqkl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gttnmuksjn.html

[U20] Py：缓存函数结果
来源：http://hz.yangfankeji.com/gtpdomjtic.html

@functools.lru_cache(maxsize=None)
来源：http://hz.9152youxi.cn/gtxofpsgzu.html


<!-- 参考信息 -->