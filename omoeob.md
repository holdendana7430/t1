代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.zhoulong.xyz/gtythokpvz.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtlzcfayis.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gtrogjunmf.html

[R71] 日期格式化
来源：http://hz.chenlongwang.top/gtkihomguw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtbljqvtmc.html

[R72] 等待端口就绪
来源：http://hz.shuidangran.top/gtfqttnrvw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtazsdgbtd.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gtahnxuxtb.html

split -l 1000 big.log part_
来源：http://hz.meibo888.top/gtatoccksp.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gtifxbjdyj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gtbhtukrrs.html

[R75] 导出环境变量
来源：http://hz.jqgufenzy.top/gtervovwwf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.c1oappe.top/gtjdmpauyt.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtjomkmmng.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtoaijvdxb.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gthnofsfdw.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gteltieyxg.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtcnlixdak.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangtech.top/gtaksdgspo.html

[R79] 解析命令行选项
来源：http://hz.yueranfly.top/gtunxscgrf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtamjwlkmt.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gtdmqtmotd.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtitjvxfqo.html

================================================================================
来源：http://hz.guowangkeji.top/gttshgpvxm.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gtoqtnzwzz.html

================================================================================
来源：http://hz.tianlin.xyz/gtudvykvfb.html

[S01] C：Hello World
来源：http://hz.yonumen.top/gtfrhvbcbk.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtuinhvoew.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ybcxt.top/gtyqebswly.html

[S02] C：变量与格式化输出
来源：http://hz.wangshuangyany.cn/gthbdqsjlf.html

int a = 10; printf("%d\n", a);
来源：http://hz.iojbl.cn/gtvwrmirxl.html

[S03] C：读入整数
来源：http://hz.cdnleiting.top/gtbeuczait.html

int x; scanf("%d", &x);
来源：http://hz.hnqzz.top/gtexphmmmx.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtwercehrk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtkmjshpdn.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtddvapqow.html

strlen(s)
来源：http://hz.mhx1999.top/gtvgvcfkna.html

[S06] C：字符串比较
来源：http://hz.jinghuilouyu.cn/gthcsmbjzd.html

strcmp(a, b) == 0
来源：http://hz.chenjidiqi.icu/gtynlxuhsv.html

[S07] C：数组遍历求和
来源：http://hz.mhx1999.top/gtsbkhxqrl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xinyue.icu/gtylswidkj.html

[S08] C：动态内存分配与释放
来源：http://hz.jyoumei.cn/gtkbqsrcor.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtiamsyyvx.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gtdgwdyoqx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.andypj.xyz/gtwhcnlazc.html

[S10] C：指针与解引用
来源：http://hz.xinyue.icu/gtkzenlwiu.html

int *p = &a;  *p = 5;
来源：http://hz.hnqzz.top/gtryfnushd.html

[S11] C：逐行读文件
来源：http://hz.gaohongyu789.top/gttywfbkja.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtrrijgutf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangtech.top/gtmdvznthd.html

fclose(f);
来源：http://hz.zhiwuduotai.top/gtiejcrvci.html

[S12] C：写文件
来源：http://hz.hysaishi.cn/gtxgdijaps.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sweek.top/gtvzfxwgld.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gteyestzws.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258888.top/gtyujcryez.html

[S14] C：枚举
来源：http://hz.yonumen.top/gtwclhgjnm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hongshengwenyu.top/gttcjewjwa.html

[S15] C：类型转换
来源：http://hz.chenjidiqi.icu/gtwjrvtseb.html

(double) a / b
来源：http://hz.daria6918.cn/gtkcbnoqkz.html

[S16] C：位操作置位
来源：http://hz.dianchejie.cn/gtktavumgz.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtqskfrhmz.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtmuihvues.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtverugqvv.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtipwqqsgf.html

int main(int argc, char **argv)
来源：http://hz.zhengqikj.top/gtteiqjxmk.html

[S19] C：快速排序
来源：http://hz.zycfv.cn/gtwefhgmrb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xylfe.cn/gtfecxfjof.html

