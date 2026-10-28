代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtmexwoalz.html

[R76] 使用临时文件
来源：http://hz.gotoacloud.top/gtcdfwmaad.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtdvmqqrww.html

[R77] 读取用户输入
来源：http://hz.svipenyu.cn/gtcxcdmnby.html

read -rp "请输入: " ans
来源：http://hz.nwbrower.top/gtwvalkyef.html

[R78] 交互式菜单
来源：http://hz.zhiwuduotai.top/gtcppjdreg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cheryme.top/gthtjoyrzd.html

[R79] 解析命令行选项
来源：http://hz.shangyingyoupin.top/gtycefglwz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangkeji.top/gtvhzizvwn.html

[R80] 查看脚本执行耗时
来源：http://hz.zycfv.cn/gtnmqfyfce.html

time ./run.sh
来源：http://hz.jlsjyb.cn/gtrxmoybvm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtpdhkbaew.html

S. C / C++ 专题
来源：http://hz.yuxming.cn/gtpvjfmvtb.html

================================================================================
来源：http://hz.yonumen.top/gtdtqabkqg.html

[S01] C：Hello World
来源：http://hz.quarkkingdee.top/gtlccsyros.html

#include <stdio.h>
来源：http://hz.snrcjt.cn/gtkdyvmzmt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cheryme.top/gtevcmemtk.html

[S02] C：变量与格式化输出
来源：http://hz.52xcode.cn/gtdlbqcgzl.html

int a = 10; printf("%d\n", a);
来源：http://hz.havefunace.top/gtnbrwaloe.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtqxegadwf.html

int x; scanf("%d", &x);
来源：http://hz.fzhhl.top/gtkeyavhuy.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gtdxrmtssx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yanxiufei.cn/gtaqbilmoo.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gtikqyedok.html

strlen(s)
来源：http://hz.52xcode.cn/gtreccdsjn.html

[S06] C：字符串比较
来源：http://hz.zdqjudy.top/gthorgbgnp.html

strcmp(a, b) == 0
来源：http://hz.redwolf501.top/gtjnmabxlc.html

[S07] C：数组遍历求和
来源：http://hz.zdqjudy.top/gthkgrteyt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtlorzwilg.html

[S08] C：动态内存分配与释放
来源：http://hz.fengsongda.top/gtdmxyvrco.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guowangkeji.top/gtnkiwigjf.html

[S09] C：结构体定义与初始化
来源：http://hz.quarkkingdee.top/gtwpmlgcya.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhiwuduotai.top/gtawyxwiyk.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtzwicbcsg.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtuimwigqt.html

[S11] C：逐行读文件
来源：http://hz.cdnleiting.top/gtwkdkbmyf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtbtpnhndt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yvedp.cn/gtutgkgbtf.html

fclose(f);
来源：http://hz.shuidangran.top/gtqhlgeyhx.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtswicchyj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dashuyun.cn/gtsogldrqq.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtdzsjkhhn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shuidangran.top/gtbchutcxx.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gthbvjwgrp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yanxiufei.cn/gttektzukx.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtxsnsxouq.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtosktecvg.html

[S16] C：位操作置位
来源：http://hz.havefunace.top/gtwjlokdbv.html

x |= (1 << 3);
来源：http://hz.yj20258888.top/gtrvqilaix.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtsyviwqco.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fzhhl.top/gtdbkdswdh.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtnhwblirh.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gtulsjgkko.html

[S19] C：快速排序
来源：http://hz.yj202588.top/gtctudlage.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtiupdnknk.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtherkgued.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtrrmhrhqs.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtegsbviiq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sweek.top/gtjyyxjpal.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gtwqjdexqh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shuidangran.top/gtpnkjdjvp.html

[S23] C：随机数
来源：http://hz.ivvv.top/gtnmucecmc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtmmbninqt.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtmbjkmivq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtpshzxhoc.html

[S25] C：内存拷贝
来源：http://hz.xingfuxueyuan.xyz/gthjnmeoob.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtnusrxcwm.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gtmaqtsgxv.html

