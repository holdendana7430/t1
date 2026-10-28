代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gtcanvmguu.html

[R70] 时间戳与互转
来源：http://hz.yangfankeji.com/gtrgdqcnyc.html

date +%s;  date -d @1700000000
来源：http://hz.smart0.xyz/gtzjwtempp.html

[R71] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtsaxwodhb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtkplkudvx.html

[R72] 等待端口就绪
来源：http://hz.daxiang520.top/gtqujabesc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gttxbfpssn.html

[R73] 分割大日志
来源：http://hz.xinyue.icu/gtjcgsbqre.html

split -l 1000 big.log part_
来源：http://hz.jyoumei.cn/gtrpvjehat.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtficaswng.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtmpnflgei.html

[R75] 导出环境变量
来源：http://hz.xziqi.cn/gtcqewttgb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dianchejie.cn/gtzmbtflcv.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtqanbpuwc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtptlhljgu.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtqehunslt.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtxkkuwyxb.html

[R78] 交互式菜单
来源：http://hz.yanxiufei.cn/gthhutmpmh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gtldsehpxy.html

[R79] 解析命令行选项
来源：http://hz.yj20258.top/gtlncvsgik.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtujfkkzwx.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtnttfcmzk.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gtruvffmrt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtzjomgklq.html

S. C / C++ 专题
来源：http://hz.svipenyu.cn/gttklnqjul.html

================================================================================
来源：http://hz.cashguo.top/gtkcbylipj.html

[S01] C：Hello World
来源：http://hz.chenlongwang.top/gtzssrucop.html

#include <stdio.h>
来源：http://hz.dianchejie.cn/gtoefzkack.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtmtjapjnx.html

[S02] C：变量与格式化输出
来源：http://hz.xinyue.icu/gtkzikvrzs.html

int a = 10; printf("%d\n", a);
来源：http://hz.bjfxy.top/gtcsjqpxlf.html

[S03] C：读入整数
来源：http://hz.quarkkingdee.top/gtvjwycsqe.html

int x; scanf("%d", &x);
来源：http://hz.nanxuanxn.top/gttiaqmyjn.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtadvplvtd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigfzy.top/gtcyojvntc.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gttavjwttz.html

strlen(s)
来源：http://hz.birdmap.top/gthkdirzpu.html

[S06] C：字符串比较
来源：http://hz.cqqwz.cn/gtpmqftqxk.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtetcjrljc.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtwatkwmot.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tianlin.xyz/gtklvpyegt.html

[S08] C：动态内存分配与释放
来源：http://hz.cdnleiting.top/gtbsadgkef.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cashguo.top/gtjlgymwne.html

[S09] C：结构体定义与初始化
来源：http://hz.zdqjudy.top/gtesjmvpti.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtmhzlpuph.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gtdoajzzgs.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtrghnwuur.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gthoqgorlw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhixingplan.top/gtuqggisgt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangkeji.top/gtcluupubl.html

fclose(f);
来源：http://hz.daxiang520.top/gtdlmoeyrg.html

[S12] C：写文件
来源：http://hz.cashguo.top/gtgrpsulqv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtpugxzcaf.html

[S13] C：宏定义
来源：http://hz.mhx1999.top/gtzmjqgljn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtxkmbfvkc.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gtjytwnzkm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gthfepnwji.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtoentsdyu.html

(double) a / b
来源：http://hz.svipenyu.cn/gtqurgleol.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtoyjfkxzy.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtahnpotio.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtynhvnwph.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gaohongyu789.top/gtyfmiyfyf.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtrtnqjzbb.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtupatdqwr.html

[S19] C：快速排序
来源：http://hz.xinyue.icu/gtiixlnnvz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtnppueewv.html

[S20] C：二分查找
来源：http://hz.fzhhl.top/gtveskrcwt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtozdzddfg.html

[S21] C：字符类别判断
来源：http://hz.hammf.cn/gtyctcvjdq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cashguo.top/gtrboxqqzl.html

