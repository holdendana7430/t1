代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtjptzxtzu.html

[R76] 使用临时文件
来源：http://hz.redwolf501.top/gtxdsmtfbt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtwwltbmsp.html

[R77] 读取用户输入
来源：http://hz.cucudq.cn/gthdilgiuy.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtlrrycari.html

[R78] 交互式菜单
来源：http://hz.dashuyun.cn/gtuggsmgpd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.quarkkingdee.top/gtkbygbdkd.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtwuampkgp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydzc1.top/gtgvzrhxdy.html

[R80] 查看脚本执行耗时
来源：http://hz.sweek.top/gtkiwbwkvb.html

time ./run.sh
来源：http://hz.hnqzz.top/gtbukipwjy.html

================================================================================
来源：http://hz.cheryme.top/gtqctuusna.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gtprmzwwxf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtbxcfeore.html

[S01] C：Hello World
来源：http://hz.ywan-chungtsiang.top/gtwnihhpof.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtiapzfhnf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtjbdojxpp.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtswbpjyiu.html

int a = 10; printf("%d\n", a);
来源：http://hz.jlsjyb.cn/gtijtwlvkg.html

[S03] C：读入整数
来源：http://hz.ehwqpu.com/gtwjxaawqp.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtvbabetst.html

[S04] C：字符串复制
来源：http://hz.zhoulong.xyz/gtkijtvvyu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daxiang520.top/gtptgmuvhn.html

[S05] C：字符串长度
来源：http://hz.yueranfly.top/gtoobpxmed.html

strlen(s)
来源：http://hz.kuanghao11.cn/gtrjnyygig.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtemzqmtsw.html

strcmp(a, b) == 0
来源：http://hz.yuxming.cn/gtizrhckxg.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtvnhdggrf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zdqjudy.top/gtsoahapww.html

[S08] C：动态内存分配与释放
来源：http://hz.yuanzhike.top/gtbtvadvho.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gthbwmxmzu.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gttumfarzn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtnlmrugbb.html

[S10] C：指针与解引用
来源：http://hz.quarkkingdee.top/gtttqcxfrm.html

int *p = &a;  *p = 5;
来源：http://hz.ppjwa.cn/gtbvfospup.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtwyhmhyfp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gtoojkpwup.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zycfv.cn/gtxiysnnrd.html

fclose(f);
来源：http://hz.0kj1m.cn/gtxykcxred.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gteyszxudl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtsxbdomuk.html

[S13] C：宏定义
来源：http://hz.kuanghao11.cn/gtbfqlcell.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxinkj.top/gtzzlriili.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtfuvkieih.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtibyjyyze.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gtpainhbhg.html

(double) a / b
来源：http://hz.daria6918.cn/gtprtzlfjy.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gttelsahpl.html

x |= (1 << 3);
来源：http://hz.cashguo.top/gthucbbdsu.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtsfzbrzfd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shzxlz.cn/gtrnkxyljs.html

[S18] C：命令行参数
来源：http://hz.jinghuilouyu.cn/gtwdkctvfg.html

int main(int argc, char **argv)
来源：http://hz.sweek.top/gtfflryomo.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtcwpldkon.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtpzokhqvu.html

[S20] C：二分查找
来源：http://hz.cdnleiting.top/gtjhnxsdfc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtxtcykttf.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtnwcwmahe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtakzrbude.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtmfsxcbfc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hammf.cn/gtxlsdyjvj.html

[S23] C：随机数
来源：http://hz.c1oappe.top/gtethxrbvp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtcarnxwuy.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtekiojfbu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daria6918.cn/gtqahboedu.html

[S25] C：内存拷贝
来源：http://hz.fengsongda.top/gtckptyglb.html

memcpy(dst, src, n);
来源：http://hz.daria6918.cn/gtktzmsgya.html

[S26] C：内存清零
来源：http://hz.chenlongwang.top/gtriqhibus.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtrgijalte.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtugsatwwh.html

const double PI = 3.14159;
来源：http://hz.guannengcc.top/gttgbifdbp.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtkxdwjjfd.html