[S20] C：二分查找
来源：http://hz.gotoacloud.top/gtljsiajcb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtrqwgotqx.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtgfqssopd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cashguo.top/gtejuuyjpp.html

[S22] C：字符串转数字
来源：http://hz.snrcjt.cn/gtqvvitsnx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtimyerbxt.html

[S23] C：随机数
来源：http://hz.zhongyouzk.top/gtsxvlifai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jyoumei.cn/gtwvmtubov.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtrfvyifsw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtmpekradd.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gtdnaanzqi.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gthyeiaemn.html

[S26] C：内存清零
来源：http://hz.shzxlz.cn/gtmeamwljm.html

memset(a, 0, sizeof a);
来源：http://hz.quarkkingdee.top/gtqgppaozp.html

[S27] C：定义常量
来源：http://hz.gaohongyu789.top/gtfdlfaduv.html

const double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtcqkztcmv.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtjvyfrczp.html

static int counter = 0;
来源：http://hz.sufxvd.cn/gtqsirvxwh.html

[S29] C：变参函数
来源：http://hz.xziqi.cn/gtovbghgas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nwbrower.top/gtxyoxqutc.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gtnxqzmxus.html

#ifndef X_H
来源：http://hz.dashuyun.cn/gtsvrhebyy.html

#define X_H
来源：http://hz.zhijiandao.cn/gtytpeqdpp.html

#endif
来源：http://hz.yangfankeji.com/gtkbkepumi.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gtbuhdnnae.html

#include <iostream>
来源：http://hz.nanxuanxn.top/gtlpumpcje.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtxelefbzz.html

[S32] C++：字符串
来源：http://hz.yvedp.cn/gtczgxhhpm.html

std::string s = "hi";  s += "!";
来源：http://hz.nanxuanxn.top/gtnrmwlemq.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtbnrrekcw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yueranfly.top/gtrqkhimlw.html

[S34] C++：遍历 vector
来源：http://hz.sweek.top/gttbetobnl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gtldcmdeyf.html

[S35] C++：map
来源：http://hz.gotoacloud.top/gtcynrxbad.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gttxxadqhs.html

[S36] C++：unordered_map
来源：http://hz.dianchejie.cn/gtxzmijywk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gttsaqketd.html

[S37] C++：set
来源：http://hz.yj20258888.top/gttopljudz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cqqwz.cn/gtaznddqta.html

[S38] C++：排序
来源：http://hz.andypj.xyz/gtphejdpoh.html

std::sort(v.begin(), v.end());
来源：http://hz.jyoumei.cn/gtiilctbnk.html

[S39] C++：自定义比较器排序
来源：http://hz.sufxvd.cn/gtvsniqcpv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtwgxqjvtf.html

[S40] C++：查找元素
来源：http://hz.cqqwz.cn/gtddlzuzpo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.c1oappe.top/gttrhoaudf.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtwffraepz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuanzhike.top/gtylquncnc.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtnhqxxgmo.html

class B : public Base { public: void f() override {} };
来源：http://hz.cheryme.top/gtmsmrncxs.html

[S43] C++：智能指针
来源：http://hz.cdnleiting.top/gttijyphyg.html

auto p = std::make_unique<int>(5);
来源：http://hz.ywan-chungtsiang.top/gtcledsymz.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtdyixigqv.html

void inc(int &x) { ++x; }
来源：http://hz.tanke756.top/gtmuaamexu.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtakmedoho.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangdashe.top/gtmraojkip.html

[S46] C++：函数模板
来源：http://hz.kuanghao11.cn/gtgrweehnk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuetiantiany.cn/gtjfqthsgk.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtydauyrfd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtiadjlazj.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtlihpkugv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cheryme.top/gtthkkujuq.html

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtpemlqpdg.html

[S49] C++：写文件
来源：http://hz.yj20258.top/gthvsuhsjg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xuanzx.com/gtqgoyawjb.html

[S50] C++：格式化数字
来源：http://hz.ybcxt.top/gtdbtzaszo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yvedp.cn/gtmiykftrg.html

[S51] C++：显式类型转换
来源：http://hz.zycfv.cn/gthbecscht.html

