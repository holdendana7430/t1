代发 wailian999

openssl rand -hex 16
来源：http://hz.cheryme.top/gtcormgtym.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gtriofzuep.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtthivnkae.html

[R69] 生成随机密码
来源：http://hz.svipenyu.cn/gtiueooawb.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtjeeaomln.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtikfwuctw.html

date +%s;  date -d @1700000000
来源：http://hz.ehwqpu.com/gtlohacutj.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gtryuqwtnf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhengqikj.top/gtwxpcusdx.html

[R72] 等待端口就绪
来源：http://hz.zhoulong.xyz/gtzdhyqpmn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yangfankeji.com/gtcjnpfceq.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtiopzvpwp.html

split -l 1000 big.log part_
来源：http://hz.yj202588.top/gtesamchtb.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtalmfqpad.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nwbrower.top/gtjbxagsvn.html

[R75] 导出环境变量
来源：http://hz.quarkkingdee.top/gtrsxhejfj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.feifeiyinyue.top/gtlwsnhqrw.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtyhwviztm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtjmczrozw.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gtbssvvpig.html

read -rp "请输入: " ans
来源：http://hz.zycfv.cn/gtgjjulvbr.html

[R78] 交互式菜单
来源：http://hz.hammf.cn/gtwvodqyqx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydzc1.top/gtyshibmmu.html

[R79] 解析命令行选项
来源：http://hz.wangshuangyany.cn/gtmmsodtgf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtyhlyeiru.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtcvujxnbx.html

time ./run.sh
来源：http://hz.iojbl.cn/gtwecwzlon.html

================================================================================
来源：http://hz.jlsjyb.cn/gtduqbdtrg.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtcwuratmx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtbijyfnju.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gttjdiolhb.html

#include <stdio.h>
来源：http://hz.shzxlz.cn/gtykvonvlg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxinkj.top/gtvxbfhdwt.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtfljqchzx.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgufenzy.top/gttgrbrrdm.html

[S03] C：读入整数
来源：http://hz.daria6918.cn/gtplqskoyj.html

int x; scanf("%d", &x);
来源：http://hz.jiagoushi.top/gtfugkozil.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtzwrsxsct.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenjidiqi.icu/gtfranegdq.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtsukpdmwn.html

strlen(s)
来源：http://hz.jqgfzy.top/gtkttnrgrf.html

[S06] C：字符串比较
来源：http://hz.c1oappe.top/gtqfxytofs.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gtwxhpzubw.html

[S07] C：数组遍历求和
来源：http://hz.hysaishi.cn/gtuxfiesvg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtzxhzuwgp.html

[S08] C：动态内存分配与释放
来源：http://hz.dashuyun.cn/gtjzcsjoaj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gtejxmprro.html

[S09] C：结构体定义与初始化
来源：http://hz.zhixingplan.top/gtlqnhqtkt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gtxqmtoifd.html

[S10] C：指针与解引用
来源：http://hz.wangdashe.top/gtmpikhzvv.html

int *p = &a;  *p = 5;
来源：http://hz.iojbl.cn/gtfjbqfeav.html

[S11] C：逐行读文件
来源：http://hz.smart0.xyz/gtqhazrplk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtlzuyydpv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gtxqoyxdpj.html

fclose(f);
来源：http://hz.meibo888.top/gtvlmvmuah.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtaicxagtu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangshuangyany.cn/gtsidvlnyj.html

[S13] C：宏定义
来源：http://hz.shanyushiyangtech.top/gtmqbwbrtf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258.top/gtjjgoyszr.html

[S14] C：枚举
来源：http://hz.zdqjudy.top/gtddukpcaq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jlsjyb.cn/gtdgszfwoa.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtoucurnwq.html

(double) a / b
来源：http://hz.gzhubu.top/gtiuaqccnw.html

[S16] C：位操作置位
来源：http://hz.sweek.top/gtpjpucsij.html

x |= (1 << 3);
来源：http://hz.vqdsnc.cn/gtwqemivuv.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtqboywwsl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gaohongyu789.top/gtzyxgegio.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gttdlyovrx.html

