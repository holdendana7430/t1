代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtponmcygi.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtccdlscrm.html

date +%s;  date -d @1700000000
来源：http://hz.hammf.cn/gtjturxkaj.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gteaunukug.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtnrlzwqhq.html

[R72] 等待端口就绪
来源：http://hz.yvedp.cn/gtnrwytqrk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gtfahjprli.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gtdwxvmnfw.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtgdjjfnji.html

[R74] 批量重命名
来源：http://hz.yanxiufei.cn/gtwqkygrpj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pycfn.com/gtmvbpfktw.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtwutypcfl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtupemjsuz.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangkeji.top/gtnulmmcgp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtidkoardm.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtnmucclpk.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangkeji.top/gtsdzmseot.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtxsodfyrk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gtqwmeucau.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangtech.top/gtazdvpfjn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtrpprzsbr.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtbqsemrde.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtpdvqgnyk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfkczczny.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gtfgdkahap.html

================================================================================
来源：http://hz.ybcxt.top/gtsnzkbvcr.html

[S01] C：Hello World
来源：http://hz.52xcode.cn/gtjvzorzxr.html

#include <stdio.h>
来源：http://hz.cheryme.top/gtrxhfmctm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtexucbexd.html

[S02] C：变量与格式化输出
来源：http://hz.sysykeji.top/gtxrqjusko.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhoulong.xyz/gttoffktnx.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtfwxgnzqg.html

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtfcdbgpso.html

[S04] C：字符串复制
来源：http://hz.havefunace.top/gtfzaokcsk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gtbkdueooy.html

[S05] C：字符串长度
来源：http://hz.yj20258.top/gtnawbsqjb.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gtqaibjvwl.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gtlnwxsmfr.html

strcmp(a, b) == 0
来源：http://hz.guowangkeji.top/gthjhtfkbf.html

[S07] C：数组遍历求和
来源：http://hz.jlsjyb.cn/gtjvkpljkc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtklgsobje.html

[S08] C：动态内存分配与释放
来源：http://hz.hywenlv.cn/gtpocamfzd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangshuangyany.cn/gtfpncnjua.html

[S09] C：结构体定义与初始化
来源：http://hz.meibo888.top/gtvfweshld.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhaomingkeji.xyz/gthbyousjb.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtrnmrbmze.html

int *p = &a;  *p = 5;
来源：http://hz.jinghuilouyu.cn/gtmonblwuh.html

[S11] C：逐行读文件
来源：http://hz.cheryme.top/gtrsgghgtd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtlgjlxlos.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gotoacloud.top/gtjywhbjdc.html

fclose(f);
来源：http://hz.gzhubu.top/gtqfgijaxl.html

[S12] C：写文件
来源：http://hz.jinyuanbaomall.cn/gtkjnvhzfy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.smart0.xyz/gtrigddsbq.html

[S13] C：宏定义
来源：http://hz.ywan-chungtsiang.top/gthxpzbpms.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hysaishi.cn/gtsmvrodcq.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gttekdifzv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258888.top/gtxqyobdkt.html

[S15] C：类型转换
来源：http://hz.bjfxy.top/gtoqpjmaya.html

(double) a / b
来源：http://hz.yj202588.top/gtfpewcuvz.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gthtkxquyv.html

x |= (1 << 3);
来源：http://hz.zhengqikj.top/gtzmcweymc.html

[S17] C：安全拼接字符串
来源：http://hz.kuanghao11.cn/gtxtvapmqs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jyoumei.cn/gtuvzfliys.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gtgcfsftwm.html

int main(int argc, char **argv)
来源：http://hz.yuxming.cn/gtrsjppiha.html

[S19] C：快速排序
来源：http://hz.haohaochexian.top/gtqmtogvyr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtlomlzlxc.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gtcszvykrp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtgwzgbyyp.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtlgyfpiou.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gzhubu.top/gtmmicypiu.html

[S22] C：字符串转数字
来源：http://hz.sxryk.cn/gtrfelbysw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtaebpgsxk.html

