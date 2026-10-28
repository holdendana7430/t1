代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtsnqzpstt.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gthfsmkvwr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guannengcc.top/gtpbrrwkpa.html

[R77] 读取用户输入
来源：http://hz.guannengcc.top/gtojqyflnz.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gttqclqbkp.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtqinqotnu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtxmdrvqlf.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtmmvxadxc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ivvv.top/gtjficpogw.html

[R80] 查看脚本执行耗时
来源：http://hz.tianlin.xyz/gtrecgjtiz.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtefolaukm.html

================================================================================
来源：http://hz.yvedp.cn/gtkhnnijta.html

S. C / C++ 专题
来源：http://hz.daria6918.cn/gtzfktlmju.html

================================================================================
来源：http://hz.zycfv.cn/gtwjuwyyay.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtqsyzoxnh.html

#include <stdio.h>
来源：http://hz.yuxming.cn/gtjwfpuuyy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtvdpysief.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258.top/gtladpbewx.html

int a = 10; printf("%d\n", a);
来源：http://hz.52xcode.cn/gtrirwtnmo.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtlhqqjmwa.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gttqgiiywy.html

[S04] C：字符串复制
来源：http://hz.ppjwa.cn/gtodpkqepd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj202588.top/gtrgxdfwwo.html

[S05] C：字符串长度
来源：http://hz.sxryk.cn/gtxambjacl.html

strlen(s)
来源：http://hz.sweek.top/gthhfziwoa.html

[S06] C：字符串比较
来源：http://hz.hnqzz.top/gtflxbedih.html

strcmp(a, b) == 0
来源：http://hz.kuanghao11.cn/gtxuscvois.html

[S07] C：数组遍历求和
来源：http://hz.jqgfzy.top/gtkvpryrfw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigufen.top/gtjrrrxwez.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtopslykyd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fengsongda.top/gtgyiiaexn.html

[S09] C：结构体定义与初始化
来源：http://hz.xuanzx.com/gtetsdeosc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gtzhiktpqh.html

[S10] C：指针与解引用
来源：http://hz.shangyingyoupin.top/gtcvmdyasu.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtrymwowvf.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtuzrmafip.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gtvdctsoaj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dianchejie.cn/gtrvkjdsyc.html

fclose(f);
来源：http://hz.0kj1m.cn/gthjxfsdby.html

[S12] C：写文件
来源：http://hz.zhoulong.xyz/gtgetfwxem.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtircxpuwf.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtahchhsnv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtgagnmial.html

[S14] C：枚举
来源：http://hz.jlsjyb.cn/gtotakgzgb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtczolhucg.html

[S15] C：类型转换
来源：http://hz.birdmap.top/gtswsnfzid.html

(double) a / b
来源：http://hz.daria6918.cn/gtjxatarpu.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtrrzbenro.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gttnclnehf.html

[S17] C：安全拼接字符串
来源：http://hz.jqgufenzy.top/gtlccgzlbe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cheryme.top/gtezegbdls.html

[S18] C：命令行参数
来源：http://hz.vqdsnc.cn/gtqqvsvbma.html

int main(int argc, char **argv)
来源：http://hz.shuidangran.top/gthgfjuqah.html

[S19] C：快速排序
来源：http://hz.yanxiufei.cn/gtrvmfmzer.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtihkaamak.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtchdzqkba.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dianchejie.cn/gttfzoeyco.html

[S21] C：字符类别判断
来源：http://hz.hammf.cn/gthyuawigg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yonumen.top/gtlwashacc.html

[S22] C：字符串转数字
来源：http://hz.zhongyouzk.top/gtpjdquhec.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gzhubu.top/gtzbdtpzrw.html

[S23] C：随机数
来源：http://hz.sufxvd.cn/gtyipkdgfh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtrsdhtieh.html

[S24] C：获取本地时间
来源：http://hz.zhongyouzk.top/gtpykrhgyp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.0kj1m.cn/gtcfibkapt.html

