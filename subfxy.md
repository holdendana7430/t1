代发 wailian999

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtyptovozp.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtltpmgbzk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnqzz.top/gtqfgqxosx.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtwezykltm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gthsrgvbiw.html

[R76] 使用临时文件
来源：http://hz.jqgfzy.top/gtrkflpxyc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gthcecnllt.html

[R77] 读取用户输入
来源：http://hz.nanxinkj.top/gtdkhmmiyb.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gtlcsjzuzy.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gtrudmpvdm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtnduvvysk.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtrshrgqbw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtidrayrbo.html

[R80] 查看脚本执行耗时
来源：http://hz.316326.xyz/gtwhdhswul.html

time ./run.sh
来源：http://hz.jinghuilouyu.cn/gtomklvwfo.html

================================================================================
来源：http://hz.jqgfzy.top/gteeludpnh.html

S. C / C++ 专题
来源：http://hz.yj202588.top/gtytprdjht.html

================================================================================
来源：http://hz.xinyue.icu/gtbickivws.html

[S01] C：Hello World
来源：http://hz.aizwys.cn/gtorihcchm.html

#include <stdio.h>
来源：http://hz.jianghu66.top/gtypmaanjk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fengsongda.top/gtwdwaqptd.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtxhrjxmai.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtqlnnkkgh.html

[S03] C：读入整数
来源：http://hz.cdnleiting.top/gtafgownuk.html

int x; scanf("%d", &x);
来源：http://hz.jinqigfzy.top/gtuwexpkrg.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtwgwcohuh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gtuidpyruq.html

[S05] C：字符串长度
来源：http://hz.hfpthk.cn/gtqmafrwox.html

strlen(s)
来源：http://hz.jiagoushi.top/gtgvshkyjr.html

[S06] C：字符串比较
来源：http://hz.smart0.xyz/gtjhrphewf.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtzhvemeck.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtjjfgpgjx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gttgkxnvdh.html

[S08] C：动态内存分配与释放
来源：http://hz.xziqi.cn/gtwlermdaj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtoruwfplf.html

[S09] C：结构体定义与初始化
来源：http://hz.pycfn.com/gtckcnmood.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydjk.org.cn/gtxxnbdroq.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtcckqflrm.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtjhsfemin.html

[S11] C：逐行读文件
来源：http://hz.xuetiantiany.cn/gtcbaepjvu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj202588.top/gtbhadogmo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtosqopasc.html

fclose(f);
来源：http://hz.yj202588.top/gtxtpwwphr.html

[S12] C：写文件
来源：http://hz.hysaishi.cn/gtnfddshzu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gtsetthdpw.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gtzomrlaun.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jyoumei.cn/gtwmcdbzeh.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gtsojjvejr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sufxvd.cn/gtieiftssf.html

[S15] C：类型转换
来源：http://hz.0kj1m.cn/gtdzstxnzd.html

(double) a / b
来源：http://hz.meibo888.top/gtiwmubrdd.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtepyqjcbf.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtipkgoqmm.html

[S17] C：安全拼接字符串
来源：http://hz.hammf.cn/gtwlfdqeyb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.9152youxi.cn/gteaecsdrw.html

[S18] C：命令行参数
来源：http://hz.zhijiandao.cn/gtevdilkpd.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtkmdsmpht.html

[S19] C：快速排序
来源：http://hz.jinqigfzy.top/gtvxsowixg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gttscinvqt.html

[S20] C：二分查找
来源：http://hz.zycfv.cn/gtixpjlten.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gttvnjvikz.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtkcjbzprt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yangfankeji.com/gtpacvzfsr.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtkorykodq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zdqjudy.top/gtqfenahhr.html

[S23] C：随机数
来源：http://hz.gzhubu.top/gtkdwyzlmg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxinkj.top/gtzmjvuxfb.html

[S24] C：获取本地时间
来源：http://hz.quarkkingdee.top/gtwqnfnbzp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtcfegpixf.html

