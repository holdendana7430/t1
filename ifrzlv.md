代发 wailian999

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtscuswdmq.html

[R74] 批量重命名
来源：http://hz.redwolf501.top/gtrkqhvssf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtttwfdtzj.html

[R75] 导出环境变量
来源：http://hz.zycfv.cn/gtbqkpnurw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gotoacloud.top/gtmfmfkuxy.html

[R76] 使用临时文件
来源：http://hz.ydzc1.top/gtfxlrhkds.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gthklukjxp.html

[R77] 读取用户输入
来源：http://hz.jinyuanbaomall.cn/gtiapslqet.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtmowhubtq.html

[R78] 交互式菜单
来源：http://hz.ivvv.top/gthoewaqnx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gtlzuisnxq.html

[R79] 解析命令行选项
来源：http://hz.52xcode.cn/gtscpvzqua.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cucudq.cn/gtnvhpizap.html

[R80] 查看脚本执行耗时
来源：http://hz.vqdsnc.cn/gtcqutjrvz.html

time ./run.sh
来源：http://hz.jiagoushi.top/gtptcvfrzl.html

================================================================================
来源：http://hz.sufxvd.cn/gtxluoykqz.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtswrcaxdz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlorsthhj.html

[S01] C：Hello World
来源：http://hz.yuanzhike.top/gtfosssgxa.html

#include <stdio.h>
来源：http://hz.shuidangran.top/gtkrsjdgtx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gthkpbuljc.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtyoydqqpg.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gtsjzfiguo.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtydawivfc.html

int x; scanf("%d", &x);
来源：http://hz.chenzaomai.com/gtpsvcnbll.html

[S04] C：字符串复制
来源：http://hz.tanke756.top/gtgkytmylz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gtyxcvauur.html

[S05] C：字符串长度
来源：http://hz.jiagoushi.top/gtyyjgyfdz.html

strlen(s)
来源：http://hz.smart0.xyz/gteqlksmuf.html

[S06] C：字符串比较
来源：http://hz.tianlin.xyz/gtrwrlifry.html

strcmp(a, b) == 0
来源：http://hz.0kj1m.cn/gtzfhzvicb.html

[S07] C：数组遍历求和
来源：http://hz.hywenlv.cn/gtztjllpyh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhaomingkeji.xyz/gtafilncxv.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gtzhucmwby.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtcvminxpv.html

[S09] C：结构体定义与初始化
来源：http://hz.hysaishi.cn/gtgkwipvwi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sufxvd.cn/gtwofcgxpw.html

[S10] C：指针与解引用
来源：http://hz.yanxiufei.cn/gthhqquymz.html

int *p = &a;  *p = 5;
来源：http://hz.nanxinkj.top/gtgqsuinsb.html

[S11] C：逐行读文件
来源：http://hz.jianghu66.top/gtcvtibrmv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtkqadsrxm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ybcxt.top/gtnwqwumta.html

fclose(f);
来源：http://hz.hfpthk.cn/gtmmeoaacf.html

[S12] C：写文件
来源：http://hz.zhoulong.xyz/gtqtrlhaaq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtyfecgzum.html

[S13] C：宏定义
来源：http://hz.jlsjyb.cn/gtijxerhox.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtidsbalwv.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtydttrxjl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.snrcjt.cn/gtjwedaqxb.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtfginyxzm.html

(double) a / b
来源：http://hz.meibo888.top/gtlubqhlaf.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangtech.top/gtcmebaoco.html

x |= (1 << 3);
来源：http://hz.feifeiyinyue.top/gtopdtdhat.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gteccohfrx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ehwqpu.com/gtmikkmovl.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtmzkrxkba.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtgncxvbjz.html

[S19] C：快速排序
来源：http://hz.zdqjudy.top/gtlccxzcwg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gtpjdenpiu.html

[S20] C：二分查找
来源：http://hz.hywenlv.cn/gtpyamrkfz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtnzkzefyo.html

[S21] C：字符类别判断
来源：http://hz.zhaomingkeji.xyz/gtnaityfka.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hywenlv.cn/gthcejjdoj.html

[S22] C：字符串转数字
来源：http://hz.ydjk.org.cn/gtwtjoinsc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinyuanbaomall.cn/gtezvuerxq.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtivoolarr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhengqikj.top/gtszrcymti.html

