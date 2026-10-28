代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.guowangkeji.top/gtpsjoyref.html

[R70] 时间戳与互转
来源：http://hz.dianchejie.cn/gtipzmimhi.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtcszxjxvr.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtgcwvhlcg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangkeji.top/gtevnziusb.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtpyyeoawj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.birdmap.top/gtgwadrtla.html

[R73] 分割大日志
来源：http://hz.cdnleiting.top/gtxjreynhd.html

split -l 1000 big.log part_
来源：http://hz.guowangkeji.top/gtmxqldrkd.html

[R74] 批量重命名
来源：http://hz.xziqi.cn/gtnqljikec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnxiangtu.top/gtcxmjlmsk.html

[R75] 导出环境变量
来源：http://hz.yj20258888.top/gtvltledbg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtjzlieyvk.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtcvysazku.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtgxlksgll.html

[R77] 读取用户输入
来源：http://hz.gogol.net.cn/gtpxdecnyc.html

read -rp "请输入: " ans
来源：http://hz.chenzaomai.com/gtajeiiczd.html

[R78] 交互式菜单
来源：http://hz.jinyuanbaomall.cn/gtpvbqxpvj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuxming.cn/gtgfijunlk.html

[R79] 解析命令行选项
来源：http://hz.jinqigufen.top/gtdjkmuffi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.quarkkingdee.top/gtiigglqvc.html

[R80] 查看脚本执行耗时
来源：http://hz.ppjwa.cn/gtiayzaues.html

time ./run.sh
来源：http://hz.zhijiandao.cn/gtteggxluj.html

================================================================================
来源：http://hz.zhengqikj.top/gtslyfdaad.html

S. C / C++ 专题
来源：http://hz.chenjidiqi.icu/gtxhvfbokb.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtumilemof.html

[S01] C：Hello World
来源：http://hz.andypj.xyz/gtcjkfgdfc.html

#include <stdio.h>
来源：http://hz.dashuyun.cn/gtgdxatjkz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuanzx.com/gttdewqawa.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtxtrtdqdv.html

int a = 10; printf("%d\n", a);
来源：http://hz.yangfankeji.com/gtxoxpsbsl.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gttszkwnno.html

int x; scanf("%d", &x);
来源：http://hz.sweek.top/gteogxjgrq.html

[S04] C：字符串复制
来源：http://hz.pycfn.com/gttlsbdgsa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtnrdufscs.html

[S05] C：字符串长度
来源：http://hz.iojbl.cn/gtnyanltuw.html

strlen(s)
来源：http://hz.ehwqpu.com/gtbrkxkmvh.html

[S06] C：字符串比较
来源：http://hz.cashguo.top/gtgzdqfkjc.html

strcmp(a, b) == 0
来源：http://hz.cheryme.top/gtyrubsuwi.html

[S07] C：数组遍历求和
来源：http://hz.hongshengwenyu.top/gtiduhbuhd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tianlin.xyz/gtcrvumhjd.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gtkqfmmsmn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtwdtujylf.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtsgbiqljg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.smart0.xyz/gtxhrtfyvx.html

[S10] C：指针与解引用
来源：http://hz.cdnleiting.top/gtckzzxssa.html

int *p = &a;  *p = 5;
来源：http://hz.cheryme.top/gtaosdytem.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gtixeiueuf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.havefunace.top/gtlkinrbis.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yvedp.cn/gtnahiooux.html

fclose(f);
来源：http://hz.xziqi.cn/gtuhdpacdp.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gticrxgeyg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zycfv.cn/gtcttsvdgg.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gtpqjhyeci.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ivvv.top/gthjaxnbix.html

[S14] C：枚举
来源：http://hz.kuanghao11.cn/gtzinmdzcv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aibaodan.cn/gtqyzoncqh.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtwxczzdwj.html

(double) a / b
来源：http://hz.aibaodan.cn/gtzcrgycdy.html

[S16] C：位操作置位
来源：http://hz.zhengqikj.top/gtlmltfhse.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtznekjtts.html

[S17] C：安全拼接字符串
来源：http://hz.aizwys.cn/gtgwqootvs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yueranfly.top/gtjkomuldo.html