static int counter = 0;
来源：http://hz.xziqi.cn/gtsalxlwkg.html

[S29] C：变参函数
来源：http://hz.yanxiufei.cn/gtchmakpwn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtepaabzcc.html

[S30] C：头文件保护
来源：http://hz.ehwqpu.com/gtpbjmziql.html

#ifndef X_H
来源：http://hz.hysaishi.cn/gtschftofs.html

#define X_H
来源：http://hz.nanxinkj.top/gtmizbmjrq.html

#endif
来源：http://hz.zhaomingkeji.xyz/gtbknlhqfm.html

[S31] C++：Hello World
来源：http://hz.meibo888.top/gtgcobohhz.html

#include <iostream>
来源：http://hz.jinghuilouyu.cn/gtovlrjwgr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtragbuhns.html

[S32] C++：字符串
来源：http://hz.gotoacloud.top/gtvjnpegmk.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gthcdxfjaz.html

[S33] C++：vector 增删
来源：http://hz.shangyingyoupin.top/gthokyzmnq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cucudq.cn/gtxzzrprei.html

[S34] C++：遍历 vector
来源：http://hz.haohaochexian.top/gtwlsyrvyj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sysykeji.top/gtonoogxie.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtxuubhldf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtkqrtkpgj.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gtclofpnob.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtjrdwkpwv.html

[S37] C++：set
来源：http://hz.nanxuanxn.top/gtxnjgpptk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtlkdikfkk.html

[S38] C++：排序
来源：http://hz.jinqigufen.top/gtxhulwgww.html

std::sort(v.begin(), v.end());
来源：http://hz.fengsongda.top/gtcaidfrgr.html

[S39] C++：自定义比较器排序
来源：http://hz.mhx1999.top/gtgndhanku.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtsdjhuuya.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtdlcadqfo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtocqcumlo.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gtmukowthm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtmqenzusr.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtelioxpve.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtvycikkkw.html

[S43] C++：智能指针
来源：http://hz.52xcode.cn/gtbdyvpiyi.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtdazeomyo.html

[S44] C++：引用传参
来源：http://hz.zhoulong.xyz/gtxltwphun.html

void inc(int &x) { ++x; }
来源：http://hz.havefunace.top/gthzyxzihl.html

[S45] C++：lambda
来源：http://hz.gaohongyu789.top/gtdvdhbtmf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shzxlz.cn/gtrpyqqugf.html

[S46] C++：函数模板
来源：http://hz.hnxiangtu.top/gtllvrcwww.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydzc1.top/gtmocmccgl.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gtsrzlwgvp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinghuilouyu.cn/gtpcgdnngu.html

[S48] C++：逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gthmppjrfw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.316326.xyz/gtklkqywdq.html

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtcxwbfbvo.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtwconsaic.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtxowpkfzg.html

[S50] C++：格式化数字
来源：http://hz.pengpengdd.cyou/gtwzbevyag.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtixvlyfgj.html

[S51] C++：显式类型转换
来源：http://hz.zhixingplan.top/gtrgtrehlp.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtopldogho.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gthrfoxdvn.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtuhgcztxp.html

[S53] C++：移动语义
来源：http://hz.tian-w.cn/gtqxeigsth.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gtgwwwktew.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gtflriikac.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinghuilouyu.cn/gtndrbihbj.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gtfqkgntdn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuanzhike.top/gtzbcdkpsf.html

[S56] C++：optional
来源：http://hz.hongshengwenyu.top/gtkgjxkzth.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhoulong.xyz/gtxfwgmkud.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gtslmnxrno.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtcjuekudc.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtbwfnuqeq.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gtxcycuocq.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtgzhzgqwm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258.top/gtgfmzorva.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtvlyrwiss.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnxiangtu.top/gtbxflewre.html

================================================================================
来源：http://hz.jinqigfzy.top/gtldyrqhpr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtbilatnok.html

================================================================================
来源：http://hz.jinqigufen.top/gtgkpcrrno.html

[T01] Kotlin：Hello World
来源：http://hz.jianghu66.top/gtlunpqxol.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtdihvrmfr.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtuifpufpd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.pycfn.com/gtcuvvypce.html

