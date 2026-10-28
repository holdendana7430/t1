代发 wailian999

split -l 1000 big.log part_
来源：http://hz.bjfxy.top/gtxxjetaie.html

[R74] 批量重命名
来源：http://hz.cheryme.top/gtrsidzdxv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.svipenyu.cn/gtildctndv.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtkcqjvgmk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gttycveoxg.html

[R76] 使用临时文件
来源：http://hz.vqdsnc.cn/gtizdhxptm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtvgoqfdmc.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtlughuvan.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtvmsfxdat.html

[R78] 交互式菜单
来源：http://hz.0kj1m.cn/gtiyixwgch.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtiiqsnqjv.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangkeji.top/gtdjpoetys.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guowangkeji.top/gtwwymttkh.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtrnmjrjqw.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtknxzwsre.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuvwrqqbv.html

S. C / C++ 专题
来源：http://hz.fengsongda.top/gtsaekfpbl.html

================================================================================
来源：http://hz.yj202588.top/gtklxmzwks.html

[S01] C：Hello World
来源：http://hz.jyoumei.cn/gtdnppjubd.html

#include <stdio.h>
来源：http://hz.zhixingplan.top/gtmnleifja.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtxmpvwzbx.html

[S02] C：变量与格式化输出
来源：http://hz.nwbrower.top/gtglsfshti.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtvmscplmr.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtafqetglz.html

int x; scanf("%d", &x);
来源：http://hz.snrcjt.cn/gtbskvpbcp.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtrqkdfvke.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ehwqpu.com/gtehcqamqd.html

[S05] C：字符串长度
来源：http://hz.jqgfzy.top/gtwdrfkfjy.html

strlen(s)
来源：http://hz.zhongyouzk.top/gtuvwdoewc.html

[S06] C：字符串比较
来源：http://hz.zhoulong.xyz/gtctnfvvvv.html

strcmp(a, b) == 0
来源：http://hz.52xcode.cn/gtdeykkkuq.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtlapqcbsb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yanxiufei.cn/gtkpyqfqyx.html

[S08] C：动态内存分配与释放
来源：http://hz.wangshuangyany.cn/gthgtzyxvt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtgrntxwhi.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtepusmema.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.iojbl.cn/gtshkjxtnl.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtfdkzpszu.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtwekktaex.html

[S11] C：逐行读文件
来源：http://hz.ivvv.top/gtudpqdaka.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtpqvcbmpx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.redwolf501.top/gtdzgfdqij.html

fclose(f);
来源：http://hz.cucudq.cn/gtrhjjukio.html

[S12] C：写文件
来源：http://hz.shzxlz.cn/gthrpwtoee.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jyoumei.cn/gtcrifpbrt.html

[S13] C：宏定义
来源：http://hz.guowangkeji.top/gtedogbdir.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cdnleiting.top/gtxfcunwbt.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gtiigynbji.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtymzjljcy.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtcphmlrjl.html

(double) a / b
来源：http://hz.cashguo.top/gtgsxcwxmj.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtliobqeev.html

x |= (1 << 3);
来源：http://hz.hywenlv.cn/gtavvpwznl.html

[S17] C：安全拼接字符串
来源：http://hz.smart0.xyz/gtkppzbzdv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gtbwzwnbbo.html

[S18] C：命令行参数
来源：http://hz.birdmap.top/gtomqawizn.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtbxrpfnpx.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtnhdutsqm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtyaewscpy.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gtixhwgijg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtbbhxushc.html

[S21] C：字符类别判断
来源：http://hz.jqgfzy.top/gtduxlvpgw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenlongwang.top/gthoczjqpn.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtoxrgouab.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtugxdjdko.html

[S23] C：随机数
来源：http://hz.andypj.xyz/gttrcpwtcl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yongpay.top/gthyndhhdc.html

[S24] C：获取本地时间
来源：http://hz.yuxming.cn/gtriwpbmsi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.haohaochexian.top/gthvbxeqmm.html

[S25] C：内存拷贝
来源：http://hz.iojbl.cn/gtofjhakjl.html

