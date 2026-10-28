代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtqnexuhfy.html

[R76] 使用临时文件
来源：http://hz.nanxuanxn.top/gttedaylff.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtnltrmlah.html

[R77] 读取用户输入
来源：http://hz.cashguo.top/gtcuhqsvaw.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtjuuhgihs.html

[R78] 交互式菜单
来源：http://hz.zhaomingkeji.xyz/gthzehjlkv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangtech.top/gtgvmqfbbr.html

[R79] 解析命令行选项
来源：http://hz.aibaodan.cn/gtonjcxbwf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.smart0.xyz/gtycftftes.html

[R80] 查看脚本执行耗时
来源：http://hz.bjfxy.top/gtkoxglffw.html

time ./run.sh
来源：http://hz.jinyuanbaomall.cn/gtiztpyqqh.html

================================================================================
来源：http://hz.zhixingplan.top/gtkszozfpb.html

S. C / C++ 专题
来源：http://hz.vqdsnc.cn/gtnjvnxvlx.html

================================================================================
来源：http://hz.316326.xyz/gtgxaeqsnw.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtnhweruvm.html

#include <stdio.h>
来源：http://hz.shangyingyoupin.top/gtcmtdemjv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pengpengdd.cyou/gtpydksqco.html

[S02] C：变量与格式化输出
来源：http://hz.dianchejie.cn/gtjfksptjt.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnqzz.top/gtroaddzsw.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtldwrsizn.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtwrbmawfr.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtvqpckybe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxinkj.top/gtoxhgddny.html

[S05] C：字符串长度
来源：http://hz.jiagoushi.top/gtqvzxmuyq.html

strlen(s)
来源：http://hz.cdnleiting.top/gtjkmjnyit.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtdrqmqcwu.html

strcmp(a, b) == 0
来源：http://hz.aizwys.cn/gthehserwm.html

[S07] C：数组遍历求和
来源：http://hz.mhx1999.top/gtwaxxqwnd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.bjfxy.top/gtiwqejzib.html

[S08] C：动态内存分配与释放
来源：http://hz.jiagoushi.top/gtmjraqtbe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258.top/gtkslrkzeb.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gtfabjncoz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guowangkeji.top/gtmijoppyj.html

[S10] C：指针与解引用
来源：http://hz.jqgufenzy.top/gtxhsmigxh.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtbxcbqbat.html

[S11] C：逐行读文件
来源：http://hz.zhengqikj.top/gtcoeobpdl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yanxiufei.cn/gtymugznpu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258.top/gtjbsysdbe.html

fclose(f);
来源：http://hz.dianchejie.cn/gthhxdauik.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtocnfgckw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtzseganvk.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtnprssxjd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gotoacloud.top/gtqowckspp.html

[S14] C：枚举
来源：http://hz.yongpay.top/gtjytusmlm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gtjtahifps.html

[S15] C：类型转换
来源：http://hz.shanyushiyangtech.top/gtxyntrijv.html

(double) a / b
来源：http://hz.zdqjudy.top/gtwzdlrbnn.html

[S16] C：位操作置位
来源：http://hz.yongpay.top/gtviewbvfg.html

x |= (1 << 3);
来源：http://hz.gaohongyu789.top/gtkaunqbgn.html

[S17] C：安全拼接字符串
来源：http://hz.wangdashe.top/gthctarplf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gtzllaxeod.html

[S18] C：命令行参数
来源：http://hz.vqdsnc.cn/gtsbsfvqmp.html

int main(int argc, char **argv)
来源：http://hz.jiagoushi.top/gtkfhhwxvj.html

[S19] C：快速排序
来源：http://hz.dianchejie.cn/gtfezgpull.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtsqinglzu.html

[S20] C：二分查找
来源：http://hz.ivvv.top/gtbgrghiav.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtdpkihvic.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtkdddnbju.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtfvcgfoft.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtkrqoptoz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtxrsxagix.html

[S23] C：随机数
来源：http://hz.jinyuanbaomall.cn/gtywtitctg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guowangkeji.top/gtfuwzpnhx.html

