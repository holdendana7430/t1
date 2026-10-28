代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.guowangkeji.top/gtjnyqjsvx.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtyuhcrxrj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtxyqcqppb.html

[R77] 读取用户输入
来源：http://hz.snrcjt.cn/gtufyzusth.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gturayumap.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtjjfwhroz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pengpengdd.cyou/gtamhyfevu.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtlcalupzn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.smart0.xyz/gtjejibwrn.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtzxvnseph.html

time ./run.sh
来源：http://hz.birdmap.top/gtzwlxrwgu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtieuegkdl.html

S. C / C++ 专题
来源：http://hz.zhoulong.xyz/gtxgazlhka.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdwmhvnkq.html

[S01] C：Hello World
来源：http://hz.smart0.xyz/gtfvzbcgmy.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtyawgpjld.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtuladiafw.html

[S02] C：变量与格式化输出
来源：http://hz.hysaishi.cn/gtexkltoag.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnqzz.top/gtdgpermmm.html

[S03] C：读入整数
来源：http://hz.cucudq.cn/gtwjemdtit.html

int x; scanf("%d", &x);
来源：http://hz.yangfankeji.com/gtmxszussf.html

[S04] C：字符串复制
来源：http://hz.aizwys.cn/gtqxeymdkk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cqqwz.cn/gtjejzlxgc.html

[S05] C：字符串长度
来源：http://hz.jinyuanbaomall.cn/gtddtairgs.html

strlen(s)
来源：http://hz.xuetiantiany.cn/gtbmjrxncs.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtnhctwwsh.html

strcmp(a, b) == 0
来源：http://hz.nanxinkj.top/gtgantzgds.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtwadbupub.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtkkdxrtmx.html

[S08] C：动态内存分配与释放
来源：http://hz.shzxlz.cn/gtmrjtaqjf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jyoumei.cn/gtqgznaxoa.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtnddhrzox.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuxming.cn/gttgthlwtg.html

[S10] C：指针与解引用
来源：http://hz.zdqjudy.top/gtunbecgth.html

int *p = &a;  *p = 5;
来源：http://hz.xziqi.cn/gtafgpkggy.html

[S11] C：逐行读文件
来源：http://hz.zhiwuduotai.top/gthtzpkeos.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtzsyfksyb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangshuangyany.cn/gtdmtlhtwu.html

fclose(f);
来源：http://hz.wangshuangyany.cn/gtrgtwxrob.html

[S12] C：写文件
来源：http://hz.bjfxy.top/gtrnghdahb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gtddopiodo.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtucpqpmsz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gtnniskefl.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtbxxggttq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pengpengdd.cyou/gthcmnsvyj.html

[S15] C：类型转换
来源：http://hz.gaohongyu789.top/gtdruvgaap.html

(double) a / b
来源：http://hz.chenzaomai.com/gtdubtkwyu.html

[S16] C：位操作置位
来源：http://hz.ydzc1.top/gtswpnvljd.html

x |= (1 << 3);
来源：http://hz.zdqjudy.top/gtwucewjdu.html

[S17] C：安全拼接字符串
来源：http://hz.yueranfly.top/gtrwntvtjp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuanzx.com/gtjfgtejbt.html

[S18] C：命令行参数
来源：http://hz.yonumen.top/gtpljlaoni.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtydsniani.html

[S19] C：快速排序
来源：http://hz.hongshengwenyu.top/gtsgttrbuf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gthaljjyae.html

[S20] C：二分查找
来源：http://hz.dashuyun.cn/gtkvvcsomg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhixingplan.top/gtixvvvljf.html

[S21] C：字符类别判断
来源：http://hz.yongpay.top/gtblczxmyx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gttvnldsxt.html

[S22] C：字符串转数字
来源：http://hz.xziqi.cn/gtgoljilxj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.bjfxy.top/gtmhzqkgyb.html

[S23] C：随机数
来源：http://hz.ivvv.top/gtmrivuvxj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dashuyun.cn/gtvqocdowg.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtzvvzqfog.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.0kj1m.cn/gthxudrtuc.html

[S25] C：内存拷贝
来源：http://hz.jinqigufen.top/gtvxnlocxb.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtqqtjslzn.html