int main(int argc, char **argv)
来源：http://hz.svipenyu.cn/gtaifemjxp.html

[S19] C：快速排序
来源：http://hz.svipenyu.cn/gtpglknxnw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtutekijwi.html

[S20] C：二分查找
来源：http://hz.zhixingplan.top/gtoddwnpyv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtfsymreln.html

[S21] C：字符类别判断
来源：http://hz.yangfankeji.com/gtouyusdej.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydzc1.top/gtsailldtk.html

[S22] C：字符串转数字
来源：http://hz.tanke756.top/gtrdtnhwgm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zdqjudy.top/gtwvmazibc.html

[S23] C：随机数
来源：http://hz.jinqigfzy.top/gtzxdxfjbb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtkjkbxwht.html

[S24] C：获取本地时间
来源：http://hz.daria6918.cn/gtrogmvvgg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258.top/gtdxkfmwjh.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtwzmekqqx.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtdclzlwac.html

[S26] C：内存清零
来源：http://hz.yuanzhike.top/gtlpicwdbo.html

memset(a, 0, sizeof a);
来源：http://hz.guannengcc.top/gtfaqdfumt.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gtmalkkpun.html

const double PI = 3.14159;
来源：http://hz.ivvv.top/gtmkfcvsux.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtbpagoukl.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtqwkwckad.html

[S29] C：变参函数
来源：http://hz.hongshengwenyu.top/gtveqvfjma.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yuanzhike.top/gtsfvtwaod.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtmhyqosog.html

#ifndef X_H
来源：http://hz.yuanzhike.top/gtatznbvou.html

#define X_H
来源：http://hz.gotoacloud.top/gtpifhgocl.html

#endif
来源：http://hz.yj202588.top/gtyvjqujbf.html

[S31] C++：Hello World
来源：http://hz.shzxlz.cn/gtgohkuknd.html

#include <iostream>
来源：http://hz.quarkkingdee.top/gthrfmykne.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ppjwa.cn/gtvzgbaufp.html

[S32] C++：字符串
来源：http://hz.cdnleiting.top/gtjhekxtzy.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtwbcxmrjd.html

[S33] C++：vector 增删
来源：http://hz.shuidangran.top/gtvqnyjokf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgufenzy.top/gtbmspemij.html

[S34] C++：遍历 vector
来源：http://hz.hysaishi.cn/gtfpcvhhki.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtggiuenkn.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtifjgxlii.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtjuqkdgqu.html

[S36] C++：unordered_map
来源：http://hz.cucudq.cn/gtdqoifrdv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtzfkdghzi.html

[S37] C++：set
来源：http://hz.svipenyu.cn/gtiayohwgq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangshuangyany.cn/gtaxpjetzr.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gttkehqglx.html

std::sort(v.begin(), v.end());
来源：http://hz.chenzaomai.com/gtwjtimfqe.html

[S39] C++：自定义比较器排序
来源：http://hz.yanxiufei.cn/gttjlvwzxo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yongpay.top/gtmxiawkzv.html

[S40] C++：查找元素
来源：http://hz.aizwys.cn/gtyaelizum.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shuidangran.top/gtxkkczltv.html

[S41] C++：类与构造函数
来源：http://hz.yongpay.top/gteuwbtlyr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hywenlv.cn/gtbrpfwnel.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gthqpqzwkk.html

class B : public Base { public: void f() override {} };
来源：http://hz.52xcode.cn/gtpkeknmgh.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtkoecsyfu.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtqlfrwjbb.html

[S44] C++：引用传参
来源：http://hz.gotoacloud.top/gtsggodbqs.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtavgwdttv.html

[S45] C++：lambda
来源：http://hz.gotoacloud.top/gtykljyrsh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gtorwkyltp.html

[S46] C++：函数模板
来源：http://hz.gotoacloud.top/gtfvoouawj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tianlin.xyz/gtyxsvfqzv.html

[S47] C++：结构化绑定遍历
来源：http://hz.tanke756.top/gtrvfnllax.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtkqurviwy.html

[S48] C++：逐行读文件
来源：http://hz.chenjidiqi.icu/gtlejqbnbf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtpfthwhwa.html