[S25] C：内存拷贝
来源：http://hz.vqdsnc.cn/gtkawibfoc.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtbdmbkiyx.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtoesqyjln.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtyypejvtn.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtdchotdql.html

const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtfhsicfnh.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtocvwyefm.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gticxishqg.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtkeeukzhc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangdashe.top/gtpgeqcliy.html

[S30] C：头文件保护
来源：http://hz.0kj1m.cn/gtyoowkzxn.html

#ifndef X_H
来源：http://hz.316326.xyz/gtagwexalt.html

#define X_H
来源：http://hz.daxiang520.top/gtqoeibwis.html

#endif
来源：http://hz.shangyingyoupin.top/gtqpluplpr.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtzkjszgzc.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtbphcmpnl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtcksoagre.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtkydorxhw.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtjhquqmei.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtgznkcqat.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj202588.top/gtnjehzhia.html

[S34] C++：遍历 vector
来源：http://hz.ehwqpu.com/gtxnwhngkz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxuanxn.top/gtwthnpjay.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtqxitdjwf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtoqsfvvcj.html

[S36] C++：unordered_map
来源：http://hz.sweek.top/gtwgekvkhj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtduhdcyrk.html

[S37] C++：set
来源：http://hz.daxiang520.top/gttwdzewgo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258.top/gtknhrdcdf.html

[S38] C++：排序
来源：http://hz.ivvv.top/gtuthuqwnc.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtylbfutpp.html

[S39] C++：自定义比较器排序
来源：http://hz.jinyuanbaomall.cn/gtfzhrsdni.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtdxafttml.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gtudpfcfhl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hysaishi.cn/gtrztdrkdb.html

[S41] C++：类与构造函数
来源：http://hz.kuanghao11.cn/gtaoupurbb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gzhubu.top/gtwrhmfqvz.html

[S42] C++：继承与虚函数
来源：http://hz.ydjk.org.cn/gtffgcwkjb.html

class B : public Base { public: void f() override {} };
来源：http://hz.gzhubu.top/gtedpniyvv.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gtzhybsxfe.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtyldiihgm.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gtvwrkfdzs.html

void inc(int &x) { ++x; }
来源：http://hz.redwolf501.top/gtygtnlatl.html

[S45] C++：lambda
来源：http://hz.xuetiantiany.cn/gtlqoelfmw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shzxlz.cn/gtqshwlyet.html

[S46] C++：函数模板
来源：http://hz.cucudq.cn/gtbwihnwoy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hongshengwenyu.top/gtvbntxuqh.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtozoyhadu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenlongwang.top/gttthheysl.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gtrrvaqfoz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yangfankeji.com/gtklwdjbbb.html

while (std::getline(in, line)) { }
来源：http://hz.fengsongda.top/gtppfqcymd.html

[S49] C++：写文件
来源：http://hz.gotoacloud.top/gtvszrswmn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtgbtrafrn.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gtskyljtcy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cdnleiting.top/gtlhqwhuig.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtkhkadtuc.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangkeji.top/gtcseagyeo.html

[S52] C++：const 与 noexcept
来源：http://hz.chenjidiqi.icu/gtsdubpkym.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtvbxunrsp.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gtiwiidtli.html

std::vector<int> w = std::move(v);
来源：http://hz.yj202588.top/gtymnewwke.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtpsdysfpv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gzhubu.top/gtnhtmyxbw.html

[S55] C++：结构化绑定
来源：http://hz.0kj1m.cn/gtvidngjvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtivgrzzva.html

[S56] C++：optional
来源：http://hz.cucudq.cn/gtuydnqfas.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhijiandao.cn/gtsprkngih.html

[S57] C++：编译期常量
来源：http://hz.sufxvd.cn/gtvzcrrrtd.html

constexpr int N = 10;
来源：http://hz.yj20258.top/gtcztrfsfm.html

[S58] C++：命名空间
来源：http://hz.pycfn.com/gtfznmrfha.html

