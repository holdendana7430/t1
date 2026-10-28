代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gtdatsdnyn.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtvskhehqw.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtwufzfobc.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtdtteadiu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.svipenyu.cn/gtwcclsbzn.html

[R72] 等待端口就绪
来源：http://hz.hysaishi.cn/gtiefqwtqd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtrohgteyv.html

[R73] 分割大日志
来源：http://hz.ydzc1.top/gtopjaloni.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtyeeoommo.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtuxerhojy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigfzy.top/gtoszkbipl.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtpnmmatiw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgfzy.top/gtbjvklzfu.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtaswqxxje.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtidoqnhpt.html

[R77] 读取用户输入
来源：http://hz.c1oappe.top/gtavrgjpzi.html

read -rp "请输入: " ans
来源：http://hz.cheryme.top/gthxmzticq.html

[R78] 交互式菜单
来源：http://hz.kuanghao11.cn/gtejrfhyld.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gogol.net.cn/gtelnxldbk.html

[R79] 解析命令行选项
来源：http://hz.mhx1999.top/gtmuaahewk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtufkjygwx.html

[R80] 查看脚本执行耗时
来源：http://hz.gaohongyu789.top/gthqiylubq.html

time ./run.sh
来源：http://hz.ydzc1.top/gtfpclzduh.html

================================================================================
来源：http://hz.xziqi.cn/gttcnxfdes.html

S. C / C++ 专题
来源：http://hz.hammf.cn/gtiavgwhnr.html

================================================================================
来源：http://hz.yanxiufei.cn/gttqmoqeim.html

[S01] C：Hello World
来源：http://hz.zhaomingkeji.xyz/gttztblxfb.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtynponenu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.quarkkingdee.top/gtzpuwpzgj.html

[S02] C：变量与格式化输出
来源：http://hz.zhijiandao.cn/gtzpyxvnze.html

int a = 10; printf("%d\n", a);
来源：http://hz.gaohongyu789.top/gttxecmkgy.html

[S03] C：读入整数
来源：http://hz.nwbrower.top/gtttucwkku.html

int x; scanf("%d", &x);
来源：http://hz.yanxiufei.cn/gtefocbigf.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtwzjdbhie.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtecvccryz.html

[S05] C：字符串长度
来源：http://hz.zhiwuduotai.top/gtxpcrcwtu.html

strlen(s)
来源：http://hz.52xcode.cn/gtsinopevz.html

[S06] C：字符串比较
来源：http://hz.yanxiufei.cn/gtmmvfamzn.html

strcmp(a, b) == 0
来源：http://hz.pengpengdd.cyou/gtulirpblu.html

[S07] C：数组遍历求和
来源：http://hz.ywan-chungtsiang.top/gtomragggb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtaqspwoae.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtkslvwdlc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtfuonenap.html

[S09] C：结构体定义与初始化
来源：http://hz.zhongyouzk.top/gtbhczpene.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtrrburscd.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtfudmswmh.html

int *p = &a;  *p = 5;
来源：http://hz.daxiang520.top/gtlgdywgbe.html

[S11] C：逐行读文件
来源：http://hz.tianlin.xyz/gtylcuoqmy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xinyue.icu/gtrxlcttll.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hongshengwenyu.top/gtjjitgqyh.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtjcvpoifd.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtojgjjrho.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gthwrioeyf.html

[S13] C：宏定义
来源：http://hz.wangshuangyany.cn/gtuzkvomjq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.feifeiyinyue.top/gtixipdbxs.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtwyrupgfb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xylfe.cn/gtwqabeyws.html

[S15] C：类型转换
来源：http://hz.yj20258888.top/gtvbojslkg.html

(double) a / b
来源：http://hz.ivvv.top/gtojazdbsw.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtzrrzveut.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtthvqbjpy.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtrolfpnzm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtjlgyamkq.html

[S18] C：命令行参数
来源：http://hz.zdqjudy.top/gtxqzjscmo.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gtepvgvpfb.html

[S19] C：快速排序
来源：http://hz.fengsongda.top/gtlkoehqbq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtrmoqmdjb.html

