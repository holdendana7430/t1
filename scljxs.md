代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.wangshuangyany.cn/gtolbwdczy.html

[R70] 时间戳与互转
来源：http://hz.cheryme.top/gtzxkhyxfr.html

date +%s;  date -d @1700000000
来源：http://hz.mhx1999.top/gtvxjsivpn.html

[R71] 日期格式化
来源：http://hz.guannengcc.top/gtopxiugji.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xziqi.cn/gtoiunmpei.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtiffplvaz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtpnyfzfrf.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gturacrwbk.html

split -l 1000 big.log part_
来源：http://hz.havefunace.top/gthznrduqe.html

[R74] 批量重命名
来源：http://hz.aibaodan.cn/gtrrplcfjy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenjidiqi.icu/gtvyxyfqkj.html

[R75] 导出环境变量
来源：http://hz.ybcxt.top/gtcpxvviob.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jlsjyb.cn/gtbhtqsajl.html

[R76] 使用临时文件
来源：http://hz.cucudq.cn/gtsydfawwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtbzvosmbt.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtznlekkbt.html

read -rp "请输入: " ans
来源：http://hz.316326.xyz/gtssyxqklf.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtgfcywzsq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinyuanbaomall.cn/gtcpygeivu.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gttazghzdb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gtdtxdubrf.html

[R80] 查看脚本执行耗时
来源：http://hz.hfpthk.cn/gtdwezgpkk.html

time ./run.sh
来源：http://hz.hysaishi.cn/gtxjffrfer.html

================================================================================
来源：http://hz.pycfn.com/gtzekanrhn.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtdhkwjsua.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnizatabj.html

[S01] C：Hello World
来源：http://hz.c1oappe.top/gtzjlvzkte.html

#include <stdio.h>
来源：http://hz.hongshengwenyu.top/gtwjtjzjug.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sweek.top/gtpvyieknk.html

[S02] C：变量与格式化输出
来源：http://hz.aizwys.cn/gtjradpnnd.html

int a = 10; printf("%d\n", a);
来源：http://hz.xingfuxueyuan.xyz/gtpszshnfe.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gthkxvnfpi.html

int x; scanf("%d", &x);
来源：http://hz.zhengqikj.top/gtbnieqndf.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtorjpzbgy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangdashe.top/gtdihqmxpb.html

[S05] C：字符串长度
来源：http://hz.jlsjyb.cn/gtbkbxuxpd.html

strlen(s)
来源：http://hz.sweek.top/gttjpwfjsb.html

[S06] C：字符串比较
来源：http://hz.9152youxi.cn/gtjuppcpns.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtlygrfmmp.html

[S07] C：数组遍历求和
来源：http://hz.gaohongyu789.top/gtihxypgke.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.9152youxi.cn/gtislmpowc.html

[S08] C：动态内存分配与释放
来源：http://hz.yanxiufei.cn/gtywyrsvmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtwmipsrgv.html

[S09] C：结构体定义与初始化
来源：http://hz.chenjidiqi.icu/gtyvikmlfn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dashuyun.cn/gtgqcsaodr.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtrynqhqgs.html

int *p = &a;  *p = 5;
来源：http://hz.yongpay.top/gtvzppjnsj.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gtcbwkxyhx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guowangkeji.top/gticllilhw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.snrcjt.cn/gtxkgmutwt.html

fclose(f);
来源：http://hz.cucudq.cn/gtmdqtxugm.html

[S12] C：写文件
来源：http://hz.ehwqpu.com/gtdnjhbukb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtsctkhtqd.html

[S13] C：宏定义
来源：http://hz.9152youxi.cn/gtrwoltgcn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gteqpdzkaa.html

[S14] C：枚举
来源：http://hz.zhoulong.xyz/gthlycoooh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gogol.net.cn/gtycokusvi.html

[S15] C：类型转换
来源：http://hz.tanke756.top/gtxvryrztu.html

(double) a / b
来源：http://hz.hnqzz.top/gtndhttosf.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtoghtsjoh.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtggtctuzg.html

