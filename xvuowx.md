代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gthnkqmggf.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtrxppxpvm.html

date +%s;  date -d @1700000000
来源：http://hz.9152youxi.cn/gtpngxucvt.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gtyjvdawks.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.svipenyu.cn/gtsxxucoze.html

[R72] 等待端口就绪
来源：http://hz.ivvv.top/gtnjoeqgmv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sxryk.cn/gtekvlcvnp.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtpiwarotm.html

split -l 1000 big.log part_
来源：http://hz.daxiang520.top/gttkibigxu.html

[R74] 批量重命名
来源：http://hz.yonumen.top/gttnzcrnko.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtbcjfguzz.html

[R75] 导出环境变量
来源：http://hz.nanxinkj.top/gtjukacdgl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtbbfovkgm.html

[R76] 使用临时文件
来源：http://hz.ehwqpu.com/gtrvrlphik.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtmxacwytd.html

[R77] 读取用户输入
来源：http://hz.hnxiangtu.top/gtctaudhub.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtmggwsely.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtrgfyzxmv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shuidangran.top/gtuefimzmf.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtbuwkgqju.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gturgfohll.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtlccuuxcy.html

time ./run.sh
来源：http://hz.snrcjt.cn/gtkkwiigec.html

================================================================================
来源：http://hz.aizwys.cn/gtxupaguno.html

S. C / C++ 专题
来源：http://hz.shanyushiyangkeji.top/gtggmmehmj.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtszyjjmia.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtvarbadwt.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtzbcztftq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.0kj1m.cn/gtcmsaoxis.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtmbumtygy.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gthyunrvaf.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtyzwtnrcr.html

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtfigqlboi.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtukafioqx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtyiptmajx.html

[S05] C：字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtcgebmwkc.html

strlen(s)
来源：http://hz.zhixingplan.top/gtdfhohknz.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtihuzbeub.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtjxverfyb.html

[S07] C：数组遍历求和
来源：http://hz.316326.xyz/gtvdugpeta.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zdqjudy.top/gtmbbjxahq.html

[S08] C：动态内存分配与释放
来源：http://hz.cucudq.cn/gtsskuriam.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtdbrxrfal.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtezvftahs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yanxiufei.cn/gtvsklmwqe.html

[S10] C：指针与解引用
来源：http://hz.feifeiyinyue.top/gtdngnhmpi.html

int *p = &a;  *p = 5;
来源：http://hz.shuidangran.top/gtwugntqao.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtdwtslzev.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aibaodan.cn/gtkxhztlwj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daria6918.cn/gtietklrrk.html

fclose(f);
来源：http://hz.zhiwuduotai.top/gtywkhdcdt.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gtnbokezec.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gthwnjcnuw.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtceteyxbi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gtqoturafm.html

[S14] C：枚举
来源：http://hz.yj20258.top/gtnxneylct.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtgyqjxqrv.html

[S15] C：类型转换
来源：http://hz.bjfxy.top/gtqyfeuyig.html

(double) a / b
来源：http://hz.guowangkeji.top/gtnwrqieut.html

[S16] C：位操作置位
来源：http://hz.hysaishi.cn/gtfpaypozz.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtemzstzsi.html

[S17] C：安全拼接字符串
来源：http://hz.guowangkeji.top/gtaiixfpmr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuxming.cn/gtibrmlwus.html

[S18] C：命令行参数
来源：http://hz.sysykeji.top/gtllwqzhuz.html

int main(int argc, char **argv)
来源：http://hz.yj202588.top/gtrdsvownj.html

[S19] C：快速排序
来源：http://hz.daria6918.cn/gtncuifudr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtjtrxumrt.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gtbhokmmfm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtcrteivpj.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gtwsvwhbdc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gtjbsuzngl.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gtsewabafc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtlkerbhxe.html

[S23] C：随机数
来源：http://hz.sweek.top/gticjaoykg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shangyingyoupin.top/gtbxcyogbv.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtgqawgixp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xinyue.icu/gtojqzdadb.html

[S25] C：内存拷贝
来源：http://hz.52xcode.cn/gtlaxlgmfj.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtfqoxerhi.html

[S26] C：内存清零
来源：http://hz.cucudq.cn/gtvmndmaei.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtdniwnpid.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtvtzskcox.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtbdfxeito.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtruqpzlvh.html

static int counter = 0;
来源：http://hz.daxiang520.top/gtqtrzjxes.html

[S29] C：变参函数
来源：http://hz.nwbrower.top/gteoooxvbf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtveorzcot.html

[S30] C：头文件保护
来源：http://hz.xingfuxueyuan.xyz/gtqyjpgcyt.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtmkhkqqgk.html