[S23] C：随机数
来源：http://hz.gzhubu.top/gtyetwejma.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtzsjcifya.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtqaijvoft.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.havefunace.top/gtepheultd.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gthwpajbso.html

memcpy(dst, src, n);
来源：http://hz.fzhhl.top/gtxtrapjga.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtdreyuqmf.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtgunqxbyc.html

[S27] C：定义常量
来源：http://hz.shuidangran.top/gtxzoxdovt.html

const double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtpvuefgyh.html

[S28] C：静态变量
来源：http://hz.nanxinkj.top/gtwpqgztlw.html

static int counter = 0;
来源：http://hz.daria6918.cn/gtomxxgqqa.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtzsxkglas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.havefunace.top/gteyfgsbcg.html

[S30] C：头文件保护
来源：http://hz.hysaishi.cn/gtodohhhlv.html

#ifndef X_H
来源：http://hz.yj202588.top/gtmtznmrak.html

#define X_H
来源：http://hz.yongpay.top/gtnahavkfa.html

#endif
来源：http://hz.jlsjyb.cn/gtiefgwdvw.html

[S31] C++：Hello World
来源：http://hz.52xcode.cn/gteouzxaht.html

#include <iostream>
来源：http://hz.tanke756.top/gtpiuzjgdl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtdkmuszdl.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtxkgfpjgs.html

std::string s = "hi";  s += "!";
来源：http://hz.nwbrower.top/gteaudlkzc.html

[S33] C++：vector 增删
来源：http://hz.iojbl.cn/gtujkcflnn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ivvv.top/gtrzaxfyxz.html

[S34] C++：遍历 vector
来源：http://hz.yangfankeji.com/gtvufmmjtj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gtavmtbmdb.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtlzjdkdkg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtrjuxsnkw.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtckiotzri.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtwokeqlep.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtyatsvime.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cqqwz.cn/gtnftcarps.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtqrwathtc.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtmsqxrkbs.html

[S39] C++：自定义比较器排序
来源：http://hz.cqqwz.cn/gtokdtjgyx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.svipenyu.cn/gtbhfpncjr.html

[S40] C++：查找元素
来源：http://hz.cqqwz.cn/gtfhgzrqfl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtxfippvgy.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gthtvztqkb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gtwadvnxhw.html

[S42] C++：继承与虚函数
来源：http://hz.xuanzx.com/gtcbnzxpkr.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangshuangyany.cn/gtrntiijcy.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtzbcgvjjn.html

auto p = std::make_unique<int>(5);
来源：http://hz.jlsjyb.cn/gtkwjurksi.html

[S44] C++：引用传参
来源：http://hz.hywenlv.cn/gtphwxjnfc.html

void inc(int &x) { ++x; }
来源：http://hz.ydjk.org.cn/gtaavudgqn.html

[S45] C++：lambda
来源：http://hz.fzhhl.top/gtvxfghfsb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtirvowihn.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtcthejtmn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gtlytlavai.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtetctpiaj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sxryk.cn/gtcoodyljc.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gthvxhpmcc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gtraqgyyvn.html

while (std::getline(in, line)) { }
来源：http://hz.snrcjt.cn/gtjqgxqywn.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtotkvtptd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gtlfoftzst.html

[S50] C++：格式化数字
来源：http://hz.vqdsnc.cn/gtdgfmobde.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtnoakavth.html

[S51] C++：显式类型转换
来源：http://hz.hammf.cn/gtykhdrnsa.html

static_cast<double>(a) / b
来源：http://hz.jinqigfzy.top/gtugtdpluk.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtspvgrcyj.html

int size() const noexcept { return n_; }
来源：http://hz.sufxvd.cn/gtqspamjlg.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtydwyxyuj.html

std::vector<int> w = std::move(v);
来源：http://hz.nwbrower.top/gtjzpxnldv.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gtllmbpeqf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenzaomai.com/gtgtsfygsk.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtyrspvxpk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuetiantiany.cn/gtiutlsokw.html