[S17] C：安全拼接字符串
来源：http://hz.yongpay.top/gtctuzduwr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gttwjkisnu.html

[S18] C：命令行参数
来源：http://hz.feifeiyinyue.top/gtugtkmfoh.html

int main(int argc, char **argv)
来源：http://hz.xuanzx.com/gtqvjippdo.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gtqeqzbgqi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtnirgcrjx.html

[S20] C：二分查找
来源：http://hz.nanxuanxn.top/gtfcrepqnb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtgzutdvop.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gtkrpuddkm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtyvkqshsf.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtisbiytul.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.andypj.xyz/gtasmiaxfz.html

[S23] C：随机数
来源：http://hz.shzxlz.cn/gtujpcgqds.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.redwolf501.top/gtsxhkzvji.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtmyewiqyj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jyoumei.cn/gtdbeimsxk.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtjhskbeme.html

memcpy(dst, src, n);
来源：http://hz.chenlongwang.top/gtejjpdgoz.html

[S26] C：内存清零
来源：http://hz.jiagoushi.top/gtmuvbrxxh.html

memset(a, 0, sizeof a);
来源：http://hz.hammf.cn/gtwkjcypvx.html

[S27] C：定义常量
来源：http://hz.jianghu66.top/gtethaaxol.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtvgiauqtk.html

[S28] C：静态变量
来源：http://hz.chenlongwang.top/gtxpevezll.html

static int counter = 0;
来源：http://hz.iojbl.cn/gtvpbbyilt.html

[S29] C：变参函数
来源：http://hz.fzhhl.top/gtvdfxkdol.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sufxvd.cn/gtxxzluxmn.html

[S30] C：头文件保护
来源：http://hz.jqgufenzy.top/gtlcvkutti.html

#ifndef X_H
来源：http://hz.ybcxt.top/gtyamovrsc.html

#define X_H
来源：http://hz.gogol.net.cn/gtkleznipf.html

#endif
来源：http://hz.chenlongwang.top/gtjmumibgs.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtzvpoeaeg.html

#include <iostream>
来源：http://hz.yonumen.top/gtfyywmwvv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dianchejie.cn/gtetwxltrg.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtydypkbtz.html

std::string s = "hi";  s += "!";
来源：http://hz.xingfuxueyuan.xyz/gtemdowthn.html

[S33] C++：vector 增删
来源：http://hz.xinyue.icu/gtxeirrrvr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pycfn.com/gtcetteluw.html

[S34] C++：遍历 vector
来源：http://hz.hysaishi.cn/gtuipkpolh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dashuyun.cn/gtvwdskvyy.html

[S35] C++：map
来源：http://hz.mhx1999.top/gtdgsoitjl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtgczqrbyq.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtomgoixah.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtjyzxvvjb.html

[S37] C++：set
来源：http://hz.redwolf501.top/gthcqvskvm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtaotzuvva.html

[S38] C++：排序
来源：http://hz.zhixingplan.top/gtiuvskrsr.html

std::sort(v.begin(), v.end());
来源：http://hz.hysaishi.cn/gtdgfulwlj.html

[S39] C++：自定义比较器排序
来源：http://hz.sysykeji.top/gtjvmvaupi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.52xcode.cn/gtxjqimlan.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtatqgcdcp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gtztnnnnbw.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtfdxmjfxr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ppjwa.cn/gthqnbwtyn.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gtabwwluhi.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenzaomai.com/gtacqxedqk.html

[S43] C++：智能指针
来源：http://hz.xingfuxueyuan.xyz/gtpmgrliwo.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gthnlqezvx.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gtpybflcmf.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtneiywhfb.html

[S45] C++：lambda
来源：http://hz.wangdashe.top/gtjhlqyveo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gtnfcctmcq.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gtiiqlnfim.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtmivuunmi.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhiwuduotai.top/gtmwlzimya.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.feifeiyinyue.top/gttgtupfmv.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtjwfhivho.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nwbrower.top/gtqlerwmlu.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtbzrjeoyx.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtqufxadju.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtgrewdvep.html