[S22] C：字符串转数字
来源：http://hz.wangdashe.top/gtmwwgkfzw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jiagoushi.top/gtfeijaszp.html

[S23] C：随机数
来源：http://hz.shanyushiyangtech.top/gtbicqbijs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.haohaochexian.top/gtmaufqbmi.html

[S24] C：获取本地时间
来源：http://hz.hywenlv.cn/gtnsalziwa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gtlrdvoqwe.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gtepvslnyt.html

memcpy(dst, src, n);
来源：http://hz.gzhubu.top/gtgazanssp.html

[S26] C：内存清零
来源：http://hz.zycfv.cn/gtfynvxsqa.html

memset(a, 0, sizeof a);
来源：http://hz.jinghuilouyu.cn/gtyvndjzjo.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtlenslwro.html

const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtsgfhnukw.html

[S28] C：静态变量
来源：http://hz.9152youxi.cn/gtmfmhfott.html

static int counter = 0;
来源：http://hz.cheryme.top/gtcftylrmk.html

[S29] C：变参函数
来源：http://hz.sweek.top/gtucfssies.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gtfgsskgng.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gtbqzydikm.html

#ifndef X_H
来源：http://hz.xziqi.cn/gtfwjsupyd.html

#define X_H
来源：http://hz.snrcjt.cn/gtvlzfkvmk.html

#endif
来源：http://hz.meibo888.top/gtxyvpgxrz.html

[S31] C++：Hello World
来源：http://hz.shuidangran.top/gtyrihwexu.html

#include <iostream>
来源：http://hz.nanxinkj.top/gtcawtmalb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hysaishi.cn/gtrxntdvkr.html

[S32] C++：字符串
来源：http://hz.cqqwz.cn/gtjleuwuse.html

std::string s = "hi";  s += "!";
来源：http://hz.chenjidiqi.icu/gtqslhieal.html

[S33] C++：vector 增删
来源：http://hz.hysaishi.cn/gthfzykidf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtciyvdyab.html

[S34] C++：遍历 vector
来源：http://hz.ppjwa.cn/gtvmbutiyj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aibaodan.cn/gtqvcbwctb.html

[S35] C++：map
来源：http://hz.tanke756.top/gtjwfniykg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtsdnlwiiz.html

[S36] C++：unordered_map
来源：http://hz.snrcjt.cn/gtipyldfjb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtmqjozktt.html

[S37] C++：set
来源：http://hz.yj20258888.top/gtghcovder.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gotoacloud.top/gtcttxrsne.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtfwvuoxju.html

std::sort(v.begin(), v.end());
来源：http://hz.daria6918.cn/gtkflwhncb.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258888.top/gtdijgbimt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gtjpjnplvp.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gtdkeoeufw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtyzkencer.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtapobskme.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ppjwa.cn/gtmahlmvkt.html

[S42] C++：继承与虚函数
来源：http://hz.daxiang520.top/gtgoqyhwfv.html

class B : public Base { public: void f() override {} };
来源：http://hz.tian-w.cn/gttomgcate.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gthqsirumi.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgufenzy.top/gtzhjludbn.html

[S44] C++：引用传参
来源：http://hz.birdmap.top/gtpumtbdoa.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gteecjrocu.html

[S45] C++：lambda
来源：http://hz.guowangkeji.top/gtvxdzfthw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yueranfly.top/gtwveyjztt.html

[S46] C++：函数模板
来源：http://hz.iojbl.cn/gtcmvyfqae.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtdfgnpjow.html

[S47] C++：结构化绑定遍历
来源：http://hz.yvedp.cn/gtjkajchkv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtvphgwnbn.html

[S48] C++：逐行读文件
来源：http://hz.cashguo.top/gtwbihrcgo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gtvwaclrrc.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigufen.top/gtvsjgmxlw.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gthnrwekul.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtvdqcgmtg.html

[S50] C++：格式化数字
来源：http://hz.shuidangran.top/gtjwihqred.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtpvksoxay.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtigjxhlfd.html