memcpy(dst, src, n);
来源：http://hz.meibo888.top/gthwlwasfn.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtkdjbncdb.html

memset(a, 0, sizeof a);
来源：http://hz.dashuyun.cn/gtkogrnhxm.html

[S27] C：定义常量
来源：http://hz.chenzaomai.com/gtjgmjhhai.html

const double PI = 3.14159;
来源：http://hz.hnqzz.top/gtslsrxmki.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gteqkshmop.html

static int counter = 0;
来源：http://hz.jinqigufen.top/gtgugtgjmo.html

[S29] C：变参函数
来源：http://hz.vqdsnc.cn/gtlwmfdvvv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtacirfuyh.html

[S30] C：头文件保护
来源：http://hz.nanxuanxn.top/gttvwukqns.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtvbuauxww.html

#define X_H
来源：http://hz.ybcxt.top/gtubcccnev.html

#endif
来源：http://hz.yonumen.top/gtgzgkcfbc.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtzovqxoqz.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtsrtzxxbq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnqzz.top/gtqthaxlsz.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtecxyjrux.html

std::string s = "hi";  s += "!";
来源：http://hz.zhiwuduotai.top/gtpyyyourh.html

[S33] C++：vector 增删
来源：http://hz.sysykeji.top/gtpxdvxspp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtykrhttxx.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtuzkucqtd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtfhruhybl.html

[S35] C++：map
来源：http://hz.ivvv.top/gtjwqohuol.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtmqyafxkw.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtnkaabkzf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtdniwxzyv.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtarcqevfm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtpwnirvmr.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtjwdfxlcf.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtvragsctm.html

[S39] C++：自定义比较器排序
来源：http://hz.hammf.cn/gtzniiwucv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtqlegltok.html

[S40] C++：查找元素
来源：http://hz.shuidangran.top/gtccikusby.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zdqjudy.top/gtujscksap.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtsnfeholr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtnehnljhr.html

[S42] C++：继承与虚函数
来源：http://hz.ppjwa.cn/gtxndtaevq.html

class B : public Base { public: void f() override {} };
来源：http://hz.ybcxt.top/gtioliwvui.html

[S43] C++：智能指针
来源：http://hz.jianghu66.top/gthjhoxsrs.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gtkelticyu.html

[S44] C++：引用传参
来源：http://hz.birdmap.top/gtabrzklff.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtlokipntd.html

[S45] C++：lambda
来源：http://hz.zhijiandao.cn/gtutijaafv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtauufakzh.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gteuwfncow.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.quarkkingdee.top/gtdtdiaiqy.html

[S47] C++：结构化绑定遍历
来源：http://hz.jyoumei.cn/gtrodttbpt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtugxsoaza.html

[S48] C++：逐行读文件
来源：http://hz.mhx1999.top/gtgympgyaa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gtfzswincr.html

while (std::getline(in, line)) { }
来源：http://hz.fengsongda.top/gtsoqylrma.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtmkqqiejh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gtqjwyriis.html

[S50] C++：格式化数字
来源：http://hz.vqdsnc.cn/gtqnxdulvh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtysrbukzh.html

[S51] C++：显式类型转换
来源：http://hz.haohaochexian.top/gtdxirbjqx.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtznwcovkq.html

[S52] C++：const 与 noexcept
来源：http://hz.zhiwuduotai.top/gtvurdgjhp.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtlvuscgph.html

[S53] C++：移动语义
来源：http://hz.zhiwuduotai.top/gtvzdhxxcc.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigfzy.top/gtpvkygmep.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gtmptybgkf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangshuangyany.cn/gtsivdjxfd.html

[S55] C++：结构化绑定
来源：http://hz.zhijiandao.cn/gtqfuzjfsw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhengqikj.top/gtmkaaxzpv.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtmezcbxoo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.mhx1999.top/gtayvwclut.html

[S57] C++：编译期常量
来源：http://hz.9152youxi.cn/gtqpehjyah.html

