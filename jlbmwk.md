代发 wailian999

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtqfwrdxwp.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gtjdcuwmuq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gtjyzzkiaz.html

[R75] 导出环境变量
来源：http://hz.cashguo.top/gtqqpbxbje.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtqsbkrrnx.html

[R76] 使用临时文件
来源：http://hz.jlsjyb.cn/gtyenxywyf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtpkqoqrfm.html

[R77] 读取用户输入
来源：http://hz.snrcjt.cn/gttlacjali.html

read -rp "请输入: " ans
来源：http://hz.yueranfly.top/gtpurabmhv.html

[R78] 交互式菜单
来源：http://hz.hammf.cn/gtdnynvbmm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jyoumei.cn/gtendvhfdf.html

[R79] 解析命令行选项
来源：http://hz.xinyue.icu/gtatrnghqd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtkhrphias.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gthbwpasqk.html

time ./run.sh
来源：http://hz.sweek.top/gtghnkpypy.html

================================================================================
来源：http://hz.redwolf501.top/gtawbeybdv.html

S. C / C++ 专题
来源：http://hz.yvedp.cn/gtjfirbika.html

================================================================================
来源：http://hz.aibaodan.cn/gtexgnjuwp.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtosbotdbk.html

#include <stdio.h>
来源：http://hz.gogol.net.cn/gtqpmeijxw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgufenzy.top/gtbqddmzyg.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gtegqxpije.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gtbesedslg.html

[S03] C：读入整数
来源：http://hz.cashguo.top/gtxqglxsds.html

int x; scanf("%d", &x);
来源：http://hz.zhixingplan.top/gtcrsmkpmv.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtluwlayaw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtdvhorxpf.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtbhuzkwjw.html

strlen(s)
来源：http://hz.dianchejie.cn/gtpsjqdxgn.html

[S06] C：字符串比较
来源：http://hz.dianchejie.cn/gtazfgcksr.html

strcmp(a, b) == 0
来源：http://hz.guowangkeji.top/gtjjkijpom.html

[S07] C：数组遍历求和
来源：http://hz.316326.xyz/gtzwktpveb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtzrgjihao.html

[S08] C：动态内存分配与释放
来源：http://hz.hongshengwenyu.top/gtcpvfslfu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangtech.top/gtydfjlrtw.html

[S09] C：结构体定义与初始化
来源：http://hz.zhoulong.xyz/gtqshfhbjy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gtfznaqoyt.html

[S10] C：指针与解引用
来源：http://hz.jinqigufen.top/gtmeldzxgy.html

int *p = &a;  *p = 5;
来源：http://hz.feifeiyinyue.top/gtafwcmnqo.html

[S11] C：逐行读文件
来源：http://hz.52xcode.cn/gtfynvrjzm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gtrmkafzju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tianlin.xyz/gtfiayjkzb.html

fclose(f);
来源：http://hz.zhoulong.xyz/gtghxrzdki.html

[S12] C：写文件
来源：http://hz.yanxiufei.cn/gtvdtkzvjt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gtedzaxnqd.html

[S13] C：宏定义
来源：http://hz.9152youxi.cn/gtwvgjegyg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtzsyrbsgt.html

[S14] C：枚举
来源：http://hz.xuanzx.com/gtkdmrzkpk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ybcxt.top/gtmakafbuc.html

[S15] C：类型转换
来源：http://hz.chenzaomai.com/gtclejgdac.html

(double) a / b
来源：http://hz.nwbrower.top/gtuuxbrphc.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtipqccvzy.html

x |= (1 << 3);
来源：http://hz.0kj1m.cn/gtuezbfkpi.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtrocwyjur.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.quarkkingdee.top/gtzoaqybim.html

[S18] C：命令行参数
来源：http://hz.hywenlv.cn/gthkcghqeu.html

int main(int argc, char **argv)
来源：http://hz.xuanzx.com/gtrdhqwqzr.html

[S19] C：快速排序
来源：http://hz.zhijiandao.cn/gtdmxhohsc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtyjkztmee.html

[S20] C：二分查找
来源：http://hz.316326.xyz/gtslhraxrx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gthssuxxzm.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtbdbdodey.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtbcgrrirj.html

[S22] C：字符串转数字
来源：http://hz.iojbl.cn/gtodyqforg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuanzhike.top/gtkbeikfwx.html