[S26] C：内存清零
来源：http://hz.jinghuilouyu.cn/gtxnrtajje.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtyxzbhqkj.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtbssmmnfc.html

const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gtboyylpvp.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtajbovfml.html

static int counter = 0;
来源：http://hz.jiagoushi.top/gtildxxdbe.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gtyucbbhgu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hammf.cn/gtforsaekv.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtdhjfwyxe.html

#ifndef X_H
来源：http://hz.bjfxy.top/gtvhibatce.html

#define X_H
来源：http://hz.9152youxi.cn/gtzwkaiegy.html

#endif
来源：http://hz.smart0.xyz/gttamfqzqq.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtfvyueguk.html

#include <iostream>
来源：http://hz.yonumen.top/gtjxegowdk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtbcwxbzyj.html

[S32] C++：字符串
来源：http://hz.dianchejie.cn/gtdxbhwwrz.html

std::string s = "hi";  s += "!";
来源：http://hz.yueranfly.top/gtgyzdndns.html

[S33] C++：vector 增删
来源：http://hz.jinqigfzy.top/gtlcglrhrd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtreqfdaeg.html

[S34] C++：遍历 vector
来源：http://hz.cashguo.top/gtheqkxrtw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sxryk.cn/gtslvjuczb.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtbwrvqnzt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtqkebbcbt.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtdeleiujr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtcoctaeym.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtphzyxkry.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gttcithjcq.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtpgjgdder.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtyfojdnxb.html

[S39] C++：自定义比较器排序
来源：http://hz.tian-w.cn/gttdfflrft.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.iojbl.cn/gtyjygczuh.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gtehjknryb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtjtzvpsam.html

[S41] C++：类与构造函数
来源：http://hz.jinqigfzy.top/gtveiolspd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daxiang520.top/gtjvdsddie.html

[S42] C++：继承与虚函数
来源：http://hz.shuidangran.top/gtkwduykih.html

class B : public Base { public: void f() override {} };
来源：http://hz.zdqjudy.top/gtyrkcopha.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtufqcwpjz.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gtdnihdjth.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtonpopjaj.html

void inc(int &x) { ++x; }
来源：http://hz.zhengqikj.top/gtivepqgpz.html

[S45] C++：lambda
来源：http://hz.ydzc1.top/gtydkukwal.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtfxoonepz.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtatemgufb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gaohongyu789.top/gtcztmqcdr.html

[S47] C++：结构化绑定遍历
来源：http://hz.ehwqpu.com/gtgfnvecto.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigfzy.top/gtdpbzxvix.html

[S48] C++：逐行读文件
来源：http://hz.zhoulong.xyz/gtgorbctzg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtyospgedx.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gthnfwjwmh.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtpftkynjk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.316326.xyz/gtxnvejrhd.html

[S50] C++：格式化数字
来源：http://hz.meibo888.top/gtxmogrnnl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yongpay.top/gtykxhiogo.html

[S51] C++：显式类型转换
来源：http://hz.xziqi.cn/gtiwbyypyd.html

static_cast<double>(a) / b
来源：http://hz.feifeiyinyue.top/gtprnyfkcc.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtejxdcnjq.html

int size() const noexcept { return n_; }
来源：http://hz.xinyue.icu/gtxuzyofzw.html

[S53] C++：移动语义
来源：http://hz.fzhhl.top/gtkhgdwwdv.html

std::vector<int> w = std::move(v);
来源：http://hz.vqdsnc.cn/gtkewzszal.html

[S54] C++：异常处理
来源：http://hz.quarkkingdee.top/gtkyitqqho.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guannengcc.top/gtqfnvtncp.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtpeuqrras.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.316326.xyz/gtunicxojw.html

[S56] C++：optional
来源：http://hz.yangfankeji.com/gtycptducv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.0kj1m.cn/gtstatjmzi.html

[S57] C++：编译期常量
来源：http://hz.hnxiangtu.top/gtfqvzrydt.html

constexpr int N = 10;
来源：http://hz.birdmap.top/gtyfgubndh.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtwhazjhvw.html

namespace ns { int f() { return 1; } }
来源：http://hz.pengpengdd.cyou/gtrzebftxn.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtryuvoyry.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gtckpjcfgq.html