while (std::getline(in, line)) { }
来源：http://hz.zhiwuduotai.top/gtwyznnbgx.html

[S49] C++：写文件
来源：http://hz.xuanzx.com/gtcdekpfce.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nwbrower.top/gtsynyonzb.html

[S50] C++：格式化数字
来源：http://hz.daxiang520.top/gteqxfjbxs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hfpthk.cn/gtbmyeqyrr.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtmegvbrjl.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gtgpvkqxud.html

[S52] C++：const 与 noexcept
来源：http://hz.jianghu66.top/gtenumgizh.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gttrnhzyhw.html

[S53] C++：移动语义
来源：http://hz.tanke756.top/gtdxxckulh.html

std::vector<int> w = std::move(v);
来源：http://hz.yvedp.cn/gtbyontzgo.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gtluyxiwlx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gogol.net.cn/gtyxchfyro.html

[S55] C++：结构化绑定
来源：http://hz.c1oappe.top/gtdmowijpp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.vqdsnc.cn/gtulsobvqd.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtivhenped.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gtyoiupsrv.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtoflhpsad.html

constexpr int N = 10;
来源：http://hz.ppjwa.cn/gtvdmaufhy.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gtjmmulvpa.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtpomboywg.html

[S59] C++：静态断言
来源：http://hz.yueranfly.top/gtkkdihsll.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yonumen.top/gtnxtzxbbo.html

[S60] C++：遍历并删除元素
来源：http://hz.yanxiufei.cn/gtqgatrjay.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtiplwxciv.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtfvsqqfvg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnxiangtu.top/gtbiwtmwmh.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvscgiowl.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gttrvhoxpz.html

println("Hello")
来源：http://hz.hnqzz.top/gtfyzkbzra.html

[T02] Kotlin：变量
来源：http://hz.9152youxi.cn/gtxyupjkuc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenzaomai.com/gtyjbemztn.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtuhwhioek.html

"值: $b"
来源：http://hz.0kj1m.cn/gtbuczwgnt.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtdqhxwtlk.html

val n: String? = null;  n?.length
来源：http://hz.zhongyouzk.top/gtwfjkmyri.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtxewkioqv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gttnmhhxfp.html

[T06] Kotlin：集合映射
来源：http://hz.fengsongda.top/gtokrbtvpa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tianlin.xyz/gtzwmsqowq.html

[T07] Kotlin：集合过滤
来源：http://hz.havefunace.top/gtwifajspb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgfzy.top/gtfbmphdvp.html

[T08] Kotlin：数据类
来源：http://hz.hysaishi.cn/gthaamcmxn.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtxhgdlsua.html

[T09] Kotlin：扩展函数
来源：http://hz.sxryk.cn/gtmahdvbdn.html

fun String.exclaim() = this + "!"
来源：http://hz.aizwys.cn/gtwgtrhwxc.html

[T10] Kotlin：默认参数
来源：http://hz.zhoulong.xyz/gtmyasrlpn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtiktjtqfv.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtvvigjdjh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tanke756.top/gtkzxouket.html

[T12] Kotlin：解构声明
来源：http://hz.pengpengdd.cyou/gtogixwaqo.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtlgbpgfdj.html

[T13] Kotlin：只读 Map
来源：http://hz.316326.xyz/gtanbhrxme.html

val m = mapOf("a" to 1)
来源：http://hz.ywan-chungtsiang.top/gtphqzpndo.html

[T14] Kotlin：循环
来源：http://hz.sysykeji.top/gtqxpeierw.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtylqemvec.html

[T15] Kotlin：接口
来源：http://hz.bjfxy.top/gthziaeauv.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtfglqjhcn.html

[T16] Swift：Hello World
来源：http://hz.gotoacloud.top/gtiqblncjy.html

print("Hello")
来源：http://hz.andypj.xyz/gtxusyrrng.html

[T17] Swift：变量与常量
来源：http://hz.hnqzz.top/gtvnswpjxk.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtjbinvqhe.html

[T18] Swift：字符串插值
来源：http://hz.pengpengdd.cyou/gtgtmwpqfg.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gttospifcd.html