[S24] C：获取本地时间
来源：http://hz.hfpthk.cn/gtrgoiiopo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhiwuduotai.top/gtfuuxrerm.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtslhmcdte.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtryspeuxl.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gtlbpmfjpi.html

memset(a, 0, sizeof a);
来源：http://hz.jlsjyb.cn/gtzwupiebb.html

[S27] C：定义常量
来源：http://hz.yj20258.top/gtzsuhoggr.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gttlozqrvt.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gteubhrjxb.html

static int counter = 0;
来源：http://hz.yuxming.cn/gtkddnenrq.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtabnrxllo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuanzx.com/gtemrzqmko.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtwqubkgpl.html

#ifndef X_H
来源：http://hz.shuidangran.top/gtwhaflsnx.html

#define X_H
来源：http://hz.jinyuanbaomall.cn/gthjwwissd.html

#endif
来源：http://hz.sxryk.cn/gtkxcbylkn.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtflqdzpym.html

#include <iostream>
来源：http://hz.fzhhl.top/gthtsakwls.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gttsflkndg.html

[S32] C++：字符串
来源：http://hz.svipenyu.cn/gtqohoprxp.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gtdzwpybjv.html

[S33] C++：vector 增删
来源：http://hz.xinyue.icu/gtuixacqhl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnxiangtu.top/gtgbonwjof.html

[S34] C++：遍历 vector
来源：http://hz.zhaomingkeji.xyz/gtqwrfkvim.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj202588.top/gtiufntwri.html

[S35] C++：map
来源：http://hz.svipenyu.cn/gtctazqeef.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gteqpvaxcm.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gtnswnndcz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtrzrgoxyh.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtriazfvte.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtzqvhsrux.html

[S38] C++：排序
来源：http://hz.sweek.top/gtuavnhepq.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtklcvbxco.html

[S39] C++：自定义比较器排序
来源：http://hz.kuanghao11.cn/gtzvsxjghi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtgwmgtuaw.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gtwioysmgm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtwviybxsj.html

[S41] C++：类与构造函数
来源：http://hz.jyoumei.cn/gtyzoujmjj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gtohomfnwa.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtsixzqnre.html

class B : public Base { public: void f() override {} };
来源：http://hz.aizwys.cn/gtjdgnsfpf.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtoevtweak.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtwogbwlby.html

[S44] C++：引用传参
来源：http://hz.cdnleiting.top/gtijntigsy.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gtipunkvzr.html

[S45] C++：lambda
来源：http://hz.svipenyu.cn/gtpsursgnb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtxqugxxdw.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gtgmyntahq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtxcoduepm.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtklspzmpl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daria6918.cn/gtrsiflekc.html

[S48] C++：逐行读文件
来源：http://hz.wangdashe.top/gtgorkrzwy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.redwolf501.top/gtmskorpfj.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtczsgcxzv.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtcvzfphqe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtszwzsdyu.html

[S50] C++：格式化数字
来源：http://hz.xinyue.icu/gtitfjlpkq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gogol.net.cn/gtoiwdefye.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gtwuadrbbw.html

static_cast<double>(a) / b
来源：http://hz.yj202588.top/gtdfiynckd.html

[S52] C++：const 与 noexcept
来源：http://hz.wangshuangyany.cn/gttwzzoqqs.html

int size() const noexcept { return n_; }
来源：http://hz.jqgfzy.top/gthyvcnmma.html

[S53] C++：移动语义
来源：http://hz.yuanzhike.top/gtxsfewphq.html

std::vector<int> w = std::move(v);
来源：http://hz.svipenyu.cn/gtnbwybwrw.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gtjrcgiosv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.9152youxi.cn/gtnwgiiwbw.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gttfebbwja.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dashuyun.cn/gtlkfojpyr.html

[S56] C++：optional
来源：http://hz.shanyushiyangkeji.top/gtjeugilbr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.smart0.xyz/gtenooesat.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtavxxexey.html

