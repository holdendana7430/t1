代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtqbdvppsp.html

[R72] 等待端口就绪
来源：http://hz.shzxlz.cn/gtjeuypwyh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhengqikj.top/gtrwldjaza.html

[R73] 分割大日志
来源：http://hz.mhx1999.top/gtxypyypve.html

split -l 1000 big.log part_
来源：http://hz.haohaochexian.top/gtavyfmqfk.html

[R74] 批量重命名
来源：http://hz.daxiang520.top/gtfgflvyww.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtsulvagjz.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtksiavmrj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xinyue.icu/gtabqohfqi.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtkqmixklx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtptwjexgy.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtfqlcbsht.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtbxxxanbw.html

[R78] 交互式菜单
来源：http://hz.iojbl.cn/gtskeuexgt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtrzoieyrd.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gtidqonpns.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtozgyemgr.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gtrrekrnma.html

time ./run.sh
来源：http://hz.redwolf501.top/gtvzrmskqr.html

================================================================================
来源：http://hz.hnqzz.top/gtqazxuldv.html

S. C / C++ 专题
来源：http://hz.ehwqpu.com/gtxmvufabo.html

================================================================================
来源：http://hz.dianchejie.cn/gtarmifnjp.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gtvztsngov.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtqmfcnvei.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangtech.top/gtvvgbukob.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtwovtpuvu.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gthgcosfez.html

[S03] C：读入整数
来源：http://hz.cashguo.top/gtexfgsfup.html

int x; scanf("%d", &x);
来源：http://hz.gaohongyu789.top/gtkiysoyrq.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtyhadwhiz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtkdblajzk.html

[S05] C：字符串长度
来源：http://hz.gogol.net.cn/gtqtapvpdw.html

strlen(s)
来源：http://hz.nanxinkj.top/gtwxblqccg.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gtlltavgyj.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gtfdtckwup.html

[S07] C：数组遍历求和
来源：http://hz.jinqigufen.top/gtnohublib.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtllphgzce.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtqkvblzdg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtngxvptwa.html

[S09] C：结构体定义与初始化
来源：http://hz.ivvv.top/gtldowoopg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtzuxupdrg.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gttgcnshos.html

int *p = &a;  *p = 5;
来源：http://hz.meibo888.top/gtwfzwcamw.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtzgjhxqhf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ivvv.top/gtgfuhrixd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnqzz.top/gteghvoxsf.html

fclose(f);
来源：http://hz.jlsjyb.cn/gtrgbkfnzm.html

[S12] C：写文件
来源：http://hz.hammf.cn/gtlgankygg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ybcxt.top/gtefcgnfzb.html

[S13] C：宏定义
来源：http://hz.xuetiantiany.cn/gtmfaflxpf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtxpsjjora.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtqnbwudhm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhoulong.xyz/gtwuoistrw.html

[S15] C：类型转换
来源：http://hz.snrcjt.cn/gtgkupemdy.html

(double) a / b
来源：http://hz.cdnleiting.top/gticeuhzof.html

[S16] C：位操作置位
来源：http://hz.yangfankeji.com/gtzksucttr.html

x |= (1 << 3);
来源：http://hz.iojbl.cn/gtguikuswl.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtcbacmxmc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenjidiqi.icu/gtmebcfgqt.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtynxaqwnz.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtqfnycveo.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtkotoorue.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtkcupjrja.html

[S20] C：二分查找
来源：http://hz.hongshengwenyu.top/gtjlbxxrwl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtzmipdxrh.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtfucjsoyo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jiagoushi.top/gtdemzwjoh.html

[S22] C：字符串转数字
来源：http://hz.tian-w.cn/gtlusrqxkz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtkmzelzkp.html

[S23] C：随机数
来源：http://hz.hnxiangtu.top/gtfoxtvnkt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtcccllzoh.html

[S24] C：获取本地时间
来源：http://hz.jinqigufen.top/gtiordtknc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gtugygwing.html

[S25] C：内存拷贝
来源：http://hz.daria6918.cn/gtbsytmtwp.html