[S25] C：内存拷贝
来源：http://hz.birdmap.top/gtustklrjt.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtytykbrhk.html

[S26] C：内存清零
来源：http://hz.chenlongwang.top/gtythwxtai.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtzrzhjsvb.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtpswgxdoh.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtbjrgumgv.html

[S28] C：静态变量
来源：http://hz.yangfankeji.com/gtdwfqkbtu.html

static int counter = 0;
来源：http://hz.tianlin.xyz/gtbpfuvqif.html

[S29] C：变参函数
来源：http://hz.daxiang520.top/gtaxzvamrh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aibaodan.cn/gtqncsrdfs.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtatikwhaq.html

#ifndef X_H
来源：http://hz.yj20258888.top/gtilgqboyu.html

#define X_H
来源：http://hz.andypj.xyz/gtjrdlfbms.html

#endif
来源：http://hz.jyoumei.cn/gtmccsyoen.html

[S31] C++：Hello World
来源：http://hz.yj20258.top/gtmttykcuj.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtfdjmryxg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtczslkebi.html

[S32] C++：字符串
来源：http://hz.nanxuanxn.top/gtdrtuwirs.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gttirrkxxl.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtquvoebxt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtkzkfhzck.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtvqcmawdn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenjidiqi.icu/gtzqluxlfg.html

[S35] C++：map
来源：http://hz.hywenlv.cn/gtubytebjm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gturefwssv.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gtedzogmno.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtiryqrdko.html

[S37] C++：set
来源：http://hz.cashguo.top/gtyhttmnco.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydjk.org.cn/gtzsmpwxgi.html

[S38] C++：排序
来源：http://hz.redwolf501.top/gtlwvrbhit.html

std::sort(v.begin(), v.end());
来源：http://hz.pycfn.com/gtvgetstqz.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtcxozizwv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtoaapnicl.html

[S40] C++：查找元素
来源：http://hz.nanxinkj.top/gtiyqavqpz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtmfhlfmpu.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangtech.top/gtvkiwjzdj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtpjggptzb.html

[S42] C++：继承与虚函数
来源：http://hz.hnqzz.top/gtuttaupng.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtgmrmipvm.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtpoalnonv.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydzc1.top/gtcxmjhzcx.html

[S44] C++：引用传参
来源：http://hz.wangshuangyany.cn/gtzvqvextc.html

void inc(int &x) { ++x; }
来源：http://hz.zdqjudy.top/gtuwpuxlsj.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtxuuevcpd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gtkyjzhake.html

[S46] C++：函数模板
来源：http://hz.mhx1999.top/gtrslqolrp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuanzhike.top/gtcgzpaguf.html

[S47] C++：结构化绑定遍历
来源：http://hz.sysykeji.top/gtgmdrdpid.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtalhvgadh.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtfnnurqym.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dashuyun.cn/gtbkebehka.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtgtqqkykz.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtryuprsof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxinkj.top/gtipckvzkm.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gtgunufrts.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtjengscla.html

[S51] C++：显式类型转换
来源：http://hz.cucudq.cn/gtendvnhrd.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtnvafdfaf.html

[S52] C++：const 与 noexcept
来源：http://hz.feifeiyinyue.top/gtcqtsuuzm.html

int size() const noexcept { return n_; }
来源：http://hz.andypj.xyz/gtkchcyugn.html

[S53] C++：移动语义
来源：http://hz.jiagoushi.top/gtzwcvhjbh.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gtwqkusjxg.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtnukbvson.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yonumen.top/gtbzzbprrk.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gtjufkncpg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cqqwz.cn/gtmhpionij.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtkxsvhffq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtitnvnvff.html

[S57] C++：编译期常量
来源：http://hz.zhengqikj.top/gtchndjedi.html

constexpr int N = 10;
来源：http://hz.yvedp.cn/gttdvfznep.html

[S58] C++：命名空间
来源：http://hz.cdnleiting.top/gtlrbkozkm.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtgyzdaimf.html

