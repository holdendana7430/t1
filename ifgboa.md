代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.vqdsnc.cn/gtwhvzalac.html

[R72] 等待端口就绪
来源：http://hz.xuanzx.com/gtexqpkudk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ivvv.top/gtmzpwjnrd.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtfiufhtxb.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtuipxpqec.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtmcmvsbpz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenzaomai.com/gtvizlzwrh.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtuctiwkev.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigfzy.top/gtcnoepkqy.html

[R76] 使用临时文件
来源：http://hz.zdqjudy.top/gtgpqeurtl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtlaoympdt.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtsgfikicl.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtiodkloys.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gtscrfaeju.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenjidiqi.icu/gtylgrignw.html

[R79] 解析命令行选项
来源：http://hz.jinyuanbaomall.cn/gtsevdlbbw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangtech.top/gtomdxiumb.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gtwdzigrjp.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtfrcpxdgu.html

================================================================================
来源：http://hz.yj202588.top/gteqmayymo.html

S. C / C++ 专题
来源：http://hz.ydzc1.top/gtzdioblqv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtateetirj.html

[S01] C：Hello World
来源：http://hz.jinqigufen.top/gthvxhkssq.html

#include <stdio.h>
来源：http://hz.wangshuangyany.cn/gtghvbpxnk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pycfn.com/gtkhwavucm.html

[S02] C：变量与格式化输出
来源：http://hz.yuanzhike.top/gtthnhhyvu.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gtievqhdfz.html

[S03] C：读入整数
来源：http://hz.yonumen.top/gtmzbpgyih.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtndfuvzxx.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtscslhhgb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtsrphehgg.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtatzwlbfb.html

strlen(s)
来源：http://hz.jyoumei.cn/gtsjdfxsik.html

[S06] C：字符串比较
来源：http://hz.fengsongda.top/gtnydnhevc.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtgsdzfful.html

[S07] C：数组遍历求和
来源：http://hz.aibaodan.cn/gtofevdhog.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gtktweheyk.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtssuvaymo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtsewbcryy.html

[S09] C：结构体定义与初始化
来源：http://hz.sweek.top/gtbouconav.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xziqi.cn/gtuucsixut.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtiixqufzq.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtoiuusibv.html

[S11] C：逐行读文件
来源：http://hz.aibaodan.cn/gtdpdzenlb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shzxlz.cn/gtllitiose.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sweek.top/gtyjytulql.html

fclose(f);
来源：http://hz.0kj1m.cn/gtzhwfyvpo.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gtazpiprgi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtuftnrsnz.html

[S13] C：宏定义
来源：http://hz.xuanzx.com/gtkhitmbyr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jianghu66.top/gtxootslya.html

[S14] C：枚举
来源：http://hz.fzhhl.top/gtfqiqyrdl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhijiandao.cn/gtkxxuvcyl.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtoipiuqft.html

(double) a / b
来源：http://hz.fzhhl.top/gtgjcagfjc.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtciqlscrq.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtugyoopdd.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtsyffemam.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.mhx1999.top/gtglepvkny.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gtrjrjhbme.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtrvhxeqbl.html

[S19] C：快速排序
来源：http://hz.hfpthk.cn/gtcoxnisft.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhiwuduotai.top/gtperkkhoh.html

[S20] C：二分查找
来源：http://hz.yangfankeji.com/gtcvwukkwy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtdfbimxzc.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gtxnpltakp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zycfv.cn/gtwnxrepxk.html

[S22] C：字符串转数字
来源：http://hz.xingfuxueyuan.xyz/gtvgsdqcyu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangshuangyany.cn/gtiiakvnxr.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtzbfnbrmw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dashuyun.cn/gtcejlyden.html

[S24] C：获取本地时间
来源：http://hz.smart0.xyz/gtkgxgptiy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cdnleiting.top/gtobogwtve.html

[S25] C：内存拷贝
来源：http://hz.redwolf501.top/gtilzufdhe.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtfwpfurjh.html

[S26] C：内存清零
来源：http://hz.gogol.net.cn/gtsgqcbkoz.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtqserdiwf.html