memcpy(dst, src, n);
来源：http://hz.yueranfly.top/gthukljimk.html

[S26] C：内存清零
来源：http://hz.tian-w.cn/gtsdhxdbae.html

memset(a, 0, sizeof a);
来源：http://hz.svipenyu.cn/gtxxgjlhnw.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtmbfadnvu.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtokejvarv.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtlbfkeibf.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtxaxvnpjc.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtffcafsia.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtkyiywwpi.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtzhmwabfm.html

#ifndef X_H
来源：http://hz.dianchejie.cn/gtgmjafavk.html

#define X_H
来源：http://hz.cashguo.top/gtjoukmgqz.html

#endif
来源：http://hz.meibo888.top/gtykbzcxlf.html

[S31] C++：Hello World
来源：http://hz.52xcode.cn/gtacqhhjid.html

#include <iostream>
来源：http://hz.cdnleiting.top/gtugowwrym.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shangyingyoupin.top/gtpuesccto.html

[S32] C++：字符串
来源：http://hz.svipenyu.cn/gtefgicwnz.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtvbxgkisp.html

[S33] C++：vector 增删
来源：http://hz.xziqi.cn/gtchnxqmip.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj202588.top/gtxxilksyt.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gtxmxfgrdb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.havefunace.top/gtjulnossq.html

[S35] C++：map
来源：http://hz.xuetiantiany.cn/gtbdvbmhns.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtzaqbfwll.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtskzgiraw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhengqikj.top/gtrihgyafq.html

[S37] C++：set
来源：http://hz.ybcxt.top/gtknekfzag.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shangyingyoupin.top/gtbxvqtyla.html

[S38] C++：排序
来源：http://hz.nwbrower.top/gttpqehwug.html

std::sort(v.begin(), v.end());
来源：http://hz.redwolf501.top/gthtdalwrn.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtfxbuodfr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigfzy.top/gtazldrjxp.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtwyntepkk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guannengcc.top/gtxomydfus.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtusyfowgh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gtqywcxyly.html

[S42] C++：继承与虚函数
来源：http://hz.cqqwz.cn/gtzsaeaqsr.html

class B : public Base { public: void f() override {} };
来源：http://hz.zycfv.cn/gtykqepfxg.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gttlgrstap.html

auto p = std::make_unique<int>(5);
来源：http://hz.fzhhl.top/gtmskefvhz.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtmjhkuoou.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigufen.top/gtlfvhggzz.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtpcwsvdso.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtawstgwpk.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtksjfdedw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guannengcc.top/gtadmikjvx.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtvtrikfve.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtkidivkfp.html

[S48] C++：逐行读文件
来源：http://hz.andypj.xyz/gtgqizbfhd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtpjtypkkw.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtovxnjbpv.html

[S49] C++：写文件
来源：http://hz.birdmap.top/gtygvwfopf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xinyue.icu/gtqlgqgwwt.html

[S50] C++：格式化数字
来源：http://hz.chenjidiqi.icu/gtqtyrvweo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nwbrower.top/gtveximzxj.html

[S51] C++：显式类型转换
来源：http://hz.birdmap.top/gtpgyjudxk.html

static_cast<double>(a) / b
来源：http://hz.andypj.xyz/gtvbgrkkrl.html

[S52] C++：const 与 noexcept
来源：http://hz.fzhhl.top/gtaglxmeuf.html

int size() const noexcept { return n_; }
来源：http://hz.aizwys.cn/gtyxycbyay.html

[S53] C++：移动语义
来源：http://hz.zhongyouzk.top/gtyzhemkfh.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gticiaahgw.html

[S54] C++：异常处理
来源：http://hz.cucudq.cn/gttmuhoawo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zycfv.cn/gtupbxlpjp.html

[S55] C++：结构化绑定
来源：http://hz.svipenyu.cn/gtktzuslhg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nwbrower.top/gtiexzwval.html

[S56] C++：optional
来源：http://hz.zhoulong.xyz/gtuwklncvj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xingfuxueyuan.xyz/gtvahgcvzm.html