[S59] C++：静态断言
来源：http://hz.tianlin.xyz/gtkskriqmy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fengsongda.top/gtlizfttkf.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtuobqhwfa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guannengcc.top/gtheutxggr.html

================================================================================
来源：http://hz.redwolf501.top/gtfxbdchho.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuanzx.com/gttfiwisml.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwhpnbcww.html

[T01] Kotlin：Hello World
来源：http://hz.cashguo.top/gtfqcheydu.html

println("Hello")
来源：http://hz.chenzaomai.com/gtwmpatvxi.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gtmxuftsoa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ybcxt.top/gtcalgzzxb.html

[T03] Kotlin：字符串模板
来源：http://hz.tianlin.xyz/gtrixcqebi.html

"值: $b"
来源：http://hz.birdmap.top/gtkfwsohgs.html

[T04] Kotlin：空安全
来源：http://hz.nwbrower.top/gtzztjbses.html

val n: String? = null;  n?.length
来源：http://hz.hammf.cn/gturozeyue.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtrlksdnth.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtruqqsstx.html

[T06] Kotlin：集合映射
来源：http://hz.daria6918.cn/gtioejrzdu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtawepreor.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtjbfkrzjz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuxming.cn/gtuetvqbus.html

[T08] Kotlin：数据类
来源：http://hz.jiagoushi.top/gtthenkduc.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gteymsabru.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtfusmgrcd.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtqoostmry.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtuklhpcrk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pycfn.com/gttcqodnpi.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtkgnzvrxf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guowangkeji.top/gtrkhqqrex.html

[T12] Kotlin：解构声明
来源：http://hz.ehwqpu.com/gtsloetlnc.html

val (a, b) = Pair(1, 2)
来源：http://hz.zdqjudy.top/gtnkfwhhuz.html

[T13] Kotlin：只读 Map
来源：http://hz.jianghu66.top/gtfbmmhlng.html

val m = mapOf("a" to 1)
来源：http://hz.yuxming.cn/gtshgjmfyo.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtgemfjmui.html

for (i in 1..10) println(i)
来源：http://hz.yanxiufei.cn/gtpiwqowfo.html

[T15] Kotlin：接口
来源：http://hz.gaohongyu789.top/gthiouwfyi.html

interface Shape { fun area(): Double }
来源：http://hz.ehwqpu.com/gtiaykwmav.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtfwzrmcgi.html

print("Hello")
来源：http://hz.ydzc1.top/gtikpvkals.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtyqphngqv.html

var a = 1;  let b = 2
来源：http://hz.gogol.net.cn/gtsupipozc.html

[T18] Swift：字符串插值
来源：http://hz.jqgfzy.top/gtbujknzwp.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtqtaluryn.html

[T19] Swift：可选绑定
来源：http://hz.yuxming.cn/gtmhjugmme.html

if let n = opt { print(n) }
来源：http://hz.shangyingyoupin.top/gthroapixe.html

[T20] Swift：数组操作
来源：http://hz.yanxiufei.cn/gtbwttejog.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sweek.top/gtlnrxogcs.html

[T21] Swift：遍历
来源：http://hz.yvedp.cn/gtrawztqpq.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtuneqyjld.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtxkjflftm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sysykeji.top/gtqcaudtog.html

[T23] Swift：函数
来源：http://hz.sysykeji.top/gtydnlpcoc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnqzz.top/gtencxrovy.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangkeji.top/gtxeefegdi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhoulong.xyz/gtoysizghc.html

[T25] Swift：结构体
来源：http://hz.sweek.top/gtgrsbmlwt.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtxkfkophs.html

[T26] Swift：类与重写
来源：http://hz.tanke756.top/gtnndttbki.html

class A: Base { override func f() {} }
来源：http://hz.zhijiandao.cn/gtjaxfoqij.html

[T27] Swift：错误处理
来源：http://hz.jinqigufen.top/gtakcjyszy.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gtdezvmegz.html

[T28] Swift：枚举
来源：http://hz.zycfv.cn/gtypmwotcs.html