#define X_H
来源：http://hz.cdnleiting.top/gttryfbuwk.html

#endif
来源：http://hz.hnxiangtu.top/gtqfsanvay.html

[S31] C++：Hello World
来源：http://hz.xziqi.cn/gthlthjkgz.html

#include <iostream>
来源：http://hz.yonumen.top/gtolalnteu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gtkrlyhozh.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtnkpxzpms.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtekftjaww.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtcafoxaxc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dianchejie.cn/gtasrgbrtq.html

[S34] C++：遍历 vector
来源：http://hz.nanxinkj.top/gtajtorzsi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtdxivrxdp.html

[S35] C++：map
来源：http://hz.sweek.top/gtpapdmogk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtyihhccpw.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gteeejfqfl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtufilkpvg.html

[S37] C++：set
来源：http://hz.zhaomingkeji.xyz/gtslmxiyxp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tianlin.xyz/gtvtatungq.html

[S38] C++：排序
来源：http://hz.chenlongwang.top/gtviyckjiy.html

std::sort(v.begin(), v.end());
来源：http://hz.mhx1999.top/gtuqrebzof.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtxxkumshv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zdqjudy.top/gtddvwvlpe.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gtpdwwruup.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtdjbglled.html

[S41] C++：类与构造函数
来源：http://hz.jianghu66.top/gtaqahlryg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shangyingyoupin.top/gtizoovftg.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangtech.top/gtzffwowid.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gtpkxdfyoe.html

[S43] C++：智能指针
来源：http://hz.pengpengdd.cyou/gtvxofzfrg.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gttuqvvoje.html

[S44] C++：引用传参
来源：http://hz.ppjwa.cn/gthzzbuwft.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtcrezamtc.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gtxzsryiud.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtgofvtfvt.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtvfdrtbpk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.bjfxy.top/gtiibbkjkh.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtstztqyrm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tanke756.top/gtkhijgrlw.html

[S48] C++：逐行读文件
来源：http://hz.zhoulong.xyz/gtlaeyvjum.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gtoyrxedwd.html

while (std::getline(in, line)) { }
来源：http://hz.daria6918.cn/gtgezmgowh.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtbucyrjoa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gtcyuoihbu.html

[S50] C++：格式化数字
来源：http://hz.feifeiyinyue.top/gtvplqzivc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtxowfuhdz.html

[S51] C++：显式类型转换
来源：http://hz.jqgufenzy.top/gtuxitegnt.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtpimfqaow.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtnykfxohg.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtgwmipnhf.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtsmveibjr.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtofhflidc.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gthwxemxes.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gtjkwauuus.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gtxonalshh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangtech.top/gtdxaqnapn.html

[S56] C++：optional
来源：http://hz.yj202588.top/gtqlgmdplt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtohphlwaz.html

[S57] C++：编译期常量
来源：http://hz.aibaodan.cn/gtwwqcdaoe.html

constexpr int N = 10;
来源：http://hz.0kj1m.cn/gtmvfbclwy.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtlozdvwdk.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigfzy.top/gtewehpbgh.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtvbbswzsd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtgwbxtqvh.html

[S60] C++：遍历并删除元素
来源：http://hz.hongshengwenyu.top/gtdgguenin.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gtdbhecfek.html

================================================================================
来源：http://hz.cucudq.cn/gtwswxtstt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtzhczmkso.html

================================================================================
来源：http://hz.hnqzz.top/gtjljvlcbz.html

[T01] Kotlin：Hello World
来源：http://hz.jqgufenzy.top/gtiggwxuvu.html

println("Hello")
来源：http://hz.nwbrower.top/gtnemzdduy.html

[T02] Kotlin：变量
来源：http://hz.hnxiangtu.top/gtmamcuqis.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gtnkqqulcj.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtjmdehqsy.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtaduaodjx.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtrplsdrwo.html

val n: String? = null;  n?.length
来源：http://hz.sxryk.cn/gtmwelafma.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258888.top/gtstnqotgm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtzeluvugw.html

[T06] Kotlin：集合映射
来源：http://hz.tianlin.xyz/gtpjvhaifc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtbetrtdsr.html

[T07] Kotlin：集合过滤
来源：http://hz.chenjidiqi.icu/gtcbxqpdwq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtpfbmohhq.html

[T08] Kotlin：数据类
来源：http://hz.feifeiyinyue.top/gtenrfaoaz.html

data class User(val name: String, val age: Int)
来源：http://hz.nwbrower.top/gtcxpfnywo.html