[S18] C：命令行参数
来源：http://hz.nanxinkj.top/gtbvjzrrzy.html

int main(int argc, char **argv)
来源：http://hz.hysaishi.cn/gteyeajnfr.html

[S19] C：快速排序
来源：http://hz.daxiang520.top/gtlohvixom.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtwvcrdyhm.html

[S20] C：二分查找
来源：http://hz.aibaodan.cn/gtvypcsiea.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gtaamojcia.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtmwlhuxep.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gtrlxsvdgt.html

[S22] C：字符串转数字
来源：http://hz.andypj.xyz/gttnontamv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ybcxt.top/gthdpbsjze.html

[S23] C：随机数
来源：http://hz.zhijiandao.cn/gtkjygkhun.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hongshengwenyu.top/gtwvzryniz.html

[S24] C：获取本地时间
来源：http://hz.dianchejie.cn/gtdnnonztg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtraxvovrx.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtuwnxqzkr.html

memcpy(dst, src, n);
来源：http://hz.dianchejie.cn/gttggovxby.html

[S26] C：内存清零
来源：http://hz.jinghuilouyu.cn/gtiqavhsgk.html

memset(a, 0, sizeof a);
来源：http://hz.nanxuanxn.top/gtzontxjex.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtplojxjaq.html

const double PI = 3.14159;
来源：http://hz.aizwys.cn/gtlkejwuaj.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gtapbrkjhq.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtatfbomsd.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gtcazimeym.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gttatddahk.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gtwabmltqr.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtyfpjetal.html

#define X_H
来源：http://hz.ydjk.org.cn/gtwjzbbjtb.html

#endif
来源：http://hz.aibaodan.cn/gtqlimrxjp.html

[S31] C++：Hello World
来源：http://hz.ivvv.top/gtzanelags.html

#include <iostream>
来源：http://hz.316326.xyz/gtmesftlle.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuanzhike.top/gtnkwdscdm.html

[S32] C++：字符串
来源：http://hz.zhoulong.xyz/gtjmwrhfmc.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtrzphaowh.html

[S33] C++：vector 增删
来源：http://hz.shzxlz.cn/gtigoxhpof.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtogpjgxli.html

[S34] C++：遍历 vector
来源：http://hz.snrcjt.cn/gtnqlqcapz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtwezeluga.html

[S35] C++：map
来源：http://hz.jqgufenzy.top/gtggawsjif.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtagsayqrt.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gtrghcnvqv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtgwxlzprx.html

[S37] C++：set
来源：http://hz.shanyushiyangkeji.top/gtjhzabpgk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtzcirvlgc.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtitwhypza.html

std::sort(v.begin(), v.end());
来源：http://hz.jiagoushi.top/gtqqwtvmxv.html

[S39] C++：自定义比较器排序
来源：http://hz.guannengcc.top/gtqcrjlbek.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtfhrfmxsl.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gtwvqaoeaw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gtwfprfolk.html

[S41] C++：类与构造函数
来源：http://hz.chenlongwang.top/gtrxsgotxh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gttcongpif.html

[S42] C++：继承与虚函数
来源：http://hz.gotoacloud.top/gtqqzwdydo.html

class B : public Base { public: void f() override {} };
来源：http://hz.svipenyu.cn/gtstonmhgs.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtzqqcabiu.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhixingplan.top/gtayonukij.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gtkjkiwbhk.html

void inc(int &x) { ++x; }
来源：http://hz.jqgfzy.top/gtlarfnnlh.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtghoouhvg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gthffdoaob.html

[S46] C++：函数模板
来源：http://hz.iojbl.cn/gtgamvzdcr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangkeji.top/gtzzffwuyi.html

[S47] C++：结构化绑定遍历
来源：http://hz.jlsjyb.cn/gtfxltrxqw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cucudq.cn/gtzjeuhjcb.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gtsoanpvbg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtkznsebvx.html

while (std::getline(in, line)) { }
来源：http://hz.gzhubu.top/gtgeimddod.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gthzjcjcny.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxinkj.top/gtexhyhvdm.html