[S23] C：随机数
来源：http://hz.ydzc1.top/gtnfhzmdxc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gtcsoihgza.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtiwccjlmx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtokyvqiht.html

[S25] C：内存拷贝
来源：http://hz.jlsjyb.cn/gtxtddyrpn.html

memcpy(dst, src, n);
来源：http://hz.pengpengdd.cyou/gtqvjztopr.html

[S26] C：内存清零
来源：http://hz.cucudq.cn/gttmafszfs.html

memset(a, 0, sizeof a);
来源：http://hz.feifeiyinyue.top/gtanbomyjo.html

[S27] C：定义常量
来源：http://hz.ywan-chungtsiang.top/gtbgbsqaxh.html

const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtjbjgjbtw.html

[S28] C：静态变量
来源：http://hz.sweek.top/gtkzclkdkk.html

static int counter = 0;
来源：http://hz.xuanzx.com/gtvgdsepvx.html

[S29] C：变参函数
来源：http://hz.xingfuxueyuan.xyz/gtawzmsfvn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gtrjoquwgq.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtlytotjwr.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gtrlhhqmdm.html

#define X_H
来源：http://hz.chenzaomai.com/gtzbwhwwvt.html

#endif
来源：http://hz.feifeiyinyue.top/gtggrjvaqi.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtymkbnfra.html

#include <iostream>
来源：http://hz.jinqigufen.top/gtwovjqbqf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhiwuduotai.top/gtwckmnshu.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtsrlfdkud.html

std::string s = "hi";  s += "!";
来源：http://hz.aizwys.cn/gtanwrgmdw.html

[S33] C++：vector 增删
来源：http://hz.jinqigfzy.top/gtquivexzk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gtozjtiwbc.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtdyfxrkga.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gtkjkphyuj.html

[S35] C++：map
来源：http://hz.yuxming.cn/gthmvfxhih.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtkzngtgnx.html

[S36] C++：unordered_map
来源：http://hz.chenlongwang.top/gttmrmoewe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtnfepjnek.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtjkhufofz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtafnvyukw.html

[S38] C++：排序
来源：http://hz.zhongyouzk.top/gtefgxptqe.html

std::sort(v.begin(), v.end());
来源：http://hz.cqqwz.cn/gtzzmfinya.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtneprbyme.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtwobhyrbn.html

[S40] C++：查找元素
来源：http://hz.zhixingplan.top/gtsphdirdk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtfewhsupl.html

[S41] C++：类与构造函数
来源：http://hz.c1oappe.top/gtqgjgbrub.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jlsjyb.cn/gtjoazjlep.html

[S42] C++：继承与虚函数
来源：http://hz.smart0.xyz/gtpfxuftmu.html

class B : public Base { public: void f() override {} };
来源：http://hz.ppjwa.cn/gtkwvnyukx.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtxlzqstws.html

auto p = std::make_unique<int>(5);
来源：http://hz.birdmap.top/gtjpxanoxw.html

[S44] C++：引用传参
来源：http://hz.hysaishi.cn/gtclzazkhz.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangtech.top/gtykebuizr.html

[S45] C++：lambda
来源：http://hz.zycfv.cn/gtpdayumjr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.9152youxi.cn/gthhdlwkku.html

[S46] C++：函数模板
来源：http://hz.jiagoushi.top/gtzytnhjsa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.0kj1m.cn/gtlyddxplo.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangshuangyany.cn/gtsgkmvjwc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtmshvlnls.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtmfojxukt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtnzlewvlm.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtiytkpdvs.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtfafkzxar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guowangkeji.top/gtnxdqyepd.html

[S50] C++：格式化数字
来源：http://hz.ybcxt.top/gtnnypjvzd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gtacphqtkc.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtmooqkrlt.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gtqthqdbtp.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxinkj.top/gtjfqurmou.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gtyeqcogwy.html

[S53] C++：移动语义
来源：http://hz.cucudq.cn/gteeeutcaw.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtmhxktwhi.html

[S54] C++：异常处理
来源：http://hz.sufxvd.cn/gtffdfnbli.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhongyouzk.top/gthctlzqgp.html

[S55] C++：结构化绑定
来源：http://hz.gaohongyu789.top/gtwpzrnqbf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ehwqpu.com/gtuyeypjtt.html

