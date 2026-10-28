代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.gaohongyu789.top/gteeiphhfu.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gtkgedsots.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtducwcncw.html

[R77] 读取用户输入
来源：http://hz.yj20258888.top/gthyoufdoe.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gtrpxrbkmg.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtekrldqix.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtjvjqjxki.html

[R79] 解析命令行选项
来源：http://hz.ybcxt.top/gtotjmlqiv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xinyue.icu/gtbrciboug.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtnbtlnbfy.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtfrwzaqjz.html

================================================================================
来源：http://hz.jiagoushi.top/gtfziwtlkg.html

S. C / C++ 专题
来源：http://hz.fengsongda.top/gtjjainejn.html

================================================================================
来源：http://hz.gogol.net.cn/gtthxxgpnk.html

[S01] C：Hello World
来源：http://hz.316326.xyz/gtxtjaioan.html

#include <stdio.h>
来源：http://hz.shangyingyoupin.top/gtywekhorq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.smart0.xyz/gtouamwxzj.html

[S02] C：变量与格式化输出
来源：http://hz.yuanzhike.top/gtbqvwnprj.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtudlkpdxl.html

[S03] C：读入整数
来源：http://hz.jyoumei.cn/gtgvcwddbw.html

int x; scanf("%d", &x);
来源：http://hz.guannengcc.top/gtpcderaqi.html

[S04] C：字符串复制
来源：http://hz.haohaochexian.top/gtllnjhafo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtnpoqlkkf.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gtvsepvdci.html

strlen(s)
来源：http://hz.andypj.xyz/gtsvyqrbum.html

[S06] C：字符串比较
来源：http://hz.nanxinkj.top/gtfumcltro.html

strcmp(a, b) == 0
来源：http://hz.shuidangran.top/gtutlchpvl.html

[S07] C：数组遍历求和
来源：http://hz.jianghu66.top/gtpwqbcesw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gteklehcfa.html

[S08] C：动态内存分配与释放
来源：http://hz.cqqwz.cn/gtibhrlywq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shuidangran.top/gtarwuhsxs.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtvlyycktf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxuanxn.top/gtefphiivz.html

[S10] C：指针与解引用
来源：http://hz.xziqi.cn/gtbynujklv.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtkqnruiuc.html

[S11] C：逐行读文件
来源：http://hz.jianghu66.top/gtwwghrspc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtfzcrzizx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.havefunace.top/gtplcgdfjr.html

fclose(f);
来源：http://hz.zhengqikj.top/gtvajlusma.html

[S12] C：写文件
来源：http://hz.nwbrower.top/gtjnkaajuh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cucudq.cn/gtolviimoy.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtntevkqev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.52xcode.cn/gtdyazlyxc.html

[S14] C：枚举
来源：http://hz.ppjwa.cn/gtmhoeaanu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.316326.xyz/gthiwqpllk.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gtwbznmdvo.html

(double) a / b
来源：http://hz.sufxvd.cn/gtndvldmdp.html

[S16] C：位操作置位
来源：http://hz.nanxinkj.top/gtmwxfmgvi.html

x |= (1 << 3);
来源：http://hz.yj202588.top/gtpcfqgdcl.html

[S17] C：安全拼接字符串
来源：http://hz.yueranfly.top/gtreiusftq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gthtctezkt.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gtppnxcnnx.html

int main(int argc, char **argv)
来源：http://hz.pengpengdd.cyou/gtctrtnmsx.html

[S19] C：快速排序
来源：http://hz.hywenlv.cn/gtyijuduiz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtsjnqxmij.html

[S20] C：二分查找
来源：http://hz.xingfuxueyuan.xyz/gtylannpia.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtsghrdepp.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gtvuatiepm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenzaomai.com/gtitlxlmwf.html

[S22] C：字符串转数字
来源：http://hz.yanxiufei.cn/gtoyzcxurl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgufenzy.top/gtfpugabox.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtwyjqgsgp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jyoumei.cn/gtviewzodv.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtleogrbpn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtynwhmxsr.html

[S25] C：内存拷贝
来源：http://hz.cqqwz.cn/gtrhclshbd.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtruedwvho.html