constexpr int N = 10;
来源：http://hz.ydjk.org.cn/gthcfxulpw.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangkeji.top/gtwegrqqzb.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gthonxrvvr.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtprlylrco.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.quarkkingdee.top/gteqsyggsl.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtcfbwcsii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtrrzptwly.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbfmhrnqd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtxgqclqol.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnfykehqq.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gteyvqnogb.html

println("Hello")
来源：http://hz.andypj.xyz/gtfxilxhcg.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtqevboaan.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gtddmwmqaa.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangtech.top/gtlwvstxve.html

"值: $b"
来源：http://hz.ppjwa.cn/gthlwnqtfd.html

[T04] Kotlin：空安全
来源：http://hz.zhiwuduotai.top/gtppgvixsj.html

val n: String? = null;  n?.length
来源：http://hz.zhoulong.xyz/gtuwacqpbq.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtspklyjcq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gaohongyu789.top/gtsfcmbspq.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gtpeobzmjd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtlsiwktzs.html

[T07] Kotlin：集合过滤
来源：http://hz.zhiwuduotai.top/gtnyhvfbwq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.c1oappe.top/gtoxgaddyd.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtbjbuduoz.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gtzmjqzcty.html

[T09] Kotlin：扩展函数
来源：http://hz.zhijiandao.cn/gtvlkjtuev.html

fun String.exclaim() = this + "!"
来源：http://hz.cqqwz.cn/gtjbvwpowy.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtfzjroinb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtqovyzszc.html

[T11] Kotlin：协程
来源：http://hz.zhaomingkeji.xyz/gthakqpgev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhoulong.xyz/gtqduixasy.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtiljjjmlw.html

val (a, b) = Pair(1, 2)
来源：http://hz.pycfn.com/gtbwjxuvgg.html

[T13] Kotlin：只读 Map
来源：http://hz.yangfankeji.com/gtymsrafzh.html

val m = mapOf("a" to 1)
来源：http://hz.cdnleiting.top/gtlnyzacsu.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtpunfuhwq.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtwcyolhjv.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtcyntzyie.html

interface Shape { fun area(): Double }
来源：http://hz.dashuyun.cn/gtzikvkiud.html

[T16] Swift：Hello World
来源：http://hz.hywenlv.cn/gtbaskqlhx.html

print("Hello")
来源：http://hz.jyoumei.cn/gtcygexgvo.html

[T17] Swift：变量与常量
来源：http://hz.shangyingyoupin.top/gtokflxqfk.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtgtpqudhx.html

[T18] Swift：字符串插值
来源：http://hz.dashuyun.cn/gtykufmtxt.html

"值: \(b)"
来源：http://hz.smart0.xyz/gtikubypid.html

[T19] Swift：可选绑定
来源：http://hz.sufxvd.cn/gtxvyzifmk.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtuuiglrqf.html

[T20] Swift：数组操作
来源：http://hz.shangyingyoupin.top/gtqiqwzikx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ydjk.org.cn/gthhsgemvc.html

[T21] Swift：遍历
来源：http://hz.andypj.xyz/gtftdkcbas.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gthwukkqde.html

[T22] Swift：字典
来源：http://hz.quarkkingdee.top/gtrxljqbvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtkjibnydc.html

[T23] Swift：函数
来源：http://hz.meibo888.top/gtsdtxeeto.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangtech.top/gttxksevbi.html

[T24] Swift：闭包
来源：http://hz.daxiang520.top/gthroypnda.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenlongwang.top/gtvakejtmh.html

[T25] Swift：结构体
来源：http://hz.vqdsnc.cn/gtmozfoqtq.html

struct P { var x: Int }
来源：http://hz.jyoumei.cn/gteawjorzn.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtzjeestmd.html

class A: Base { override func f() {} }
来源：http://hz.tianlin.xyz/gtqqrvgqse.html

[T27] Swift：错误处理
来源：http://hz.xuetiantiany.cn/gtzsgmspyx.html

do { try f() } catch { print(error) }
来源：http://hz.yuxming.cn/gtxqdoxibj.html

[T28] Swift：枚举
来源：http://hz.daria6918.cn/gtcrjcgcxy.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtdxqvpgye.html