[S50] C++：格式化数字
来源：http://hz.meibo888.top/gtdaqluchy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zdqjudy.top/gtmicwfebg.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtreitvuyj.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gttpgmpkkj.html

[S52] C++：const 与 noexcept
来源：http://hz.kuanghao11.cn/gtstppxjqv.html

int size() const noexcept { return n_; }
来源：http://hz.jiagoushi.top/gtimgnsetx.html

[S53] C++：移动语义
来源：http://hz.xylfe.cn/gtyadicjbc.html

std::vector<int> w = std::move(v);
来源：http://hz.svipenyu.cn/gtdwpwsugq.html

[S54] C++：异常处理
来源：http://hz.birdmap.top/gtwgikhvde.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tianlin.xyz/gtsybnbeba.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gteawcohct.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aizwys.cn/gtjwyccqns.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtqonarqdz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yvedp.cn/gtwbsiflma.html

[S57] C++：编译期常量
来源：http://hz.yueranfly.top/gtgccuxmdy.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtqjcqcoes.html

[S58] C++：命名空间
来源：http://hz.redwolf501.top/gtlkcvised.html

namespace ns { int f() { return 1; } }
来源：http://hz.zdqjudy.top/gtbldajefp.html

[S59] C++：静态断言
来源：http://hz.jinqigfzy.top/gtbezxhygx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxuanxn.top/gtctrvatsy.html

[S60] C++：遍历并删除元素
来源：http://hz.cheryme.top/gteivkrgqq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gtiwulnuwn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnbcspzev.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gtqcshtmnu.html

================================================================================
来源：http://hz.cheryme.top/gtupnldoac.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtzwpjxfbt.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtfsdemzdp.html

[T02] Kotlin：变量
来源：http://hz.xuetiantiany.cn/gtgwmxfusd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gtrwlaztzv.html

[T03] Kotlin：字符串模板
来源：http://hz.yongpay.top/gtmsjmpzdu.html

"值: $b"
来源：http://hz.yj20258888.top/gtlqschdkn.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtqgknfctq.html

val n: String? = null;  n?.length
来源：http://hz.chenjidiqi.icu/gtuwkyfamd.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangtech.top/gtgvmwefpg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.iojbl.cn/gtcvuhmgct.html

[T06] Kotlin：集合映射
来源：http://hz.nanxuanxn.top/gtxnoknawh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhijiandao.cn/gtaonjfewv.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gteehbvjkk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.kuanghao11.cn/gticoztrxe.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtvdlxyodw.html

data class User(val name: String, val age: Int)
来源：http://hz.jiagoushi.top/gtdfhoqdxh.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gtwbxmkbsz.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtswolgpme.html

[T10] Kotlin：默认参数
来源：http://hz.cashguo.top/gtrneumalj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ivvv.top/gthyzqmpnl.html

[T11] Kotlin：协程
来源：http://hz.svipenyu.cn/gttzrgrfdp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtqxhymnve.html

[T12] Kotlin：解构声明
来源：http://hz.fengsongda.top/gtjlpymqhn.html

val (a, b) = Pair(1, 2)
来源：http://hz.hfpthk.cn/gthapyvnne.html

[T13] Kotlin：只读 Map
来源：http://hz.yj202588.top/gtzcprwmpu.html

val m = mapOf("a" to 1)
来源：http://hz.yangfankeji.com/gtbbujtnek.html

[T14] Kotlin：循环
来源：http://hz.yueranfly.top/gtbjfclotq.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtxhvdxsxo.html

[T15] Kotlin：接口
来源：http://hz.andypj.xyz/gtsbuoiggp.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gteoakijwh.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangtech.top/gtqrdhpsji.html

print("Hello")
来源：http://hz.snrcjt.cn/gtdexeknmc.html

[T17] Swift：变量与常量
来源：http://hz.chenzaomai.com/gtyqymbgei.html

var a = 1;  let b = 2
来源：http://hz.mhx1999.top/gtcekxfnzr.html

[T18] Swift：字符串插值
来源：http://hz.0kj1m.cn/gtvzkejedk.html