[S24] C：获取本地时间
来源：http://hz.daxiang520.top/gtxwvippxn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sufxvd.cn/gturhkhtvw.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtravrxwkf.html

memcpy(dst, src, n);
来源：http://hz.ppjwa.cn/gtccwoabwk.html

[S26] C：内存清零
来源：http://hz.cheryme.top/gtnzrjdjdp.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtdferwbgb.html

[S27] C：定义常量
来源：http://hz.ydzc1.top/gtxqsqhnpr.html

const double PI = 3.14159;
来源：http://hz.aizwys.cn/gtazywouux.html

[S28] C：静态变量
来源：http://hz.guowangkeji.top/gtkuyzzrnk.html

static int counter = 0;
来源：http://hz.quarkkingdee.top/gtleqxapop.html

[S29] C：变参函数
来源：http://hz.zhengqikj.top/gtppsxhorl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cucudq.cn/gtaqhpmrvv.html

[S30] C：头文件保护
来源：http://hz.iojbl.cn/gtutnyvyvk.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtxoouxcpg.html

#define X_H
来源：http://hz.cucudq.cn/gtqlggsxsb.html

#endif
来源：http://hz.tanke756.top/gtllkkbbvr.html

[S31] C++：Hello World
来源：http://hz.snrcjt.cn/gtpqwgwndi.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtfinauocc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnqzz.top/gtjymdxcqj.html

[S32] C++：字符串
来源：http://hz.fengsongda.top/gttdztidxl.html

std::string s = "hi";  s += "!";
来源：http://hz.smart0.xyz/gtykyjeqod.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gtodowtqwu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtvvpxadbj.html

[S34] C++：遍历 vector
来源：http://hz.haohaochexian.top/gtjpogyfii.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gthjhdqiom.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtplxqrtlf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtjpvqnyvf.html

[S36] C++：unordered_map
来源：http://hz.ydjk.org.cn/gtbrfyjddc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtjbfxjasz.html

[S37] C++：set
来源：http://hz.shanyushiyangkeji.top/gtsvlhvvmm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daxiang520.top/gtaokitozv.html

[S38] C++：排序
来源：http://hz.hnxiangtu.top/gtgoivdtia.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gtefeholha.html

[S39] C++：自定义比较器排序
来源：http://hz.xuetiantiany.cn/gtfjkaunlc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jiagoushi.top/gtncptoxpn.html

[S40] C++：查找元素
来源：http://hz.chenzaomai.com/gtpfuyhyqy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gtotjeudfi.html

[S41] C++：类与构造函数
来源：http://hz.wangdashe.top/gtlgutmcym.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hammf.cn/gtbndjnuxy.html

[S42] C++：继承与虚函数
来源：http://hz.jqgfzy.top/gtunmudwai.html

class B : public Base { public: void f() override {} };
来源：http://hz.gaohongyu789.top/gtzdylhrzu.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtcvjqikzu.html

auto p = std::make_unique<int>(5);
来源：http://hz.yanxiufei.cn/gtcbqakwdq.html

[S44] C++：引用传参
来源：http://hz.andypj.xyz/gtwvtlhtxx.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtvvbkiwpg.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gtyeptlbij.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtbtfhhhih.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gtmgwmzhbz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgufenzy.top/gtpcreqvgr.html

[S47] C++：结构化绑定遍历
来源：http://hz.jlsjyb.cn/gtkneinosi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gthsjehmgi.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtvokdcbat.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gtjmegscan.html

while (std::getline(in, line)) { }
来源：http://hz.zhongyouzk.top/gtssixdapb.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtxlsjctrd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.mhx1999.top/gtkjozjnyp.html

[S50] C++：格式化数字
来源：http://hz.cdnleiting.top/gtechjvtxw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtvyornpmw.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gthyoiuiqq.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtsmqmhwlh.html

[S52] C++：const 与 noexcept
来源：http://hz.gzhubu.top/gtqahwytge.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtkfnwhmww.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtqgujdgxz.html

std::vector<int> w = std::move(v);
来源：http://hz.havefunace.top/gthgmtbrgg.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtdghyytjf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jiagoushi.top/gtnszujzqy.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtnwjntcfl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigufen.top/gtzeirlfcw.html