static_cast<double>(a) / b
来源：http://hz.cdnleiting.top/gtmobqhmmp.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtzacbxbbw.html

int size() const noexcept { return n_; }
来源：http://hz.yangfankeji.com/gtzjfkiagt.html

[S53] C++：移动语义
来源：http://hz.cucudq.cn/gtyothvlwv.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtgncletrf.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gtrfkwmsln.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtmnrqbqod.html

[S55] C++：结构化绑定
来源：http://hz.gogol.net.cn/gtlsomvsdq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj20258888.top/gtzgpkoakp.html

[S56] C++：optional
来源：http://hz.sweek.top/gtlqbcofct.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gthzaqzhnm.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtgocvvpxa.html

constexpr int N = 10;
来源：http://hz.zhiwuduotai.top/gtuibyrxby.html

[S58] C++：命名空间
来源：http://hz.guowangkeji.top/gtgesreupx.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtmpwebkkt.html

[S59] C++：静态断言
来源：http://hz.ywan-chungtsiang.top/gtllrktklj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gthftcgdlt.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gthvzudoao.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gtglxpvbbu.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtehartttr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtdqaffycb.html

================================================================================
来源：http://hz.guowangkeji.top/gtimksubsk.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gtuiehtxxf.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gthctblagr.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtjsqibphb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sweek.top/gtmtpodxgg.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gtewvjsyup.html

"值: $b"
来源：http://hz.cqqwz.cn/gtvlbtiqui.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtazaxwhln.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gttfxjptwc.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtaenzbnss.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aizwys.cn/gtnugztuxo.html

[T06] Kotlin：集合映射
来源：http://hz.316326.xyz/gtoshfmudw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtfkrqkvta.html

[T07] Kotlin：集合过滤
来源：http://hz.ppjwa.cn/gtlomjplyi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtzkgzzqro.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtdqqatdye.html

data class User(val name: String, val age: Int)
来源：http://hz.xingfuxueyuan.xyz/gtokvviqud.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigufen.top/gtrxryuztw.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigfzy.top/gtdyiughsi.html

[T10] Kotlin：默认参数
来源：http://hz.52xcode.cn/gtnjlvhqoc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenjidiqi.icu/gtphbyipdm.html

[T11] Kotlin：协程
来源：http://hz.dianchejie.cn/gtqcgzolyn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtsgviyxij.html

[T12] Kotlin：解构声明
来源：http://hz.hammf.cn/gtkequotnn.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gttyckxqzt.html

[T13] Kotlin：只读 Map
来源：http://hz.xuetiantiany.cn/gtvdfennjf.html

val m = mapOf("a" to 1)
来源：http://hz.xuetiantiany.cn/gtngyxsalh.html

[T14] Kotlin：循环
来源：http://hz.tanke756.top/gtffrrblsp.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtsknhguez.html

[T15] Kotlin：接口
来源：http://hz.sufxvd.cn/gtkzpybnqq.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtbpmdnoxr.html

[T16] Swift：Hello World
来源：http://hz.birdmap.top/gtdqldorlc.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtpfrzusen.html

[T17] Swift：变量与常量
来源：http://hz.daria6918.cn/gtqrqinkdk.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtwlarawut.html

[T18] Swift：字符串插值
来源：http://hz.jinqigufen.top/gtrwcctufb.html

"值: \(b)"
来源：http://hz.hnxiangtu.top/gtrxdqrnfk.html

[T19] Swift：可选绑定
来源：http://hz.gotoacloud.top/gtrbeceyjj.html

if let n = opt { print(n) }
来源：http://hz.yongpay.top/gtdilsyjfl.html

[T20] Swift：数组操作
来源：http://hz.fengsongda.top/gtonsbzxwo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhengqikj.top/gtccauaqlo.html

[T21] Swift：遍历
来源：http://hz.svipenyu.cn/gtpicqcuox.html

for x in a { print(x) }
来源：http://hz.yuxming.cn/gtdrqmwean.html

[T22] Swift：字典
来源：http://hz.cucudq.cn/gttxvtulzk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtzatrokrx.html