[T09] Kotlin：扩展函数
来源：http://hz.pengpengdd.cyou/gtsvyidnpl.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gtcwvjxvlw.html

[T10] Kotlin：默认参数
来源：http://hz.nanxinkj.top/gtyxdabdvy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.svipenyu.cn/gtqypikebc.html

[T11] Kotlin：协程
来源：http://hz.zycfv.cn/gtjtgvbhwd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydzc1.top/gtbbckczri.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtwqmdudiz.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gtmvgrdbfv.html

[T13] Kotlin：只读 Map
来源：http://hz.ehwqpu.com/gtamkdbxga.html

val m = mapOf("a" to 1)
来源：http://hz.nanxinkj.top/gtfwtxnssn.html

[T14] Kotlin：循环
来源：http://hz.aibaodan.cn/gtddkohymj.html

for (i in 1..10) println(i)
来源：http://hz.yj202588.top/gtjisbygcb.html

[T15] Kotlin：接口
来源：http://hz.dianchejie.cn/gtcdgegjrr.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtphtljffq.html

[T16] Swift：Hello World
来源：http://hz.0kj1m.cn/gtoovujyxe.html

print("Hello")
来源：http://hz.chenlongwang.top/gtzfoptvpk.html

[T17] Swift：变量与常量
来源：http://hz.zdqjudy.top/gtfcuyrzvg.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtpunjvmem.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtvsuxumlm.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtunhnhhpe.html

[T19] Swift：可选绑定
来源：http://hz.smart0.xyz/gtsjdxztkw.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtmrkcoalb.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtlckhvgym.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtmjqjudzr.html

[T21] Swift：遍历
来源：http://hz.tianlin.xyz/gtyrnhvywc.html

for x in a { print(x) }
来源：http://hz.yuxming.cn/gtzervhoqj.html

[T22] Swift：字典
来源：http://hz.yj202588.top/gtnvzawcfp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtdgitzfui.html

[T23] Swift：函数
来源：http://hz.shanyushiyangkeji.top/gtbtddvzkh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtsclzimqq.html

[T24] Swift：闭包
来源：http://hz.hnxiangtu.top/gtlqitwfcb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhongyouzk.top/gtqrpdebdw.html

[T25] Swift：结构体
来源：http://hz.dianchejie.cn/gtvestulay.html

struct P { var x: Int }
来源：http://hz.ydjk.org.cn/gtnyaspwak.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtgjaemvyt.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtxfrqdwef.html

[T27] Swift：错误处理
来源：http://hz.pengpengdd.cyou/gtdfhmoonn.html

do { try f() } catch { print(error) }
来源：http://hz.hfpthk.cn/gtvuouvyod.html

[T28] Swift：枚举
来源：http://hz.jiagoushi.top/gttiknxcgg.html

enum Color { case red, green }
来源：http://hz.xziqi.cn/gtjpnidiwy.html

[T29] Swift：guard 提前返回
来源：http://hz.zhiwuduotai.top/gtskthcydl.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gtxvfxeath.html

[T30] Swift：协议
来源：http://hz.kuanghao11.cn/gtpwdfsdoq.html

protocol Shape { func area() -> Double }
来源：http://hz.cheryme.top/gtldlmjjbg.html

[T31] Lua：Hello World
来源：http://hz.gogol.net.cn/gtdmidmnxy.html

print("Hello")
来源：http://hz.fengsongda.top/gtreodsvso.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gtfmbzpihu.html

local a = 1
来源：http://hz.tanke756.top/gtfbxbtage.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangtech.top/gtyjdvnkrz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gtbngtmtfg.html

[T34] Lua：遍历表
来源：http://hz.tian-w.cn/gtunwpdert.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ivvv.top/gtgelcxyos.html

[T35] Lua：字典表
来源：http://hz.tianlin.xyz/gtctwirosj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yvedp.cn/gtydnovqva.html

[T36] Lua：函数
来源：http://hz.jinyuanbaomall.cn/gtbbffbjbd.html

function add(a, b) return a + b end
来源：http://hz.316326.xyz/gtmchutghl.html

[T37] Lua：字符串拼接
来源：http://hz.xuetiantiany.cn/gtvpklbhas.html

"a" .. "b"
来源：http://hz.hnxiangtu.top/gtoplolvwc.html

[T38] Lua：条件
来源：http://hz.zhiwuduotai.top/gtkkzrgalc.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gttxbahmnx.html

[T39] Lua：模式匹配
来源：http://hz.gzhubu.top/gtjxzqxewf.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtfsyxhcza.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtugjnkywv.html

setmetatable({}, { __index = base })
来源：http://hz.zdqjudy.top/gtfmfqpvyo.html