[S20] C：二分查找
来源：http://hz.xuetiantiany.cn/gtpddanfem.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtrytjczsq.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gttlfabsbc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtdzvbjsmk.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gtqndunhko.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gtzivvirsp.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtodurmfon.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.aibaodan.cn/gtfdwmjjnq.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtymalyzjw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtaqsrdmia.html

[S25] C：内存拷贝
来源：http://hz.hysaishi.cn/gtoyllwgib.html

memcpy(dst, src, n);
来源：http://hz.zhaomingkeji.xyz/gthltsheci.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gtvwjhpfrj.html

memset(a, 0, sizeof a);
来源：http://hz.yuxming.cn/gtpwcxvtdm.html

[S27] C：定义常量
来源：http://hz.nanxinkj.top/gtfcmjekki.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtqulfgcas.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtbobpovlk.html

static int counter = 0;
来源：http://hz.hywenlv.cn/gtdsbkxnqm.html

[S29] C：变参函数
来源：http://hz.jyoumei.cn/gtztfbvkbu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtcmhdiabb.html

[S30] C：头文件保护
来源：http://hz.ybcxt.top/gtzvbkinub.html

#ifndef X_H
来源：http://hz.c1oappe.top/gtklbturzs.html

#define X_H
来源：http://hz.andypj.xyz/gtwgqwfitk.html

#endif
来源：http://hz.yj20258.top/gthbbwkthn.html

[S31] C++：Hello World
来源：http://hz.jianghu66.top/gtjrwtzqtj.html

#include <iostream>
来源：http://hz.kuanghao11.cn/gtxfgdtgct.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtxfdbapry.html

[S32] C++：字符串
来源：http://hz.yvedp.cn/gtqwsjkmje.html

std::string s = "hi";  s += "!";
来源：http://hz.cqqwz.cn/gtirgnlzvu.html

[S33] C++：vector 增删
来源：http://hz.yongpay.top/gtfkvvsoaq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhaomingkeji.xyz/gtetpmzjcf.html

[S34] C++：遍历 vector
来源：http://hz.cdnleiting.top/gtqbascpzv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinyuanbaomall.cn/gtmxgzsxgu.html

[S35] C++：map
来源：http://hz.shangyingyoupin.top/gtdfwuckui.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtjxcmbzob.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtxrcqcpaj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtbcwpkewn.html

[S37] C++：set
来源：http://hz.yj202588.top/gthinxbqdl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtxduaicnv.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtcsxjoecw.html

std::sort(v.begin(), v.end());
来源：http://hz.zhixingplan.top/gtkpetlfvt.html

[S39] C++：自定义比较器排序
来源：http://hz.yvedp.cn/gtbqfmsihd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtgdatoqoj.html

[S40] C++：查找元素
来源：http://hz.aizwys.cn/gtnvbdxtcb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtendmoann.html

[S41] C++：类与构造函数
来源：http://hz.cqqwz.cn/gtqhrkohhi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sxryk.cn/gtgiqepvip.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtzejgoesz.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtwstmwmda.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtjunzbtns.html

auto p = std::make_unique<int>(5);
来源：http://hz.ppjwa.cn/gtwuxnqlpa.html

[S44] C++：引用传参
来源：http://hz.zhoulong.xyz/gtvcpbbveq.html

void inc(int &x) { ++x; }
来源：http://hz.xziqi.cn/gtwftlywxl.html

[S45] C++：lambda
来源：http://hz.ivvv.top/gtglydvfcz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtskjwqhdk.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gthgsolega.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtggocdclt.html

[S47] C++：结构化绑定遍历
来源：http://hz.xinyue.icu/gtnozrkzlj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.snrcjt.cn/gtoepcfyzk.html

[S48] C++：逐行读文件
来源：http://hz.jinqigfzy.top/gthrcvzxsr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gteufijicm.html

while (std::getline(in, line)) { }
来源：http://hz.aibaodan.cn/gtuzzcjnjb.html

[S49] C++：写文件
来源：http://hz.ydjk.org.cn/gtrjybuwuj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenzaomai.com/gtbjzsgghy.html