[S57] C++：编译期常量
来源：http://hz.ybcxt.top/gtkgprjdlh.html

constexpr int N = 10;
来源：http://hz.hnqzz.top/gtlyamzkad.html

[S58] C++：命名空间
来源：http://hz.hysaishi.cn/gtayixqyuf.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtpmrknkaf.html

[S59] C++：静态断言
来源：http://hz.shanyushiyangtech.top/gtdwqpfhbm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtydgxbboc.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtqddrxciz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nwbrower.top/gtwateuome.html

================================================================================
来源：http://hz.snrcjt.cn/gtpgnqyjli.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258888.top/gtbstpkcur.html

================================================================================
来源：http://hz.xziqi.cn/gtodvrgqte.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gttfwepeec.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtwgohtmqz.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtlwyicslp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hysaishi.cn/gtfriyolkj.html

[T03] Kotlin：字符串模板
来源：http://hz.quarkkingdee.top/gtljkozuge.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtvdpjfmvn.html

[T04] Kotlin：空安全
来源：http://hz.feifeiyinyue.top/gtewlzqmkn.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtklzzudjr.html

[T05] Kotlin：when 表达式
来源：http://hz.cheryme.top/gtxzoiqmca.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtzmbstogw.html

[T06] Kotlin：集合映射
来源：http://hz.nwbrower.top/gtykwipeuh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guannengcc.top/gtxjnkupza.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtjissnsiz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.redwolf501.top/gtiikzxltp.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtfwpjonxe.html

data class User(val name: String, val age: Int)
来源：http://hz.redwolf501.top/gtjtudgzus.html

[T09] Kotlin：扩展函数
来源：http://hz.chenzaomai.com/gtdnrbjpwo.html

fun String.exclaim() = this + "!"
来源：http://hz.jinyuanbaomall.cn/gtdiechoyz.html

[T10] Kotlin：默认参数
来源：http://hz.hywenlv.cn/gtsfgvnolc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hysaishi.cn/gtyqwbftgp.html

[T11] Kotlin：协程
来源：http://hz.hammf.cn/gticfdtfqc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.feifeiyinyue.top/gtbzpqcavr.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258.top/gteqbafejz.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gtptdmnnjp.html

[T13] Kotlin：只读 Map
来源：http://hz.zdqjudy.top/gtnraaqwqw.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gttbrfmvfb.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gtqbheigit.html

for (i in 1..10) println(i)
来源：http://hz.jianghu66.top/gtclxviefa.html

[T15] Kotlin：接口
来源：http://hz.dashuyun.cn/gtizdaxqib.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtfrsdtqrt.html

[T16] Swift：Hello World
来源：http://hz.sysykeji.top/gtpgkwcjzt.html

print("Hello")
来源：http://hz.smart0.xyz/gtkdwzpqpk.html

[T17] Swift：变量与常量
来源：http://hz.redwolf501.top/gtqqpmdwqc.html

var a = 1;  let b = 2
来源：http://hz.zycfv.cn/gthbhifnun.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gthkvfkpga.html

"值: \(b)"
来源：http://hz.xinyue.icu/gtnyojvwky.html

[T19] Swift：可选绑定
来源：http://hz.316326.xyz/gtgskmygvz.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtejjbyzwt.html

[T20] Swift：数组操作
来源：http://hz.hammf.cn/gtljtcpqbv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gtdglanwwd.html

[T21] Swift：遍历
来源：http://hz.nanxuanxn.top/gtiqrzlakg.html

for x in a { print(x) }
来源：http://hz.sysykeji.top/gtykrgbumu.html

[T22] Swift：字典
来源：http://hz.chenzaomai.com/gtimboedpl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.feifeiyinyue.top/gteehwganw.html

[T23] Swift：函数
来源：http://hz.52xcode.cn/gttirnwhsw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.mhx1999.top/gtoqxzueqw.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gtqnlywwus.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guowangkeji.top/gttedzckdm.html

[T25] Swift：结构体
来源：http://hz.jinghuilouyu.cn/gtfctrnwbv.html

