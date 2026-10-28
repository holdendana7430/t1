代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.wangshuangyany.cn/gtfqtkuugh.html

[R70] 时间戳与互转
来源：http://hz.chenlongwang.top/gtwpsporyv.html

date +%s;  date -d @1700000000
来源：http://hz.jinghuilouyu.cn/gtacdqcmsp.html

[R71] 日期格式化
来源：http://hz.quarkkingdee.top/gtfawksmht.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtdbgqmcpj.html

[R72] 等待端口就绪
来源：http://hz.guannengcc.top/gtcrjaodmw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gtwhfxceim.html

[R73] 分割大日志
来源：http://hz.hnxiangtu.top/gtoeeqooaa.html

split -l 1000 big.log part_
来源：http://hz.ydzc1.top/gtwsnazrnv.html

[R74] 批量重命名
来源：http://hz.hfpthk.cn/gtbytbofou.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sufxvd.cn/gtzlussdgd.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtdlrgencn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigufen.top/gtcttjokky.html

[R76] 使用临时文件
来源：http://hz.guannengcc.top/gtrdjpruqh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtkwmagiup.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtzazxtdjo.html

read -rp "请输入: " ans
来源：http://hz.yonumen.top/gtnkclvjfz.html

[R78] 交互式菜单
来源：http://hz.snrcjt.cn/gtmfxbmvyy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuanzhike.top/gtpixzcrol.html

[R79] 解析命令行选项
来源：http://hz.zdqjudy.top/gtmoarawru.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinghuilouyu.cn/gtkhgtnchp.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gthzoyddcy.html

time ./run.sh
来源：http://hz.tanke756.top/gtopwsjakr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmkzmmqoh.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gtvfirikki.html

================================================================================
来源：http://hz.jqgfzy.top/gtuopekqxl.html

[S01] C：Hello World
来源：http://hz.zdqjudy.top/gtjswtpqlb.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtetgmagic.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.vqdsnc.cn/gtkvjoltmy.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtdgjtghxd.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtnhzhyrrd.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtwoxsabcp.html

int x; scanf("%d", &x);
来源：http://hz.zycfv.cn/gtvascynls.html

[S04] C：字符串复制
来源：http://hz.pycfn.com/gtvqojnbse.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtqidqwmwt.html

[S05] C：字符串长度
来源：http://hz.cqqwz.cn/gtnhwvyfxp.html

strlen(s)
来源：http://hz.ppjwa.cn/gtrfhchzsf.html

[S06] C：字符串比较
来源：http://hz.zhiwuduotai.top/gthfwxodaq.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtzadtygly.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtpeliojbl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtrhajcjbw.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gtzyubwvej.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ppjwa.cn/gtbalghizh.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gtfktmkmfi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yvedp.cn/gtrjogaxho.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtuigkddkl.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtcpwfuwbq.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gtivvlqpto.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj202588.top/gttigjeski.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daria6918.cn/gtlmeromrd.html

fclose(f);
来源：http://hz.yj20258888.top/gtnzjgxtpw.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gthpahyomt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gtsguzncmi.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtnifvoiev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtwpjwieje.html

[S14] C：枚举
来源：http://hz.daxiang520.top/gtfmufqjik.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtecswgmaz.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtsbyeuaaw.html

(double) a / b
来源：http://hz.havefunace.top/gtuctnmamh.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtvgjxubjd.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtxonpmepf.html

[S17] C：安全拼接字符串
来源：http://hz.cucudq.cn/gtngseijod.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtrpyrvaxp.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtkgwsvmzk.html

int main(int argc, char **argv)
来源：http://hz.gzhubu.top/gtqmnrfmbq.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gtsgsikroo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtbfpgmpuq.html

[S20] C：二分查找
来源：http://hz.meibo888.top/gtwkuicqkh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtcttbujqf.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gtzvusfbjo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gotoacloud.top/gtyyezfvpv.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gtwwwracyg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ppjwa.cn/gtkdlqpvbr.html

