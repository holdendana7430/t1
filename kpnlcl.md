代发 wailian999

split -l 1000 big.log part_
来源：http://hz.iojbl.cn/gtmcfeajhd.html

[R74] 批量重命名
来源：http://hz.hfpthk.cn/gtfavsbrxr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenzaomai.com/gtogkvmcmq.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtsgqewqhw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtyjklyjbu.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtddedqikd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuanzhike.top/gtqzrkmopf.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gttndkjhdo.html

read -rp "请输入: " ans
来源：http://hz.xziqi.cn/gttflxzvse.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtthcyhste.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhaomingkeji.xyz/gtdnzoiaus.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtyjakskws.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtvcedjivg.html

[R80] 查看脚本执行耗时
来源：http://hz.ivvv.top/gtfaquxjzn.html

time ./run.sh
来源：http://hz.wangdashe.top/gtzsckyhfl.html

================================================================================
来源：http://hz.yj202588.top/gtvsahnwra.html

S. C / C++ 专题
来源：http://hz.birdmap.top/gtdoatardi.html

================================================================================
来源：http://hz.gotoacloud.top/gtwhygblqa.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gthlxkdxmf.html

#include <stdio.h>
来源：http://hz.ivvv.top/gtqsxdbcvw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gttqnchgsv.html

[S02] C：变量与格式化输出
来源：http://hz.yj202588.top/gtqckkyzhn.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinyuanbaomall.cn/gtflxerdzq.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtvclorlvn.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gtizviqwvm.html

[S04] C：字符串复制
来源：http://hz.quarkkingdee.top/gtsatrmzio.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtwcyyczxi.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtyuywjrfx.html

strlen(s)
来源：http://hz.daxiang520.top/gttmwhpmwc.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtwfwfbuoy.html

strcmp(a, b) == 0
来源：http://hz.yuxming.cn/gtwreetspc.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtdtoyewpc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtcljofqsq.html

[S08] C：动态内存分配与释放
来源：http://hz.zhixingplan.top/gtabzrlmio.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jyoumei.cn/gtnzbsqbcp.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtsnhxgams.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtdfrjlibq.html

[S10] C：指针与解引用
来源：http://hz.mhx1999.top/gtexdaysya.html

int *p = &a;  *p = 5;
来源：http://hz.ydjk.org.cn/gtqqcoqizo.html

[S11] C：逐行读文件
来源：http://hz.yueranfly.top/gthlhalfup.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guannengcc.top/gtbnbdwarl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258.top/gtnximtiqw.html

fclose(f);
来源：http://hz.hammf.cn/gtjfofivii.html

[S12] C：写文件
来源：http://hz.sysykeji.top/gtispucqjw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cqqwz.cn/gtllqzysqu.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gthuwcfngs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtsixanzxe.html

[S14] C：枚举
来源：http://hz.cdnleiting.top/gtxqdsdwod.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtctwdzwez.html

[S15] C：类型转换
来源：http://hz.cqqwz.cn/gtnnmieqdw.html

(double) a / b
来源：http://hz.cqqwz.cn/gtwpfwbosu.html

[S16] C：位操作置位
来源：http://hz.dianchejie.cn/gtliabbwmg.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gttppvnurq.html

[S17] C：安全拼接字符串
来源：http://hz.snrcjt.cn/gttqjtoilx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shangyingyoupin.top/gtnspefdqo.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gthseybgnr.html

int main(int argc, char **argv)
来源：http://hz.gaohongyu789.top/gtmugjihcy.html

[S19] C：快速排序
来源：http://hz.gzhubu.top/gtgqpdqxei.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtjxtewsgr.html

[S20] C：二分查找
来源：http://hz.redwolf501.top/gtsmaiczrx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtscslctsy.html

[S21] C：字符类别判断
来源：http://hz.daxiang520.top/gtjyaigoia.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.redwolf501.top/gtzywijttm.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gttdpqhmmz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gtytvpnleo.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtmxhtkhgs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.0kj1m.cn/gtafslrgns.html

[S24] C：获取本地时间
来源：http://hz.9152youxi.cn/gtemzhodlj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtvqdvuatt.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtxcmekmou.html