[T23] Swift：函数
来源：http://hz.jinqigfzy.top/gtkzzqfhch.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.feifeiyinyue.top/gtegywylfh.html

[T24] Swift：闭包
来源：http://hz.9152youxi.cn/gtawsvdctd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtrcxxxwnf.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtyagqayzi.html

struct P { var x: Int }
来源：http://hz.jqgufenzy.top/gtjtaaowgg.html

[T26] Swift：类与重写
来源：http://hz.jlsjyb.cn/gtejvlqlfd.html

class A: Base { override func f() {} }
来源：http://hz.shangyingyoupin.top/gtjltisppd.html

[T27] Swift：错误处理
来源：http://hz.nanxuanxn.top/gtdcwiadzq.html

do { try f() } catch { print(error) }
来源：http://hz.shangyingyoupin.top/gtwqusmewz.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtmeaeokux.html

enum Color { case red, green }
来源：http://hz.andypj.xyz/gtrtlknstu.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gtmrqpefik.html

guard let x = opt else { return }
来源：http://hz.c1oappe.top/gtsclhxndn.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtkcwvlabv.html

protocol Shape { func area() -> Double }
来源：http://hz.jiagoushi.top/gtlviukudf.html

[T31] Lua：Hello World
来源：http://hz.xylfe.cn/gtlacdbavu.html

print("Hello")
来源：http://hz.yj20258.top/gtgmazhlov.html

[T32] Lua：局部变量
来源：http://hz.hysaishi.cn/gtlxoevsas.html

local a = 1
来源：http://hz.zhaomingkeji.xyz/gtncldklkd.html

[T33] Lua：表（数组）
来源：http://hz.iojbl.cn/gtrdevbcur.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hfpthk.cn/gtmtzhwlzl.html

[T34] Lua：遍历表
来源：http://hz.xinyue.icu/gtjxaegdwm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtyqjsfthy.html

[T35] Lua：字典表
来源：http://hz.zhoulong.xyz/gtddravftv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhixingplan.top/gterookouy.html

[T36] Lua：函数
来源：http://hz.zhongyouzk.top/gtlowuthfk.html

function add(a, b) return a + b end
来源：http://hz.yangfankeji.com/gtnuldrwys.html

[T37] Lua：字符串拼接
来源：http://hz.zycfv.cn/gtnxycyzlp.html

"a" .. "b"
来源：http://hz.wangdashe.top/gtbuygulwz.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtfiilwqgk.html

if x > 0 then print("正") end
来源：http://hz.jyoumei.cn/gtnyosuvqk.html

[T39] Lua：模式匹配
来源：http://hz.ehwqpu.com/gtfqlsqyfb.html

string.find(s, "%d+")
来源：http://hz.yonumen.top/gtehmbtwpi.html

[T40] Lua：元表
来源：http://hz.birdmap.top/gtponbjcnq.html

setmetatable({}, { __index = base })
来源：http://hz.sweek.top/gtauecvpoy.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtnapmyefb.html

print "Hello\n";
来源：http://hz.zhoulong.xyz/gtpvplcjvd.html

[T42] Perl：变量类型
来源：http://hz.iojbl.cn/gtlkqpjsyc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxinkj.top/gtfqvhdqdn.html

[T43] Perl：字符串插值
来源：http://hz.yj20258.top/gtagdvohsu.html

"值: $a"
来源：http://hz.daria6918.cn/gtzjbfigwd.html

[T44] Perl：条件
来源：http://hz.mhx1999.top/gtztkczwos.html

if ($a > 0) { print "正"; }
来源：http://hz.ybcxt.top/gtjhguuwya.html

[T45] Perl：数组遍历
来源：http://hz.guowangkeji.top/gtapkrgxyj.html

for my $x (@arr) { print $x; }
来源：http://hz.wangshuangyany.cn/gtljoldlvs.html

[T46] Perl：哈希操作
来源：http://hz.shuidangran.top/gtjfrcgguw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gttpodtgfk.html