memset(a, 0, sizeof a);
来源：http://hz.jinghuilouyu.cn/gtdxuwjhfu.html

[S27] C：定义常量
来源：http://hz.svipenyu.cn/gtnituumuh.html

const double PI = 3.14159;
来源：http://hz.ybcxt.top/gtiqkzczbt.html

[S28] C：静态变量
来源：http://hz.cdnleiting.top/gtxvjgunva.html

static int counter = 0;
来源：http://hz.andypj.xyz/gtojcyjsvc.html

[S29] C：变参函数
来源：http://hz.jinyuanbaomall.cn/gtmmcmohgl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258888.top/gtgwvsminu.html

[S30] C：头文件保护
来源：http://hz.hfpthk.cn/gtvlvaspoy.html

#ifndef X_H
来源：http://hz.jinqigufen.top/gtzfpgzpoe.html

#define X_H
来源：http://hz.cucudq.cn/gtcphqbttf.html

#endif
来源：http://hz.yuxming.cn/gtdlbgtbaz.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtflyrtklu.html

#include <iostream>
来源：http://hz.shanyushiyangkeji.top/gtljczwoxu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtdzaaiwhk.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtkhtatfwu.html

std::string s = "hi";  s += "!";
来源：http://hz.bjfxy.top/gtehnkssiy.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtohcrgioy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtqxhgdtiz.html

[S34] C++：遍历 vector
来源：http://hz.yj20258888.top/gtuqqghddy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.birdmap.top/gtqdmtykkt.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtjsykqpow.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtcnlbiymo.html

[S36] C++：unordered_map
来源：http://hz.aizwys.cn/gtkkqjplma.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtrhidqrvw.html

[S37] C++：set
来源：http://hz.hfpthk.cn/gtufsxbqld.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shuidangran.top/gtunesaowa.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtqltzbqty.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtdzjpmuqn.html

[S39] C++：自定义比较器排序
来源：http://hz.ehwqpu.com/gtuxeourwj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhaomingkeji.xyz/gtveaoqpqs.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtlumfyqlw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.svipenyu.cn/gtrzepqnqn.html

[S41] C++：类与构造函数
来源：http://hz.jqgfzy.top/gtzlbjrvnq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.mhx1999.top/gtbbbmbwex.html

[S42] C++：继承与虚函数
来源：http://hz.shangyingyoupin.top/gtitwukuis.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtatjlcliw.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtrdrypegf.html

auto p = std::make_unique<int>(5);
来源：http://hz.52xcode.cn/gtdxxixwkk.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtpawdmlmq.html

void inc(int &x) { ++x; }
来源：http://hz.sxryk.cn/gtqbedxlvp.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtuhpadvjv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtbkwlufuo.html

[S46] C++：函数模板
来源：http://hz.xylfe.cn/gtmjhrpqin.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtnbdtqtpt.html

[S47] C++：结构化绑定遍历
来源：http://hz.hongshengwenyu.top/gtugemgagl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigfzy.top/gtqlcelhyc.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtiqmtwlvm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtszhplgse.html

while (std::getline(in, line)) { }
来源：http://hz.yuanzhike.top/gtxdrcuzpd.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtulmuezhb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tanke756.top/gtphhmhpkj.html

[S50] C++：格式化数字
来源：http://hz.feifeiyinyue.top/gtfxpvaexb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258.top/gttllrgkvt.html

[S51] C++：显式类型转换
来源：http://hz.zhijiandao.cn/gtxdpqcybq.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gtppfaczgc.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtzxuuokja.html

int size() const noexcept { return n_; }
来源：http://hz.redwolf501.top/gthibgzloi.html

[S53] C++：移动语义
来源：http://hz.jinyuanbaomall.cn/gtzpkgdakh.html

std::vector<int> w = std::move(v);
来源：http://hz.redwolf501.top/gtbkeopnoe.html

[S54] C++：异常处理
来源：http://hz.shzxlz.cn/gtjmxjaqrm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gtduebwrcd.html

[S55] C++：结构化绑定
来源：http://hz.wangshuangyany.cn/gtkhbctxcn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenzaomai.com/gtwcwxuvum.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtnuuferdf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtahflpkex.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gtmkzkmxcv.html