static_cast<double>(a) / b
来源：http://hz.yvedp.cn/gtqgwzhmqu.html

[S52] C++：const 与 noexcept
来源：http://hz.xylfe.cn/gtxplxyynh.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtlufpxdze.html

[S53] C++：移动语义
来源：http://hz.cheryme.top/gtfzwigbcm.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtbiwnayru.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtwyxfkmts.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dianchejie.cn/gtygjqsedr.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtzwjougkj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhengqikj.top/gtjcqburur.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gtoqoaealv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.iojbl.cn/gtdvpmziec.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtffxoosmd.html

constexpr int N = 10;
来源：http://hz.yj20258.top/gtxddfunbl.html

[S58] C++：命名空间
来源：http://hz.c1oappe.top/gttpeydaiw.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtojcuygpj.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtqwpsgruc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtvfwtdhht.html

[S60] C++：遍历并删除元素
来源：http://hz.hfpthk.cn/gtlsngkbou.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtbzpxjmtt.html

================================================================================
来源：http://hz.bjfxy.top/gtqsssscin.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtzwazruus.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpijspybr.html

[T01] Kotlin：Hello World
来源：http://hz.zdqjudy.top/gtgldjcmcs.html

println("Hello")
来源：http://hz.dashuyun.cn/gtidmkzdvo.html

[T02] Kotlin：变量
来源：http://hz.yj20258.top/gtbexrmkqz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxinkj.top/gthuaidajl.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtdhfosflp.html

"值: $b"
来源：http://hz.hywenlv.cn/gtjaevshoa.html

[T04] Kotlin：空安全
来源：http://hz.nanxuanxn.top/gtpvcvbfez.html

val n: String? = null;  n?.length
来源：http://hz.shanyushiyangtech.top/gtxikjuihi.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigufen.top/gtqhqvvjfd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtfnbozwcn.html

[T06] Kotlin：集合映射
来源：http://hz.yj202588.top/gtmhxcozyi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gtijyibfqw.html

[T07] Kotlin：集合过滤
来源：http://hz.havefunace.top/gthvtiaavx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtdlmcchsw.html

[T08] Kotlin：数据类
来源：http://hz.c1oappe.top/gtmtxottvu.html

data class User(val name: String, val age: Int)
来源：http://hz.yanxiufei.cn/gtazkhgcap.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtzmxnapks.html

fun String.exclaim() = this + "!"
来源：http://hz.xingfuxueyuan.xyz/gtubfrlfue.html

[T10] Kotlin：默认参数
来源：http://hz.gotoacloud.top/gtuhxsduso.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuetiantiany.cn/gtthcdrksw.html

[T11] Kotlin：协程
来源：http://hz.zhiwuduotai.top/gtxhhklgif.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgfzy.top/gtovbyfkwe.html

[T12] Kotlin：解构声明
来源：http://hz.zhongyouzk.top/gtspvvwsgv.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtzkeqkbnf.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtyyyaodow.html

val m = mapOf("a" to 1)
来源：http://hz.hywenlv.cn/gtbsxbzemx.html

[T14] Kotlin：循环
来源：http://hz.xuanzx.com/gthttnvxqs.html

for (i in 1..10) println(i)
来源：http://hz.yanxiufei.cn/gtbfvffken.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gtzruqbuhh.html

interface Shape { fun area(): Double }
来源：http://hz.jinghuilouyu.cn/gtjexqboys.html

[T16] Swift：Hello World
来源：http://hz.sweek.top/gtcfupxdcx.html

print("Hello")
来源：http://hz.birdmap.top/gtxltcqqxl.html

[T17] Swift：变量与常量
来源：http://hz.yueranfly.top/gtlamwkfhj.html

var a = 1;  let b = 2
来源：http://hz.feifeiyinyue.top/gthuovdhcz.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtdjnfysoc.html

"值: \(b)"
来源：http://hz.ydzc1.top/gtfdvbcpqz.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtvszghvrl.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtmzbvjvfi.html