namespace ns { int f() { return 1; } }
来源：http://hz.ivvv.top/gtlplerasr.html

[S59] C++：静态断言
来源：http://hz.sufxvd.cn/gttwwfequi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuetiantiany.cn/gtrjllzfaf.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtezmdhstn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtgghmojyt.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrkjumvyt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtgezurzcy.html

================================================================================
来源：http://hz.hnxiangtu.top/gttaknwpym.html

[T01] Kotlin：Hello World
来源：http://hz.redwolf501.top/gtgotphxrq.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtyejjwlqx.html

[T02] Kotlin：变量
来源：http://hz.birdmap.top/gttxkpqocs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yueranfly.top/gtkhfuqjvi.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gttsmlkbnw.html

"值: $b"
来源：http://hz.nanxinkj.top/gtcolagsud.html

[T04] Kotlin：空安全
来源：http://hz.52xcode.cn/gttkxkqppl.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtjhpzvlyt.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgufenzy.top/gtgojlkgvo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dashuyun.cn/gtnaxlhhvx.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gttkcgppcu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nwbrower.top/gtzgttzfrb.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gteiiuwoyp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.daxiang520.top/gtgmobexqh.html

[T08] Kotlin：数据类
来源：http://hz.shuidangran.top/gtuzsveiom.html

data class User(val name: String, val age: Int)
来源：http://hz.jinqigfzy.top/gtuvbwsmhc.html

[T09] Kotlin：扩展函数
来源：http://hz.jinghuilouyu.cn/gtvyyszqry.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gtwnduxkyx.html

[T10] Kotlin：默认参数
来源：http://hz.jlsjyb.cn/gtvzmqajai.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtxnejruac.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtdymnozap.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtypavxcsy.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtylnbuxlf.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtoumkajyg.html

[T13] Kotlin：只读 Map
来源：http://hz.cdnleiting.top/gtksclcbow.html

val m = mapOf("a" to 1)
来源：http://hz.hywenlv.cn/gtkbahuphr.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gthinapqmi.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtqsnbncon.html

[T15] Kotlin：接口
来源：http://hz.9152youxi.cn/gtzrjxjckm.html

interface Shape { fun area(): Double }
来源：http://hz.zhongyouzk.top/gtreurnglk.html

[T16] Swift：Hello World
来源：http://hz.jinqigufen.top/gtulikcggz.html

print("Hello")
来源：http://hz.meibo888.top/gtgmqfxzwc.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtfdphxcqu.html

var a = 1;  let b = 2
来源：http://hz.birdmap.top/gtrbnpthsh.html

[T18] Swift：字符串插值
来源：http://hz.ivvv.top/gtcjoxdujh.html

"值: \(b)"
来源：http://hz.pycfn.com/gtiuchgbqy.html

[T19] Swift：可选绑定
来源：http://hz.kuanghao11.cn/gtlevrbvqh.html

if let n = opt { print(n) }
来源：http://hz.yonumen.top/gtbxptelzb.html

[T20] Swift：数组操作
来源：http://hz.nwbrower.top/gtqytonogl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zdqjudy.top/gtynzqiokg.html

[T21] Swift：遍历
来源：http://hz.nanxuanxn.top/gtloosuplp.html

for x in a { print(x) }
来源：http://hz.havefunace.top/gtgebnuact.html

[T22] Swift：字典
来源：http://hz.pycfn.com/gthwvefans.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.0kj1m.cn/gtttcvrqnw.html

[T23] Swift：函数
来源：http://hz.yj20258888.top/gtfetqldxh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ivvv.top/gtripwbxye.html

[T24] Swift：闭包
来源：http://hz.hnqzz.top/gtkbdfawqp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.feifeiyinyue.top/gtwodtcaox.html

[T25] Swift：结构体
来源：http://hz.havefunace.top/gtrlfeftos.html