[S50] C++：格式化数字
来源：http://hz.svipenyu.cn/gtautoavcf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhengqikj.top/gtnxkyftlo.html

[S51] C++：显式类型转换
来源：http://hz.feifeiyinyue.top/gtvrottswl.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtjsmatohx.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtuucdxplc.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtcydaopjq.html

[S53] C++：移动语义
来源：http://hz.yj202588.top/gthisqhxts.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtjttfheuc.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gtaooaoqki.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gtmknmdzft.html

[S55] C++：结构化绑定
来源：http://hz.andypj.xyz/gtllbpsrkj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.birdmap.top/gtktbwaibo.html

[S56] C++：optional
来源：http://hz.ydzc1.top/gtpsairlra.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.birdmap.top/gtlnbdhkxo.html

[S57] C++：编译期常量
来源：http://hz.dianchejie.cn/gtaeyrrmec.html

constexpr int N = 10;
来源：http://hz.guannengcc.top/gtozmjmyya.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gtqvzossmu.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gtjqxnxvwm.html

[S59] C++：静态断言
来源：http://hz.havefunace.top/gtxldhofmu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtbzsbhtsa.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtegrusoib.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gtohkzcwqd.html

================================================================================
来源：http://hz.xziqi.cn/gtamljqohx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gttrmnnhys.html

================================================================================
来源：http://hz.guowangkeji.top/gttiyetugq.html

[T01] Kotlin：Hello World
来源：http://hz.nwbrower.top/gtcgrxjxzz.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtwhefzrwm.html

[T02] Kotlin：变量
来源：http://hz.guowangkeji.top/gtjqhqrbqe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgufenzy.top/gtjhrrlbct.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258888.top/gttlvgiawj.html

"值: $b"
来源：http://hz.guowangkeji.top/gtaxsnoloy.html

[T04] Kotlin：空安全
来源：http://hz.jqgufenzy.top/gtxriamvlu.html

val n: String? = null;  n?.length
来源：http://hz.yueranfly.top/gtfiteqjsp.html

[T05] Kotlin：when 表达式
来源：http://hz.chenzaomai.com/gttuclgdoa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtlrblknnq.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtuudkpbnh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gtmoyzvdxt.html

[T07] Kotlin：集合过滤
来源：http://hz.yueranfly.top/gtffqnnaly.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ywan-chungtsiang.top/gtxjciyiyj.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtgqsidsjp.html

data class User(val name: String, val age: Int)
来源：http://hz.ybcxt.top/gtoafbwykb.html

[T09] Kotlin：扩展函数
来源：http://hz.jianghu66.top/gtpuozbheg.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtuurofbzu.html

[T10] Kotlin：默认参数
来源：http://hz.jyoumei.cn/gtnmtyhddk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.havefunace.top/gteoxaigaj.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtkucsjwwt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cqqwz.cn/gtlvgbfena.html

[T12] Kotlin：解构声明
来源：http://hz.hnqzz.top/gtrscnnrww.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtcbgwjcth.html

[T13] Kotlin：只读 Map
来源：http://hz.ehwqpu.com/gtqnsocwul.html

val m = mapOf("a" to 1)
来源：http://hz.ywan-chungtsiang.top/gtxnbwjtoq.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gtukhsiiud.html

for (i in 1..10) println(i)
来源：http://hz.hfpthk.cn/gtjypdcsxs.html

[T15] Kotlin：接口
来源：http://hz.ydzc1.top/gtfvwsftix.html

interface Shape { fun area(): Double }
来源：http://hz.nanxuanxn.top/gtgndnkyhp.html

[T16] Swift：Hello World
来源：http://hz.aizwys.cn/gtlpdgtwgr.html

print("Hello")
来源：http://hz.jyoumei.cn/gtpcbgvkik.html

[T17] Swift：变量与常量
来源：http://hz.ppjwa.cn/gtwmbnzzan.html

var a = 1;  let b = 2
来源：http://hz.hnqzz.top/gtpljmmcgc.html

[T18] Swift：字符串插值
来源：http://hz.c1oappe.top/gtpamlmzvu.html