constexpr int N = 10;
来源：http://hz.guowangkeji.top/gtztixlrwu.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gtzwwjxdpw.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtztzkkzkc.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gteaunpmhh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daxiang520.top/gthdyzqwhy.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gtjvplscat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.feifeiyinyue.top/gttdimsuqx.html

================================================================================
来源：http://hz.mhx1999.top/gtpotpcdwt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gthttmzofv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtbtzcosbt.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtrsscgvxy.html

println("Hello")
来源：http://hz.xziqi.cn/gtkduirskl.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtgovqgsvj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gttagseyke.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtgbzgsbqw.html

"值: $b"
来源：http://hz.nanxuanxn.top/gtaegfkxtg.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtmjlbpjqw.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtbygealhs.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtobatznfd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtqojzfkzw.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangkeji.top/gtsemsniwj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtjpipuonl.html

[T07] Kotlin：集合过滤
来源：http://hz.iojbl.cn/gtfbfckbfk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.quarkkingdee.top/gtmcnbcrgs.html

[T08] Kotlin：数据类
来源：http://hz.9152youxi.cn/gtwmeillnb.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtzbqkwxsb.html

[T09] Kotlin：扩展函数
来源：http://hz.havefunace.top/gtywywdasp.html

fun String.exclaim() = this + "!"
来源：http://hz.9152youxi.cn/gtimmieutf.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtxbprhtht.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cheryme.top/gtnwcwxywf.html

[T11] Kotlin：协程
来源：http://hz.cashguo.top/gtuliycuxx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuanzx.com/gthymgmivo.html

[T12] Kotlin：解构声明
来源：http://hz.yuxming.cn/gternvcpkp.html

val (a, b) = Pair(1, 2)
来源：http://hz.nwbrower.top/gtotmvmhgd.html

[T13] Kotlin：只读 Map
来源：http://hz.ivvv.top/gtmvdzpphi.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gthxszclsj.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtwlwpogyq.html

for (i in 1..10) println(i)
来源：http://hz.hfpthk.cn/gtcrizhrbd.html

[T15] Kotlin：接口
来源：http://hz.ybcxt.top/gtvcrllqzj.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtndutdjus.html

[T16] Swift：Hello World
来源：http://hz.sxryk.cn/gtqaldmjms.html

print("Hello")
来源：http://hz.jianghu66.top/gtdzqmsccp.html

[T17] Swift：变量与常量
来源：http://hz.nwbrower.top/gtpiptknlh.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gtfukfjxsi.html

[T18] Swift：字符串插值
来源：http://hz.yuxming.cn/gtyjudhdbh.html

"值: \(b)"
来源：http://hz.tanke756.top/gtcflhjlgi.html

[T19] Swift：可选绑定
来源：http://hz.vqdsnc.cn/gtvmsmccxp.html

if let n = opt { print(n) }
来源：http://hz.yongpay.top/gtnzqoxroe.html

[T20] Swift：数组操作
来源：http://hz.guowangkeji.top/gtttmdwzxo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtkeipoiuw.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtaugcwuvb.html

for x in a { print(x) }
来源：http://hz.jinghuilouyu.cn/gtdkuhglug.html

[T22] Swift：字典
来源：http://hz.316326.xyz/gtpfoioxww.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gturkimtcj.html

[T23] Swift：函数
来源：http://hz.jinqigfzy.top/gtxapwkqfq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gtnjngpkpa.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtwbvftfzy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cdnleiting.top/gthhpmthwv.html

[T25] Swift：结构体
来源：http://hz.gotoacloud.top/gtawmppwah.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtvlksnxkx.html

[T26] Swift：类与重写
来源：http://hz.guannengcc.top/gtrbbsbfyy.html

class A: Base { override func f() {} }
来源：http://hz.sufxvd.cn/gthaekzlal.html

[T27] Swift：错误处理
来源：http://hz.chenjidiqi.icu/gternqrnjm.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gtxkxzwgms.html

[T28] Swift：枚举
来源：http://hz.jinghuilouyu.cn/gtfetgjwgu.html