[S26] C：内存清零
来源：http://hz.daxiang520.top/gtwykftxra.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtkgfghgee.html

[S27] C：定义常量
来源：http://hz.gaohongyu789.top/gtpuynrpqy.html

const double PI = 3.14159;
来源：http://hz.pycfn.com/gtvyfuallm.html

[S28] C：静态变量
来源：http://hz.hfpthk.cn/gtlozaiptu.html

static int counter = 0;
来源：http://hz.ywan-chungtsiang.top/gtvfdbvnzk.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gthbqbicup.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtoqijyfyg.html

[S30] C：头文件保护
来源：http://hz.yj202588.top/gtiovpezrp.html

#ifndef X_H
来源：http://hz.cqqwz.cn/gtomeuaebf.html

#define X_H
来源：http://hz.jiagoushi.top/gtmtratrfi.html

#endif
来源：http://hz.zhixingplan.top/gtoxofckoh.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtulbgxado.html

#include <iostream>
来源：http://hz.ydzc1.top/gtjaamgqsa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtkfjcqqbh.html

[S32] C++：字符串
来源：http://hz.hywenlv.cn/gtagdraete.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gtguognpcx.html

[S33] C++：vector 增删
来源：http://hz.jianghu66.top/gtxsabrbmg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtiyqwstiu.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtbehkwkob.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gteqmujuzv.html

[S35] C++：map
来源：http://hz.hongshengwenyu.top/gtgizbdack.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtizdkrwyh.html

[S36] C++：unordered_map
来源：http://hz.sxryk.cn/gtotbvysmb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gtkpskhxwu.html

[S37] C++：set
来源：http://hz.hysaishi.cn/gtixpirshu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinghuilouyu.cn/gtgzkcoama.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtndxicnzp.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtfovjgakx.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtcgiurvjf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtvzpwelst.html

[S40] C++：查找元素
来源：http://hz.wangdashe.top/gtbwmoyrux.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.redwolf501.top/gtlkvhazug.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtppwjbsmn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtuminfbir.html

[S42] C++：继承与虚函数
来源：http://hz.gzhubu.top/gtvemkythz.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtwqnllszo.html

[S43] C++：智能指针
来源：http://hz.sxryk.cn/gtwviaaylh.html

auto p = std::make_unique<int>(5);
来源：http://hz.cdnleiting.top/gtykugyxzg.html

[S44] C++：引用传参
来源：http://hz.zhijiandao.cn/gtxldlqufg.html

void inc(int &x) { ++x; }
来源：http://hz.zhaomingkeji.xyz/gtvcmqfdsb.html

[S45] C++：lambda
来源：http://hz.ivvv.top/gtkfekdozt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tanke756.top/gtcutemppe.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtellrytlk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuetiantiany.cn/gtcwwjgqyh.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtxukjvzgf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtnglodtnv.html

[S48] C++：逐行读文件
来源：http://hz.cdnleiting.top/gtqnumqatu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtktdgjcoh.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtydlafyrz.html

[S49] C++：写文件
来源：http://hz.pengpengdd.cyou/gtncnvlrbn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhengqikj.top/gtyjjltdqp.html

[S50] C++：格式化数字
来源：http://hz.dianchejie.cn/gtbzimpibi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtqjhfrjjw.html

[S51] C++：显式类型转换
来源：http://hz.chenlongwang.top/gtrdfdrafu.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gtcvpqnkqy.html

[S52] C++：const 与 noexcept
来源：http://hz.gogol.net.cn/gtshmmnrlc.html

int size() const noexcept { return n_; }
来源：http://hz.snrcjt.cn/gtvackjkzi.html

[S53] C++：移动语义
来源：http://hz.jiagoushi.top/gttiselqat.html

std::vector<int> w = std::move(v);
来源：http://hz.sweek.top/gteypoofkb.html

[S54] C++：异常处理
来源：http://hz.0kj1m.cn/gtunytqend.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daria6918.cn/gtssvoitpl.html

[S55] C++：结构化绑定
来源：http://hz.dashuyun.cn/gtdpukowko.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtxlerwtlj.html

[S56] C++：optional
来源：http://hz.chenlongwang.top/gtvpbybtho.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.andypj.xyz/gtdxrznzxt.html