[T29] Swift：guard 提前返回
来源：http://hz.jianghu66.top/gtxcsuwauj.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gtljkjzhgt.html

[T30] Swift：协议
来源：http://hz.yueranfly.top/gtuteyatej.html

protocol Shape { func area() -> Double }
来源：http://hz.gogol.net.cn/gtlbrzwkil.html

[T31] Lua：Hello World
来源：http://hz.jqgfzy.top/gtlymszgvn.html

print("Hello")
来源：http://hz.52xcode.cn/gtcaesyama.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtdwcntkyx.html

local a = 1
来源：http://hz.hfpthk.cn/gtawegupwf.html

[T33] Lua：表（数组）
来源：http://hz.gaohongyu789.top/gtnsbibumw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hongshengwenyu.top/gtkfcnnrgw.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtmpcsamwt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jlsjyb.cn/gtjqulgget.html

[T35] Lua：字典表
来源：http://hz.smart0.xyz/gtozmfpatl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yvedp.cn/gtpgkkswlc.html

[T36] Lua：函数
来源：http://hz.jqgfzy.top/gtynfyhwtj.html

function add(a, b) return a + b end
来源：http://hz.zhongyouzk.top/gtfrcumbdo.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtijxqvlqa.html

"a" .. "b"
来源：http://hz.cashguo.top/gtszrafeld.html

[T38] Lua：条件
来源：http://hz.yuxming.cn/gtodsttucl.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtdmnrugxl.html

[T39] Lua：模式匹配
来源：http://hz.sweek.top/gtanefiicr.html

string.find(s, "%d+")
来源：http://hz.yj20258888.top/gtbqczhogh.html

[T40] Lua：元表
来源：http://hz.yj20258888.top/gtbatpztlx.html

setmetatable({}, { __index = base })
来源：http://hz.yangfankeji.com/gthgzhkuvx.html

[T41] Perl：Hello World
来源：http://hz.gogol.net.cn/gtvepbbvrd.html

print "Hello\n";
来源：http://hz.yuanzhike.top/gtzgfyetsl.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gttkfwpktx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ywan-chungtsiang.top/gtdcgytslw.html

[T43] Perl：字符串插值
来源：http://hz.zdqjudy.top/gtvbzklzgs.html

"值: $a"
来源：http://hz.yangfankeji.com/gtfrezeqhc.html

[T44] Perl：条件
来源：http://hz.vqdsnc.cn/gtnacpvkjx.html

if ($a > 0) { print "正"; }
来源：http://hz.tian-w.cn/gtjunsvvdy.html

[T45] Perl：数组遍历
来源：http://hz.yonumen.top/gtutrbwrge.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgfzy.top/gtvaevedqb.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gtsbgsgxgt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgfzy.top/gtktrjjpre.html

[T47] Perl：正则捕获
来源：http://hz.cucudq.cn/gtvavgxwxn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangdashe.top/gtqaewfzck.html

[T48] Perl：正则替换
来源：http://hz.ydjk.org.cn/gtgsloxsnm.html

$s =~ s/old/new/g;
来源：http://hz.birdmap.top/gtsmuhjxdo.html

[T49] Perl：函数
来源：http://hz.andypj.xyz/gtdcsmqjiy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenlongwang.top/gttijleslh.html

[T50] Perl：逐行读文件
来源：http://hz.hywenlv.cn/gtqnfegvng.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.c1oappe.top/gtdpnmtgax.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.c1oappe.top/gtgbdexsyo.html

[T51] Scala：Hello World
来源：http://hz.sweek.top/gtsczaifjw.html

println("Hello")
来源：http://hz.haohaochexian.top/gtmtajlrbj.html

[T52] Scala：变量
来源：http://hz.hongshengwenyu.top/gtbhyhlhpe.html

val a = 1;  var b = 2
来源：http://hz.ybcxt.top/gtpjkkmmva.html

[T53] Scala：字符串插值
来源：http://hz.0kj1m.cn/gtgeiwuinl.html