"值: \(b)"
来源：http://hz.daxiang520.top/gtthzrjmky.html

[T19] Swift：可选绑定
来源：http://hz.svipenyu.cn/gtznlvaetd.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangkeji.top/gtflfgyqht.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtoqnulmqo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hfpthk.cn/gtybzpdsfd.html

[T21] Swift：遍历
来源：http://hz.jinqigfzy.top/gtkfxztcqa.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtbzsewgkt.html

[T22] Swift：字典
来源：http://hz.jinqigfzy.top/gtjutdaqfo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.quarkkingdee.top/gtjisrklos.html

[T23] Swift：函数
来源：http://hz.kuanghao11.cn/gtxqhvrrdq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhengqikj.top/gtdhlbapey.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gtwjxtyfgi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtivozzkvg.html

[T25] Swift：结构体
来源：http://hz.jiagoushi.top/gtouvllfru.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gtqcfkeidy.html

[T26] Swift：类与重写
来源：http://hz.nwbrower.top/gtkymrvacn.html

class A: Base { override func f() {} }
来源：http://hz.fzhhl.top/gtmrlevopr.html

[T27] Swift：错误处理
来源：http://hz.chenjidiqi.icu/gtrxqmaipv.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gticzzlyni.html

[T28] Swift：枚举
来源：http://hz.dashuyun.cn/gtjkwqtqgj.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtryqnchhj.html

[T29] Swift：guard 提前返回
来源：http://hz.xuanzx.com/gtrlvafmka.html

guard let x = opt else { return }
来源：http://hz.gotoacloud.top/gtqjacbcvp.html

[T30] Swift：协议
来源：http://hz.fengsongda.top/gtpouzrbnq.html

protocol Shape { func area() -> Double }
来源：http://hz.birdmap.top/gtuygaminl.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gtdbpgwehy.html

print("Hello")
来源：http://hz.52xcode.cn/gtbsphlelj.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtdrlnthyo.html

local a = 1
来源：http://hz.wangdashe.top/gtbcrfxrwg.html

[T33] Lua：表（数组）
来源：http://hz.tanke756.top/gtpuuexsae.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ivvv.top/gthvhofcsv.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtgehjdykl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jyoumei.cn/gtezyqmqnd.html

[T35] Lua：字典表
来源：http://hz.aibaodan.cn/gtyjqjocvm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.vqdsnc.cn/gtmsifaobd.html

[T36] Lua：函数
来源：http://hz.jqgfzy.top/gtuqvkuosi.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtokhojjna.html

[T37] Lua：字符串拼接
来源：http://hz.gotoacloud.top/gtyhvvsaza.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtzchhebrx.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gtllukhskf.html

if x > 0 then print("正") end
来源：http://hz.gaohongyu789.top/gtqcxggiux.html

[T39] Lua：模式匹配
来源：http://hz.yanxiufei.cn/gtxpdxpyhl.html

string.find(s, "%d+")
来源：http://hz.bjfxy.top/gteqjeisdj.html

[T40] Lua：元表
来源：http://hz.nwbrower.top/gtudhgrfcm.html

setmetatable({}, { __index = base })
来源：http://hz.fengsongda.top/gtpkfpjjbk.html

[T41] Perl：Hello World
来源：http://hz.xylfe.cn/gtcxbdkbkm.html

print "Hello\n";
来源：http://hz.shzxlz.cn/gttaxxyjfe.html

[T42] Perl：变量类型
来源：http://hz.cdnleiting.top/gtrukivjgr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj202588.top/gtngnvmsbp.html

[T43] Perl：字符串插值
来源：http://hz.xinyue.icu/gtyrxhkfhq.html

"值: $a"
来源：http://hz.yueranfly.top/gthqilguhp.html

[T44] Perl：条件
来源：http://hz.aizwys.cn/gtuplidcnu.html

if ($a > 0) { print "正"; }
来源：http://hz.hnqzz.top/gtprxsbmhg.html

[T45] Perl：数组遍历
来源：http://hz.zhiwuduotai.top/gtxpatujkx.html