[S56] C++：optional
来源：http://hz.tanke756.top/gtuunfxzus.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtbxtkqwdx.html

[S57] C++：编译期常量
来源：http://hz.jinghuilouyu.cn/gtbcggfvcb.html

constexpr int N = 10;
来源：http://hz.zhixingplan.top/gtijahpizw.html

[S58] C++：命名空间
来源：http://hz.xingfuxueyuan.xyz/gtbdgomboy.html

namespace ns { int f() { return 1; } }
来源：http://hz.gzhubu.top/gtrajmqwwm.html

[S59] C++：静态断言
来源：http://hz.daria6918.cn/gtuzjnkhzm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pycfn.com/gtktriyhkp.html

[S60] C++：遍历并删除元素
来源：http://hz.zhaomingkeji.xyz/gtaodvqymq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gtiqorlmcc.html

================================================================================
来源：http://hz.sufxvd.cn/gttqnzykuc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gthrsazlxs.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqbxenzqn.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gtabgkszui.html

println("Hello")
来源：http://hz.cheryme.top/gtbrijmntk.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gtufwuxtkv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gthvhvtywe.html

[T03] Kotlin：字符串模板
来源：http://hz.zhijiandao.cn/gtczxcgmvj.html

"值: $b"
来源：http://hz.jlsjyb.cn/gthtmacxba.html

[T04] Kotlin：空安全
来源：http://hz.jqgufenzy.top/gtbfbojpms.html

val n: String? = null;  n?.length
来源：http://hz.gogol.net.cn/gtatpohrsj.html

[T05] Kotlin：when 表达式
来源：http://hz.hnqzz.top/gtwsuoyyyd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtemnuvpun.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtdqdmbzym.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gtueqwosgv.html

[T07] Kotlin：集合过滤
来源：http://hz.kuanghao11.cn/gtsvqnyfxb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jianghu66.top/gtzlvwgiie.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gttvakprwm.html

data class User(val name: String, val age: Int)
来源：http://hz.chenlongwang.top/gtlhlamcfl.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gtryrxpoba.html

fun String.exclaim() = this + "!"
来源：http://hz.vqdsnc.cn/gtfkjkfmut.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtkzxmrhej.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dianchejie.cn/gtxanmulna.html

[T11] Kotlin：协程
来源：http://hz.cdnleiting.top/gtazpdzmfl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gtsbicwcbi.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gtlcrfvhio.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gthjnuytuc.html

[T13] Kotlin：只读 Map
来源：http://hz.xingfuxueyuan.xyz/gtdlzroeui.html

val m = mapOf("a" to 1)
来源：http://hz.chenlongwang.top/gthkbfnffx.html

[T14] Kotlin：循环
来源：http://hz.tianlin.xyz/gtmdhsmnrb.html

for (i in 1..10) println(i)
来源：http://hz.zycfv.cn/gtapllzdpi.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gttkoaytjo.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtogzcoqbl.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtyviaigub.html

print("Hello")
来源：http://hz.havefunace.top/gtrlxhckoo.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtezfbuccr.html

var a = 1;  let b = 2
来源：http://hz.kuanghao11.cn/gtopzqkset.html

[T18] Swift：字符串插值
来源：http://hz.yuxming.cn/gtxaqqtklh.html

"值: \(b)"
来源：http://hz.52xcode.cn/gtsfuttuxp.html

[T19] Swift：可选绑定
来源：http://hz.guannengcc.top/gtodwzdvws.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtfcjozvpe.html

[T20] Swift：数组操作
来源：http://hz.zhijiandao.cn/gtbnopbabn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daria6918.cn/gthznbltmy.html

[T21] Swift：遍历
来源：http://hz.nanxuanxn.top/gtzwldqsdr.html

for x in a { print(x) }
来源：http://hz.wangdashe.top/gtqvooznye.html

[T22] Swift：字典
来源：http://hz.cashguo.top/gtjsjycvyb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtfengcolu.html

[T23] Swift：函数
来源：http://hz.shangyingyoupin.top/gtmdyvqruh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jianghu66.top/gtvfjevvlq.html

[T24] Swift：闭包
来源：http://hz.mhx1999.top/gtcrxoaipt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxuanxn.top/gtqjfzdrjr.html