[S56] C++：optional
来源：http://hz.ydzc1.top/gtiwkrscdx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cashguo.top/gtmlkcktmz.html

[S57] C++：编译期常量
来源：http://hz.yvedp.cn/gtsqjwsoec.html

constexpr int N = 10;
来源：http://hz.zdqjudy.top/gtaaykzcqp.html

[S58] C++：命名空间
来源：http://hz.zhixingplan.top/gtxdqozdll.html

namespace ns { int f() { return 1; } }
来源：http://hz.meibo888.top/gtfnvbmlpb.html

[S59] C++：静态断言
来源：http://hz.ivvv.top/gtdyhgzkeg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtjwzmcvhx.html

[S60] C++：遍历并删除元素
来源：http://hz.xylfe.cn/gtwldgvtxe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ywan-chungtsiang.top/gtpzxarfqg.html

================================================================================
来源：http://hz.pycfn.com/gthazbfilt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.svipenyu.cn/gtqcbzeadk.html

================================================================================
来源：http://hz.chenlongwang.top/gtctipolsz.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gttqprirbw.html

println("Hello")
来源：http://hz.shuidangran.top/gtaojpspgi.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtjvnzsjta.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xinyue.icu/gtxzwmkwic.html

[T03] Kotlin：字符串模板
来源：http://hz.svipenyu.cn/gtcafterlr.html

"值: $b"
来源：http://hz.dashuyun.cn/gtkibwfozt.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtiqiviotx.html

val n: String? = null;  n?.length
来源：http://hz.yj20258.top/gtaluznpji.html

[T05] Kotlin：when 表达式
来源：http://hz.snrcjt.cn/gtbjvrxxtw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jiagoushi.top/gthadwcxqk.html

[T06] Kotlin：集合映射
来源：http://hz.9152youxi.cn/gtdjnrwgco.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tian-w.cn/gtfbhcwwws.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtdzkvmphv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtymmkddnp.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtoopnmgta.html

data class User(val name: String, val age: Int)
来源：http://hz.iojbl.cn/gtkebvhzvg.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtzkhwfvkf.html

fun String.exclaim() = this + "!"
来源：http://hz.gogol.net.cn/gtdgbiywro.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtdpxbgxyo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ywan-chungtsiang.top/gtcoxrhejc.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gthmrztxri.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nwbrower.top/gtoxdebeer.html

[T12] Kotlin：解构声明
来源：http://hz.aibaodan.cn/gtoyeoepbr.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtuntpeujb.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxinkj.top/gtebhhlvbf.html

val m = mapOf("a" to 1)
来源：http://hz.ywan-chungtsiang.top/gtlidqxtbg.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gtiwpvryxy.html

for (i in 1..10) println(i)
来源：http://hz.jinqigufen.top/gtjbauiyhe.html

[T15] Kotlin：接口
来源：http://hz.tian-w.cn/gtuejjdvtc.html

interface Shape { fun area(): Double }
来源：http://hz.gaohongyu789.top/gtiigwwaqc.html

[T16] Swift：Hello World
来源：http://hz.yj20258.top/gtmkpumfra.html

print("Hello")
来源：http://hz.svipenyu.cn/gtgjbhinaa.html

[T17] Swift：变量与常量
来源：http://hz.ybcxt.top/gteuwgkmcu.html

var a = 1;  let b = 2
来源：http://hz.feifeiyinyue.top/gttubdffut.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtnfuokpfs.html

"值: \(b)"
来源：http://hz.sysykeji.top/gtilpdhyhi.html

[T19] Swift：可选绑定
来源：http://hz.sxryk.cn/gtlitrovgy.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtutepihid.html

[T20] Swift：数组操作
来源：http://hz.redwolf501.top/gtnkuggiet.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtsfpubtqv.html

[T21] Swift：遍历
来源：http://hz.xuetiantiany.cn/gtqofonmfc.html

for x in a { print(x) }
来源：http://hz.zycfv.cn/gtdpngooic.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtoqdfsxkn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fengsongda.top/gtxjgeklky.html

[T23] Swift：函数
来源：http://hz.cheryme.top/gtmcxcasqw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuxming.cn/gtvkigeusw.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gtmhckwmqg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.aibaodan.cn/gtohnilbeu.html