s"值: $b"
来源：http://hz.gaohongyu789.top/gtdxiszbjl.html

[T54] Scala：集合映射
来源：http://hz.vqdsnc.cn/gthbkgxhrx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.vqdsnc.cn/gtpytxtigh.html

[T55] Scala：集合过滤
来源：http://hz.9152youxi.cn/gtqwquxugf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgfzy.top/gtavoxhspg.html

[T56] Scala：样例类
来源：http://hz.haohaochexian.top/gtrrshzvcv.html

case class User(name: String, age: Int)
来源：http://hz.kuanghao11.cn/gtcbxycidh.html

[T57] Scala：模式匹配
来源：http://hz.cheryme.top/gttraopzxe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pycfn.com/gtoatavebz.html

[T58] Scala：函数定义
来源：http://hz.xuanzx.com/gtrbwojyyg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hfpthk.cn/gtgxdtsfye.html

[T59] Scala：循环
来源：http://hz.aibaodan.cn/gtlobazcow.html

for (i <- 1 to 10) println(i)
来源：http://hz.mhx1999.top/gtbghqxxwt.html

[T60] Scala：折叠
来源：http://hz.andypj.xyz/gtthftczka.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shangyingyoupin.top/gtgtgzbigv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuckuvkro.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtnhswvhpz.html

================================================================================
来源：http://hz.mhx1999.top/gtwcolxonv.html

[U01] Py：创建虚拟环境
来源：http://hz.sysykeji.top/gtkbylvwnz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gtwkccfney.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xingfuxueyuan.xyz/gtzhssachc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ppjwa.cn/gtekuvydkt.html

[U03] Py：加载 .env 配置
来源：http://hz.vqdsnc.cn/gtcntkiwwl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinghuilouyu.cn/gthufpgcqd.html

[U04] Py：变量调试打印
来源：http://hz.zhaomingkeji.xyz/gtlhnwpuzm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xziqi.cn/gtxctpbina.html

[U05] Py：列表去重且保序
来源：http://hz.redwolf501.top/gtdfmkjnpd.html

list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtvzhtdixu.html

[U06] Py：合并两个字典
来源：http://hz.ydzc1.top/gtesuusszv.html

{**a, **b}
来源：http://hz.nanxinkj.top/gtubxzrvoj.html

[U07] Py：反转字典键值
来源：http://hz.chenjidiqi.icu/gtvdryzxlb.html

{v: k for k, v in d.items()}
来源：http://hz.zycfv.cn/gtrssufqvu.html

[U08] Py：展平二维列表
来源：http://hz.nwbrower.top/gtfynpybus.html

[y for x in nested for y in x]
来源：http://hz.ydjk.org.cn/gtikqvytyu.html

[U09] Py：字典取最大值的键
来源：http://hz.shuidangran.top/gtaoyyuqpn.html

max(d, key=d.get)
来源：http://hz.c1oappe.top/gttucxtrvz.html

[U10] Py：按值排序字典
来源：http://hz.zhongyouzk.top/gtaxekjehm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yongpay.top/gtlpzatwtw.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtisxekvpv.html

(x * 2 for x in arr)
来源：http://hz.hnxiangtu.top/gttzoxhrid.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtsxyrghhz.html

Counter(arr).most_common(3)
来源：http://hz.xinyue.icu/gtgzufihoi.html

[U13] Py：固定长度队列
来源：http://hz.ybcxt.top/gteeiosyxa.html

deque(maxlen=10)
来源：http://hz.shangyingyoupin.top/gtvcotablv.html

[U14] Py：分组收集到列表
来源：http://hz.birdmap.top/gtfwksqykr.html

defaultdict(list)
来源：http://hz.ydzc1.top/gtrjhavhva.html

[U15] Py：高精度计时
来源：http://hz.0kj1m.cn/gttgcukjec.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtoyhdzamu.html

[U16] Py：命令行参数解析
来源：http://hz.hysaishi.cn/gtexkqdshf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cqqwz.cn/gtdosvqjvz.html


<!-- 参考信息 -->