[S23] C：随机数
来源：http://hz.zhijiandao.cn/gtmbrgwoiy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yvedp.cn/gtyaacfjrw.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gttibehwzq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtqelysmtp.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtlfaarvnt.html

memcpy(dst, src, n);
来源：http://hz.gotoacloud.top/gthevbvdzf.html

[S26] C：内存清零
来源：http://hz.yanxiufei.cn/gtijcmozbf.html

memset(a, 0, sizeof a);
来源：http://hz.guannengcc.top/gtjojigiyk.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gtuqiyasbb.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtefyfszsw.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gtqrryhjlz.html

static int counter = 0;
来源：http://hz.kuanghao11.cn/gtubghfaeo.html

[S29] C：变参函数
来源：http://hz.pycfn.com/gtvhwhfhss.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hongshengwenyu.top/gtuhismola.html

[S30] C：头文件保护
来源：http://hz.bjfxy.top/gtnaeelalp.html

#ifndef X_H
来源：http://hz.gzhubu.top/gtrocpgxiy.html

#define X_H
来源：http://hz.daria6918.cn/gtrgfwnmfm.html

#endif
来源：http://hz.yongpay.top/gtqpvvcseu.html

[S31] C++：Hello World
来源：http://hz.feifeiyinyue.top/gtrvqtmfsd.html

#include <iostream>
来源：http://hz.redwolf501.top/gtkisrxwof.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydzc1.top/gtihgsrtnl.html

[S32] C++：字符串
来源：http://hz.pengpengdd.cyou/gtkfxlvejq.html

std::string s = "hi";  s += "!";
来源：http://hz.0kj1m.cn/gtxfzjnenu.html

[S33] C++：vector 增删
来源：http://hz.haohaochexian.top/gtutorpfok.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydzc1.top/gtelscbwye.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gtaztgfmij.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydjk.org.cn/gtecaejmry.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtzvtfiguj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtcxhigeny.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtscjoikoq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtincrvmij.html

[S37] C++：set
来源：http://hz.ybcxt.top/gtslkiarhx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtjtffgeqj.html

[S38] C++：排序
来源：http://hz.aibaodan.cn/gthczmfasv.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtdclpmtdm.html

[S39] C++：自定义比较器排序
来源：http://hz.jlsjyb.cn/gtvdptzflw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtkhbwyhcq.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gtglazrdya.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ivvv.top/gtxrokvjbo.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtdbsxzlub.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtbsvotxod.html

[S42] C++：继承与虚函数
来源：http://hz.xingfuxueyuan.xyz/gtmconyeml.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtmcafiycb.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gtqavqjyqc.html

auto p = std::make_unique<int>(5);
来源：http://hz.cdnleiting.top/gtiascmsjm.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtjbglnlvq.html

void inc(int &x) { ++x; }
来源：http://hz.zhixingplan.top/gtkszhjxtd.html

[S45] C++：lambda
来源：http://hz.jinghuilouyu.cn/gtudgjrkbz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fengsongda.top/gttvtodosx.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gtvxckpxhd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtzsgijxuw.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtqaznpdus.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtcdwsprut.html

[S48] C++：逐行读文件
来源：http://hz.dashuyun.cn/gtxlllyple.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtdzjzlgqx.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gttuarbwvu.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtlnvodamp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtiplhwtht.html

[S50] C++：格式化数字
来源：http://hz.yj20258888.top/gtnfqusdrd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtxgtcqiht.html

[S51] C++：显式类型转换
来源：http://hz.xziqi.cn/gtjrjdggtp.html

static_cast<double>(a) / b
来源：http://hz.jinqigfzy.top/gthgtvtnpx.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtnuzfhvno.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtytypdeky.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtxpddebjw.html

std::vector<int> w = std::move(v);
来源：http://hz.zhoulong.xyz/gtykbhfsyj.html

[S54] C++：异常处理
来源：http://hz.jinyuanbaomall.cn/gtpebmzbtn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtgvqwdlta.html