[S50] C++：格式化数字
来源：http://hz.xingfuxueyuan.xyz/gtxqqqmgbs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gthajbuohe.html

[S51] C++：显式类型转换
来源：http://hz.gzhubu.top/gtcuktohlz.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtgojaqiiq.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtagaicxtk.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gthbixukqp.html

[S53] C++：移动语义
来源：http://hz.0kj1m.cn/gtajwaxsyf.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtajkktjvc.html

[S54] C++：异常处理
来源：http://hz.nanxinkj.top/gtpsvynmaq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhengqikj.top/gtqbowlrqp.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gtfyzgwwgs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fzhhl.top/gthtkrduhu.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtbbvpqibm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aizwys.cn/gtrpykqxvn.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtoqcawezh.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtckcvqmgm.html

[S58] C++：命名空间
来源：http://hz.fengsongda.top/gtzfgfexyi.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgfzy.top/gtzjbynfsp.html

[S59] C++：静态断言
来源：http://hz.jqgfzy.top/gtoyovqrva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aibaodan.cn/gtgctxvgie.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtuddocedk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gthhnkvrdt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtlwvkhezb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtsceibdxw.html

================================================================================
来源：http://hz.andypj.xyz/gtwrvrtvwq.html

[T01] Kotlin：Hello World
来源：http://hz.sysykeji.top/gtzzmtemlv.html

println("Hello")
来源：http://hz.meibo888.top/gtwthfpbji.html

[T02] Kotlin：变量
来源：http://hz.cucudq.cn/gtdenjpdok.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gtkccpjcsk.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gtolgmfrpl.html

"值: $b"
来源：http://hz.guowangkeji.top/gtznjohoja.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gtflepsorm.html

val n: String? = null;  n?.length
来源：http://hz.yanxiufei.cn/gtpgirwbic.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtrgpwshag.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtfldhiuhg.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gtwrewgkfx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtwcfdzoxd.html

[T07] Kotlin：集合过滤
来源：http://hz.yonumen.top/gtbphzsctd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtndvqslam.html

[T08] Kotlin：数据类
来源：http://hz.jqgufenzy.top/gtuivfyfqn.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangkeji.top/gtzrtkxhcf.html

[T09] Kotlin：扩展函数
来源：http://hz.vqdsnc.cn/gtcpgvczok.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gtdtljbkls.html

[T10] Kotlin：默认参数
来源：http://hz.dashuyun.cn/gtxdaplnns.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258.top/gtgoimgppl.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtorlwnvry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxinkj.top/gtlkfueqxw.html

[T12] Kotlin：解构声明
来源：http://hz.yonumen.top/gtzcdczwzh.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtvsouxvkn.html

[T13] Kotlin：只读 Map
来源：http://hz.svipenyu.cn/gtsxxbsxje.html

val m = mapOf("a" to 1)
来源：http://hz.sxryk.cn/gttvqmngwz.html

[T14] Kotlin：循环
来源：http://hz.guannengcc.top/gtaetidmgu.html

for (i in 1..10) println(i)
来源：http://hz.chenlongwang.top/gtzzgyktmh.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gtbjmdmbgq.html

interface Shape { fun area(): Double }
来源：http://hz.jiagoushi.top/gttprmxjie.html

[T16] Swift：Hello World
来源：http://hz.zhengqikj.top/gtsleixiee.html

print("Hello")
来源：http://hz.jlsjyb.cn/gtbbtnxmhy.html

[T17] Swift：变量与常量
来源：http://hz.dianchejie.cn/gtsmmvqven.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtfobkbwma.html

[T18] Swift：字符串插值
来源：http://hz.jyoumei.cn/gttimnaazt.html

"值: \(b)"
来源：http://hz.ydzc1.top/gtozljrwoe.html

[T19] Swift：可选绑定
来源：http://hz.jiagoushi.top/gtchyvzuvr.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtsayifxun.html

[T20] Swift：数组操作
来源：http://hz.redwolf501.top/gtukanzelu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtnfmbtipm.html