[T20] Swift：数组操作
来源：http://hz.xingfuxueyuan.xyz/gtpupuhily.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nwbrower.top/gtpmlwxuzw.html

[T21] Swift：遍历
来源：http://hz.yongpay.top/gtscukxutx.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtvkcwgrkj.html

[T22] Swift：字典
来源：http://hz.ivvv.top/gtegdcrsrm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.wangshuangyany.cn/gtiieasgyw.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gtxhmjdcyn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydjk.org.cn/gtittsnula.html

[T24] Swift：闭包
来源：http://hz.pycfn.com/gtgzmeahcb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.c1oappe.top/gtkwvlssqt.html

[T25] Swift：结构体
来源：http://hz.xuanzx.com/gtaunzbnny.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtfcvlxrwa.html

[T26] Swift：类与重写
来源：http://hz.yj202588.top/gtmjfxxbzv.html

class A: Base { override func f() {} }
来源：http://hz.aizwys.cn/gtktnopjzc.html

[T27] Swift：错误处理
来源：http://hz.zhongyouzk.top/gtklrnnkfc.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gteydojabx.html

[T28] Swift：枚举
来源：http://hz.dianchejie.cn/gttftjpjgy.html

enum Color { case red, green }
来源：http://hz.ivvv.top/gtrkkmqlyh.html

[T29] Swift：guard 提前返回
来源：http://hz.dashuyun.cn/gtpzygyeux.html

guard let x = opt else { return }
来源：http://hz.jqgufenzy.top/gtdksjwnzf.html

[T30] Swift：协议
来源：http://hz.meibo888.top/gtdqeeaizb.html

protocol Shape { func area() -> Double }
来源：http://hz.xuanzx.com/gtyritgfqh.html

[T31] Lua：Hello World
来源：http://hz.hfpthk.cn/gtaijzhslw.html

print("Hello")
来源：http://hz.hnxiangtu.top/gtvvswvjhz.html

[T32] Lua：局部变量
来源：http://hz.dashuyun.cn/gtapxvdsse.html

local a = 1
来源：http://hz.tianlin.xyz/gtubxnsggh.html

[T33] Lua：表（数组）
来源：http://hz.svipenyu.cn/gtdyehitxr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yonumen.top/gtxoejfjzu.html

[T34] Lua：遍历表
来源：http://hz.yonumen.top/gtydhtfmtz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tianlin.xyz/gtgvbxmhju.html

[T35] Lua：字典表
来源：http://hz.daxiang520.top/gtvknoqsch.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cdnleiting.top/gtgopsvyyh.html

[T36] Lua：函数
来源：http://hz.smart0.xyz/gturqqufre.html

function add(a, b) return a + b end
来源：http://hz.9152youxi.cn/gtvrmtvvia.html

[T37] Lua：字符串拼接
来源：http://hz.nwbrower.top/gtthnxfnuk.html

"a" .. "b"
来源：http://hz.yangfankeji.com/gtcyzmfgbk.html

[T38] Lua：条件
来源：http://hz.jqgfzy.top/gtnvnthrtf.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gtwazwfccw.html

[T39] Lua：模式匹配
来源：http://hz.zycfv.cn/gtrtbkgjbz.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtdlyrzpbq.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtbhttkojg.html

setmetatable({}, { __index = base })
来源：http://hz.yuxming.cn/gtjfksfseq.html

[T41] Perl：Hello World
来源：http://hz.hongshengwenyu.top/gtsmbnkngn.html

print "Hello\n";
来源：http://hz.bjfxy.top/gtcpsjijsn.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gtkomvwfco.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hongshengwenyu.top/gteteemomr.html

[T43] Perl：字符串插值
来源：http://hz.nwbrower.top/gthfubdllw.html

"值: $a"
来源：http://hz.cdnleiting.top/gtnycadbol.html

[T44] Perl：条件
来源：http://hz.smart0.xyz/gtleseespn.html

if ($a > 0) { print "正"; }
来源：http://hz.havefunace.top/gtvhcqxdju.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtophvcxbs.html