[S56] C++：optional
来源：http://hz.feifeiyinyue.top/gttvmhprmj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtsoqmiivd.html

[S57] C++：编译期常量
来源：http://hz.shzxlz.cn/gtljssabyj.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtfcodjurc.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gtuxgumrjj.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenlongwang.top/gtagohvgqh.html

[S59] C++：静态断言
来源：http://hz.shzxlz.cn/gtyakezdgb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtzhtdajml.html

[S60] C++：遍历并删除元素
来源：http://hz.pengpengdd.cyou/gtamtvsarn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtneordijb.html

================================================================================
来源：http://hz.hnqzz.top/gtcknqqeoi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtgbuhsqjw.html

================================================================================
来源：http://hz.zhixingplan.top/gtvveigftu.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gthpulxugw.html

println("Hello")
来源：http://hz.sufxvd.cn/gtgroadysp.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtstuftmje.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gtqwlaggdu.html

[T03] Kotlin：字符串模板
来源：http://hz.svipenyu.cn/gtkwfwewoh.html

"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtpgslfjkw.html

[T04] Kotlin：空安全
来源：http://hz.pycfn.com/gteynlzpio.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtuybolryq.html

[T05] Kotlin：when 表达式
来源：http://hz.hnxiangtu.top/gtuvlczycw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gtlcujsgbr.html

[T06] Kotlin：集合映射
来源：http://hz.daria6918.cn/gttllrqvjc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtoqiabigv.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gtkhldiewe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhixingplan.top/gtahyclwkt.html

[T08] Kotlin：数据类
来源：http://hz.zycfv.cn/gtrknfsyai.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gtwzcxzzcj.html

[T09] Kotlin：扩展函数
来源：http://hz.cucudq.cn/gtekbioqdz.html

fun String.exclaim() = this + "!"
来源：http://hz.zhijiandao.cn/gtmlyoyrvr.html

[T10] Kotlin：默认参数
来源：http://hz.shangyingyoupin.top/gthrrclxgp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gthtaczgvl.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtgczkdwxp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.svipenyu.cn/gtnvseuhpt.html

[T12] Kotlin：解构声明
来源：http://hz.hammf.cn/gtgkxfxtbc.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gttwkzjrfx.html

[T13] Kotlin：只读 Map
来源：http://hz.guannengcc.top/gtndxsguzp.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gtglplvcge.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtjfiqpxsg.html

for (i in 1..10) println(i)
来源：http://hz.andypj.xyz/gtjshsyexv.html

[T15] Kotlin：接口
来源：http://hz.zhaomingkeji.xyz/gtirkexhld.html

interface Shape { fun area(): Double }
来源：http://hz.gzhubu.top/gtgjrmnpht.html

[T16] Swift：Hello World
来源：http://hz.tianlin.xyz/gtaedihyxo.html

print("Hello")
来源：http://hz.cheryme.top/gtzjedhney.html

[T17] Swift：变量与常量
来源：http://hz.yj202588.top/gtuhnszoby.html

var a = 1;  let b = 2
来源：http://hz.0kj1m.cn/gtttjtiita.html

[T18] Swift：字符串插值
来源：http://hz.svipenyu.cn/gtddrojfrj.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gtvzkumdmp.html

[T19] Swift：可选绑定
来源：http://hz.yuanzhike.top/gtzvjcjquj.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtmhtucltx.html

[T20] Swift：数组操作
来源：http://hz.zhixingplan.top/gttvpilmxl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gtqvqegyew.html

[T21] Swift：遍历
来源：http://hz.ivvv.top/gtdiiqwszr.html

for x in a { print(x) }
来源：http://hz.jianghu66.top/gthlaalqpr.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtiinzurzv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yangfankeji.com/gtccyfpdxk.html

[T23] Swift：函数
来源：http://hz.cdnleiting.top/gtqgeijtnb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtutadlmjp.html