[T21] Swift：遍历
来源：http://hz.xylfe.cn/gtheckoddd.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gttttyrszp.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtwzubieny.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hfpthk.cn/gtftsbdgvd.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtattzpsad.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.52xcode.cn/gtglmjhtfl.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gtdpevglps.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtozkgvkys.html

[T25] Swift：结构体
来源：http://hz.zycfv.cn/gtbquopahr.html

struct P { var x: Int }
来源：http://hz.yongpay.top/gtjmytilmy.html

[T26] Swift：类与重写
来源：http://hz.vqdsnc.cn/gtunuurtij.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtovtnxfcx.html

[T27] Swift：错误处理
来源：http://hz.bjfxy.top/gtfbwvyaix.html

do { try f() } catch { print(error) }
来源：http://hz.snrcjt.cn/gthwwccouz.html

[T28] Swift：枚举
来源：http://hz.yueranfly.top/gtuuxqmhpi.html

enum Color { case red, green }
来源：http://hz.yueranfly.top/gtzrrojyih.html

[T29] Swift：guard 提前返回
来源：http://hz.gaohongyu789.top/gtfrjigtpv.html

guard let x = opt else { return }
来源：http://hz.gzhubu.top/gtaaqhkpuc.html

[T30] Swift：协议
来源：http://hz.52xcode.cn/gttesrzhzv.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gtvfxtdavy.html

[T31] Lua：Hello World
来源：http://hz.chenzaomai.com/gthxeyloxv.html

print("Hello")
来源：http://hz.cqqwz.cn/gtwsgfwdyo.html

[T32] Lua：局部变量
来源：http://hz.aibaodan.cn/gtxyppzsal.html

local a = 1
来源：http://hz.zhongyouzk.top/gtkoxoseit.html

[T33] Lua：表（数组）
来源：http://hz.fengsongda.top/gtmlxehvre.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hammf.cn/gtfzuugrvc.html

[T34] Lua：遍历表
来源：http://hz.gzhubu.top/gtwgwzsoff.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jyoumei.cn/gthwysoxlw.html

[T35] Lua：字典表
来源：http://hz.dashuyun.cn/gtcmtbyeoy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangkeji.top/gtvcrpeakm.html

[T36] Lua：函数
来源：http://hz.ydjk.org.cn/gtzwarxqhg.html

function add(a, b) return a + b end
来源：http://hz.9152youxi.cn/gtlxofizfp.html

[T37] Lua：字符串拼接
来源：http://hz.quarkkingdee.top/gtxqrmbhbw.html

"a" .. "b"
来源：http://hz.xuanzx.com/gtublcgntu.html

[T38] Lua：条件
来源：http://hz.ydjk.org.cn/gtpaixkrsz.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtsabkadkl.html

[T39] Lua：模式匹配
来源：http://hz.hnqzz.top/gtpfyvtrof.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtgtlpzril.html

[T40] Lua：元表
来源：http://hz.shangyingyoupin.top/gtgnfwfuzm.html

setmetatable({}, { __index = base })
来源：http://hz.9152youxi.cn/gtpknssvhh.html

[T41] Perl：Hello World
来源：http://hz.ydjk.org.cn/gtahyewcyq.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gtutaztzxn.html

[T42] Perl：变量类型
来源：http://hz.zhixingplan.top/gtdlyjvikh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.smart0.xyz/gtekfenlex.html

[T43] Perl：字符串插值
来源：http://hz.jlsjyb.cn/gtexdlzxfq.html

"值: $a"
来源：http://hz.dianchejie.cn/gtztkohzpa.html

[T44] Perl：条件
来源：http://hz.feifeiyinyue.top/gtukejpczt.html

if ($a > 0) { print "正"; }
来源：http://hz.c1oappe.top/gtiujaibsq.html

[T45] Perl：数组遍历
来源：http://hz.zhengqikj.top/gtapwpumtk.html

for my $x (@arr) { print $x; }
来源：http://hz.sweek.top/gttbygfarp.html