[T03] Kotlin：字符串模板
来源：http://hz.snrcjt.cn/gtmftuzudu.html

"值: $b"
来源：http://hz.xziqi.cn/gtjuhkvkuo.html

[T04] Kotlin：空安全
来源：http://hz.xuanzx.com/gtsfwuxqcx.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtrinhzcdv.html

[T05] Kotlin：when 表达式
来源：http://hz.ywan-chungtsiang.top/gtwqkqvyiz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gthoqoxzuh.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtqevtrpuy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gtluffstqb.html

[T07] Kotlin：集合过滤
来源：http://hz.chenjidiqi.icu/gtkgttuuse.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gtbhrokned.html

[T08] Kotlin：数据类
来源：http://hz.316326.xyz/gtrqvpwhmq.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtyhtjafqq.html

[T09] Kotlin：扩展函数
来源：http://hz.ybcxt.top/gtxldtwrsr.html

fun String.exclaim() = this + "!"
来源：http://hz.zhijiandao.cn/gtzykqbwhf.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gtwjyxzlag.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tanke756.top/gtjivtxdmx.html

[T11] Kotlin：协程
来源：http://hz.xingfuxueyuan.xyz/gtlxfqnlue.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtyyszuvkp.html

[T12] Kotlin：解构声明
来源：http://hz.fengsongda.top/gtgqxvhbta.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gttkziqnxm.html

[T13] Kotlin：只读 Map
来源：http://hz.havefunace.top/gtbymgrctk.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtvtgoxtiz.html

[T14] Kotlin：循环
来源：http://hz.yj20258.top/gtvgaumnbz.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtufnzvwtw.html

[T15] Kotlin：接口
来源：http://hz.52xcode.cn/gtpjcvihrt.html

interface Shape { fun area(): Double }
来源：http://hz.shuidangran.top/gtgqhciyya.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtmtjvjkaq.html

print("Hello")
来源：http://hz.sufxvd.cn/gtlteobsoc.html

[T17] Swift：变量与常量
来源：http://hz.xylfe.cn/gtlchfhdtv.html

var a = 1;  let b = 2
来源：http://hz.xuetiantiany.cn/gtdmtuuino.html

[T18] Swift：字符串插值
来源：http://hz.guannengcc.top/gtoqvxowsz.html

"值: \(b)"
来源：http://hz.jinghuilouyu.cn/gtsfmisxhn.html

[T19] Swift：可选绑定
来源：http://hz.aizwys.cn/gthxnayiag.html

if let n = opt { print(n) }
来源：http://hz.sxryk.cn/gtsensxgfr.html

[T20] Swift：数组操作
来源：http://hz.jqgfzy.top/gtsgybkivd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sxryk.cn/gtmmtrwbty.html

[T21] Swift：遍历
来源：http://hz.0kj1m.cn/gtpsxqtuoc.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtdvpdvtjk.html

[T22] Swift：字典
来源：http://hz.0kj1m.cn/gtmqvqvipf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hongshengwenyu.top/gtvecnbcar.html

[T23] Swift：函数
来源：http://hz.jqgufenzy.top/gtwbljspyj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.svipenyu.cn/gtrdfcfzvd.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gtfykkfveb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhixingplan.top/gtaxdyapov.html

[T25] Swift：结构体
来源：http://hz.gaohongyu789.top/gtboxrfomg.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtsrspkhvn.html

[T26] Swift：类与重写
来源：http://hz.fzhhl.top/gtkyfdxter.html

class A: Base { override func f() {} }
来源：http://hz.feifeiyinyue.top/gtivrmzttc.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtjahdngac.html

do { try f() } catch { print(error) }
来源：http://hz.dashuyun.cn/gtfgvwncil.html

[T28] Swift：枚举
来源：http://hz.yvedp.cn/gtpruvyovf.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gtamisiapu.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgufenzy.top/gtozqjbpns.html

guard let x = opt else { return }
来源：http://hz.jinqigufen.top/gthtaljrsf.html