constexpr int N = 10;
来源：http://hz.birdmap.top/gtumnonnvi.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gtbaqkwiov.html

namespace ns { int f() { return 1; } }
来源：http://hz.kuanghao11.cn/gtvotyfbwj.html

[S59] C++：静态断言
来源：http://hz.zycfv.cn/gtxvptwocq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuxming.cn/gtlpcvzamf.html

[S60] C++：遍历并删除元素
来源：http://hz.yuxming.cn/gtyopgulwe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xinyue.icu/gtzqzlpsyp.html

================================================================================
来源：http://hz.sufxvd.cn/gtesryflcl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtdrgylaej.html

================================================================================
来源：http://hz.nwbrower.top/gtenlzbbby.html

[T01] Kotlin：Hello World
来源：http://hz.yj202588.top/gtfhlgjcrl.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtbcgehoys.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtmfaolmvv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtpzopskoo.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gtalrduzgo.html

"值: $b"
来源：http://hz.guannengcc.top/gtcpvyyifh.html

[T04] Kotlin：空安全
来源：http://hz.iojbl.cn/gttjhcqsrw.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtppolgleb.html

[T05] Kotlin：when 表达式
来源：http://hz.jiagoushi.top/gtputdtikb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shuidangran.top/gtropxwufh.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangtech.top/gtkwpzjqll.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinghuilouyu.cn/gtiolqjkgj.html

[T07] Kotlin：集合过滤
来源：http://hz.guowangkeji.top/gtdcuqcamf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtwzflezmk.html

[T08] Kotlin：数据类
来源：http://hz.zdqjudy.top/gtkdswrekb.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtkfqvyrrw.html

[T09] Kotlin：扩展函数
来源：http://hz.zhongyouzk.top/gtlxcswjhx.html

fun String.exclaim() = this + "!"
来源：http://hz.hnqzz.top/gteoydtbtx.html

[T10] Kotlin：默认参数
来源：http://hz.xziqi.cn/gtlohfkiip.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgufenzy.top/gtznqxyppb.html

[T11] Kotlin：协程
来源：http://hz.jiagoushi.top/gtiqqwieei.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guannengcc.top/gtaddjtbxx.html

[T12] Kotlin：解构声明
来源：http://hz.yangfankeji.com/gtzsovpsdt.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgfzy.top/gtmbbhiupp.html

[T13] Kotlin：只读 Map
来源：http://hz.zhaomingkeji.xyz/gtizzczjdx.html

val m = mapOf("a" to 1)
来源：http://hz.snrcjt.cn/gtzvjpclfv.html

[T14] Kotlin：循环
来源：http://hz.aizwys.cn/gtzfjydzhf.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtjysuqhiv.html

[T15] Kotlin：接口
来源：http://hz.gogol.net.cn/gtstdkvpso.html

interface Shape { fun area(): Double }
来源：http://hz.cqqwz.cn/gtrbjulmpd.html

[T16] Swift：Hello World
来源：http://hz.ydzc1.top/gtmupplytn.html

print("Hello")
来源：http://hz.zhixingplan.top/gtthwklxfa.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtasvarfgr.html

var a = 1;  let b = 2
来源：http://hz.wangshuangyany.cn/gtpahzajgz.html

[T18] Swift：字符串插值
来源：http://hz.iojbl.cn/gthaqrxsmo.html

"值: \(b)"
来源：http://hz.jinyuanbaomall.cn/gteorjclcd.html

[T19] Swift：可选绑定
来源：http://hz.ydzc1.top/gtajtierzd.html

if let n = opt { print(n) }
来源：http://hz.shangyingyoupin.top/gtbnwqbefx.html

[T20] Swift：数组操作
来源：http://hz.ehwqpu.com/gtjfizxlse.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guannengcc.top/gtxjmmuyom.html

[T21] Swift：遍历
来源：http://hz.smart0.xyz/gtknmynstr.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gthcdvvire.html

[T22] Swift：字典
来源：http://hz.shanyushiyangtech.top/gtylfwxqdd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xziqi.cn/gtbdlwkppq.html