[T25] Swift：结构体
来源：http://hz.quarkkingdee.top/gtwgqxnhdp.html

struct P { var x: Int }
来源：http://hz.cashguo.top/gtitcylnqm.html

[T26] Swift：类与重写
来源：http://hz.gzhubu.top/gtmnhhtbfi.html

class A: Base { override func f() {} }
来源：http://hz.tanke756.top/gtwwkywhfz.html

[T27] Swift：错误处理
来源：http://hz.zycfv.cn/gtrvokvtze.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtevgouzgn.html

[T28] Swift：枚举
来源：http://hz.gzhubu.top/gtegbuuyqd.html

enum Color { case red, green }
来源：http://hz.gotoacloud.top/gtkkeeqfky.html

[T29] Swift：guard 提前返回
来源：http://hz.iojbl.cn/gtmeavfmaf.html

guard let x = opt else { return }
来源：http://hz.sweek.top/gtomuhfvlh.html

[T30] Swift：协议
来源：http://hz.pengpengdd.cyou/gtaigjchbg.html

protocol Shape { func area() -> Double }
来源：http://hz.jiagoushi.top/gtqdgjfxfp.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtxzhwvcza.html

print("Hello")
来源：http://hz.smart0.xyz/gtkwpvywdz.html

[T32] Lua：局部变量
来源：http://hz.wangshuangyany.cn/gtzhcggayw.html

local a = 1
来源：http://hz.jianghu66.top/gtpzyvhklx.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtrjeyupqc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxinkj.top/gtgekhdrkq.html

[T34] Lua：遍历表
来源：http://hz.aizwys.cn/gtfrljymyw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xingfuxueyuan.xyz/gtzskeaecc.html

[T35] Lua：字典表
来源：http://hz.nwbrower.top/gtftvzvulo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gtizkxnkfc.html

[T36] Lua：函数
来源：http://hz.guannengcc.top/gtnwxvqklh.html

function add(a, b) return a + b end
来源：http://hz.sxryk.cn/gtavhduotr.html

[T37] Lua：字符串拼接
来源：http://hz.cdnleiting.top/gtyujqombq.html

"a" .. "b"
来源：http://hz.chenzaomai.com/gtlozkpujv.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtuqufdakl.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gterrueevp.html

[T39] Lua：模式匹配
来源：http://hz.jiagoushi.top/gtotgsedma.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtvwzbffli.html

[T40] Lua：元表
来源：http://hz.hammf.cn/gtugkwvybt.html

setmetatable({}, { __index = base })
来源：http://hz.smart0.xyz/gtlkuiksbg.html

[T41] Perl：Hello World
来源：http://hz.shangyingyoupin.top/gtytvpsrwy.html

print "Hello\n";
来源：http://hz.mhx1999.top/gtccstrsio.html

[T42] Perl：变量类型
来源：http://hz.snrcjt.cn/gtocmipkbr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nwbrower.top/gthhtqeywe.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtrlkbnlea.html

"值: $a"
来源：http://hz.zdqjudy.top/gttmfoqlbx.html

[T44] Perl：条件
来源：http://hz.xuanzx.com/gtedusmhgj.html

if ($a > 0) { print "正"; }
来源：http://hz.shuidangran.top/gtmnafneto.html

[T45] Perl：数组遍历
来源：http://hz.gzhubu.top/gtozmyrmvi.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtmcbgslas.html

[T46] Perl：哈希操作
来源：http://hz.tian-w.cn/gtjysfehjd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tian-w.cn/gtyxlbwsjs.html

[T47] Perl：正则捕获
来源：http://hz.ppjwa.cn/gtdihwqpas.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ivvv.top/gtqrjzrgea.html

[T48] Perl：正则替换
来源：http://hz.fengsongda.top/gtmhcxfpki.html

$s =~ s/old/new/g;
来源：http://hz.zycfv.cn/gtxvamozso.html

[T49] Perl：函数
来源：http://hz.nanxuanxn.top/gtcksiqbsc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hysaishi.cn/gtmiwwpiar.html