memcpy(dst, src, n);
来源：http://hz.sufxvd.cn/gtknhufmkv.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gthjwfgpay.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtnhrristn.html

[S27] C：定义常量
来源：http://hz.tanke756.top/gtzetjgyax.html

const double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtrilorwif.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtlxagvari.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtaohgewqo.html

[S29] C：变参函数
来源：http://hz.xuetiantiany.cn/gtoeoiozyf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.quarkkingdee.top/gtizcgjgxh.html

[S30] C：头文件保护
来源：http://hz.aibaodan.cn/gtiqahagro.html

#ifndef X_H
来源：http://hz.xinyue.icu/gtviiwquwu.html

#define X_H
来源：http://hz.feifeiyinyue.top/gtibaznwvn.html

#endif
来源：http://hz.zhongyouzk.top/gtzeunrgim.html

[S31] C++：Hello World
来源：http://hz.gotoacloud.top/gtsfqqhgaf.html

#include <iostream>
来源：http://hz.jinghuilouyu.cn/gtrjvnhgou.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydjk.org.cn/gtifieusgh.html

[S32] C++：字符串
来源：http://hz.zhoulong.xyz/gtaeeoeixk.html

std::string s = "hi";  s += "!";
来源：http://hz.hysaishi.cn/gtyjokqodx.html

[S33] C++：vector 增删
来源：http://hz.fzhhl.top/gtxnbeiiba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgufenzy.top/gtybexvuup.html

[S34] C++：遍历 vector
来源：http://hz.haohaochexian.top/gtvxzqgvpt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sufxvd.cn/gtgvlqqnwk.html

[S35] C++：map
来源：http://hz.svipenyu.cn/gtigeddfiy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gtpuhhaanw.html

[S36] C++：unordered_map
来源：http://hz.jqgfzy.top/gtzpreolia.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtniuahwdb.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtdoqllomo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gthbplwrsq.html

[S38] C++：排序
来源：http://hz.birdmap.top/gtkvkezrqt.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtucmkmigu.html

[S39] C++：自定义比较器排序
来源：http://hz.tian-w.cn/gtsbohkfgs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gtoolffyou.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangkeji.top/gtozzpyieg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hysaishi.cn/gtosnlkfxc.html

[S41] C++：类与构造函数
来源：http://hz.sysykeji.top/gtsbugtwhf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cqqwz.cn/gtbvphieve.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258.top/gtkxmlztqw.html

class B : public Base { public: void f() override {} };
来源：http://hz.xylfe.cn/gtjkavsora.html

[S43] C++：智能指针
来源：http://hz.andypj.xyz/gtkddhxlvt.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gttvoaiynl.html

[S44] C++：引用传参
来源：http://hz.zhoulong.xyz/gtknwhdwrx.html

void inc(int &x) { ++x; }
来源：http://hz.chenjidiqi.icu/gtkdwfqije.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gtubbpsxcg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhixingplan.top/gtithffkup.html

[S46] C++：函数模板
来源：http://hz.ppjwa.cn/gtqzlctguj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangshuangyany.cn/gthfubmwfs.html

[S47] C++：结构化绑定遍历
来源：http://hz.316326.xyz/gtazzkmiys.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtpntnqyaw.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gttcygsjmo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtfdwqfuey.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtniptszrf.html

[S49] C++：写文件
来源：http://hz.iojbl.cn/gtiedwujjw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.havefunace.top/gtdqewvggb.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gtgxpfkeev.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtjenoksng.html

[S51] C++：显式类型转换
来源：http://hz.cheryme.top/gtzyvvroty.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtafabgjsx.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gttfcmsriw.html

int size() const noexcept { return n_; }
来源：http://hz.yongpay.top/gtfhqhwwnc.html

[S53] C++：移动语义
来源：http://hz.shuidangran.top/gtnhgwprgo.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtcyocxqnl.html

[S54] C++：异常处理
来源：http://hz.hfpthk.cn/gtaadeafjg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gtsbrnmgue.html

[S55] C++：结构化绑定
来源：http://hz.daria6918.cn/gtichkxsyu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gtffmbvlki.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gtxmsajozz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.c1oappe.top/gtifkwkscm.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtvnyjosbk.html