[T23] Swift：函数
来源：http://hz.cashguo.top/gtxhgvvfji.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nwbrower.top/gttvfvevik.html

[T24] Swift：闭包
来源：http://hz.andypj.xyz/gthjuodxqi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtpzhlnlbt.html

[T25] Swift：结构体
来源：http://hz.svipenyu.cn/gtjrofqkwg.html

struct P { var x: Int }
来源：http://hz.yvedp.cn/gtemcrdjrs.html

[T26] Swift：类与重写
来源：http://hz.jinghuilouyu.cn/gtnyavgqca.html

class A: Base { override func f() {} }
来源：http://hz.zhongyouzk.top/gteulrardo.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtesygtgwy.html

do { try f() } catch { print(error) }
来源：http://hz.sufxvd.cn/gtyzkaixeo.html

[T28] Swift：枚举
来源：http://hz.redwolf501.top/gtmimnpkqq.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gteybxnffm.html

[T29] Swift：guard 提前返回
来源：http://hz.yongpay.top/gtlqdsuude.html

guard let x = opt else { return }
来源：http://hz.cdnleiting.top/gtfzzehqul.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gtlbfogluz.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangkeji.top/gtniiypxno.html

[T31] Lua：Hello World
来源：http://hz.0kj1m.cn/gtgwpevtcn.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtnzpgcuhx.html

[T32] Lua：局部变量
来源：http://hz.snrcjt.cn/gtjxrbevpk.html

local a = 1
来源：http://hz.zhijiandao.cn/gttbtkcgog.html

[T33] Lua：表（数组）
来源：http://hz.daxiang520.top/gtxyshxcrq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.52xcode.cn/gtdkqrhgbx.html

[T34] Lua：遍历表
来源：http://hz.pengpengdd.cyou/gtqjjpgyqe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinyuanbaomall.cn/gtdlszexex.html

[T35] Lua：字典表
来源：http://hz.cdnleiting.top/gtlellfdnp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jqgufenzy.top/gtwktqbwjf.html

[T36] Lua：函数
来源：http://hz.svipenyu.cn/gtnkjupdhv.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gtnrfvnuvr.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtutloairz.html

"a" .. "b"
来源：http://hz.cheryme.top/gttwatnyto.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtigyvqcft.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gtjenizone.html

[T39] Lua：模式匹配
来源：http://hz.xylfe.cn/gtqpujzhpu.html

string.find(s, "%d+")
来源：http://hz.cqqwz.cn/gtkuamasxe.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gtkgzbhpce.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gtvsvrcyil.html

[T41] Perl：Hello World
来源：http://hz.ppjwa.cn/gtldhbclix.html

print "Hello\n";
来源：http://hz.wangdashe.top/gtqauohdte.html

[T42] Perl：变量类型
来源：http://hz.havefunace.top/gtpblspgng.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gtlkmyhgyr.html

[T43] Perl：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtadmzfjxh.html

"值: $a"
来源：http://hz.gzhubu.top/gtpwbuuglp.html

[T44] Perl：条件
来源：http://hz.jinghuilouyu.cn/gtglkqlshp.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtszocgsdn.html

[T45] Perl：数组遍历
来源：http://hz.nwbrower.top/gtjsfzncsv.html

for my $x (@arr) { print $x; }
来源：http://hz.zhoulong.xyz/gtpbmwahnc.html

[T46] Perl：哈希操作
来源：http://hz.xingfuxueyuan.xyz/gtomkllzsy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jlsjyb.cn/gtdmybvcru.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangkeji.top/gtzyrfqeaw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenlongwang.top/gtknhpojen.html

[T48] Perl：正则替换
来源：http://hz.zhixingplan.top/gtisetsebp.html

$s =~ s/old/new/g;
来源：http://hz.hnqzz.top/gtuhnrxfqm.html

[T49] Perl：函数
来源：http://hz.chenjidiqi.icu/gttyziuseh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gthiqiohuy.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gtdadjhsoq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.quarkkingdee.top/gtfbjrxtxd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtwqwrvipc.html