[S27] C：定义常量
来源：http://hz.birdmap.top/gtkyqsnzfu.html

const double PI = 3.14159;
来源：http://hz.xziqi.cn/gtmbgvpoid.html

[S28] C：静态变量
来源：http://hz.c1oappe.top/gtayywpkpi.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtbjixskdu.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtphbhzqsp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gthgixgmfm.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtscsklire.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtsokdpjgw.html

#define X_H
来源：http://hz.cdnleiting.top/gtkqjxofyw.html

#endif
来源：http://hz.vqdsnc.cn/gtallznfah.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtsosfgifg.html

#include <iostream>
来源：http://hz.feifeiyinyue.top/gtwqlbnggg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtmlrlqffh.html

[S32] C++：字符串
来源：http://hz.xuetiantiany.cn/gtjbvqydep.html

std::string s = "hi";  s += "!";
来源：http://hz.fzhhl.top/gtmvkcdegx.html

[S33] C++：vector 增删
来源：http://hz.shuidangran.top/gtiyldpscu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hfpthk.cn/gttoabvylw.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtvbadffzo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtyqssfwrm.html

[S35] C++：map
来源：http://hz.wangshuangyany.cn/gtetrctquh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtmvjzwbfc.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtjiziwmql.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gttjpwhxuk.html

[S37] C++：set
来源：http://hz.zhoulong.xyz/gtyxcrlqyj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.bjfxy.top/gtpzttwzfj.html

[S38] C++：排序
来源：http://hz.cucudq.cn/gtlfeakrhi.html

std::sort(v.begin(), v.end());
来源：http://hz.pycfn.com/gtluaivitl.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtmjsynczm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dashuyun.cn/gtvflsmqzp.html

[S40] C++：查找元素
来源：http://hz.ppjwa.cn/gtzgfdyefm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydjk.org.cn/gtkiwiiqwp.html

[S41] C++：类与构造函数
来源：http://hz.52xcode.cn/gtathxijqd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtqdyhasza.html

[S42] C++：继承与虚函数
来源：http://hz.sysykeji.top/gtjvjmegnz.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtbwdkyxpe.html

[S43] C++：智能指针
来源：http://hz.hnqzz.top/gtcsnuxqeq.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtjomggenk.html

[S44] C++：引用传参
来源：http://hz.shuidangran.top/gtxxjsepat.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtfkkfsutf.html

[S45] C++：lambda
来源：http://hz.jyoumei.cn/gtwlpdgsii.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.svipenyu.cn/gtqwqooinx.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gtcwaopgfp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sufxvd.cn/gtugeuexzo.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gtbsscosla.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cqqwz.cn/gtgqdbcufh.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtyuoloynr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cashguo.top/gtvfyhsnmv.html

while (std::getline(in, line)) { }
来源：http://hz.jqgfzy.top/gtgyuplrtb.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtzapibqfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fzhhl.top/gtteyetfmv.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtxgevhblg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtyiymycpf.html

[S51] C++：显式类型转换
来源：http://hz.zhixingplan.top/gtqqsfwbgu.html

static_cast<double>(a) / b
来源：http://hz.meibo888.top/gtksmcoeys.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtulijvxlh.html

int size() const noexcept { return n_; }
来源：http://hz.ppjwa.cn/gtfjipssob.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtikoodvej.html

std::vector<int> w = std::move(v);
来源：http://hz.sysykeji.top/gtgzoxmeqc.html

[S54] C++：异常处理
来源：http://hz.hnxiangtu.top/gtvseozckm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gttshqvcqu.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gtyuygdihu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daria6918.cn/gtscbxiskn.html

[S56] C++：optional
来源：http://hz.yonumen.top/gttungbeom.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtgfqrioph.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gtgrirtqty.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtrburdzfx.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtmwbswpaz.html

namespace ns { int f() { return 1; } }
来源：http://hz.gzhubu.top/gtjjbvxucl.html

[S59] C++：静态断言
来源：http://hz.cqqwz.cn/gtgvqztvyu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258888.top/gtizojyewi.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gtdzgtwidw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gtfhbpcfbn.html