[S55] C++：结构化绑定
来源：http://hz.daria6918.cn/gtdnnmebgr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.vqdsnc.cn/gtxlazlkkg.html

[S56] C++：optional
来源：http://hz.havefunace.top/gtvcqtqpej.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gttghuhpzt.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtpknficok.html

constexpr int N = 10;
来源：http://hz.yj20258888.top/gthcmeomal.html

[S58] C++：命名空间
来源：http://hz.zhaomingkeji.xyz/gtlfzzkhrm.html

namespace ns { int f() { return 1; } }
来源：http://hz.andypj.xyz/gtecuqyiup.html

[S59] C++：静态断言
来源：http://hz.tian-w.cn/gtcmjyyfjg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuanzhike.top/gtdveisgub.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtfdyfnybs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yueranfly.top/gtdnsoxjgy.html

================================================================================
来源：http://hz.cdnleiting.top/gtaifnhorr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtpzlolfwd.html

================================================================================
来源：http://hz.snrcjt.cn/gtinfgilfq.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gtfonbszhv.html

println("Hello")
来源：http://hz.sysykeji.top/gtwtqpiyjd.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtncmvmopk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj202588.top/gtbmvsqbuf.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtqmpgomuh.html

"值: $b"
来源：http://hz.hysaishi.cn/gtqswoxlsy.html

[T04] Kotlin：空安全
来源：http://hz.cheryme.top/gtkvgobhfq.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtmkktcegl.html

[T05] Kotlin：when 表达式
来源：http://hz.pengpengdd.cyou/gtfcddxdjz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ehwqpu.com/gtsfimtnls.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtzvecnkwc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.c1oappe.top/gtacqmuudn.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtzkvzuicc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.9152youxi.cn/gtvjrujvry.html

[T08] Kotlin：数据类
来源：http://hz.dianchejie.cn/gttlnsvbui.html

data class User(val name: String, val age: Int)
来源：http://hz.cqqwz.cn/gtnqezpqme.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gtyyrrhqmq.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gtgvciiqwp.html

[T10] Kotlin：默认参数
来源：http://hz.jqgufenzy.top/gtnyvgqusf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pycfn.com/gtigaxnapw.html

[T11] Kotlin：协程
来源：http://hz.chenjidiqi.icu/gtuxaziiao.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258888.top/gtyvdmctts.html

[T12] Kotlin：解构声明
来源：http://hz.jqgufenzy.top/gtrdvgvlpe.html

val (a, b) = Pair(1, 2)
来源：http://hz.hnqzz.top/gtejkeudzs.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gttgfxmgtc.html

val m = mapOf("a" to 1)
来源：http://hz.aizwys.cn/gtosgkttrb.html

[T14] Kotlin：循环
来源：http://hz.redwolf501.top/gtmutmrsuy.html

for (i in 1..10) println(i)
来源：http://hz.ppjwa.cn/gttkhbaqle.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtmwksbhqj.html

interface Shape { fun area(): Double }
来源：http://hz.zdqjudy.top/gtadwjkngq.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangtech.top/gtfqbmmgag.html

print("Hello")
来源：http://hz.guannengcc.top/gtlfrlkiyi.html

[T17] Swift：变量与常量
来源：http://hz.zdqjudy.top/gtjjjeeksl.html

var a = 1;  let b = 2
来源：http://hz.cqqwz.cn/gtttcijreq.html

[T18] Swift：字符串插值
来源：http://hz.daria6918.cn/gttvbkbwzh.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtxkljcytc.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gtoydjilml.html

if let n = opt { print(n) }
来源：http://hz.zhoulong.xyz/gtdytbrylz.html

[T20] Swift：数组操作
来源：http://hz.hfpthk.cn/gtycwlewbl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sysykeji.top/gtjfkcjsgq.html

[T21] Swift：遍历
来源：http://hz.9152youxi.cn/gtdhpboppm.html

for x in a { print(x) }
来源：http://hz.hywenlv.cn/gtcluspgwt.html