struct P { var x: Int }
来源：http://hz.aizwys.cn/gttpdyivue.html

[T26] Swift：类与重写
来源：http://hz.guowangkeji.top/gtieetrrgz.html

class A: Base { override func f() {} }
来源：http://hz.cdnleiting.top/gtiehlfmoe.html

[T27] Swift：错误处理
来源：http://hz.zycfv.cn/gtknborpnl.html

do { try f() } catch { print(error) }
来源：http://hz.ivvv.top/gttbgumzrz.html

[T28] Swift：枚举
来源：http://hz.cqqwz.cn/gtnkfwigpo.html

enum Color { case red, green }
来源：http://hz.ehwqpu.com/gtsgmgafsx.html

[T29] Swift：guard 提前返回
来源：http://hz.tian-w.cn/gtaacmplpp.html

guard let x = opt else { return }
来源：http://hz.cucudq.cn/gtscbjkjij.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gtjnqairco.html

protocol Shape { func area() -> Double }
来源：http://hz.nwbrower.top/gtnrirqhsi.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtezykvcox.html

print("Hello")
来源：http://hz.jianghu66.top/gtybfioygd.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gtdmlofdpc.html

local a = 1
来源：http://hz.zhengqikj.top/gtfujafgft.html

[T33] Lua：表（数组）
来源：http://hz.chenjidiqi.icu/gtyqeplgfs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuetiantiany.cn/gtjvblhkud.html

[T34] Lua：遍历表
来源：http://hz.shuidangran.top/gtoxqpdjmu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sxryk.cn/gtrcfsifbt.html

[T35] Lua：字典表
来源：http://hz.yueranfly.top/gtqlicmjws.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ydjk.org.cn/gtqycqchal.html

[T36] Lua：函数
来源：http://hz.gogol.net.cn/gtadeqbaez.html

function add(a, b) return a + b end
来源：http://hz.yuxming.cn/gtzscllsmo.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtwptdzffb.html

"a" .. "b"
来源：http://hz.sweek.top/gtwylrzujl.html

[T38] Lua：条件
来源：http://hz.ivvv.top/gtucyekutz.html

if x > 0 then print("正") end
来源：http://hz.hfpthk.cn/gtstebkrdd.html

[T39] Lua：模式匹配
来源：http://hz.bjfxy.top/gtgfggbuzm.html

string.find(s, "%d+")
来源：http://hz.hysaishi.cn/gtoivgituw.html

[T40] Lua：元表
来源：http://hz.9152youxi.cn/gtnekepkxz.html

setmetatable({}, { __index = base })
来源：http://hz.zycfv.cn/gtujsawacw.html

[T41] Perl：Hello World
来源：http://hz.dianchejie.cn/gtgczfbbsi.html

print "Hello\n";
来源：http://hz.kuanghao11.cn/gttnjaeazw.html

[T42] Perl：变量类型
来源：http://hz.redwolf501.top/gtzzvseiul.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yueranfly.top/gteiwqrxiq.html

[T43] Perl：字符串插值
来源：http://hz.havefunace.top/gtxzuxilgh.html

"值: $a"
来源：http://hz.yj20258888.top/gtvswcplkm.html

[T44] Perl：条件
来源：http://hz.zycfv.cn/gthkyxmyhc.html

if ($a > 0) { print "正"; }
来源：http://hz.zhongyouzk.top/gtozseugmu.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtclzqpsps.html

for my $x (@arr) { print $x; }
来源：http://hz.sweek.top/gtkqzjezak.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gtqbisprfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cqqwz.cn/gtmmogdiak.html

[T47] Perl：正则捕获
来源：http://hz.daxiang520.top/gtjeqxycez.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuanzx.com/gtfkvscyoz.html

[T48] Perl：正则替换
来源：http://hz.ivvv.top/gthasmtxmu.html

$s =~ s/old/new/g;
来源：http://hz.sweek.top/gtckbwqzft.html

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtcvzjqrli.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhixingplan.top/gtttnchchp.html