for my $x (@arr) { print $x; }
来源：http://hz.tian-w.cn/gtvtjfrnrl.html

[T46] Perl：哈希操作
来源：http://hz.daxiang520.top/gtxwcvpdzq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aibaodan.cn/gtaovpmhox.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangkeji.top/gtynvwvzdh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xingfuxueyuan.xyz/gtravxmexg.html

[T48] Perl：正则替换
来源：http://hz.yuanzhike.top/gtepkbglof.html

$s =~ s/old/new/g;
来源：http://hz.jqgfzy.top/gtulpoeunv.html

[T49] Perl：函数
来源：http://hz.zhengqikj.top/gtunxxtvig.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ehwqpu.com/gthiwfluik.html

[T50] Perl：逐行读文件
来源：http://hz.xziqi.cn/gtrrtsiapj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhixingplan.top/gtimbohmaz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gtdaejqoae.html

[T51] Scala：Hello World
来源：http://hz.mhx1999.top/gtzwjkwahk.html

println("Hello")
来源：http://hz.yvedp.cn/gtdqsxzglj.html

[T52] Scala：变量
来源：http://hz.jlsjyb.cn/gtfjzlkrmh.html

val a = 1;  var b = 2
来源：http://hz.cheryme.top/gtcgsnburp.html

[T53] Scala：字符串插值
来源：http://hz.0kj1m.cn/gtccelitgz.html

s"值: $b"
来源：http://hz.yj20258888.top/gtcfndzcpt.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gttgtrmrbu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jlsjyb.cn/gtouteeddb.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gtymkaaggg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sysykeji.top/gtngpxxwcz.html

[T56] Scala：样例类
来源：http://hz.9152youxi.cn/gtlzyrwenk.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtgumfqksa.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtyokddfax.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gogol.net.cn/gtfrrwbvbm.html

[T58] Scala：函数定义
来源：http://hz.hammf.cn/gtivafyobp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtkffkgtht.html

[T59] Scala：循环
来源：http://hz.guowangkeji.top/gtbkrwjrhz.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhengqikj.top/gtfxivnhfq.html

[T60] Scala：折叠
来源：http://hz.zhongyouzk.top/gtdsupkxbp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hammf.cn/gtnhgmkkjs.html

================================================================================
来源：http://hz.chenlongwang.top/gtvnmsacwm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ywan-chungtsiang.top/gttrucqdse.html

================================================================================
来源：http://hz.sweek.top/gtofvhvtvp.html

[U01] Py：创建虚拟环境
来源：http://hz.zhijiandao.cn/gtgpasrgae.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aizwys.cn/gtjfzkmyzc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hywenlv.cn/gtpirkumib.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aibaodan.cn/gtszvlbawr.html

[U03] Py：加载 .env 配置
来源：http://hz.52xcode.cn/gtdyxapeyb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenjidiqi.icu/gtedmcezmu.html

[U04] Py：变量调试打印
来源：http://hz.zhiwuduotai.top/gteijfdrgg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gtvyghtizn.html

[U05] Py：列表去重且保序
来源：http://hz.sxryk.cn/gtrnfswceu.html

list(dict.fromkeys(arr))
来源：http://hz.dashuyun.cn/gtcpsjqict.html

[U06] Py：合并两个字典
来源：http://hz.wangshuangyany.cn/gtitncyitb.html

{**a, **b}
来源：http://hz.cashguo.top/gtwnspkdvj.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gtnseoyfqf.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gtoumbztrb.html

[U08] Py：展平二维列表
来源：http://hz.feifeiyinyue.top/gtfpgdcmdv.html

[y for x in nested for y in x]
来源：http://hz.0kj1m.cn/gtzgekpedo.html

[U09] Py：字典取最大值的键
来源：http://hz.52xcode.cn/gtalyjycsp.html

max(d, key=d.get)
来源：http://hz.ydjk.org.cn/gtcchvcbmj.html

[U10] Py：按值排序字典
来源：http://hz.haohaochexian.top/gtjcipjpta.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gotoacloud.top/gtctvurwdb.html


<!-- 参考信息 -->