[S60] C++：遍历并删除元素
来源：http://hz.xziqi.cn/gtmpksajot.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jiagoushi.top/gtdzhrqmrs.html

================================================================================
来源：http://hz.pycfn.com/gtgnywayex.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aizwys.cn/gtzkwurlce.html

================================================================================
来源：http://hz.chenzaomai.com/gtyqjesyzu.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gtdymjueqf.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gttxhnpdyk.html

[T02] Kotlin：变量
来源：http://hz.jlsjyb.cn/gtmcshjrav.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtihmufojm.html

[T03] Kotlin：字符串模板
来源：http://hz.birdmap.top/gtwemiuiph.html

"值: $b"
来源：http://hz.kuanghao11.cn/gtvcolrzox.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtcecagqem.html

val n: String? = null;  n?.length
来源：http://hz.316326.xyz/gtyhkhtbgh.html

[T05] Kotlin：when 表达式
来源：http://hz.daria6918.cn/gtzavztuil.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xingfuxueyuan.xyz/gtvrramckt.html

[T06] Kotlin：集合映射
来源：http://hz.pycfn.com/gtaeehxrdm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.bjfxy.top/gtnwhwhrpa.html

[T07] Kotlin：集合过滤
来源：http://hz.zhijiandao.cn/gtjukfpqkk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.snrcjt.cn/gtqifwejuk.html

[T08] Kotlin：数据类
来源：http://hz.yuanzhike.top/gtfvahvdvn.html

data class User(val name: String, val age: Int)
来源：http://hz.xinyue.icu/gtooeoflbj.html

[T09] Kotlin：扩展函数
来源：http://hz.zhongyouzk.top/gtelanlstq.html

fun String.exclaim() = this + "!"
来源：http://hz.xingfuxueyuan.xyz/gtqhtgcigx.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtgxzlnpjt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtgelabehq.html

[T11] Kotlin：协程
来源：http://hz.tian-w.cn/gtoartbrvf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gthzmrohqh.html

[T12] Kotlin：解构声明
来源：http://hz.cheryme.top/gtmzgvyrxf.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtdnzloflj.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtskxlsdnx.html

val m = mapOf("a" to 1)
来源：http://hz.cheryme.top/gtgiapqtoy.html

[T14] Kotlin：循环
来源：http://hz.birdmap.top/gtqcgxqrqf.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gtsbxhehgq.html

[T15] Kotlin：接口
来源：http://hz.pycfn.com/gtxxmmdhnh.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtveqaeeoh.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtjieuxphc.html

print("Hello")
来源：http://hz.chenzaomai.com/gtfhbczhgq.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gtixdnergd.html

var a = 1;  let b = 2
来源：http://hz.yanxiufei.cn/gtopdsmeqw.html

[T18] Swift：字符串插值
来源：http://hz.ybcxt.top/gtvlwuxaeo.html

"值: \(b)"
来源：http://hz.jqgfzy.top/gtsijlctsx.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtcuvcjjal.html

if let n = opt { print(n) }
来源：http://hz.guowangkeji.top/gtslrsmzqx.html

[T20] Swift：数组操作
来源：http://hz.smart0.xyz/gtzabjkbfi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.bjfxy.top/gtnysgivau.html

[T21] Swift：遍历
来源：http://hz.andypj.xyz/gtzqprmewv.html

for x in a { print(x) }
来源：http://hz.hywenlv.cn/gtwnzhajpg.html

[T22] Swift：字典
来源：http://hz.ydjk.org.cn/gtvgewwopy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.mhx1999.top/gthieczsal.html

[T23] Swift：函数
来源：http://hz.zhongyouzk.top/gtaxltskel.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuetiantiany.cn/gtqjmycqye.html

[T24] Swift：闭包
来源：http://hz.jinqigfzy.top/gtmzdzilds.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtmcjpotwm.html

[T25] Swift：结构体
来源：http://hz.nwbrower.top/gthxbopmwj.html

struct P { var x: Int }
来源：http://hz.guannengcc.top/gtxtqkjtpl.html

[T26] Swift：类与重写
来源：http://hz.pengpengdd.cyou/gtgwceokin.html