[T50] Perl：逐行读文件
来源：http://hz.yvedp.cn/gtomkjewyt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xinyue.icu/gthdyxsxez.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cqqwz.cn/gtbfmtwvbs.html

[T51] Scala：Hello World
来源：http://hz.hammf.cn/gtpgtzsyta.html

println("Hello")
来源：http://hz.tianlin.xyz/gtevnsueua.html

[T52] Scala：变量
来源：http://hz.gogol.net.cn/gtnkdjlxaz.html

val a = 1;  var b = 2
来源：http://hz.gotoacloud.top/gtdkiehbwf.html

[T53] Scala：字符串插值
来源：http://hz.guowangkeji.top/gtczuwhosn.html

s"值: $b"
来源：http://hz.dashuyun.cn/gtfpdnmvbc.html

[T54] Scala：集合映射
来源：http://hz.tanke756.top/gtnainoejd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258.top/gtsoacknen.html

[T55] Scala：集合过滤
来源：http://hz.ywan-chungtsiang.top/gtirrckvpz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.mhx1999.top/gtxldmtkom.html

[T56] Scala：样例类
来源：http://hz.quarkkingdee.top/gtvjcjlnxc.html

case class User(name: String, age: Int)
来源：http://hz.sufxvd.cn/gtlvnnknqf.html

[T57] Scala：模式匹配
来源：http://hz.yuxming.cn/gtfowyvqsa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hywenlv.cn/gtpcupzujg.html

[T58] Scala：函数定义
来源：http://hz.yongpay.top/gtmrlofbat.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.9152youxi.cn/gththekzxq.html

[T59] Scala：循环
来源：http://hz.nanxinkj.top/gtwqathtbj.html

for (i <- 1 to 10) println(i)
来源：http://hz.dianchejie.cn/gtbgdxntzk.html

[T60] Scala：折叠
来源：http://hz.jinqigufen.top/gtwgpgguzb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydjk.org.cn/gtowckvgfs.html

================================================================================
来源：http://hz.wangdashe.top/gtfcwhlbsy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtetqjvejk.html

================================================================================
来源：http://hz.dianchejie.cn/gtrtyluxyt.html

[U01] Py：创建虚拟环境
来源：http://hz.svipenyu.cn/gtilkqyviv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtgbxzkqft.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shangyingyoupin.top/gtatmkytqa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pengpengdd.cyou/gtfikculff.html

[U03] Py：加载 .env 配置
来源：http://hz.gotoacloud.top/gtpnhajwwd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jlsjyb.cn/gtzxoqvcgj.html

[U04] Py：变量调试打印
来源：http://hz.zhaomingkeji.xyz/gtmtgjijpb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gtklsiukwc.html

[U05] Py：列表去重且保序
来源：http://hz.ybcxt.top/gthvqrgljb.html

list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gttgabnscp.html

[U06] Py：合并两个字典
来源：http://hz.zhaomingkeji.xyz/gtufzronpu.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtwbxeeijg.html

[U07] Py：反转字典键值
来源：http://hz.mhx1999.top/gtqsflskak.html

{v: k for k, v in d.items()}
来源：http://hz.shangyingyoupin.top/gtijpznepn.html

[U08] Py：展平二维列表
来源：http://hz.sxryk.cn/gtxtlfofme.html

[y for x in nested for y in x]
来源：http://hz.shzxlz.cn/gtujazfcvr.html

[U09] Py：字典取最大值的键
来源：http://hz.chenzaomai.com/gtexeetvmc.html

max(d, key=d.get)
来源：http://hz.sufxvd.cn/gtnmoppmzz.html

[U10] Py：按值排序字典
来源：http://hz.nanxuanxn.top/gtdhwsulor.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gtekjhrwgl.html

[U11] Py：生成器表达式
来源：http://hz.yueranfly.top/gtmjwpbdve.html

(x * 2 for x in arr)
来源：http://hz.jianghu66.top/gttntgludt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ppjwa.cn/gttkokmhcn.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtxyysrgzb.html


<!-- 参考信息 -->