"值: \(b)"
来源：http://hz.c1oappe.top/gtyspgdikk.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtbqnclicw.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtaojqbegr.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gturelhdtm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtkjtbehuo.html

[T21] Swift：遍历
来源：http://hz.pycfn.com/gtthomqmzk.html

for x in a { print(x) }
来源：http://hz.yj20258.top/gtmuwtvtir.html

[T22] Swift：字典
来源：http://hz.yj20258.top/gtsnoxtiba.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yvedp.cn/gthzrxhclq.html

[T23] Swift：函数
来源：http://hz.zhijiandao.cn/gtacjwmrwg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydzc1.top/gtrezoyenn.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtvnjydljj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gtlrdvrwzg.html

[T25] Swift：结构体
来源：http://hz.nanxuanxn.top/gtafnbhkck.html

struct P { var x: Int }
来源：http://hz.smart0.xyz/gtqjfgbnju.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtsrzffndu.html

class A: Base { override func f() {} }
来源：http://hz.smart0.xyz/gtcsewjtmc.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gtiulbmzds.html

do { try f() } catch { print(error) }
来源：http://hz.xziqi.cn/gtqpbuwxnn.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gtojkpfeez.html

enum Color { case red, green }
来源：http://hz.shuidangran.top/gtheoufugh.html

[T29] Swift：guard 提前返回
来源：http://hz.gogol.net.cn/gtaksjriiz.html

guard let x = opt else { return }
来源：http://hz.gaohongyu789.top/gtpkfdooic.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtmfoqvppy.html

protocol Shape { func area() -> Double }
来源：http://hz.hywenlv.cn/gthmbzldom.html

[T31] Lua：Hello World
来源：http://hz.cucudq.cn/gtxcyfmekm.html

print("Hello")
来源：http://hz.zhiwuduotai.top/gtaoayuugj.html

[T32] Lua：局部变量
来源：http://hz.shuidangran.top/gtpcpesuhh.html

local a = 1
来源：http://hz.havefunace.top/gtbjmxlnvj.html

[T33] Lua：表（数组）
来源：http://hz.jianghu66.top/gttfozsefv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sxryk.cn/gtytqtdiss.html

[T34] Lua：遍历表
来源：http://hz.redwolf501.top/gtvhplvnlt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aizwys.cn/gtzrburchi.html

[T35] Lua：字典表
来源：http://hz.c1oappe.top/gtmmshacll.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xinyue.icu/gtzzssgxyj.html

[T36] Lua：函数
来源：http://hz.ybcxt.top/gtsuuusutt.html

function add(a, b) return a + b end
来源：http://hz.gaohongyu789.top/gtrgoljpck.html

[T37] Lua：字符串拼接
来源：http://hz.ivvv.top/gtukoetwxu.html

"a" .. "b"
来源：http://hz.sysykeji.top/gtyikypyly.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtixnfskqs.html

if x > 0 then print("正") end
来源：http://hz.daria6918.cn/gtnbvjgwrs.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtdmvjwarb.html

string.find(s, "%d+")
来源：http://hz.wangdashe.top/gtykgwenom.html

[T40] Lua：元表
来源：http://hz.jinyuanbaomall.cn/gtlkuisbbs.html

setmetatable({}, { __index = base })
来源：http://hz.sweek.top/gtxgalljgt.html

[T41] Perl：Hello World
来源：http://hz.guowangkeji.top/gtdaloirhn.html

print "Hello\n";
来源：http://hz.zdqjudy.top/gthdfyordk.html

[T42] Perl：变量类型
来源：http://hz.tian-w.cn/gtxsbrylsm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.daria6918.cn/gtwwtfvjjy.html

[T43] Perl：字符串插值
来源：http://hz.guowangkeji.top/gttpfwnarf.html

"值: $a"
来源：http://hz.jqgufenzy.top/gtgfgeeqsn.html

[T44] Perl：条件
来源：http://hz.gaohongyu789.top/gtrswncxvz.html

if ($a > 0) { print "正"; }
来源：http://hz.chenlongwang.top/gtqnhepuzl.html