for my $x (@arr) { print $x; }
来源：http://hz.chenlongwang.top/gtwpdubcge.html

[T46] Perl：哈希操作
来源：http://hz.birdmap.top/gtlbjjszqh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.c1oappe.top/gttjhaigkc.html

[T47] Perl：正则捕获
来源：http://hz.xuanzx.com/gtxhhdrptw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydjk.org.cn/gthgsetoof.html

[T48] Perl：正则替换
来源：http://hz.shanyushiyangkeji.top/gtbztjziyn.html

$s =~ s/old/new/g;
来源：http://hz.hnqzz.top/gtbnpkxjnf.html

[T49] Perl：函数
来源：http://hz.redwolf501.top/gtbwktedwb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtjgnhaood.html

[T50] Perl：逐行读文件
来源：http://hz.52xcode.cn/gtstluljln.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.fengsongda.top/gtjyhiqbjg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhiwuduotai.top/gtrmsaimkq.html

[T51] Scala：Hello World
来源：http://hz.ivvv.top/gtbwfukaqo.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtldyterdl.html

[T52] Scala：变量
来源：http://hz.tanke756.top/gtrydptmru.html

val a = 1;  var b = 2
来源：http://hz.cashguo.top/gtvpelcuci.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtfneqvlkj.html

s"值: $b"
来源：http://hz.hnxiangtu.top/gtamzdydgv.html

[T54] Scala：集合映射
来源：http://hz.chenlongwang.top/gttbptotip.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aibaodan.cn/gtrfrosdez.html

[T55] Scala：集合过滤
来源：http://hz.nanxuanxn.top/gtnzearqig.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cashguo.top/gtlpeslvns.html

[T56] Scala：样例类
来源：http://hz.zhiwuduotai.top/gtrasumqxe.html

case class User(name: String, age: Int)
来源：http://hz.52xcode.cn/gtdmmfwawk.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gtvzcutelu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.vqdsnc.cn/gtiajqzrdx.html

[T58] Scala：函数定义
来源：http://hz.haohaochexian.top/gtmnekqiau.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cucudq.cn/gtqinvslka.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gtwigdfcoq.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtfuullbqu.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtgtgvstye.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xinyue.icu/gtypspxejq.html

================================================================================
来源：http://hz.dashuyun.cn/gtunofdcaa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xingfuxueyuan.xyz/gtrzcawikr.html

================================================================================
来源：http://hz.cqqwz.cn/gtxodgmcco.html

[U01] Py：创建虚拟环境
来源：http://hz.zdqjudy.top/gtdrqytqey.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.fzhhl.top/gtdrcyhjtq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydzc1.top/gtlximaglm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cashguo.top/gturlqljia.html

[U03] Py：加载 .env 配置
来源：http://hz.sufxvd.cn/gteluwvhyq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinqigfzy.top/gtoqxocpor.html

[U04] Py：变量调试打印
来源：http://hz.cheryme.top/gtomfjlcli.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuanzx.com/gtzrjtoguq.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtsaryryrb.html

list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtzebjrljh.html

[U06] Py：合并两个字典
来源：http://hz.bjfxy.top/gtbgcjfneu.html

{**a, **b}
来源：http://hz.gzhubu.top/gttfcjmwjl.html

[U07] Py：反转字典键值
来源：http://hz.yueranfly.top/gtqwcgglvi.html

{v: k for k, v in d.items()}
来源：http://hz.xingfuxueyuan.xyz/gtcdrcaznr.html

[U08] Py：展平二维列表
来源：http://hz.ydjk.org.cn/gtrxteeomc.html

[y for x in nested for y in x]
来源：http://hz.meibo888.top/gtiqhccuxv.html

[U09] Py：字典取最大值的键
来源：http://hz.iojbl.cn/gthvvnesxw.html

max(d, key=d.get)
来源：http://hz.gotoacloud.top/gtmcgjlhho.html

[U10] Py：按值排序字典
来源：http://hz.aibaodan.cn/gthvfvhxej.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jiagoushi.top/gtxvibnphx.html


<!-- 参考信息 -->