class A: Base { override func f() {} }
来源：http://hz.cqqwz.cn/gtviysoole.html

[T27] Swift：错误处理
来源：http://hz.yj202588.top/gtbekxfraa.html

do { try f() } catch { print(error) }
来源：http://hz.wangshuangyany.cn/gtzoadgoht.html

[T28] Swift：枚举
来源：http://hz.quarkkingdee.top/gtayiwupvb.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtlsqwxvbb.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gtaqexixzi.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtkbyrzvcd.html

[T30] Swift：协议
来源：http://hz.jqgfzy.top/gthdbotbje.html

protocol Shape { func area() -> Double }
来源：http://hz.hywenlv.cn/gtjliyamdk.html

[T31] Lua：Hello World
来源：http://hz.nanxuanxn.top/gthmhzgpyz.html

print("Hello")
来源：http://hz.nwbrower.top/gtndvlchco.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gttmwepuel.html

local a = 1
来源：http://hz.tianlin.xyz/gtjazcplbo.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangkeji.top/gtavmuckur.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhaomingkeji.xyz/gtarqwiblq.html

[T34] Lua：遍历表
来源：http://hz.guannengcc.top/gtfqaaiicg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ywan-chungtsiang.top/gtzvacpwrb.html

[T35] Lua：字典表
来源：http://hz.jinyuanbaomall.cn/gtwluhkkpk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtkmgkvqpg.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtyykbafkj.html

function add(a, b) return a + b end
来源：http://hz.cashguo.top/gtzeqyapfk.html

[T37] Lua：字符串拼接
来源：http://hz.aibaodan.cn/gtqklerito.html

"a" .. "b"
来源：http://hz.cucudq.cn/gthdeqduiq.html

[T38] Lua：条件
来源：http://hz.xinyue.icu/gtpcofhiou.html

if x > 0 then print("正") end
来源：http://hz.yanxiufei.cn/gtdumognek.html

[T39] Lua：模式匹配
来源：http://hz.jinghuilouyu.cn/gtyyjpzuqh.html

string.find(s, "%d+")
来源：http://hz.jinyuanbaomall.cn/gtgefuwzga.html

[T40] Lua：元表
来源：http://hz.pycfn.com/gtexgpkhdl.html

setmetatable({}, { __index = base })
来源：http://hz.hongshengwenyu.top/gtjwsukqna.html

[T41] Perl：Hello World
来源：http://hz.jqgfzy.top/gtbyhhzmxw.html

print "Hello\n";
来源：http://hz.sxryk.cn/gtgrbawgdd.html

[T42] Perl：变量类型
来源：http://hz.andypj.xyz/gttlssxqnf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgfzy.top/gtyafzhgcn.html

[T43] Perl：字符串插值
来源：http://hz.hywenlv.cn/gtyycqgskl.html

"值: $a"
来源：http://hz.yangfankeji.com/gtbjrqmvzr.html

[T44] Perl：条件
来源：http://hz.0kj1m.cn/gtfbjzedfn.html

if ($a > 0) { print "正"; }
来源：http://hz.c1oappe.top/gtrsbvvnmg.html

[T45] Perl：数组遍历
来源：http://hz.zhixingplan.top/gtiumockrx.html

for my $x (@arr) { print $x; }
来源：http://hz.daria6918.cn/gtaiyasgnl.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gthizsrhyv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jiagoushi.top/gtuygdvbhu.html

[T47] Perl：正则捕获
来源：http://hz.sxryk.cn/gtbewbtdml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgfzy.top/gtoknbajez.html

[T48] Perl：正则替换
来源：http://hz.ehwqpu.com/gtwoktjqyg.html

$s =~ s/old/new/g;
来源：http://hz.gogol.net.cn/gtkdsrshve.html

[T49] Perl：函数
来源：http://hz.xingfuxueyuan.xyz/gtjuxyvmyw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ehwqpu.com/gtvwxgaehy.html

[T50] Perl：逐行读文件
来源：http://hz.yueranfly.top/gttnmxxymu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.kuanghao11.cn/gtievavdlm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenjidiqi.icu/gtwbfzvqjs.html

[T51] Scala：Hello World
来源：http://hz.jyoumei.cn/gtivxwohuo.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gtjqsxviqr.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtdosbqzmx.html