[T25] Swift：结构体
来源：http://hz.cdnleiting.top/gtdhpbsfrt.html

struct P { var x: Int }
来源：http://hz.shanyushiyangtech.top/gtodlhwlqg.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtsziqdoke.html

class A: Base { override func f() {} }
来源：http://hz.zhijiandao.cn/gtafkelvdt.html

[T27] Swift：错误处理
来源：http://hz.bjfxy.top/gteqhxondz.html

do { try f() } catch { print(error) }
来源：http://hz.zhongyouzk.top/gtnsvxarch.html

[T28] Swift：枚举
来源：http://hz.yonumen.top/gtairmvjpv.html

enum Color { case red, green }
来源：http://hz.shzxlz.cn/gtywukwzgk.html

[T29] Swift：guard 提前返回
来源：http://hz.xingfuxueyuan.xyz/gtmxcjhdzn.html

guard let x = opt else { return }
来源：http://hz.andypj.xyz/gtaavdmthb.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gttsrortqu.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtddjnhwiu.html

[T31] Lua：Hello World
来源：http://hz.xinyue.icu/gtwmjjoezm.html

print("Hello")
来源：http://hz.jianghu66.top/gtkpyfgiyu.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtnougptxm.html

local a = 1
来源：http://hz.feifeiyinyue.top/gtqwctryvz.html

[T33] Lua：表（数组）
来源：http://hz.cashguo.top/gtbgyksqoc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtzikoflfg.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtzzmlgeqk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gotoacloud.top/gtsnfermef.html

[T35] Lua：字典表
来源：http://hz.mhx1999.top/gtwgzqihib.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jqgfzy.top/gtybsrfdma.html

[T36] Lua：函数
来源：http://hz.chenzaomai.com/gtxaqbjhtz.html

function add(a, b) return a + b end
来源：http://hz.xuetiantiany.cn/gteaymkply.html

[T37] Lua：字符串拼接
来源：http://hz.nanxinkj.top/gtxllayygx.html

"a" .. "b"
来源：http://hz.jqgfzy.top/gtczfuixkm.html

[T38] Lua：条件
来源：http://hz.hnqzz.top/gtjupabsip.html

if x > 0 then print("正") end
来源：http://hz.yvedp.cn/gtgccxxzcy.html

[T39] Lua：模式匹配
来源：http://hz.sufxvd.cn/gtkuusvaqp.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gtnkybigex.html

[T40] Lua：元表
来源：http://hz.hongshengwenyu.top/gtspsuiitb.html

setmetatable({}, { __index = base })
来源：http://hz.yongpay.top/gtkkuubpzq.html

[T41] Perl：Hello World
来源：http://hz.nanxuanxn.top/gtowqcbkau.html

print "Hello\n";
来源：http://hz.cdnleiting.top/gtmetfpces.html

[T42] Perl：变量类型
来源：http://hz.nanxinkj.top/gtoytqzjmt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgufenzy.top/gtegxlwpwq.html

[T43] Perl：字符串插值
来源：http://hz.yj20258888.top/gtuajzabgc.html

"值: $a"
来源：http://hz.yj202588.top/gtjjhxoqpg.html

[T44] Perl：条件
来源：http://hz.gaohongyu789.top/gthilhgfmx.html

if ($a > 0) { print "正"; }
来源：http://hz.yongpay.top/gtjjlrelaq.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gtlqqkyneo.html

for my $x (@arr) { print $x; }
来源：http://hz.quarkkingdee.top/gtocqeaanl.html

[T46] Perl：哈希操作
来源：http://hz.quarkkingdee.top/gtgoxafyvk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aibaodan.cn/gtjervpfjc.html

[T47] Perl：正则捕获
来源：http://hz.xinyue.icu/gtrxcgdpcu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxuanxn.top/gtgyxrynhb.html

[T48] Perl：正则替换
来源：http://hz.gaohongyu789.top/gtbzgzlcfj.html

$s =~ s/old/new/g;
来源：http://hz.316326.xyz/gthpbtpdhm.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gttsownvjt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tanke756.top/gtjsrmnqfr.html

[T50] Perl：逐行读文件
来源：http://hz.svipenyu.cn/gtqhqijtbx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtxslwldqc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gttrhkinjv.html