[T24] Swift：闭包
来源：http://hz.ppjwa.cn/gtjmcrxlrg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gttltvtikp.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtgkgrtfah.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtpsdongly.html

[T26] Swift：类与重写
来源：http://hz.hnqzz.top/gtcrnqjokq.html

class A: Base { override func f() {} }
来源：http://hz.tian-w.cn/gtesfvwhcm.html

[T27] Swift：错误处理
来源：http://hz.shangyingyoupin.top/gtbfcpvgyv.html

do { try f() } catch { print(error) }
来源：http://hz.xuanzx.com/gtigewofjh.html

[T28] Swift：枚举
来源：http://hz.zycfv.cn/gtsivyrsma.html

enum Color { case red, green }
来源：http://hz.yuxming.cn/gtoffbqnro.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtfpkjnbdt.html

guard let x = opt else { return }
来源：http://hz.9152youxi.cn/gtjydzwzom.html

[T30] Swift：协议
来源：http://hz.haohaochexian.top/gtotwyqzhy.html

protocol Shape { func area() -> Double }
来源：http://hz.jinghuilouyu.cn/gtkxbwppcw.html

[T31] Lua：Hello World
来源：http://hz.yangfankeji.com/gtdnejofoe.html

print("Hello")
来源：http://hz.ydzc1.top/gtqpdbvqel.html

[T32] Lua：局部变量
来源：http://hz.iojbl.cn/gtmtysrnar.html

local a = 1
来源：http://hz.tian-w.cn/gtycrixbbn.html

[T33] Lua：表（数组）
来源：http://hz.aibaodan.cn/gtwmoeroxg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtjahjdkck.html

[T34] Lua：遍历表
来源：http://hz.shzxlz.cn/gtqrpzrgtt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj20258888.top/gtvhziorsw.html

[T35] Lua：字典表
来源：http://hz.jlsjyb.cn/gtxhgppdde.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenjidiqi.icu/gtwlijrfcl.html

[T36] Lua：函数
来源：http://hz.xylfe.cn/gtmzrcryyv.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtpqpbniyq.html

[T37] Lua：字符串拼接
来源：http://hz.ydjk.org.cn/gtbhfcvisa.html

"a" .. "b"
来源：http://hz.sweek.top/gtfzvxdltu.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gtyogehjjd.html

if x > 0 then print("正") end
来源：http://hz.zhoulong.xyz/gtmznxatfk.html

[T39] Lua：模式匹配
来源：http://hz.shangyingyoupin.top/gtqyiizcof.html

string.find(s, "%d+")
来源：http://hz.tianlin.xyz/gtoducmask.html

[T40] Lua：元表
来源：http://hz.yj20258888.top/gthleefuiz.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtnwxmbaie.html

[T41] Perl：Hello World
来源：http://hz.pycfn.com/gtorzoecoz.html

print "Hello\n";
来源：http://hz.guannengcc.top/gtxwfxnrpw.html

[T42] Perl：变量类型
来源：http://hz.daria6918.cn/gtbdacvixk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cqqwz.cn/gtjlkbuoik.html

[T43] Perl：字符串插值
来源：http://hz.tian-w.cn/gtbdvjabwx.html

"值: $a"
来源：http://hz.hongshengwenyu.top/gtmkybozha.html

[T44] Perl：条件
来源：http://hz.zhijiandao.cn/gtdbeelago.html

if ($a > 0) { print "正"; }
来源：http://hz.gogol.net.cn/gtpwqpkbsk.html

[T45] Perl：数组遍历
来源：http://hz.dashuyun.cn/gtnzhwnpeo.html

for my $x (@arr) { print $x; }
来源：http://hz.svipenyu.cn/gtukcnarzq.html

[T46] Perl：哈希操作
来源：http://hz.fzhhl.top/gtzbujoamy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnxiangtu.top/gtbqjyfstk.html

[T47] Perl：正则捕获
来源：http://hz.gzhubu.top/gthomzoeco.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xylfe.cn/gtotilhrlo.html