================================================================================
来源：http://hz.xinyue.icu/gtylvoturc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtrswbkfgf.html

================================================================================
来源：http://hz.jyoumei.cn/gthgxxzhfl.html

[T01] Kotlin：Hello World
来源：http://hz.zycfv.cn/gtpuablatp.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtgdjchcch.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtoobjdzeu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnqzz.top/gtbdlrwgkb.html

[T03] Kotlin：字符串模板
来源：http://hz.snrcjt.cn/gtyrkttins.html

"值: $b"
来源：http://hz.tian-w.cn/gtuevyasob.html

[T04] Kotlin：空安全
来源：http://hz.ywan-chungtsiang.top/gtqfctuefy.html

val n: String? = null;  n?.length
来源：http://hz.ywan-chungtsiang.top/gtdxsenkzm.html

[T05] Kotlin：when 表达式
来源：http://hz.zhaomingkeji.xyz/gtvdkfjtlm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtxubistyo.html

[T06] Kotlin：集合映射
来源：http://hz.smart0.xyz/gtphlslbbc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pycfn.com/gthvatvxgg.html

[T07] Kotlin：集合过滤
来源：http://hz.chenjidiqi.icu/gtoctcnlcu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pycfn.com/gtaruakxnw.html

[T08] Kotlin：数据类
来源：http://hz.vqdsnc.cn/gtppfzlgdt.html

data class User(val name: String, val age: Int)
来源：http://hz.zhixingplan.top/gtbgabiznp.html

[T09] Kotlin：扩展函数
来源：http://hz.ybcxt.top/gtymgnlszn.html

fun String.exclaim() = this + "!"
来源：http://hz.svipenyu.cn/gtbhkcaekf.html

[T10] Kotlin：默认参数
来源：http://hz.52xcode.cn/gthkhccafr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zdqjudy.top/gtabwvhrpy.html

[T11] Kotlin：协程
来源：http://hz.shzxlz.cn/gtqrkuzjzv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guannengcc.top/gtucbbenvw.html

[T12] Kotlin：解构声明
来源：http://hz.xylfe.cn/gtnbtjnmhl.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtfxbhcczi.html

[T13] Kotlin：只读 Map
来源：http://hz.hnqzz.top/gtwvbdzqtb.html

val m = mapOf("a" to 1)
来源：http://hz.yj202588.top/gtmbzivjtn.html

[T14] Kotlin：循环
来源：http://hz.jinyuanbaomall.cn/gthcgehnen.html

for (i in 1..10) println(i)
来源：http://hz.nwbrower.top/gtgqtmuret.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtvcjixnry.html

interface Shape { fun area(): Double }
来源：http://hz.iojbl.cn/gttlyixjpu.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtmqnqjojv.html

print("Hello")
来源：http://hz.xziqi.cn/gtpqxasbyd.html

[T17] Swift：变量与常量
来源：http://hz.bjfxy.top/gtwrdkcwhz.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtluzxzmis.html

[T18] Swift：字符串插值
来源：http://hz.yj202588.top/gtensbncca.html

"值: \(b)"
来源：http://hz.9152youxi.cn/gtwbgatgfb.html

[T19] Swift：可选绑定
来源：http://hz.mhx1999.top/gtfdfnqhld.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtiszoclkt.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtszupvnqk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gtbontszak.html

[T21] Swift：遍历
来源：http://hz.xuanzx.com/gtaoqjjwjb.html

for x in a { print(x) }
来源：http://hz.zhongyouzk.top/gtlgydtsoy.html

[T22] Swift：字典
来源：http://hz.bjfxy.top/gtzpdfwadr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenjidiqi.icu/gtwranfhad.html

[T23] Swift：函数
来源：http://hz.jianghu66.top/gtkokmrrro.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yanxiufei.cn/gtnoetcgjy.html

[T24] Swift：闭包
来源：http://hz.yj20258.top/gtkoxniugd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gteltvesnl.html

[T25] Swift：结构体
来源：http://hz.zhengqikj.top/gtnxykixhd.html

struct P { var x: Int }
来源：http://hz.jianghu66.top/gtaxwvrpoc.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtndciyzmy.html