[T19] Swift：可选绑定
来源：http://hz.jqgufenzy.top/gtvfmzabpo.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtycpvohda.html

[T20] Swift：数组操作
来源：http://hz.tanke756.top/gtiotxwtxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgufenzy.top/gtspkasysm.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtawepswkt.html

for x in a { print(x) }
来源：http://hz.zhiwuduotai.top/gtykarywzf.html

[T22] Swift：字典
来源：http://hz.shanyushiyangkeji.top/gtcypnnbza.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhongyouzk.top/gtpplwogwu.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtwygcvbct.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtgpmyaxgn.html

[T24] Swift：闭包
来源：http://hz.zdqjudy.top/gtnlcztcad.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.daxiang520.top/gtqrzwfknk.html

[T25] Swift：结构体
来源：http://hz.wangdashe.top/gtoflwtdht.html

struct P { var x: Int }
来源：http://hz.jinyuanbaomall.cn/gtpccavhoc.html

[T26] Swift：类与重写
来源：http://hz.jinghuilouyu.cn/gtebvtxcuu.html

class A: Base { override func f() {} }
来源：http://hz.jinqigfzy.top/gtezcffbnd.html

[T27] Swift：错误处理
来源：http://hz.hongshengwenyu.top/gtsvvchbvy.html

do { try f() } catch { print(error) }
来源：http://hz.52xcode.cn/gtdprrplnt.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtiskikrin.html

enum Color { case red, green }
来源：http://hz.shanyushiyangtech.top/gtbloffjma.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgufenzy.top/gtkdwfzwps.html

guard let x = opt else { return }
来源：http://hz.svipenyu.cn/gtkzladhxc.html

[T30] Swift：协议
来源：http://hz.kuanghao11.cn/gtsxtvfaqo.html

protocol Shape { func area() -> Double }
来源：http://hz.shangyingyoupin.top/gtxquzleir.html

[T31] Lua：Hello World
来源：http://hz.hnxiangtu.top/gtjdddcqoa.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtuohshnej.html

[T32] Lua：局部变量
来源：http://hz.shuidangran.top/gthewuvirb.html

local a = 1
来源：http://hz.jqgfzy.top/gtkbzvmlcq.html

[T33] Lua：表（数组）
来源：http://hz.gzhubu.top/gtsqpbruzf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangtech.top/gtzdjdjkio.html

[T34] Lua：遍历表
来源：http://hz.wangdashe.top/gtzuzvojfm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.iojbl.cn/gtjgzftyda.html

[T35] Lua：字典表
来源：http://hz.meibo888.top/gtrjzkbmyq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gtsksmbrgj.html

[T36] Lua：函数
来源：http://hz.hfpthk.cn/gtftlkzldn.html

function add(a, b) return a + b end
来源：http://hz.0kj1m.cn/gtzzodvdfi.html

[T37] Lua：字符串拼接
来源：http://hz.nanxinkj.top/gtvuwqszzj.html

"a" .. "b"
来源：http://hz.chenjidiqi.icu/gtglkiavxi.html

[T38] Lua：条件
来源：http://hz.316326.xyz/gtewidvzle.html

if x > 0 then print("正") end
来源：http://hz.316326.xyz/gteldvlcrl.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gtcnwnorni.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gteznowhuq.html

[T40] Lua：元表
来源：http://hz.0kj1m.cn/gtumljuwyi.html

setmetatable({}, { __index = base })
来源：http://hz.meibo888.top/gtgmegczww.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gttfbniwcs.html

print "Hello\n";
来源：http://hz.ivvv.top/gtldcwjtpo.html

[T42] Perl：变量类型
来源：http://hz.9152youxi.cn/gtljozohcn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.daxiang520.top/gtyoupeost.html

[T43] Perl：字符串插值
来源：http://hz.yvedp.cn/gtndordpqd.html

"值: $a"
来源：http://hz.xylfe.cn/gteotofqiy.html

[T44] Perl：条件
来源：http://hz.zhijiandao.cn/gtxqfzihle.html