[T30] Swift：协议
来源：http://hz.tianlin.xyz/gtkafjxepp.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtdergblrl.html

[T31] Lua：Hello World
来源：http://hz.yuanzhike.top/gtzdbzwcvh.html

print("Hello")
来源：http://hz.yj202588.top/gtmrxmldlq.html

[T32] Lua：局部变量
来源：http://hz.cqqwz.cn/gtluvrtsvn.html

local a = 1
来源：http://hz.guannengcc.top/gtoaeikavb.html

[T33] Lua：表（数组）
来源：http://hz.meibo888.top/gthmjfwksb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gaohongyu789.top/gtcanmnang.html

[T34] Lua：遍历表
来源：http://hz.xingfuxueyuan.xyz/gtdfltiydp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gzhubu.top/gtpvmqiicl.html

[T35] Lua：字典表
来源：http://hz.hnxiangtu.top/gtnnmqvttw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sysykeji.top/gtjynlcxvu.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtwxtjszpi.html

function add(a, b) return a + b end
来源：http://hz.yj20258888.top/gtraoxvwlj.html

[T37] Lua：字符串拼接
来源：http://hz.gaohongyu789.top/gtqfkqpdyk.html

"a" .. "b"
来源：http://hz.shzxlz.cn/gtxgzkdcuw.html

[T38] Lua：条件
来源：http://hz.jyoumei.cn/gtedlykxfl.html

if x > 0 then print("正") end
来源：http://hz.ywan-chungtsiang.top/gtlllvlyzk.html

[T39] Lua：模式匹配
来源：http://hz.zhijiandao.cn/gtxdisbcfa.html

string.find(s, "%d+")
来源：http://hz.birdmap.top/gtlrffeyom.html

[T40] Lua：元表
来源：http://hz.redwolf501.top/gtachvxufx.html

setmetatable({}, { __index = base })
来源：http://hz.tanke756.top/gtsipalbck.html

[T41] Perl：Hello World
来源：http://hz.aibaodan.cn/gtzujtnnna.html

print "Hello\n";
来源：http://hz.c1oappe.top/gtzzdtzkgk.html

[T42] Perl：变量类型
来源：http://hz.shuidangran.top/gtfkwpgjmb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.daria6918.cn/gtvpmlcjdh.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gthmudjawy.html

"值: $a"
来源：http://hz.shuidangran.top/gtabpdagjs.html

[T44] Perl：条件
来源：http://hz.yongpay.top/gtnxvkfxfk.html

if ($a > 0) { print "正"; }
来源：http://hz.ppjwa.cn/gtnfkznilz.html

[T45] Perl：数组遍历
来源：http://hz.tian-w.cn/gtrjdaewzu.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtmlkmutsf.html

[T46] Perl：哈希操作
来源：http://hz.pengpengdd.cyou/gtuuzskhiq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258.top/gthazldcwq.html

[T47] Perl：正则捕获
来源：http://hz.yanxiufei.cn/gteqornkvp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxinkj.top/gttsmcylxz.html

[T48] Perl：正则替换
来源：http://hz.mhx1999.top/gtxjallnep.html

$s =~ s/old/new/g;
来源：http://hz.hammf.cn/gtrtxjilgm.html

[T49] Perl：函数
来源：http://hz.ehwqpu.com/gtjkkmdntz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yueranfly.top/gtuszojcud.html

[T50] Perl：逐行读文件
来源：http://hz.xziqi.cn/gtqefofpgl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sufxvd.cn/gtiydtjxdr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.havefunace.top/gteecmlgbq.html

[T51] Scala：Hello World
来源：http://hz.xylfe.cn/gtzqgydjju.html

println("Hello")
来源：http://hz.hammf.cn/gtfvhvqoip.html

[T52] Scala：变量
来源：http://hz.xylfe.cn/gtfwnsfoep.html

val a = 1;  var b = 2
来源：http://hz.guannengcc.top/gtnagtuxss.html

[T53] Scala：字符串插值
来源：http://hz.hywenlv.cn/gtxgettzdl.html