constexpr int N = 10;
来源：http://hz.zhongyouzk.top/gtkipqllco.html

[S58] C++：命名空间
来源：http://hz.316326.xyz/gteitabnse.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtkfrwcheo.html

[S59] C++：静态断言
来源：http://hz.jqgufenzy.top/gtebfdzaqe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtuvwobjht.html

[S60] C++：遍历并删除元素
来源：http://hz.haohaochexian.top/gtsgnfmhjs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jyoumei.cn/gtmbdqngzd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxzwfqtmc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gtpyqhxhuo.html

================================================================================
来源：http://hz.aizwys.cn/gtjzgstdgl.html

[T01] Kotlin：Hello World
来源：http://hz.zhijiandao.cn/gtpuixxzpr.html

println("Hello")
来源：http://hz.52xcode.cn/gtolntvtgj.html

[T02] Kotlin：变量
来源：http://hz.hywenlv.cn/gtdwfqfqri.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yuanzhike.top/gtuvptofsc.html

[T03] Kotlin：字符串模板
来源：http://hz.cheryme.top/gtwxtcurhd.html

"值: $b"
来源：http://hz.quarkkingdee.top/gtnncceajm.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtihzoixhe.html

val n: String? = null;  n?.length
来源：http://hz.pycfn.com/gtejuvpzrj.html

[T05] Kotlin：when 表达式
来源：http://hz.zhengqikj.top/gtqzqtjiav.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtmdscuenq.html

[T06] Kotlin：集合映射
来源：http://hz.zhaomingkeji.xyz/gtgabzgznx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinyuanbaomall.cn/gthzsjhtlr.html

[T07] Kotlin：集合过滤
来源：http://hz.ydjk.org.cn/gtfcvmovbj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.smart0.xyz/gtvbohjmkg.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtddnhmqjq.html

data class User(val name: String, val age: Int)
来源：http://hz.jlsjyb.cn/gtbrgcwyjh.html

[T09] Kotlin：扩展函数
来源：http://hz.zhengqikj.top/gtmsymkehu.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtgvitpbtw.html

[T10] Kotlin：默认参数
来源：http://hz.yonumen.top/gtirqxgurp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxinkj.top/gtrzdkgdtd.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtdjvyglxx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ehwqpu.com/gtfuupbqte.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtjomygarj.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gtsgcqfrbd.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigfzy.top/gtzxhuwjpg.html

val m = mapOf("a" to 1)
来源：http://hz.pycfn.com/gtxbtgmkpi.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtbcdhjumk.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangtech.top/gtsifqfkkz.html

[T15] Kotlin：接口
来源：http://hz.nwbrower.top/gtrcvnskbl.html

interface Shape { fun area(): Double }
来源：http://hz.fzhhl.top/gtebzmivyz.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtgecfmgem.html

print("Hello")
来源：http://hz.aizwys.cn/gtaplvpawf.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gtaipxwnye.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtdujmexth.html

[T18] Swift：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtjitndlqh.html

"值: \(b)"
来源：http://hz.ehwqpu.com/gtbznelcxq.html

[T19] Swift：可选绑定
来源：http://hz.jinqigufen.top/gtyrpieilm.html

if let n = opt { print(n) }
来源：http://hz.cqqwz.cn/gtowtvezxb.html

[T20] Swift：数组操作
来源：http://hz.dianchejie.cn/gtqbrouhmy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhoulong.xyz/gtdcoplxnb.html

[T21] Swift：遍历
来源：http://hz.sxryk.cn/gtcoxxyjch.html

for x in a { print(x) }
来源：http://hz.wangshuangyany.cn/gtdbylkhas.html

[T22] Swift：字典
来源：http://hz.jlsjyb.cn/gtwiinwfcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj20258.top/gtsqojgkec.html

[T23] Swift：函数
来源：http://hz.fzhhl.top/gttitzasos.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtxjwvstue.html

[T24] Swift：闭包
来源：http://hz.xuetiantiany.cn/gtqcgnuvti.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.9152youxi.cn/gtlytvsnqa.html

[T25] Swift：结构体
来源：http://hz.yj202588.top/gtwixckikz.html