class A: Base { override func f() {} }
来源：http://hz.gotoacloud.top/gtxvhgpyao.html

[T27] Swift：错误处理
来源：http://hz.haohaochexian.top/gtpuaiexad.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gtshnqigqq.html

[T28] Swift：枚举
来源：http://hz.yj202588.top/gtavwdttpv.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gthkktmkcj.html

[T29] Swift：guard 提前返回
来源：http://hz.feifeiyinyue.top/gtxlgieiep.html

guard let x = opt else { return }
来源：http://hz.hysaishi.cn/gtyablhlau.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtambrbpwu.html

protocol Shape { func area() -> Double }
来源：http://hz.nwbrower.top/gtdpldojpu.html

[T31] Lua：Hello World
来源：http://hz.sweek.top/gtdiogpjqt.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtsaflspfh.html

[T32] Lua：局部变量
来源：http://hz.xziqi.cn/gtmdjcnzgx.html

local a = 1
来源：http://hz.hnqzz.top/gtihahzwti.html

[T33] Lua：表（数组）
来源：http://hz.yueranfly.top/gtadjxeajj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ehwqpu.com/gtviuyakih.html

[T34] Lua：遍历表
来源：http://hz.xinyue.icu/gtzdghvvmx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cdnleiting.top/gtfinthxgt.html

[T35] Lua：字典表
来源：http://hz.gzhubu.top/gtqgtqdjxu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tianlin.xyz/gtiwwlrldn.html

[T36] Lua：函数
来源：http://hz.sufxvd.cn/gtmaghwylc.html

function add(a, b) return a + b end
来源：http://hz.wangdashe.top/gtgvwnabcs.html

[T37] Lua：字符串拼接
来源：http://hz.shzxlz.cn/gtnzwgihnh.html

"a" .. "b"
来源：http://hz.ehwqpu.com/gtubxidzux.html

[T38] Lua：条件
来源：http://hz.jiagoushi.top/gtxdmwsxpt.html

if x > 0 then print("正") end
来源：http://hz.cdnleiting.top/gtdosiwfbp.html

[T39] Lua：模式匹配
来源：http://hz.sysykeji.top/gtlrakcruh.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtndhouqcf.html

[T40] Lua：元表
来源：http://hz.chenjidiqi.icu/gtswjlcjpl.html

setmetatable({}, { __index = base })
来源：http://hz.pycfn.com/gttrwrcawq.html

[T41] Perl：Hello World
来源：http://hz.iojbl.cn/gtpjzlpbno.html

print "Hello\n";
来源：http://hz.fengsongda.top/gttekxvrew.html

[T42] Perl：变量类型
来源：http://hz.smart0.xyz/gtwrnrukcs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.dianchejie.cn/gticodhbio.html

[T43] Perl：字符串插值
来源：http://hz.yvedp.cn/gtoomghwiw.html

"值: $a"
来源：http://hz.haohaochexian.top/gtjzkltbyl.html

[T44] Perl：条件
来源：http://hz.yj202588.top/gtaxgjgycl.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangkeji.top/gtqfcthhhr.html

[T45] Perl：数组遍历
来源：http://hz.jyoumei.cn/gthciuhitp.html

for my $x (@arr) { print $x; }
来源：http://hz.iojbl.cn/gtoesmnhgt.html

[T46] Perl：哈希操作
来源：http://hz.bjfxy.top/gtjcgslclr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuxming.cn/gtumlonrjp.html

[T47] Perl：正则捕获
来源：http://hz.hammf.cn/gtlqbcnidz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guannengcc.top/gttkpdcurz.html

[T48] Perl：正则替换
来源：http://hz.smart0.xyz/gtuftcnlhr.html

$s =~ s/old/new/g;
来源：http://hz.cucudq.cn/gtjomrvovb.html

[T49] Perl：函数
来源：http://hz.quarkkingdee.top/gtvsqwpide.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yongpay.top/gtpqhjjhmr.html

[T50] Perl：逐行读文件
来源：http://hz.chenlongwang.top/gtlfeisdjx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ybcxt.top/gtnywxvisa.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ydzc1.top/gtkxkjskta.html