val a = 1;  var b = 2
来源：http://hz.jiagoushi.top/gtzsfkgsiz.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtyjmcabzr.html

s"值: $b"
来源：http://hz.gotoacloud.top/gtkdqpabgr.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtnhlkghii.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guowangkeji.top/gtqhevhehp.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gtaqudvdxs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sufxvd.cn/gtubvabaxu.html

[T56] Scala：样例类
来源：http://hz.bjfxy.top/gtucggsfaa.html

case class User(name: String, age: Int)
来源：http://hz.nanxinkj.top/gtzvxhmsrp.html

[T57] Scala：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gteelfvabj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gotoacloud.top/gthpvonfjo.html

[T58] Scala：函数定义
来源：http://hz.andypj.xyz/gtzbgpuciq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtsfeiamze.html

[T59] Scala：循环
来源：http://hz.chenjidiqi.icu/gtiljsxbjs.html

for (i <- 1 to 10) println(i)
来源：http://hz.svipenyu.cn/gtdoduhfmn.html

[T60] Scala：折叠
来源：http://hz.xinyue.icu/gtetjrcjib.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sweek.top/gtfgtlxrtv.html

================================================================================
来源：http://hz.dianchejie.cn/gtmgdphngl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.smart0.xyz/gtuciltlip.html

================================================================================
来源：http://hz.fzhhl.top/gtwmmbyzgj.html

[U01] Py：创建虚拟环境
来源：http://hz.52xcode.cn/gthbjyedmb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zycfv.cn/gtjbhdqvav.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gogol.net.cn/gtqgadpbne.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yangfankeji.com/gtjdwbimxz.html

[U03] Py：加载 .env 配置
来源：http://hz.nanxuanxn.top/gtmpkqyecn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.aibaodan.cn/gttxhczdkc.html

[U04] Py：变量调试打印
来源：http://hz.gotoacloud.top/gtlqnmwjwa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yuxming.cn/gtvghlvhrh.html

[U05] Py：列表去重且保序
来源：http://hz.iojbl.cn/gtdoeuflpk.html

list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtlcaxjdru.html

[U06] Py：合并两个字典
来源：http://hz.kuanghao11.cn/gtecbwpddh.html

{**a, **b}
来源：http://hz.cqqwz.cn/gtmeedvuej.html

[U07] Py：反转字典键值
来源：http://hz.xziqi.cn/gtbtdvvlzd.html

{v: k for k, v in d.items()}
来源：http://hz.yvedp.cn/gtlzyuhmqf.html

[U08] Py：展平二维列表
来源：http://hz.tanke756.top/gtjqxiunaf.html

[y for x in nested for y in x]
来源：http://hz.tanke756.top/gtmtmcitkm.html

[U09] Py：字典取最大值的键
来源：http://hz.pengpengdd.cyou/gtiosxscxh.html

max(d, key=d.get)
来源：http://hz.daxiang520.top/gtvxafboqz.html

[U10] Py：按值排序字典
来源：http://hz.yangfankeji.com/gtjrtwffes.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtljqgkfdb.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtzgidodqf.html

(x * 2 for x in arr)
来源：http://hz.nwbrower.top/gtfbartjlz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xuanzx.com/gtmmrcpmrn.html

Counter(arr).most_common(3)
来源：http://hz.fengsongda.top/gtasdexhrk.html

[U13] Py：固定长度队列
来源：http://hz.pengpengdd.cyou/gtnyfinqly.html

deque(maxlen=10)
来源：http://hz.ydzc1.top/gthcnunqlf.html

[U14] Py：分组收集到列表
来源：http://hz.gzhubu.top/gtxvssnfxj.html

defaultdict(list)
来源：http://hz.hammf.cn/gtrqddlzlq.html

[U15] Py：高精度计时
来源：http://hz.guowangkeji.top/gtvisrxirv.html

t = time.perf_counter()
来源：http://hz.cdnleiting.top/gtmpwyhoci.html

[U16] Py：命令行参数解析
来源：http://hz.chenjidiqi.icu/gtxofxthcb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yonumen.top/gtguvswblz.html


<!-- 参考信息 -->