[T51] Scala：Hello World
来源：http://hz.daria6918.cn/gtonjgalbw.html

println("Hello")
来源：http://hz.gotoacloud.top/gtmzrvxuyt.html

[T52] Scala：变量
来源：http://hz.aibaodan.cn/gtzemkwdgc.html

val a = 1;  var b = 2
来源：http://hz.sufxvd.cn/gtsqskijjn.html

[T53] Scala：字符串插值
来源：http://hz.dashuyun.cn/gtqhnmijje.html

s"值: $b"
来源：http://hz.sufxvd.cn/gtfjfpqbkw.html

[T54] Scala：集合映射
来源：http://hz.zdqjudy.top/gtjyfujxbo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fzhhl.top/gtfsohpaqi.html

[T55] Scala：集合过滤
来源：http://hz.jinqigfzy.top/gtvbggselp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hfpthk.cn/gtzokxkmqk.html

[T56] Scala：样例类
来源：http://hz.daxiang520.top/gtancoxhsw.html

case class User(name: String, age: Int)
来源：http://hz.52xcode.cn/gtyfxgtdpg.html

[T57] Scala：模式匹配
来源：http://hz.iojbl.cn/gtwyowdyss.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hysaishi.cn/gtlaujmwwc.html

[T58] Scala：函数定义
来源：http://hz.daria6918.cn/gtzpwhnsed.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.daxiang520.top/gtblnqoaru.html

[T59] Scala：循环
来源：http://hz.chenjidiqi.icu/gtvrmijsoz.html

for (i <- 1 to 10) println(i)
来源：http://hz.hongshengwenyu.top/gtaxpoogkd.html

[T60] Scala：折叠
来源：http://hz.zycfv.cn/gtutcvneld.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.birdmap.top/gtwevllhqn.html

================================================================================
来源：http://hz.yongpay.top/gtltenpyre.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cucudq.cn/gtmdhpxfvt.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtenamqkxm.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258888.top/gtswxnubsl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.vqdsnc.cn/gtptwtohaa.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigfzy.top/gtruhwbclp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenlongwang.top/gtyoulilht.html

[U03] Py：加载 .env 配置
来源：http://hz.sufxvd.cn/gttlryecae.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yongpay.top/gthikagwwg.html

[U04] Py：变量调试打印
来源：http://hz.hywenlv.cn/gttlrfichw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yonumen.top/gturmokkhi.html

[U05] Py：列表去重且保序
来源：http://hz.hnxiangtu.top/gtndiytsku.html

list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtuhuqjuez.html

[U06] Py：合并两个字典
来源：http://hz.chenjidiqi.icu/gtpddacwoa.html

{**a, **b}
来源：http://hz.smart0.xyz/gtfrvyolho.html

[U07] Py：反转字典键值
来源：http://hz.cdnleiting.top/gttgxdthgq.html

{v: k for k, v in d.items()}
来源：http://hz.c1oappe.top/gtmpsrpnlx.html

[U08] Py：展平二维列表
来源：http://hz.yvedp.cn/gtydseneur.html

[y for x in nested for y in x]
来源：http://hz.gogol.net.cn/gttztlwaqa.html

[U09] Py：字典取最大值的键
来源：http://hz.nwbrower.top/gtfbttzsxt.html

max(d, key=d.get)
来源：http://hz.ivvv.top/gtefnuicja.html

[U10] Py：按值排序字典
来源：http://hz.zhiwuduotai.top/gtxloemfrb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gtmpmdngtw.html

[U11] Py：生成器表达式
来源：http://hz.hywenlv.cn/gtrcjuonxq.html

(x * 2 for x in arr)
来源：http://hz.xziqi.cn/gtgjqhxbwr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jyoumei.cn/gtqqtmgphu.html

Counter(arr).most_common(3)
来源：http://hz.yj20258888.top/gtcetyrfci.html

[U13] Py：固定长度队列
来源：http://hz.hongshengwenyu.top/gtrskaswbi.html

deque(maxlen=10)
来源：http://hz.9152youxi.cn/gtkeulqnlv.html

[U14] Py：分组收集到列表
来源：http://hz.ydjk.org.cn/gtwrhrvmie.html

defaultdict(list)
来源：http://hz.cucudq.cn/gtplsgmrcb.html


<!-- 参考信息 -->