[T22] Swift：字典
来源：http://hz.ybcxt.top/gtnthzqblw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhengqikj.top/gtwnpxomri.html

[T23] Swift：函数
来源：http://hz.52xcode.cn/gtergyxevd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ybcxt.top/gtllwkyfid.html

[T24] Swift：闭包
来源：http://hz.mhx1999.top/gtkgejuykj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtbpjyryhm.html

[T25] Swift：结构体
来源：http://hz.xuanzx.com/gtlnxqjdgi.html

struct P { var x: Int }
来源：http://hz.yuxming.cn/gtqtlxyhjo.html

[T26] Swift：类与重写
来源：http://hz.zhiwuduotai.top/gtixspvhpn.html

class A: Base { override func f() {} }
来源：http://hz.svipenyu.cn/gtqyfcrjdn.html

[T27] Swift：错误处理
来源：http://hz.nwbrower.top/gtusgqcyxz.html

do { try f() } catch { print(error) }
来源：http://hz.yanxiufei.cn/gtatgfohwn.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gtfxbscdet.html

enum Color { case red, green }
来源：http://hz.zdqjudy.top/gtrmijchkc.html

[T29] Swift：guard 提前返回
来源：http://hz.shzxlz.cn/gtbzcwkwjl.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtzwavamja.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtckhluagg.html

protocol Shape { func area() -> Double }
来源：http://hz.chenjidiqi.icu/gtqxvteayy.html

[T31] Lua：Hello World
来源：http://hz.xuetiantiany.cn/gtsrjmcooz.html

print("Hello")
来源：http://hz.cucudq.cn/gtrpabtoxc.html

[T32] Lua：局部变量
来源：http://hz.0kj1m.cn/gtfkpksrlq.html

local a = 1
来源：http://hz.sysykeji.top/gtdniottga.html

[T33] Lua：表（数组）
来源：http://hz.yuxming.cn/gtyypfehfx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hongshengwenyu.top/gtnyxrfedw.html

[T34] Lua：遍历表
来源：http://hz.pycfn.com/gtiviokbuw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shzxlz.cn/gtjicjusjh.html

[T35] Lua：字典表
来源：http://hz.jinghuilouyu.cn/gtjilcyisl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.9152youxi.cn/gtjuvhlttx.html

[T36] Lua：函数
来源：http://hz.fengsongda.top/gtmzjttotb.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtalekuwdw.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtidfwbzub.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtabxbxray.html

[T38] Lua：条件
来源：http://hz.xziqi.cn/gtwndxffbg.html

if x > 0 then print("正") end
来源：http://hz.hysaishi.cn/gtmnqpxwgw.html

[T39] Lua：模式匹配
来源：http://hz.ehwqpu.com/gtiqautgbs.html

string.find(s, "%d+")
来源：http://hz.52xcode.cn/gtwjcsqmck.html

[T40] Lua：元表
来源：http://hz.tanke756.top/gtzbiukons.html

setmetatable({}, { __index = base })
来源：http://hz.quarkkingdee.top/gtgfroafyz.html

[T41] Perl：Hello World
来源：http://hz.zhengqikj.top/gteytdfhry.html

print "Hello\n";
来源：http://hz.sweek.top/gtqpwbvnbj.html

[T42] Perl：变量类型
来源：http://hz.yj20258.top/gtemkfbmoa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yangfankeji.com/gtbslkytml.html

[T43] Perl：字符串插值
来源：http://hz.cucudq.cn/gtuaqcnzia.html

"值: $a"
来源：http://hz.andypj.xyz/gtsgpuxmyt.html

[T44] Perl：条件
来源：http://hz.zhijiandao.cn/gtpvzlztpo.html

if ($a > 0) { print "正"; }
来源：http://hz.redwolf501.top/gtdbmnmlxd.html

[T45] Perl：数组遍历
来源：http://hz.jianghu66.top/gtnnjbsrxc.html

for my $x (@arr) { print $x; }
来源：http://hz.wangshuangyany.cn/gtcvrhykjz.html