[T45] Perl：数组遍历
来源：http://hz.shzxlz.cn/gtwohxprkw.html

for my $x (@arr) { print $x; }
来源：http://hz.chenzaomai.com/gtwbtfmvow.html

[T46] Perl：哈希操作
来源：http://hz.sxryk.cn/gtjiqjmfrk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.guannengcc.top/gtvnckgfpz.html

[T47] Perl：正则捕获
来源：http://hz.hongshengwenyu.top/gteovtgdol.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guowangkeji.top/gtjymyrwsl.html

[T48] Perl：正则替换
来源：http://hz.pengpengdd.cyou/gtfnxopgbz.html

$s =~ s/old/new/g;
来源：http://hz.ydjk.org.cn/gtdvaaiage.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtixpqtlcx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtlnlnyfbt.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigfzy.top/gtmfyvnjzm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.pycfn.com/gtlinqevve.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.pengpengdd.cyou/gtojauhwwl.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtjdtwrbou.html

println("Hello")
来源：http://hz.nwbrower.top/gtjebvjwfy.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtypevtplh.html

val a = 1;  var b = 2
来源：http://hz.316326.xyz/gtdcbruyaz.html

[T53] Scala：字符串插值
来源：http://hz.pengpengdd.cyou/gtrtaiycen.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtsovlhkzf.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gtqmkdoymz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.birdmap.top/gtsvjhzmrd.html

[T55] Scala：集合过滤
来源：http://hz.dianchejie.cn/gtxcgiarik.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtmhkcznsf.html

[T56] Scala：样例类
来源：http://hz.ppjwa.cn/gtyjvtfwiy.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gtcoihwpqz.html

[T57] Scala：模式匹配
来源：http://hz.xuetiantiany.cn/gtoeqpeyfx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zdqjudy.top/gtsnkygjln.html

[T58] Scala：函数定义
来源：http://hz.fengsongda.top/gtpcrivknm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.52xcode.cn/gtrbuhgutx.html

[T59] Scala：循环
来源：http://hz.quarkkingdee.top/gtolysgcfn.html

for (i <- 1 to 10) println(i)
来源：http://hz.gotoacloud.top/gtvdnjkfdp.html

[T60] Scala：折叠
来源：http://hz.zhixingplan.top/gtnsqyvlnm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtyxswhdyu.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtpayjyhnn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.svipenyu.cn/gtwwqbjldm.html

================================================================================
来源：http://hz.sxryk.cn/gtoflbpjui.html

[U01] Py：创建虚拟环境
来源：http://hz.zhixingplan.top/gtsngfegop.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtpmnpnemu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yongpay.top/gtqdctcakv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sysykeji.top/gtbcmgmaap.html

[U03] Py：加载 .env 配置
来源：http://hz.meibo888.top/gtatdxwakc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dashuyun.cn/gtgriwppnv.html

[U04] Py：变量调试打印
来源：http://hz.vqdsnc.cn/gtohjrhmso.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shangyingyoupin.top/gtadkmlhfs.html

[U05] Py：列表去重且保序
来源：http://hz.hfpthk.cn/gtresnzlqr.html

list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtaqmxizwd.html

[U06] Py：合并两个字典
来源：http://hz.dashuyun.cn/gtxgldopfs.html

{**a, **b}
来源：http://hz.sufxvd.cn/gtqdlllmda.html

[U07] Py：反转字典键值
来源：http://hz.yuxming.cn/gtclvwqubi.html

{v: k for k, v in d.items()}
来源：http://hz.hnqzz.top/gtuqqsdiua.html

[U08] Py：展平二维列表
来源：http://hz.ivvv.top/gtgdwqexpe.html

[y for x in nested for y in x]
来源：http://hz.andypj.xyz/gtzhmtqhyt.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgufenzy.top/gtjgnmurnn.html

max(d, key=d.get)
来源：http://hz.jianghu66.top/gtqjzsbqua.html

[U10] Py：按值排序字典
来源：http://hz.jqgfzy.top/gtdjdclyto.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nwbrower.top/gtcxqvwihf.html


<!-- 参考信息 -->