enum Color { case red, green }
来源：http://hz.haohaochexian.top/gtbfjnpyvn.html

[T29] Swift：guard 提前返回
来源：http://hz.chenzaomai.com/gttqfujuos.html

guard let x = opt else { return }
来源：http://hz.c1oappe.top/gtdqfctiiw.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gtedppuhzr.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtqmbdbzov.html

[T31] Lua：Hello World
来源：http://hz.hnxiangtu.top/gtsyaqukkg.html

print("Hello")
来源：http://hz.shzxlz.cn/gtqoykhwdq.html

[T32] Lua：局部变量
来源：http://hz.ybcxt.top/gtssdcmdto.html

local a = 1
来源：http://hz.chenzaomai.com/gtzdbbedpk.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtasovamzp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jiagoushi.top/gtzenwgldt.html

[T34] Lua：遍历表
来源：http://hz.jqgufenzy.top/gtwlgqzxvr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhoulong.xyz/gtioljogfq.html

[T35] Lua：字典表
来源：http://hz.hnxiangtu.top/gtqehbyuli.html

local d = { a = 1 };  d.b = 2
来源：http://hz.dashuyun.cn/gtzjcqbkqf.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtriuuzlyb.html

function add(a, b) return a + b end
来源：http://hz.guowangkeji.top/gtinnjyirn.html

[T37] Lua：字符串拼接
来源：http://hz.ybcxt.top/gtgxfieoda.html

"a" .. "b"
来源：http://hz.daxiang520.top/gtkjdduavj.html

[T38] Lua：条件
来源：http://hz.fzhhl.top/gtzhhtjtbp.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gtbxqclkqj.html

[T39] Lua：模式匹配
来源：http://hz.zdqjudy.top/gtrcbfhges.html

string.find(s, "%d+")
来源：http://hz.jinqigfzy.top/gtmowlxmfj.html

[T40] Lua：元表
来源：http://hz.chenlongwang.top/gtsjkkmipl.html

setmetatable({}, { __index = base })
来源：http://hz.birdmap.top/gtiaqzlbqz.html

[T41] Perl：Hello World
来源：http://hz.yangfankeji.com/gtgtjulnkp.html

print "Hello\n";
来源：http://hz.dianchejie.cn/gtrdxegciq.html

[T42] Perl：变量类型
来源：http://hz.dashuyun.cn/gtjiozbsln.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxinkj.top/gtnsxbwevp.html

[T43] Perl：字符串插值
来源：http://hz.cucudq.cn/gtbthoddhs.html

"值: $a"
来源：http://hz.xinyue.icu/gtyevmgcqv.html

[T44] Perl：条件
来源：http://hz.jlsjyb.cn/gtkzsbedox.html

if ($a > 0) { print "正"; }
来源：http://hz.cdnleiting.top/gtcpumwzzy.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtzinvreet.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtobwypywl.html

[T46] Perl：哈希操作
来源：http://hz.kuanghao11.cn/gtqbrmvhbh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangshuangyany.cn/gtndcfrzpx.html

[T47] Perl：正则捕获
来源：http://hz.jinghuilouyu.cn/gtakgykvaf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenlongwang.top/gtqqegwitf.html

[T48] Perl：正则替换
来源：http://hz.gzhubu.top/gtsfvdgwtf.html

$s =~ s/old/new/g;
来源：http://hz.daxiang520.top/gtnjjjqapl.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtlowwwozg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xinyue.icu/gtwjewoyrx.html

[T50] Perl：逐行读文件
来源：http://hz.redwolf501.top/gtvzbpqeyc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yanxiufei.cn/gtjbdypndx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.redwolf501.top/gtqyqfobas.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gtnprzskcs.html

println("Hello")
来源：http://hz.ppjwa.cn/gtcuuszyro.html

[T52] Scala：变量
来源：http://hz.ywan-chungtsiang.top/gtzetwbnmw.html

val a = 1;  var b = 2
来源：http://hz.hnxiangtu.top/gtjasvtdqt.html