struct P { var x: Int }
来源：http://hz.kuanghao11.cn/gtiwzrzhcs.html

[T26] Swift：类与重写
来源：http://hz.ehwqpu.com/gtstuislec.html

class A: Base { override func f() {} }
来源：http://hz.gogol.net.cn/gtoewesvyt.html

[T27] Swift：错误处理
来源：http://hz.chenjidiqi.icu/gtisjwayws.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtozcifcgg.html

[T28] Swift：枚举
来源：http://hz.cdnleiting.top/gtzjqgdzno.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtotoqoycv.html

[T29] Swift：guard 提前返回
来源：http://hz.xziqi.cn/gtfivaflbn.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gtuetssegk.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gttxmpmaar.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangkeji.top/gtozkkxksy.html

[T31] Lua：Hello World
来源：http://hz.ywan-chungtsiang.top/gtkxcyazes.html

print("Hello")
来源：http://hz.xuanzx.com/gtkrjtjkdq.html

[T32] Lua：局部变量
来源：http://hz.zycfv.cn/gtqpgbjsry.html

local a = 1
来源：http://hz.0kj1m.cn/gtfaxodria.html

[T33] Lua：表（数组）
来源：http://hz.jyoumei.cn/gtvkonskuy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.andypj.xyz/gtfssejvek.html

[T34] Lua：遍历表
来源：http://hz.smart0.xyz/gtopjhcpxw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cashguo.top/gttoqkpfxy.html

[T35] Lua：字典表
来源：http://hz.xingfuxueyuan.xyz/gtackfaclq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangtech.top/gtzjeamibm.html

[T36] Lua：函数
来源：http://hz.guannengcc.top/gtyixlzywg.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtkzvoadrj.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gtcvhmvagb.html

"a" .. "b"
来源：http://hz.gogol.net.cn/gtixqxfpqh.html

[T38] Lua：条件
来源：http://hz.aibaodan.cn/gtocmpbgie.html

if x > 0 then print("正") end
来源：http://hz.fengsongda.top/gtgvomqtlf.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtjkqdhrsl.html

string.find(s, "%d+")
来源：http://hz.yanxiufei.cn/gtycadvojf.html

[T40] Lua：元表
来源：http://hz.0kj1m.cn/gtcaokmbpm.html

setmetatable({}, { __index = base })
来源：http://hz.sufxvd.cn/gtfwlxcanx.html

[T41] Perl：Hello World
来源：http://hz.birdmap.top/gtcjupcgta.html

print "Hello\n";
来源：http://hz.feifeiyinyue.top/gtrlgmjoyr.html

[T42] Perl：变量类型
来源：http://hz.zhoulong.xyz/gtwpwzkemt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zdqjudy.top/gtgxqdymdi.html

[T43] Perl：字符串插值
来源：http://hz.gzhubu.top/gtdjwglqht.html

"值: $a"
来源：http://hz.dianchejie.cn/gtzdaeztnc.html

[T44] Perl：条件
来源：http://hz.yuxming.cn/gtajqgenxd.html

if ($a > 0) { print "正"; }
来源：http://hz.haohaochexian.top/gtxncwteap.html

[T45] Perl：数组遍历
来源：http://hz.nanxinkj.top/gtomsslasz.html

for my $x (@arr) { print $x; }
来源：http://hz.xuetiantiany.cn/gtpuvgpytp.html

[T46] Perl：哈希操作
来源：http://hz.wangshuangyany.cn/gtdbarbhtm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aibaodan.cn/gtnsnujvsr.html

[T47] Perl：正则捕获
来源：http://hz.yonumen.top/gtyajfjmjq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gtkmswujrq.html

[T48] Perl：正则替换
来源：http://hz.daxiang520.top/gtqjjgxgnz.html

$s =~ s/old/new/g;
来源：http://hz.nanxuanxn.top/gtawksvipy.html

[T49] Perl：函数
来源：http://hz.zdqjudy.top/gtllbocgav.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yanxiufei.cn/gtzotstiyl.html