[T51] Scala：Hello World
来源：http://hz.sysykeji.top/gtdibqkjza.html

println("Hello")
来源：http://hz.jyoumei.cn/gtzxhruyla.html

[T52] Scala：变量
来源：http://hz.shanyushiyangkeji.top/gtzlsjrvlu.html

val a = 1;  var b = 2
来源：http://hz.zhengqikj.top/gtjncyeemx.html

[T53] Scala：字符串插值
来源：http://hz.yangfankeji.com/gtwdelrics.html

s"值: $b"
来源：http://hz.fzhhl.top/gtnviwmvpp.html

[T54] Scala：集合映射
来源：http://hz.feifeiyinyue.top/gtraopfajz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuxming.cn/gtfkztpwhh.html

[T55] Scala：集合过滤
来源：http://hz.xylfe.cn/gtcdjhlnaz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xuetiantiany.cn/gtvqdklfmb.html

[T56] Scala：样例类
来源：http://hz.zdqjudy.top/gtzrhimvfu.html

case class User(name: String, age: Int)
来源：http://hz.zhengqikj.top/gtforibmoi.html

[T57] Scala：模式匹配
来源：http://hz.cheryme.top/gthnqjpevb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shangyingyoupin.top/gtaqajsvaw.html

[T58] Scala：函数定义
来源：http://hz.dashuyun.cn/gtqzhibtmj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ehwqpu.com/gtthwuvgnm.html

[T59] Scala：循环
来源：http://hz.cashguo.top/gtpegmzfrs.html

for (i <- 1 to 10) println(i)
来源：http://hz.jiagoushi.top/gtqiywgcii.html

[T60] Scala：折叠
来源：http://hz.jqgufenzy.top/gtolgwvunl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jqgufenzy.top/gtlupmahvq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgjxcfxjx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cashguo.top/gtxrpoldii.html

================================================================================
来源：http://hz.0kj1m.cn/gtqzructmp.html

[U01] Py：创建虚拟环境
来源：http://hz.vqdsnc.cn/gtgiayboor.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnqzz.top/gtimcaapbv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhijiandao.cn/gthpaacgqr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.havefunace.top/gtrklusmeu.html

[U03] Py：加载 .env 配置
来源：http://hz.nanxinkj.top/gtxycswkvj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.birdmap.top/gtqjwjztlt.html

[U04] Py：变量调试打印
来源：http://hz.zycfv.cn/gtbgpogxbh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.andypj.xyz/gtmahqsyfk.html

[U05] Py：列表去重且保序
来源：http://hz.jinyuanbaomall.cn/gtzbdakvik.html

list(dict.fromkeys(arr))
来源：http://hz.hnqzz.top/gtppynhakm.html

[U06] Py：合并两个字典
来源：http://hz.jlsjyb.cn/gttxdaqtwd.html

{**a, **b}
来源：http://hz.gotoacloud.top/gtsacjdflk.html

[U07] Py：反转字典键值
来源：http://hz.fzhhl.top/gtoiklavao.html

{v: k for k, v in d.items()}
来源：http://hz.zhongyouzk.top/gtjrmggffr.html

[U08] Py：展平二维列表
来源：http://hz.cdnleiting.top/gtmtmiusrm.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtsyihrmor.html

[U09] Py：字典取最大值的键
来源：http://hz.yueranfly.top/gtirkzvuhk.html

max(d, key=d.get)
来源：http://hz.pengpengdd.cyou/gtwsflmutx.html

[U10] Py：按值排序字典
来源：http://hz.zhongyouzk.top/gtajuccvnc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hywenlv.cn/gtflbbxtul.html

[U11] Py：生成器表达式
来源：http://hz.zhengqikj.top/gtrddkmxfb.html

(x * 2 for x in arr)
来源：http://hz.xylfe.cn/gtcbwyktol.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gogol.net.cn/gthknylybk.html

Counter(arr).most_common(3)
来源：http://hz.chenzaomai.com/gteemenkag.html


<!-- 参考信息 -->