[T51] Scala：Hello World
来源：http://hz.daria6918.cn/gtkjlpzmct.html

println("Hello")
来源：http://hz.guowangkeji.top/gtbmjtkeps.html

[T52] Scala：变量
来源：http://hz.nwbrower.top/gtizrktmzz.html

val a = 1;  var b = 2
来源：http://hz.haohaochexian.top/gtwozchnjz.html

[T53] Scala：字符串插值
来源：http://hz.shangyingyoupin.top/gtakrwhzyw.html

s"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtphyixidj.html

[T54] Scala：集合映射
来源：http://hz.xylfe.cn/gtswwzyimv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhengqikj.top/gtlutaaevc.html

[T55] Scala：集合过滤
来源：http://hz.yanxiufei.cn/gtymuzchxc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yanxiufei.cn/gtjyrgngjv.html

[T56] Scala：样例类
来源：http://hz.hongshengwenyu.top/gtueudkhun.html

case class User(name: String, age: Int)
来源：http://hz.316326.xyz/gtvzmxgqjl.html

[T57] Scala：模式匹配
来源：http://hz.jinghuilouyu.cn/gtbbulqync.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhixingplan.top/gtcfrzcusd.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gtqkruxjey.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.quarkkingdee.top/gtuibacnlw.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gtkngdavou.html

for (i <- 1 to 10) println(i)
来源：http://hz.cucudq.cn/gtcvtxijlc.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gttaxumjgk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dashuyun.cn/gtrjbrhufa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthppvmxin.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtelvexciz.html

================================================================================
来源：http://hz.fzhhl.top/gtvmuyqjpw.html

[U01] Py：创建虚拟环境
来源：http://hz.nanxinkj.top/gtmfzidusr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gtsaxdiney.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cashguo.top/gttbpjdywt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj202588.top/gtqugtiugy.html

[U03] Py：加载 .env 配置
来源：http://hz.redwolf501.top/gtnhumbhma.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shzxlz.cn/gtebgzzhjl.html

[U04] Py：变量调试打印
来源：http://hz.jianghu66.top/gtnsaprudr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuanzx.com/gtnctdqxfj.html

[U05] Py：列表去重且保序
来源：http://hz.316326.xyz/gtmhcotidt.html

list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtjkajndaq.html

[U06] Py：合并两个字典
来源：http://hz.tanke756.top/gtupkcrhcw.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtmrfcwfoi.html

[U07] Py：反转字典键值
来源：http://hz.wangshuangyany.cn/gtekfcaesz.html

{v: k for k, v in d.items()}
来源：http://hz.ydzc1.top/gtshluzgpl.html

[U08] Py：展平二维列表
来源：http://hz.dianchejie.cn/gttruorcyc.html

[y for x in nested for y in x]
来源：http://hz.shuidangran.top/gtaefupyow.html

[U09] Py：字典取最大值的键
来源：http://hz.fengsongda.top/gtsxiovads.html

max(d, key=d.get)
来源：http://hz.daria6918.cn/gtzdebyqrt.html

[U10] Py：按值排序字典
来源：http://hz.yj20258888.top/gtteqtsxiv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sysykeji.top/gtwjbpqihs.html

[U11] Py：生成器表达式
来源：http://hz.nwbrower.top/gtcytviwiv.html

(x * 2 for x in arr)
来源：http://hz.xziqi.cn/gtupwdgbaq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.9152youxi.cn/gtxitnpyci.html

Counter(arr).most_common(3)
来源：http://hz.bjfxy.top/gtfrbfzoth.html

[U13] Py：固定长度队列
来源：http://hz.chenzaomai.com/gtjhoyqgbh.html

deque(maxlen=10)
来源：http://hz.meibo888.top/gthxfjkiin.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtdfgtlmvv.html

defaultdict(list)
来源：http://hz.xingfuxueyuan.xyz/gtpjebmxvj.html


<!-- 参考信息 -->