if ($a > 0) { print "正"; }
来源：http://hz.guowangkeji.top/gthizmittn.html

[T45] Perl：数组遍历
来源：http://hz.jlsjyb.cn/gtqwmjvfid.html

for my $x (@arr) { print $x; }
来源：http://hz.havefunace.top/gtjchhyzfy.html

[T46] Perl：哈希操作
来源：http://hz.wangdashe.top/gtltnymssd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.meibo888.top/gtktemghrz.html

[T47] Perl：正则捕获
来源：http://hz.svipenyu.cn/gtvfveqibr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtqtxipzee.html

[T48] Perl：正则替换
来源：http://hz.hongshengwenyu.top/gtwqzlzwmz.html

$s =~ s/old/new/g;
来源：http://hz.xylfe.cn/gtygmpbhfo.html

[T49] Perl：函数
来源：http://hz.pengpengdd.cyou/gtoyrwlwfq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.fzhhl.top/gtksnkyide.html

[T50] Perl：逐行读文件
来源：http://hz.xziqi.cn/gtgqxgzbhn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yonumen.top/gttbhaxghu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtkiapjfum.html

[T51] Scala：Hello World
来源：http://hz.haohaochexian.top/gtixycbxpv.html

println("Hello")
来源：http://hz.yj20258.top/gtlzyprxyv.html

[T52] Scala：变量
来源：http://hz.yangfankeji.com/gtrjveusjv.html

val a = 1;  var b = 2
来源：http://hz.ehwqpu.com/gtcderupll.html

[T53] Scala：字符串插值
来源：http://hz.shzxlz.cn/gtxazppsyu.html

s"值: $b"
来源：http://hz.aizwys.cn/gtddhflkis.html

[T54] Scala：集合映射
来源：http://hz.cashguo.top/gtogbqxqbe.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hammf.cn/gteralhbxs.html

[T55] Scala：集合过滤
来源：http://hz.andypj.xyz/gtjrjwhjqe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dianchejie.cn/gtlqefwiyq.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtbgcwoqrc.html

case class User(name: String, age: Int)
来源：http://hz.xinyue.icu/gtgmifivrk.html

[T57] Scala：模式匹配
来源：http://hz.wangdashe.top/gtftwgzupu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnqzz.top/gtopcurghm.html

[T58] Scala：函数定义
来源：http://hz.kuanghao11.cn/gtmtpvzhfm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yanxiufei.cn/gtztlxbowk.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gtueisrchs.html

for (i <- 1 to 10) println(i)
来源：http://hz.bjfxy.top/gtmexjjnir.html

[T60] Scala：折叠
来源：http://hz.xylfe.cn/gttnrylkmk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhongyouzk.top/gtkmmihoju.html

================================================================================
来源：http://hz.xinyue.icu/gtvalbozrc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangshuangyany.cn/gtgvlmaowl.html

================================================================================
来源：http://hz.zhengqikj.top/gtitkqdxht.html

[U01] Py：创建虚拟环境
来源：http://hz.snrcjt.cn/gtshtlevko.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gthjnfjpqa.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtngosygfz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xylfe.cn/gtvqqsfwsn.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gtqzohscsp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zdqjudy.top/gtojhuemuk.html

[U04] Py：变量调试打印
来源：http://hz.jinqigufen.top/gtescfwbqr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gzhubu.top/gtyfaqafra.html

[U05] Py：列表去重且保序
来源：http://hz.fzhhl.top/gthebsmxyn.html

list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtsqkmiwgr.html

[U06] Py：合并两个字典
来源：http://hz.aibaodan.cn/gtevlfkwyx.html

{**a, **b}
来源：http://hz.xuetiantiany.cn/gtjgyhrlyh.html

[U07] Py：反转字典键值
来源：http://hz.zdqjudy.top/gtweloohvl.html

{v: k for k, v in d.items()}
来源：http://hz.52xcode.cn/gtwhafaukj.html

[U08] Py：展平二维列表
来源：http://hz.daria6918.cn/gtxiliwsyi.html

[y for x in nested for y in x]
来源：http://hz.yj202588.top/gtzllexkzq.html


<!-- 参考信息 -->