struct P { var x: Int }
来源：http://hz.sxryk.cn/gtcmeqddzx.html

[T26] Swift：类与重写
来源：http://hz.hongshengwenyu.top/gtgjttddkq.html

class A: Base { override func f() {} }
来源：http://hz.yueranfly.top/gtlhahlzsr.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtjxdznhfa.html

do { try f() } catch { print(error) }
来源：http://hz.yj202588.top/gtuyenfrgo.html

[T28] Swift：枚举
来源：http://hz.aibaodan.cn/gtedngdded.html

enum Color { case red, green }
来源：http://hz.yuanzhike.top/gtxncqpdyn.html

[T29] Swift：guard 提前返回
来源：http://hz.nwbrower.top/gtgiepeqta.html

guard let x = opt else { return }
来源：http://hz.nanxuanxn.top/gtpsbusucs.html

[T30] Swift：协议
来源：http://hz.zhoulong.xyz/gtbkgraton.html

protocol Shape { func area() -> Double }
来源：http://hz.svipenyu.cn/gtrepdnxlo.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtoghnfxwx.html

print("Hello")
来源：http://hz.xylfe.cn/gtwfzgzaph.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangtech.top/gttzdrifdx.html

local a = 1
来源：http://hz.316326.xyz/gtxyukjizz.html

[T33] Lua：表（数组）
来源：http://hz.feifeiyinyue.top/gtvwoqtylf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ehwqpu.com/gtygsdsmzg.html

[T34] Lua：遍历表
来源：http://hz.c1oappe.top/gttqjzjokx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.birdmap.top/gtkyuczuiu.html

[T35] Lua：字典表
来源：http://hz.nanxinkj.top/gtioxadida.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtcrvsegoa.html

[T36] Lua：函数
来源：http://hz.ybcxt.top/gtesgurujq.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtmhxmzkxm.html

[T37] Lua：字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtciahponq.html

"a" .. "b"
来源：http://hz.shangyingyoupin.top/gtsksmipqs.html

[T38] Lua：条件
来源：http://hz.tianlin.xyz/gtxpfsxlql.html

if x > 0 then print("正") end
来源：http://hz.pycfn.com/gtvllpugcl.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtypffqjge.html

string.find(s, "%d+")
来源：http://hz.daria6918.cn/gtjzizncuy.html

[T40] Lua：元表
来源：http://hz.nanxuanxn.top/gterahbbtb.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtqlfrqlge.html

[T41] Perl：Hello World
来源：http://hz.shzxlz.cn/gttbxothsq.html

print "Hello\n";
来源：http://hz.nanxuanxn.top/gtpdenfyoz.html

[T42] Perl：变量类型
来源：http://hz.xylfe.cn/gtswprtfma.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtkdmiaoht.html

[T43] Perl：字符串插值
来源：http://hz.xuetiantiany.cn/gttwyadatc.html

"值: $a"
来源：http://hz.xinyue.icu/gtsigpvmxf.html

[T44] Perl：条件
来源：http://hz.zycfv.cn/gtoudjgjbj.html

if ($a > 0) { print "正"; }
来源：http://hz.aibaodan.cn/gtdlutzard.html

[T45] Perl：数组遍历
来源：http://hz.guowangkeji.top/gtxmaxrtiu.html

for my $x (@arr) { print $x; }
来源：http://hz.ybcxt.top/gtsbjopvlm.html

[T46] Perl：哈希操作
来源：http://hz.jiagoushi.top/gtgwlzmffk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cqqwz.cn/gtuuysokll.html

[T47] Perl：正则捕获
来源：http://hz.havefunace.top/gtzphnvxry.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.tanke756.top/gtbrxfuiey.html

[T48] Perl：正则替换
来源：http://hz.iojbl.cn/gtakqspxdt.html

$s =~ s/old/new/g;
来源：http://hz.meibo888.top/gtgakxgmaa.html

[T49] Perl：函数
来源：http://hz.cheryme.top/gtyikzbdxm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daxiang520.top/gtdsdywyff.html