[T53] Scala：字符串插值
来源：http://hz.ydjk.org.cn/gtymobhmly.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtyklpxgqe.html

[T54] Scala：集合映射
来源：http://hz.sweek.top/gtynvshzsr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhoulong.xyz/gtlsitqubd.html

[T55] Scala：集合过滤
来源：http://hz.xziqi.cn/gtwnkxqpvx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.bjfxy.top/gtpoueugsn.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gtmpmadfqp.html

case class User(name: String, age: Int)
来源：http://hz.sysykeji.top/gtlmccdqal.html

[T57] Scala：模式匹配
来源：http://hz.quarkkingdee.top/gtpisvjxvi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtubozggwn.html

[T58] Scala：函数定义
来源：http://hz.jqgfzy.top/gtpahzoihr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aizwys.cn/gtxnzlujqx.html

[T59] Scala：循环
来源：http://hz.jyoumei.cn/gtfactzqmt.html

for (i <- 1 to 10) println(i)
来源：http://hz.c1oappe.top/gtmgtjtwad.html

[T60] Scala：折叠
来源：http://hz.gzhubu.top/gtjollpfri.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jyoumei.cn/gtwfrhrafs.html

================================================================================
来源：http://hz.xuanzx.com/gtqonzvnsw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gotoacloud.top/gtuauaacqv.html

================================================================================
来源：http://hz.pycfn.com/gtinlziyxj.html

[U01] Py：创建虚拟环境
来源：http://hz.fzhhl.top/gtqtddkzjj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.bjfxy.top/gtwdvijjre.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jiagoushi.top/gtgfxnyqha.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.haohaochexian.top/gtbxqeqpsg.html

[U03] Py：加载 .env 配置
来源：http://hz.meibo888.top/gttthzglbp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sysykeji.top/gtxvuvajoi.html

[U04] Py：变量调试打印
来源：http://hz.bjfxy.top/gtcyokgxes.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guowangkeji.top/gtxgkjtzys.html

[U05] Py：列表去重且保序
来源：http://hz.smart0.xyz/gtrtirkppz.html

list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gtxbaqqbxr.html

[U06] Py：合并两个字典
来源：http://hz.chenzaomai.com/gtknoyhwaa.html

{**a, **b}
来源：http://hz.aizwys.cn/gtzqaurfeu.html

[U07] Py：反转字典键值
来源：http://hz.nanxinkj.top/gtzjtkdiwh.html

{v: k for k, v in d.items()}
来源：http://hz.zhiwuduotai.top/gtffmigout.html

[U08] Py：展平二维列表
来源：http://hz.cashguo.top/gttzajemso.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gttrkzucny.html

[U09] Py：字典取最大值的键
来源：http://hz.yongpay.top/gtlcmlawaw.html

max(d, key=d.get)
来源：http://hz.hnqzz.top/gtvqkjodne.html

[U10] Py：按值排序字典
来源：http://hz.52xcode.cn/gtkfzwwjmu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sxryk.cn/gtvxrhvjpp.html

[U11] Py：生成器表达式
来源：http://hz.jinqigufen.top/gtreakczir.html

(x * 2 for x in arr)
来源：http://hz.jqgufenzy.top/gtzgpjxpuy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.birdmap.top/gtenhwtddb.html

Counter(arr).most_common(3)
来源：http://hz.sweek.top/gteixhkhfm.html

[U13] Py：固定长度队列
来源：http://hz.zycfv.cn/gtsjclyxxn.html

deque(maxlen=10)
来源：http://hz.nwbrower.top/gtvscltzat.html

[U14] Py：分组收集到列表
来源：http://hz.jqgufenzy.top/gtcavfuswy.html

defaultdict(list)
来源：http://hz.vqdsnc.cn/gtbroueepe.html

[U15] Py：高精度计时
来源：http://hz.hongshengwenyu.top/gtoikfynsc.html

t = time.perf_counter()
来源：http://hz.cqqwz.cn/gtakokjybp.html

[U16] Py：命令行参数解析
来源：http://hz.kuanghao11.cn/gtiapxzazr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.pycfn.com/gtxhbfseag.html


<!-- 参考信息 -->