[T50] Perl：逐行读文件
来源：http://hz.yanxiufei.cn/gtvtfypyrp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xylfe.cn/gtmolghclm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.0kj1m.cn/gtrsyvxvfl.html

[T51] Scala：Hello World
来源：http://hz.tianlin.xyz/gtfwygaaix.html

println("Hello")
来源：http://hz.jianghu66.top/gtzshsrtjn.html

[T52] Scala：变量
来源：http://hz.cdnleiting.top/gtmmazbqiv.html

val a = 1;  var b = 2
来源：http://hz.0kj1m.cn/gtmrwpaxjz.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtiskatxwp.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtyfkczuwo.html

[T54] Scala：集合映射
来源：http://hz.cashguo.top/gtgxfelcnf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnxiangtu.top/gtzowztwrc.html

[T55] Scala：集合过滤
来源：http://hz.hongshengwenyu.top/gtncdisioe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangdashe.top/gtogikdbxi.html

[T56] Scala：样例类
来源：http://hz.xinyue.icu/gtdvsiqxvi.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gtlodrfhoy.html

[T57] Scala：模式匹配
来源：http://hz.0kj1m.cn/gtnfgihlfh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnxiangtu.top/gtzujwlgaz.html

[T58] Scala：函数定义
来源：http://hz.bjfxy.top/gtcedfhrcn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.9152youxi.cn/gtrnbxiaqp.html

[T59] Scala：循环
来源：http://hz.nanxuanxn.top/gtmmoksjxy.html

for (i <- 1 to 10) println(i)
来源：http://hz.svipenyu.cn/gtmeznjwzu.html

[T60] Scala：折叠
来源：http://hz.fengsongda.top/gteemsmisu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtgmklyciv.html

================================================================================
来源：http://hz.nanxinkj.top/gtpeznjpeh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangkeji.top/gtlbxwqcpu.html

================================================================================
来源：http://hz.yangfankeji.com/gtddmmtqel.html

[U01] Py：创建虚拟环境
来源：http://hz.chenzaomai.com/gtpgdewlcw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gtaawdoiod.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fengsongda.top/gtkoxjnhfv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.redwolf501.top/gtuholrviz.html

[U03] Py：加载 .env 配置
来源：http://hz.wangshuangyany.cn/gtvuidtmmu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nwbrower.top/gtthsavisi.html

[U04] Py：变量调试打印
来源：http://hz.cashguo.top/gtcvxsrhfq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yongpay.top/gtcfytaett.html

[U05] Py：列表去重且保序
来源：http://hz.hywenlv.cn/gtxxlyeggd.html

list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtfzoseeou.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gtzndgaifq.html

{**a, **b}
来源：http://hz.birdmap.top/gtlpgqehlc.html

[U07] Py：反转字典键值
来源：http://hz.yueranfly.top/gtaapagkzu.html

{v: k for k, v in d.items()}
来源：http://hz.sufxvd.cn/gteotxpqmm.html

[U08] Py：展平二维列表
来源：http://hz.ybcxt.top/gtnwhrnpxx.html

[y for x in nested for y in x]
来源：http://hz.yuxming.cn/gttreetbxy.html

[U09] Py：字典取最大值的键
来源：http://hz.redwolf501.top/gtackcqbob.html

max(d, key=d.get)
来源：http://hz.nanxuanxn.top/gthzytbalh.html

[U10] Py：按值排序字典
来源：http://hz.yuxming.cn/gtqwitrtcc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jlsjyb.cn/gtstyfedjc.html

[U11] Py：生成器表达式
来源：http://hz.yanxiufei.cn/gtvtfleleb.html

(x * 2 for x in arr)
来源：http://hz.cucudq.cn/gtszxdbchk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tian-w.cn/gtatjibgeu.html

Counter(arr).most_common(3)
来源：http://hz.feifeiyinyue.top/gturkilwuf.html

[U13] Py：固定长度队列
来源：http://hz.nanxinkj.top/gttjcymjtu.html

deque(maxlen=10)
来源：http://hz.gaohongyu789.top/gtyuyneoey.html

[U14] Py：分组收集到列表
来源：http://hz.sysykeji.top/gteglmkpca.html

defaultdict(list)
来源：http://hz.ywan-chungtsiang.top/gtnuvnzbtz.html


<!-- 参考信息 -->