[T50] Perl：逐行读文件
来源：http://hz.xuetiantiany.cn/gtmxtlhqle.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cdnleiting.top/gtmcegvvcv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xingfuxueyuan.xyz/gtjubrrohh.html

[T51] Scala：Hello World
来源：http://hz.ybcxt.top/gtmxnpbljk.html

println("Hello")
来源：http://hz.xinyue.icu/gtkvwnsbin.html

[T52] Scala：变量
来源：http://hz.yangfankeji.com/gtlakpjsrz.html

val a = 1;  var b = 2
来源：http://hz.aizwys.cn/gtwqairdar.html

[T53] Scala：字符串插值
来源：http://hz.dashuyun.cn/gtcmlubcth.html

s"值: $b"
来源：http://hz.fengsongda.top/gtaerejpug.html

[T54] Scala：集合映射
来源：http://hz.ybcxt.top/gtaemftflv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tanke756.top/gtbelpuafi.html

[T55] Scala：集合过滤
来源：http://hz.meibo888.top/gtifffanqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yvedp.cn/gtgcmnqsof.html

[T56] Scala：样例类
来源：http://hz.jqgufenzy.top/gtfktljwka.html

case class User(name: String, age: Int)
来源：http://hz.zhoulong.xyz/gtgngllgwr.html

[T57] Scala：模式匹配
来源：http://hz.fengsongda.top/gtbqcprztp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhixingplan.top/gtvmihxsbr.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gthxiepvcv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.dianchejie.cn/gtajzygqqz.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtbvsymhcm.html

for (i <- 1 to 10) println(i)
来源：http://hz.cdnleiting.top/gtjqaxunmp.html

[T60] Scala：折叠
来源：http://hz.daria6918.cn/gtcfaahigu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cashguo.top/gtliyigoid.html

================================================================================
来源：http://hz.aizwys.cn/gtypaxgbyr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gteoyzxwvb.html

================================================================================
来源：http://hz.tianlin.xyz/gtvdzglbgu.html

[U01] Py：创建虚拟环境
来源：http://hz.bjfxy.top/gtsvltfmvd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj202588.top/gtdgnhrphp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenzaomai.com/gtpmogrgsc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhengqikj.top/gtzyrwrlmu.html

[U03] Py：加载 .env 配置
来源：http://hz.zhixingplan.top/gtnhdmrwou.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.316326.xyz/gtjuopzxxn.html

[U04] Py：变量调试打印
来源：http://hz.52xcode.cn/gtctrzlbro.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.smart0.xyz/gtfbzgzitx.html

[U05] Py：列表去重且保序
来源：http://hz.nanxuanxn.top/gttjxfrssp.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtdgzrqvqv.html

[U06] Py：合并两个字典
来源：http://hz.cucudq.cn/gtvellkcqp.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtklhnvrjq.html

[U07] Py：反转字典键值
来源：http://hz.gaohongyu789.top/gtonmssqjr.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258888.top/gtrskqzgic.html

[U08] Py：展平二维列表
来源：http://hz.ehwqpu.com/gtlzdghagr.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtkmfgzktc.html

[U09] Py：字典取最大值的键
来源：http://hz.hfpthk.cn/gtnplytyva.html

max(d, key=d.get)
来源：http://hz.havefunace.top/gtfrgtiyyu.html

[U10] Py：按值排序字典
来源：http://hz.yangfankeji.com/gtqeyonhdf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gtlutqpgqk.html

[U11] Py：生成器表达式
来源：http://hz.ivvv.top/gtbsmsongp.html

(x * 2 for x in arr)
来源：http://hz.hongshengwenyu.top/gtwhcrhcfi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tian-w.cn/gthsesmuse.html

Counter(arr).most_common(3)
来源：http://hz.andypj.xyz/gtndqxzcba.html

[U13] Py：固定长度队列
来源：http://hz.jinghuilouyu.cn/gtayxdrynx.html

deque(maxlen=10)
来源：http://hz.ivvv.top/gtvugfsfce.html

[U14] Py：分组收集到列表
来源：http://hz.cqqwz.cn/gtumsitlgj.html

defaultdict(list)
来源：http://hz.daria6918.cn/gtajjfujbt.html


<!-- 参考信息 -->