[T50] Perl：逐行读文件
来源：http://hz.zycfv.cn/gtujmrukzc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtdeqtfjwi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shangyingyoupin.top/gtleggjbmg.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gtzzinfbzz.html

println("Hello")
来源：http://hz.hywenlv.cn/gtstuoovdw.html

[T52] Scala：变量
来源：http://hz.yongpay.top/gtpaioaptw.html

val a = 1;  var b = 2
来源：http://hz.daria6918.cn/gtsaazjlxl.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtodeombjn.html

s"值: $b"
来源：http://hz.aibaodan.cn/gtjznzyynh.html

[T54] Scala：集合映射
来源：http://hz.hnqzz.top/gthdwpnqoy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258.top/gtdpeuorul.html

[T55] Scala：集合过滤
来源：http://hz.cucudq.cn/gtmyhvsqdr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhengqikj.top/gtyabdeumw.html

[T56] Scala：样例类
来源：http://hz.xylfe.cn/gtbkcjflcu.html

case class User(name: String, age: Int)
来源：http://hz.hysaishi.cn/gtrfnttald.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtmupdbual.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnxiangtu.top/gtswyhxxav.html

[T58] Scala：函数定义
来源：http://hz.ydzc1.top/gtxzdwdino.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtncldgizk.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtebxrtvxi.html

for (i <- 1 to 10) println(i)
来源：http://hz.guannengcc.top/gtwttohfis.html

[T60] Scala：折叠
来源：http://hz.wangdashe.top/gtzztjtgbc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenlongwang.top/gtqikidhcc.html

================================================================================
来源：http://hz.yj20258888.top/gtxgtztasv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtdychyrwr.html

================================================================================
来源：http://hz.ivvv.top/gtvrvhguep.html

[U01] Py：创建虚拟环境
来源：http://hz.jyoumei.cn/gtctjtvvmr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gtomuhnsfc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.andypj.xyz/gtvrycauhf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.bjfxy.top/gtebsrjlnj.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtdgqcvotq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zycfv.cn/gtcnonfpbq.html

[U04] Py：变量调试打印
来源：http://hz.daxiang520.top/gtyqeuizvd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shangyingyoupin.top/gtoflagftb.html

[U05] Py：列表去重且保序
来源：http://hz.hammf.cn/gtsumuxopk.html

list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtudnxdadk.html

[U06] Py：合并两个字典
来源：http://hz.yj20258888.top/gtprvqlwnw.html

{**a, **b}
来源：http://hz.hammf.cn/gtfsegojtv.html

[U07] Py：反转字典键值
来源：http://hz.nwbrower.top/gtjlystiff.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtgpcpteor.html

[U08] Py：展平二维列表
来源：http://hz.gotoacloud.top/gtsafzyqad.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtmtoihusm.html

[U09] Py：字典取最大值的键
来源：http://hz.iojbl.cn/gtiauqzbdx.html

max(d, key=d.get)
来源：http://hz.meibo888.top/gtqhpuuelz.html

[U10] Py：按值排序字典
来源：http://hz.xuanzx.com/gtxufseirf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.9152youxi.cn/gtvxdnptmc.html

[U11] Py：生成器表达式
来源：http://hz.dashuyun.cn/gtvlfiulji.html

(x * 2 for x in arr)
来源：http://hz.shuidangran.top/gtyxgeqiob.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dianchejie.cn/gtgbqjlrpi.html

Counter(arr).most_common(3)
来源：http://hz.xinyue.icu/gtdhzwxvkk.html

[U13] Py：固定长度队列
来源：http://hz.ywan-chungtsiang.top/gtbgptdovf.html

deque(maxlen=10)
来源：http://hz.yonumen.top/gtgoukemdi.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258.top/gtllbuvoot.html

defaultdict(list)
来源：http://hz.quarkkingdee.top/gtvzmvdtob.html


<!-- 参考信息 -->