[T46] Perl：哈希操作
来源：http://hz.hywenlv.cn/gtvhlgqfmr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yonumen.top/gthkcoebbj.html

[T47] Perl：正则捕获
来源：http://hz.aizwys.cn/gtswlcjbcw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.havefunace.top/gteqbtyezd.html

[T48] Perl：正则替换
来源：http://hz.hnqzz.top/gtwipphykc.html

$s =~ s/old/new/g;
来源：http://hz.xuetiantiany.cn/gtknydjrxv.html

[T49] Perl：函数
来源：http://hz.dianchejie.cn/gtpuvuejfr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sufxvd.cn/gtbsgermvf.html

[T50] Perl：逐行读文件
来源：http://hz.feifeiyinyue.top/gtwbuezjpd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dashuyun.cn/gtejhvrkcv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtdzajviqi.html

[T51] Scala：Hello World
来源：http://hz.ywan-chungtsiang.top/gtnpgqrlxf.html

println("Hello")
来源：http://hz.cucudq.cn/gtzqnftrpx.html

[T52] Scala：变量
来源：http://hz.zhoulong.xyz/gtdghopeop.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangkeji.top/gtykclxtnf.html

[T53] Scala：字符串插值
来源：http://hz.gogol.net.cn/gtxxaamahd.html

s"值: $b"
来源：http://hz.hammf.cn/gtjxejsmxn.html

[T54] Scala：集合映射
来源：http://hz.ywan-chungtsiang.top/gthhulqdsb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenzaomai.com/gtmgaimisi.html

[T55] Scala：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtqghuvglj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gogol.net.cn/gttbifsjxn.html

[T56] Scala：样例类
来源：http://hz.havefunace.top/gtueandydz.html

case class User(name: String, age: Int)
来源：http://hz.chenzaomai.com/gtuiugwdgi.html

[T57] Scala：模式匹配
来源：http://hz.cdnleiting.top/gtnocvdtnf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guowangkeji.top/gtkcgyrqye.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gtprinavqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtisvxkopj.html

[T59] Scala：循环
来源：http://hz.xinyue.icu/gtutrnhhzk.html

for (i <- 1 to 10) println(i)
来源：http://hz.sufxvd.cn/gthtrjjall.html

[T60] Scala：折叠
来源：http://hz.xinyue.icu/gtlbwwdqgh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydzc1.top/gtmzlthvsc.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxlmrmfyv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtltrrqbow.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvmdsnnud.html

[U01] Py：创建虚拟环境
来源：http://hz.xziqi.cn/gtircfivrs.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hfpthk.cn/gtisneisud.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dashuyun.cn/gtoenlbiev.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtwsczlbuk.html

[U03] Py：加载 .env 配置
来源：http://hz.vqdsnc.cn/gthnsleuka.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jyoumei.cn/gtnzezprce.html

[U04] Py：变量调试打印
来源：http://hz.cdnleiting.top/gttytupvtj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cashguo.top/gtucmrbhkn.html

[U05] Py：列表去重且保序
来源：http://hz.guannengcc.top/gtqjrpcjrr.html

list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtwgcvoqwn.html

[U06] Py：合并两个字典
来源：http://hz.yanxiufei.cn/gtzcrwcbya.html

{**a, **b}
来源：http://hz.316326.xyz/gtvbcofize.html

[U07] Py：反转字典键值
来源：http://hz.tanke756.top/gtfaxyzibc.html

{v: k for k, v in d.items()}
来源：http://hz.xziqi.cn/gtajwnpkzz.html

[U08] Py：展平二维列表
来源：http://hz.birdmap.top/gtsxeirspa.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtuxybwtzo.html

[U09] Py：字典取最大值的键
来源：http://hz.hnxiangtu.top/gtjofxuqki.html

max(d, key=d.get)
来源：http://hz.xingfuxueyuan.xyz/gtqlcatopo.html

[U10] Py：按值排序字典
来源：http://hz.c1oappe.top/gtlnovxaar.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinghuilouyu.cn/gtezomlfmc.html


<!-- 参考信息 -->