[T41] Perl：Hello World
来源：http://hz.yonumen.top/gtqgrgsmqt.html

print "Hello\n";
来源：http://hz.316326.xyz/gtigkfthhp.html

[T42] Perl：变量类型
来源：http://hz.redwolf501.top/gtbtfijwwb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgfzy.top/gttifmezhj.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtqhlnwghk.html

"值: $a"
来源：http://hz.cheryme.top/gtdzigmmhq.html

[T44] Perl：条件
来源：http://hz.jlsjyb.cn/gttgppploz.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gtwiynrsfj.html

[T45] Perl：数组遍历
来源：http://hz.pengpengdd.cyou/gtfwyxlydt.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtaxmotkhx.html

[T46] Perl：哈希操作
来源：http://hz.yvedp.cn/gtwejkmani.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gotoacloud.top/gtvxqsvfjn.html

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gtjpweppdy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtycytujop.html

[T48] Perl：正则替换
来源：http://hz.gzhubu.top/gtighdzrjx.html

$s =~ s/old/new/g;
来源：http://hz.gzhubu.top/gtjoyixukz.html

[T49] Perl：函数
来源：http://hz.ywan-chungtsiang.top/gtijodtpid.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sweek.top/gtqocqfpjg.html

[T50] Perl：逐行读文件
来源：http://hz.jiagoushi.top/gtqvujhfcg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhongyouzk.top/gtcxdguiim.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yongpay.top/gtmkpaygae.html

[T51] Scala：Hello World
来源：http://hz.0kj1m.cn/gtopxtzlyl.html

println("Hello")
来源：http://hz.havefunace.top/gtnimtudvw.html

[T52] Scala：变量
来源：http://hz.dianchejie.cn/gtzcjtjzuw.html

val a = 1;  var b = 2
来源：http://hz.tian-w.cn/gtpbnacknf.html

[T53] Scala：字符串插值
来源：http://hz.zhengqikj.top/gtmfnbwzou.html

s"值: $b"
来源：http://hz.xinyue.icu/gtfnewazdm.html

[T54] Scala：集合映射
来源：http://hz.yj20258.top/gtctvkpnfy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ppjwa.cn/gtirbimwui.html

[T55] Scala：集合过滤
来源：http://hz.tanke756.top/gtzwpvuonj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xziqi.cn/gtadyzprvk.html

[T56] Scala：样例类
来源：http://hz.316326.xyz/gtzzcsokvp.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gtxtmsrrbs.html

[T57] Scala：模式匹配
来源：http://hz.gogol.net.cn/gtaezjkuuo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.svipenyu.cn/gttimvszlt.html

[T58] Scala：函数定义
来源：http://hz.feifeiyinyue.top/gtxdafwpyr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.daria6918.cn/gtxxrmleeh.html

[T59] Scala：循环
来源：http://hz.yangfankeji.com/gtijagbame.html

for (i <- 1 to 10) println(i)
来源：http://hz.tanke756.top/gtuyiabxwz.html

[T60] Scala：折叠
来源：http://hz.yongpay.top/gtweqjwmee.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gtqroqumma.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyxreedej.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtenvowdvu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfbkaomvg.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gtvwpnmqoc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.andypj.xyz/gtgdrhcmhi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cucudq.cn/gtmprqzglu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtoajdbbdf.html

[U03] Py：加载 .env 配置
来源：http://hz.xylfe.cn/gtolpmwgjd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gtpnfsgmnx.html

[U04] Py：变量调试打印
来源：http://hz.fzhhl.top/gtkzonghwu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.bjfxy.top/gtqdcszitm.html

[U05] Py：列表去重且保序
来源：http://hz.52xcode.cn/gtdouoolgr.html

list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtjiegssdn.html

[U06] Py：合并两个字典
来源：http://hz.chenlongwang.top/gtfuihmapi.html

{**a, **b}
来源：http://hz.kuanghao11.cn/gthvryvwru.html

[U07] Py：反转字典键值
来源：http://hz.yj20258888.top/gtlwbfyyza.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtoqwcxiol.html

[U08] Py：展平二维列表
来源：http://hz.zhaomingkeji.xyz/gtokwcfhnb.html

[y for x in nested for y in x]
来源：http://hz.gogol.net.cn/gtvssgttro.html

[U09] Py：字典取最大值的键
来源：http://hz.shangyingyoupin.top/gtselmwtyd.html

max(d, key=d.get)
来源：http://hz.zhiwuduotai.top/gtcopiwpiy.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gtjnrjujua.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhoulong.xyz/gthclmsrvp.html


<!-- 参考信息 -->