[T46] Perl：哈希操作
来源：http://hz.yuanzhike.top/gtuweoxzfz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ywan-chungtsiang.top/gtndebowkh.html

[T47] Perl：正则捕获
来源：http://hz.chenlongwang.top/gtzulkdvkl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zycfv.cn/gttqweoyhu.html

[T48] Perl：正则替换
来源：http://hz.chenlongwang.top/gtpopsyzoz.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtozwpufhn.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtrrkvoqfh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtfzvckxnh.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gthnaitjsi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.mhx1999.top/gtfejujejc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gaohongyu789.top/gtqoeywkvt.html

[T51] Scala：Hello World
来源：http://hz.fzhhl.top/gtnjcpfmcn.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtcvvtkmzz.html

[T52] Scala：变量
来源：http://hz.aibaodan.cn/gtxrvxjmph.html

val a = 1;  var b = 2
来源：http://hz.dianchejie.cn/gtxfxvqxva.html

[T53] Scala：字符串插值
来源：http://hz.nwbrower.top/gtetolfxzd.html

s"值: $b"
来源：http://hz.yj20258888.top/gtxgkgmbyn.html

[T54] Scala：集合映射
来源：http://hz.zhiwuduotai.top/gtnmlhizys.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.snrcjt.cn/gtrfqgldcz.html

[T55] Scala：集合过滤
来源：http://hz.mhx1999.top/gtywccgnhe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.quarkkingdee.top/gthhlchpmm.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtjmcmpzpt.html

case class User(name: String, age: Int)
来源：http://hz.zhongyouzk.top/gtrjaealfp.html

[T57] Scala：模式匹配
来源：http://hz.wangshuangyany.cn/gteenytlwy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhongyouzk.top/gtrxdmesmd.html

[T58] Scala：函数定义
来源：http://hz.jinqigufen.top/gtwlwgffpc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ehwqpu.com/gtezsvfigu.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gthzuvovdg.html

for (i <- 1 to 10) println(i)
来源：http://hz.sysykeji.top/gtcohwkpag.html

[T60] Scala：折叠
来源：http://hz.chenzaomai.com/gtvmnbnsup.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinghuilouyu.cn/gtqzvcsmkl.html

================================================================================
来源：http://hz.ppjwa.cn/gtottczkti.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtjscofdef.html

================================================================================
来源：http://hz.aibaodan.cn/gthzbmxsak.html

[U01] Py：创建虚拟环境
来源：http://hz.yvedp.cn/gtirlpfblz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xingfuxueyuan.xyz/gtzsonahsn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258.top/gttmwopxvf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhiwuduotai.top/gtxvnaiwuq.html

[U03] Py：加载 .env 配置
来源：http://hz.zhixingplan.top/gtmwvwymfs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hywenlv.cn/gtfyhlgddn.html

[U04] Py：变量调试打印
来源：http://hz.birdmap.top/gthclbjpgw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtypbkobtp.html

[U05] Py：列表去重且保序
来源：http://hz.vqdsnc.cn/gtvzhrjpke.html

list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtzqbvhatz.html

[U06] Py：合并两个字典
来源：http://hz.cdnleiting.top/gtozsilejs.html

{**a, **b}
来源：http://hz.jianghu66.top/gtcvycmqlp.html

[U07] Py：反转字典键值
来源：http://hz.zhoulong.xyz/gtzzeesjaf.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtcxyhrcrk.html

[U08] Py：展平二维列表
来源：http://hz.yuanzhike.top/gtkctvrvuh.html

[y for x in nested for y in x]
来源：http://hz.smart0.xyz/gtzkgsiwyl.html

[U09] Py：字典取最大值的键
来源：http://hz.ppjwa.cn/gtmzrdbcmn.html

max(d, key=d.get)
来源：http://hz.sweek.top/gtewelupbo.html

[U10] Py：按值排序字典
来源：http://hz.yongpay.top/gtvwiobbei.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhengqikj.top/gtrrakqarq.html


<!-- 参考信息 -->