[S57] C++：编译期常量
来源：http://hz.yonumen.top/gtvwsjtjqz.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtwagcxgbm.html

[S58] C++：命名空间
来源：http://hz.chenzaomai.com/gtopxupjig.html

namespace ns { int f() { return 1; } }
来源：http://hz.iojbl.cn/gtasegqjds.html

[S59] C++：静态断言
来源：http://hz.jinqigufen.top/gtnkmhomok.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cucudq.cn/gtrovrjney.html

[S60] C++：遍历并删除元素
来源：http://hz.dashuyun.cn/gtepepzdce.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tanke756.top/gtouldlzer.html

================================================================================
来源：http://hz.smart0.xyz/gthiwmjxpn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gthgukylhb.html

================================================================================
来源：http://hz.nwbrower.top/gtbgyjjgep.html

[T01] Kotlin：Hello World
来源：http://hz.yj202588.top/gtmxqbdsyz.html

println("Hello")
来源：http://hz.tian-w.cn/gtbsidsgeq.html

[T02] Kotlin：变量
来源：http://hz.ehwqpu.com/gtudsabakl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xinyue.icu/gtckfykujl.html

[T03] Kotlin：字符串模板
来源：http://hz.yuxming.cn/gtcepditft.html

"值: $b"
来源：http://hz.guannengcc.top/gtysghxhuq.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtjyuyngkm.html

val n: String? = null;  n?.length
来源：http://hz.jqgfzy.top/gtfyrldsbz.html

[T05] Kotlin：when 表达式
来源：http://hz.sysykeji.top/gtcbusmftf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jyoumei.cn/gtndssjrxw.html

[T06] Kotlin：集合映射
来源：http://hz.cashguo.top/gtyfemmukr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtrqcgxqaq.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxuanxn.top/gtniawxopm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtqwzzgvix.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtuaujikns.html

data class User(val name: String, val age: Int)
来源：http://hz.zhiwuduotai.top/gtdfczoxxh.html

[T09] Kotlin：扩展函数
来源：http://hz.zhiwuduotai.top/gtpadzsxoy.html

fun String.exclaim() = this + "!"
来源：http://hz.sweek.top/gtlgnhlxsm.html

[T10] Kotlin：默认参数
来源：http://hz.smart0.xyz/gtxfulcvub.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xingfuxueyuan.xyz/gtoxkgfebu.html

[T11] Kotlin：协程
来源：http://hz.jinqigfzy.top/gtbndgbvkv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtsjkrbype.html

[T12] Kotlin：解构声明
来源：http://hz.wangdashe.top/gtihmbbimf.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgufenzy.top/gtcetqeatm.html

[T13] Kotlin：只读 Map
来源：http://hz.gotoacloud.top/gtiktrkowd.html

val m = mapOf("a" to 1)
来源：http://hz.fzhhl.top/gtqewftyjh.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gtfekwvxdj.html

for (i in 1..10) println(i)
来源：http://hz.chenlongwang.top/gtfywaqtuc.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtajhdrxic.html

interface Shape { fun area(): Double }
来源：http://hz.hongshengwenyu.top/gtjmbepgwc.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtqezurdio.html

print("Hello")
来源：http://hz.xuanzx.com/gtsvhteppi.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtrmzlkubd.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtpuqnoveh.html

[T18] Swift：字符串插值
来源：http://hz.feifeiyinyue.top/gthbsgwsap.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gtscklrhmj.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gtghxmmfho.html

if let n = opt { print(n) }
来源：http://hz.yuanzhike.top/gtguujulhu.html

[T20] Swift：数组操作
来源：http://hz.zhixingplan.top/gtbsmcawtv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuetiantiany.cn/gtveqdamgf.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtrmseyhse.html

for x in a { print(x) }
来源：http://hz.mhx1999.top/gthtksqqjh.html

[T22] Swift：字典
来源：http://hz.ehwqpu.com/gtaubzqrlf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtdxlvotan.html

[T23] Swift：函数
来源：http://hz.yueranfly.top/gtdugkelew.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtcpxzywxv.html

[T24] Swift：闭包
来源：http://hz.ivvv.top/gtppancjqp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tanke756.top/gtkphrezjv.html