[T48] Perl：正则替换
来源：http://hz.gzhubu.top/gtrnrcobhs.html

$s =~ s/old/new/g;
来源：http://hz.mhx1999.top/gtlkspptlh.html

[T49] Perl：函数
来源：http://hz.bjfxy.top/gthlonamrv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtptjfqobk.html

[T50] Perl：逐行读文件
来源：http://hz.bjfxy.top/gtwsegyvif.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.haohaochexian.top/gtxyhttszu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangkeji.top/gtxslvufic.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtfxkhxrre.html

println("Hello")
来源：http://hz.andypj.xyz/gtjmwsvrys.html

[T52] Scala：变量
来源：http://hz.hysaishi.cn/gtqevsqhqk.html

val a = 1;  var b = 2
来源：http://hz.iojbl.cn/gtsvoqhnor.html

[T53] Scala：字符串插值
来源：http://hz.hnqzz.top/gttnhodchj.html

s"值: $b"
来源：http://hz.guannengcc.top/gtvoniqfsc.html

[T54] Scala：集合映射
来源：http://hz.sufxvd.cn/gtndiyufzt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.vqdsnc.cn/gtvtxhdvfc.html

[T55] Scala：集合过滤
来源：http://hz.jqgufenzy.top/gtchjkibzv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.bjfxy.top/gtwwaygdbp.html

[T56] Scala：样例类
来源：http://hz.ywan-chungtsiang.top/gtvfthwkpw.html

case class User(name: String, age: Int)
来源：http://hz.zhixingplan.top/gtzwlhffkj.html

[T57] Scala：模式匹配
来源：http://hz.hysaishi.cn/gtbuwpgqfb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gogol.net.cn/gtufsutxez.html

[T58] Scala：函数定义
来源：http://hz.tianlin.xyz/gtmtnuzoad.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtqhtxvdty.html

[T59] Scala：循环
来源：http://hz.ywan-chungtsiang.top/gtdlurgwlp.html

for (i <- 1 to 10) println(i)
来源：http://hz.fengsongda.top/gtwlnylqyr.html

[T60] Scala：折叠
来源：http://hz.xuetiantiany.cn/gtthemrrtm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtivrrezql.html

================================================================================
来源：http://hz.guowangkeji.top/gtceudxxjq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtxjcpqfnb.html

================================================================================
来源：http://hz.yueranfly.top/gtqnjktuar.html

[U01] Py：创建虚拟环境
来源：http://hz.redwolf501.top/gticcwqqxu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aizwys.cn/gtdggkfrrh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhijiandao.cn/gtwrzzpzsp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuxming.cn/gtcbsjbwsj.html

[U03] Py：加载 .env 配置
来源：http://hz.jinyuanbaomall.cn/gtqfnqsupu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydjk.org.cn/gtjjfbutvi.html

[U04] Py：变量调试打印
来源：http://hz.tanke756.top/gtpowstgtd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yuanzhike.top/gtxsaibucm.html

[U05] Py：列表去重且保序
来源：http://hz.xingfuxueyuan.xyz/gtwrvmzmgk.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtldraveqg.html

[U06] Py：合并两个字典
来源：http://hz.cheryme.top/gtdrawrewn.html

{**a, **b}
来源：http://hz.wangdashe.top/gtisnnhoiv.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtwloezije.html

{v: k for k, v in d.items()}
来源：http://hz.ppjwa.cn/gtfdlydhup.html

[U08] Py：展平二维列表
来源：http://hz.cqqwz.cn/gtodshcexd.html

[y for x in nested for y in x]
来源：http://hz.yj20258.top/gtukjgvcvv.html

[U09] Py：字典取最大值的键
来源：http://hz.ybcxt.top/gtcqcnhbwq.html

max(d, key=d.get)
来源：http://hz.jiagoushi.top/gtgbbnstde.html

[U10] Py：按值排序字典
来源：http://hz.quarkkingdee.top/gteortzkst.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhaomingkeji.xyz/gtbkdnekkh.html


<!-- 参考信息 -->