s"值: $b"
来源：http://hz.quarkkingdee.top/gtlqfarsrt.html

[T54] Scala：集合映射
来源：http://hz.cucudq.cn/gthfgsmnkt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ehwqpu.com/gtqckuqdqd.html

[T55] Scala：集合过滤
来源：http://hz.xylfe.cn/gtyfakoxtv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgfzy.top/gtgdmmzmpq.html

[T56] Scala：样例类
来源：http://hz.jianghu66.top/gtltdwowwo.html

case class User(name: String, age: Int)
来源：http://hz.yueranfly.top/gtjezpocbg.html

[T57] Scala：模式匹配
来源：http://hz.0kj1m.cn/gtjtiqqqov.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuanzx.com/gtkgodegto.html

[T58] Scala：函数定义
来源：http://hz.zhengqikj.top/gtpcxlyvyp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.0kj1m.cn/gtjanwtgwe.html

[T59] Scala：循环
来源：http://hz.sufxvd.cn/gtojwfepiq.html

for (i <- 1 to 10) println(i)
来源：http://hz.zdqjudy.top/gtbclynhvg.html

[T60] Scala：折叠
来源：http://hz.haohaochexian.top/gtxmynebzv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cucudq.cn/gtzzwrwxvf.html

================================================================================
来源：http://hz.0kj1m.cn/gtcqjnnazu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtfsnznmon.html

================================================================================
来源：http://hz.jiagoushi.top/gtzejxnemq.html

[U01] Py：创建虚拟环境
来源：http://hz.hfpthk.cn/gtaggknvjy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.birdmap.top/gtjctohfde.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinyuanbaomall.cn/gtvmxnobcn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sysykeji.top/gtvkbtnsbg.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gtnkhluugc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zycfv.cn/gtyivsmkmn.html

[U04] Py：变量调试打印
来源：http://hz.zhongyouzk.top/gtjgeymyii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shanyushiyangkeji.top/gtcexanzrz.html

[U05] Py：列表去重且保序
来源：http://hz.yuanzhike.top/gthcucexej.html

list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtddrocczf.html

[U06] Py：合并两个字典
来源：http://hz.gzhubu.top/gtravwuneu.html

{**a, **b}
来源：http://hz.52xcode.cn/gtixlwgqut.html

[U07] Py：反转字典键值
来源：http://hz.kuanghao11.cn/gtkprccphc.html

{v: k for k, v in d.items()}
来源：http://hz.redwolf501.top/gtriifvzik.html

[U08] Py：展平二维列表
来源：http://hz.yangfankeji.com/gtqhcvwlcq.html

[y for x in nested for y in x]
来源：http://hz.jqgfzy.top/gtzprxhtav.html

[U09] Py：字典取最大值的键
来源：http://hz.tianlin.xyz/gtmjadggzg.html

max(d, key=d.get)
来源：http://hz.daria6918.cn/gtrzpmasmo.html

[U10] Py：按值排序字典
来源：http://hz.cdnleiting.top/gtpsdodmqg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.aibaodan.cn/gtsxwgxswn.html

[U11] Py：生成器表达式
来源：http://hz.ybcxt.top/gtiyblmnzv.html

(x * 2 for x in arr)
来源：http://hz.yj202588.top/gthpdxvetz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yvedp.cn/gthlvluoqa.html

Counter(arr).most_common(3)
来源：http://hz.yongpay.top/gthlaftnbi.html

[U13] Py：固定长度队列
来源：http://hz.jinqigufen.top/gthenijmcy.html

deque(maxlen=10)
来源：http://hz.ivvv.top/gtoumsujkx.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258.top/gtivkvifks.html

defaultdict(list)
来源：http://hz.daxiang520.top/gtjlupnuld.html

[U15] Py：高精度计时
来源：http://hz.xuetiantiany.cn/gtkfntlhzt.html

t = time.perf_counter()
来源：http://hz.jqgfzy.top/gtaeytqygz.html

[U16] Py：命令行参数解析
来源：http://hz.jinghuilouyu.cn/gtgkoafero.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtjlikitnp.html


<!-- 参考信息 -->