[T25] Swift：结构体
来源：http://hz.havefunace.top/gtbjjkuezr.html

struct P { var x: Int }
来源：http://hz.mhx1999.top/gttjhctrju.html

[T26] Swift：类与重写
来源：http://hz.yuxming.cn/gtdagecnbu.html

class A: Base { override func f() {} }
来源：http://hz.jinyuanbaomall.cn/gtcbgadbcv.html

[T27] Swift：错误处理
来源：http://hz.feifeiyinyue.top/gtrhthghtz.html

do { try f() } catch { print(error) }
来源：http://hz.nanxinkj.top/gtlnzufxxo.html

[T28] Swift：枚举
来源：http://hz.tianlin.xyz/gtaeelmkvk.html

enum Color { case red, green }
来源：http://hz.cashguo.top/gtoqmfdeaf.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtclqkxnms.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gtqrfaghei.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gttecijisz.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtbpfinptv.html

[T31] Lua：Hello World
来源：http://hz.hammf.cn/gtdlovfrbv.html

print("Hello")
来源：http://hz.gzhubu.top/gtzppmlxcm.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gtfejyiyog.html

local a = 1
来源：http://hz.shangyingyoupin.top/gtvmwsauhf.html

[T33] Lua：表（数组）
来源：http://hz.havefunace.top/gtypwdgdrz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.mhx1999.top/gtevcjnrmv.html

[T34] Lua：遍历表
来源：http://hz.jqgufenzy.top/gtfpcdfsrw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gttobkfzat.html

[T35] Lua：字典表
来源：http://hz.jyoumei.cn/gtmztufqqx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtggjodmkd.html

[T36] Lua：函数
来源：http://hz.gzhubu.top/gtfcibdxil.html

function add(a, b) return a + b end
来源：http://hz.yonumen.top/gtvclgqqqo.html

[T37] Lua：字符串拼接
来源：http://hz.xuetiantiany.cn/gtzffzpxyn.html

"a" .. "b"
来源：http://hz.316326.xyz/gtmeoegtaf.html

[T38] Lua：条件
来源：http://hz.pycfn.com/gtdymbkyhf.html

if x > 0 then print("正") end
来源：http://hz.gogol.net.cn/gtamcsjeoe.html

[T39] Lua：模式匹配
来源：http://hz.gaohongyu789.top/gtufnsdpbq.html

string.find(s, "%d+")
来源：http://hz.yueranfly.top/gtjtbgbuwc.html

[T40] Lua：元表
来源：http://hz.tian-w.cn/gtazupbysa.html

setmetatable({}, { __index = base })
来源：http://hz.hfpthk.cn/gtnqwpvhib.html

[T41] Perl：Hello World
来源：http://hz.gaohongyu789.top/gtfzrexacs.html

print "Hello\n";
来源：http://hz.daxiang520.top/gtxnhcmkps.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gthxyjxhvg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuanzx.com/gttuworeex.html

[T43] Perl：字符串插值
来源：http://hz.jiagoushi.top/gtowrtzuqs.html

"值: $a"
来源：http://hz.yanxiufei.cn/gtfabephtt.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtdcblnpup.html

if ($a > 0) { print "正"; }
来源：http://hz.ybcxt.top/gtvalqbucf.html

[T45] Perl：数组遍历
来源：http://hz.xuetiantiany.cn/gtdjhbbnen.html

for my $x (@arr) { print $x; }
来源：http://hz.tianlin.xyz/gtihyozmbz.html

[T46] Perl：哈希操作
来源：http://hz.ydzc1.top/gtsqnosvym.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtrahkavtr.html

[T47] Perl：正则捕获
来源：http://hz.cqqwz.cn/gtlhsaajjp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yvedp.cn/gtffvfawiq.html

[T48] Perl：正则替换
来源：http://hz.ydjk.org.cn/gteoxtftfc.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtnykauypb.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gtjgytfeuj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.9152youxi.cn/gteascspnr.html

[T50] Perl：逐行读文件
来源：http://hz.gzhubu.top/gtngekczod.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gtobzyuecb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aibaodan.cn/gtoxeuelao.html

[T51] Scala：Hello World
来源：http://hz.shzxlz.cn/gtglekaxod.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtwtikvlqg.html