enum Color { case red, green }
来源：http://hz.xinyue.icu/gtydzviuyt.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtlcgjcxuz.html

guard let x = opt else { return }
来源：http://hz.xuetiantiany.cn/gtqmpdeckx.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gtqxdudehw.html

protocol Shape { func area() -> Double }
来源：http://hz.hammf.cn/gtetgvhohs.html

[T31] Lua：Hello World
来源：http://hz.316326.xyz/gtywdxgyjt.html

print("Hello")
来源：http://hz.haohaochexian.top/gtocgcfzmc.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtyrnhgzsp.html

local a = 1
来源：http://hz.gaohongyu789.top/gtetsutkmz.html

[T33] Lua：表（数组）
来源：http://hz.shzxlz.cn/gthlypzaym.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sweek.top/gtwkrblwzh.html

[T34] Lua：遍历表
来源：http://hz.zdqjudy.top/gtmupqezja.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hfpthk.cn/gtjvihivbq.html

[T35] Lua：字典表
来源：http://hz.bjfxy.top/gtybzeauoh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuanzhike.top/gttlajwvjn.html

[T36] Lua：函数
来源：http://hz.hywenlv.cn/gtoguxareq.html

function add(a, b) return a + b end
来源：http://hz.jlsjyb.cn/gtgktvajjl.html

[T37] Lua：字符串拼接
来源：http://hz.daxiang520.top/gtysaqyumj.html

"a" .. "b"
来源：http://hz.shangyingyoupin.top/gtghvydlqe.html

[T38] Lua：条件
来源：http://hz.hfpthk.cn/gtgjxgyymp.html

if x > 0 then print("正") end
来源：http://hz.yuanzhike.top/gtymdqvaye.html

[T39] Lua：模式匹配
来源：http://hz.dashuyun.cn/gtydfzwzzt.html

string.find(s, "%d+")
来源：http://hz.shangyingyoupin.top/gtjiwobmlp.html

[T40] Lua：元表
来源：http://hz.yonumen.top/gtagaiinzh.html

setmetatable({}, { __index = base })
来源：http://hz.jinyuanbaomall.cn/gtsxytbmds.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangtech.top/gtivmjhxuk.html

print "Hello\n";
来源：http://hz.xuanzx.com/gtouehvxqs.html

[T42] Perl：变量类型
来源：http://hz.dianchejie.cn/gtsoxfksxm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.wangshuangyany.cn/gtfeatmgwb.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtfwjnlpbh.html

"值: $a"
来源：http://hz.iojbl.cn/gtfcrqakyb.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gtzvczfbbl.html

if ($a > 0) { print "正"; }
来源：http://hz.tian-w.cn/gtredyievt.html

[T45] Perl：数组遍历
来源：http://hz.xingfuxueyuan.xyz/gtgyqyuixo.html

for my $x (@arr) { print $x; }
来源：http://hz.jyoumei.cn/gtjhfifuev.html

[T46] Perl：哈希操作
来源：http://hz.aibaodan.cn/gtejpikxjn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aizwys.cn/gtvmrcajwo.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtxazwalik.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgfzy.top/gtoslphyrj.html

[T48] Perl：正则替换
来源：http://hz.shuidangran.top/gtscaijycn.html

$s =~ s/old/new/g;
来源：http://hz.yj202588.top/gtinshuntx.html

[T49] Perl：函数
来源：http://hz.ppjwa.cn/gtaeyskbtn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigufen.top/gtbxgrdmbc.html

[T50] Perl：逐行读文件
来源：http://hz.yanxiufei.cn/gtriywzvea.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xylfe.cn/gtbyguvvii.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtxbaluxcf.html

[T51] Scala：Hello World
来源：http://hz.jqgufenzy.top/gtbashvjwp.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtqbypwfpe.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtkyivcxxi.html

val a = 1;  var b = 2
来源：http://hz.fzhhl.top/gthuozfekf.html