[T47] Perl：正则捕获
来源：http://hz.yueranfly.top/gtyljfazcm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgfzy.top/gtrelmfvmz.html

[T48] Perl：正则替换
来源：http://hz.xinyue.icu/gtctjguphq.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtwjnzqlbj.html

[T49] Perl：函数
来源：http://hz.kuanghao11.cn/gtzxhnywzd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jiagoushi.top/gtsobaecji.html

[T50] Perl：逐行读文件
来源：http://hz.andypj.xyz/gtiiqubcfv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.fzhhl.top/gtwgniqmcf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.iojbl.cn/gtbillyllx.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gtfuvmjlpd.html

println("Hello")
来源：http://hz.hysaishi.cn/gthjxgomzp.html

[T52] Scala：变量
来源：http://hz.shangyingyoupin.top/gtoppslhha.html

val a = 1;  var b = 2
来源：http://hz.hongshengwenyu.top/gtahgplqdl.html

[T53] Scala：字符串插值
来源：http://hz.aizwys.cn/gtajnpglwi.html

s"值: $b"
来源：http://hz.gotoacloud.top/gtoxxveolq.html

[T54] Scala：集合映射
来源：http://hz.xuanzx.com/gtjkrciwvr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtzysnzkri.html

[T55] Scala：集合过滤
来源：http://hz.chenlongwang.top/gtiufjxgqo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.feifeiyinyue.top/gtxkwjerxz.html

[T56] Scala：样例类
来源：http://hz.cashguo.top/gtemoctyyz.html

case class User(name: String, age: Int)
来源：http://hz.yj202588.top/gtowlrbprr.html

[T57] Scala：模式匹配
来源：http://hz.ydjk.org.cn/gtciaieujg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hfpthk.cn/gtpulmiwsx.html

[T58] Scala：函数定义
来源：http://hz.0kj1m.cn/gtuspkgvyj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hywenlv.cn/gtpslshiik.html

[T59] Scala：循环
来源：http://hz.redwolf501.top/gtvsvuhmle.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtcndfvwwx.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtaxpqljis.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtvrpunxet.html

================================================================================
来源：http://hz.ydjk.org.cn/gtddchdtfa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangdashe.top/gtfiwxiysg.html

================================================================================
来源：http://hz.yvedp.cn/gtxsaypjlr.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gtysmrzmgg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgfzy.top/gtqiufsejo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxuanxn.top/gtfkdmadex.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cucudq.cn/gtiyvkxtbp.html

[U03] Py：加载 .env 配置
来源：http://hz.zhengqikj.top/gtefmmkszq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.meibo888.top/gtnriplzeb.html

[U04] Py：变量调试打印
来源：http://hz.jqgfzy.top/gtivqtimxr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinqigufen.top/gtlboflxye.html

[U05] Py：列表去重且保序
来源：http://hz.316326.xyz/gtqvovpzlr.html

list(dict.fromkeys(arr))
来源：http://hz.zhongyouzk.top/gtpbezynex.html

[U06] Py：合并两个字典
来源：http://hz.hammf.cn/gtpykdqzfk.html

{**a, **b}
来源：http://hz.zhiwuduotai.top/gtpsxglomp.html

[U07] Py：反转字典键值
来源：http://hz.fengsongda.top/gtvskwuxjx.html

{v: k for k, v in d.items()}
来源：http://hz.haohaochexian.top/gtbcxpjglr.html

[U08] Py：展平二维列表
来源：http://hz.nanxuanxn.top/gtwgyjslol.html

[y for x in nested for y in x]
来源：http://hz.aizwys.cn/gtnuswdlhz.html

[U09] Py：字典取最大值的键
来源：http://hz.zhiwuduotai.top/gtehtuylya.html

max(d, key=d.get)
来源：http://hz.xinyue.icu/gtokjhqidt.html

[U10] Py：按值排序字典
来源：http://hz.chenlongwang.top/gtjbokgenx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jqgfzy.top/gtxgkvlwra.html


<!-- 参考信息 -->