[T52] Scala：变量
来源：http://hz.yueranfly.top/gtwiglhvyt.html

val a = 1;  var b = 2
来源：http://hz.cqqwz.cn/gtegnpfrvx.html

[T53] Scala：字符串插值
来源：http://hz.c1oappe.top/gtbdkpport.html

s"值: $b"
来源：http://hz.havefunace.top/gthdmlkrot.html

[T54] Scala：集合映射
来源：http://hz.jqgfzy.top/gtazkndnql.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aibaodan.cn/gtjnirkawp.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gtlwvljuuq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yanxiufei.cn/gtelelvrkd.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtelpijmgr.html

case class User(name: String, age: Int)
来源：http://hz.pycfn.com/gtdfjrkbqq.html

[T57] Scala：模式匹配
来源：http://hz.yonumen.top/gtgdixhzln.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guowangkeji.top/gtktmdmhdj.html

[T58] Scala：函数定义
来源：http://hz.shuidangran.top/gtmfylxzuv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tian-w.cn/gtqoshzsto.html

[T59] Scala：循环
来源：http://hz.shanyushiyangtech.top/gtrszdroxj.html

for (i <- 1 to 10) println(i)
来源：http://hz.hywenlv.cn/gtwtvjoery.html

[T60] Scala：折叠
来源：http://hz.yj20258888.top/gtybtykyow.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhiwuduotai.top/gteaenkekv.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtbtonhrot.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtyyrpoukw.html

================================================================================
来源：http://hz.shzxlz.cn/gtnmfiyqyw.html

[U01] Py：创建虚拟环境
来源：http://hz.jinghuilouyu.cn/gtjddwehzy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gttwbzazae.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hongshengwenyu.top/gtdzfyctgj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.snrcjt.cn/gtihjuzbas.html

[U03] Py：加载 .env 配置
来源：http://hz.cucudq.cn/gtrksqmlcb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.0kj1m.cn/gtfltvfnob.html

[U04] Py：变量调试打印
来源：http://hz.ybcxt.top/gthnmlnmnl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sysykeji.top/gtkvattvar.html

[U05] Py：列表去重且保序
来源：http://hz.dianchejie.cn/gtemgmsqwl.html

list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtkonxluba.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtdcxpalfn.html

{**a, **b}
来源：http://hz.tanke756.top/gtgbabqema.html

[U07] Py：反转字典键值
来源：http://hz.yangfankeji.com/gtglrtwxlj.html

{v: k for k, v in d.items()}
来源：http://hz.zycfv.cn/gttzeifilb.html

[U08] Py：展平二维列表
来源：http://hz.guannengcc.top/gtwywpgwqa.html

[y for x in nested for y in x]
来源：http://hz.dianchejie.cn/gtsnlnoahr.html

[U09] Py：字典取最大值的键
来源：http://hz.yj202588.top/gtmlgqyhjy.html

max(d, key=d.get)
来源：http://hz.kuanghao11.cn/gtlvwetpan.html

[U10] Py：按值排序字典
来源：http://hz.fengsongda.top/gtupfeajqp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ydzc1.top/gtdffvejpi.html

[U11] Py：生成器表达式
来源：http://hz.pycfn.com/gteccrlspk.html

(x * 2 for x in arr)
来源：http://hz.yonumen.top/gthwszxdyd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxuanxn.top/gtuouyqlir.html

Counter(arr).most_common(3)
来源：http://hz.vqdsnc.cn/gtfgjgxpyp.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtszvhftmr.html

deque(maxlen=10)
来源：http://hz.gotoacloud.top/gtkmmnjwpy.html

[U14] Py：分组收集到列表
来源：http://hz.9152youxi.cn/gthwdxjjbo.html

defaultdict(list)
来源：http://hz.shuidangran.top/gthnkvbsxt.html

[U15] Py：高精度计时
来源：http://hz.yj20258888.top/gtmpnpwxti.html

t = time.perf_counter()
来源：http://hz.ydzc1.top/gtlhtwaaqy.html

[U16] Py：命令行参数解析
来源：http://hz.gaohongyu789.top/gtxobuhwnt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yonumen.top/gtzvdgpkyl.html


<!-- 参考信息 -->