[T53] Scala：字符串插值
来源：http://hz.bjfxy.top/gtbostiqez.html

s"值: $b"
来源：http://hz.aizwys.cn/gtpcwtdhny.html

[T54] Scala：集合映射
来源：http://hz.9152youxi.cn/gtfuklpvfi.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuxming.cn/gtlqtjkijv.html

[T55] Scala：集合过滤
来源：http://hz.hfpthk.cn/gtzduoabbj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gogol.net.cn/gtdqfuslft.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtcvxelwnw.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtfsguashi.html

[T57] Scala：模式匹配
来源：http://hz.pengpengdd.cyou/gtcxccqnxp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangshuangyany.cn/gtfcossnei.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gtvsmrhjox.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.bjfxy.top/gtleuydfas.html

[T59] Scala：循环
来源：http://hz.redwolf501.top/gtqqpkscit.html

for (i <- 1 to 10) println(i)
来源：http://hz.ywan-chungtsiang.top/gtxzqtlocz.html

[T60] Scala：折叠
来源：http://hz.zhixingplan.top/gtyvmwfpzk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.9152youxi.cn/gtcegbxyrw.html

================================================================================
来源：http://hz.zhongyouzk.top/gtogmmqutt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gtqlovreum.html

================================================================================
来源：http://hz.hnqzz.top/gtjgtlsftl.html

[U01] Py：创建虚拟环境
来源：http://hz.bjfxy.top/gtbailrqql.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.quarkkingdee.top/gtfqaxiihb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuetiantiany.cn/gtkztdazki.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gtfqrtguii.html

[U03] Py：加载 .env 配置
来源：http://hz.gaohongyu789.top/gtglhskccj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.haohaochexian.top/gtvztkduzo.html

[U04] Py：变量调试打印
来源：http://hz.andypj.xyz/gttvggkkxr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgufenzy.top/gtkycuducv.html

[U05] Py：列表去重且保序
来源：http://hz.9152youxi.cn/gtkiklhukq.html

list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtktempqeq.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gtofqnjuhq.html

{**a, **b}
来源：http://hz.snrcjt.cn/gtogltyfth.html

[U07] Py：反转字典键值
来源：http://hz.wangdashe.top/gttutxmolf.html

{v: k for k, v in d.items()}
来源：http://hz.redwolf501.top/gtacbokhnn.html

[U08] Py：展平二维列表
来源：http://hz.jianghu66.top/gtdfvuhldj.html

[y for x in nested for y in x]
来源：http://hz.nanxuanxn.top/gtpoyjncnk.html

[U09] Py：字典取最大值的键
来源：http://hz.smart0.xyz/gtywxuekdx.html

max(d, key=d.get)
来源：http://hz.cashguo.top/gtnwzdyszf.html

[U10] Py：按值排序字典
来源：http://hz.jinghuilouyu.cn/gtgjvujrfj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.wangdashe.top/gtbnbnhdwa.html

[U11] Py：生成器表达式
来源：http://hz.sxryk.cn/gttmgnamqa.html

(x * 2 for x in arr)
来源：http://hz.yongpay.top/gtwmhslsnd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigufen.top/gtrqygdbke.html

Counter(arr).most_common(3)
来源：http://hz.sufxvd.cn/gtdixrpzhz.html

[U13] Py：固定长度队列
来源：http://hz.havefunace.top/gtttbxywin.html

deque(maxlen=10)
来源：http://hz.ydzc1.top/gttvfifwpi.html

[U14] Py：分组收集到列表
来源：http://hz.vqdsnc.cn/gtbomimnoz.html

defaultdict(list)
来源：http://hz.yj20258888.top/gtzqlgqdkm.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gthhyrfoxb.html

t = time.perf_counter()
来源：http://hz.xinyue.icu/gtfpbuwvqv.html

[U16] Py：命令行参数解析
来源：http://hz.iojbl.cn/gtvedripoy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhiwuduotai.top/gtshlhxzkm.html


<!-- 参考信息 -->