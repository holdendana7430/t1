代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gtdfgmrgxx.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtubdwijol.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtjnxgdllt.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtpwogrqba.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtvazpnmjf.html

[R72] 等待端口就绪
来源：http://hz.xingfuxueyuan.xyz/gttwayxkkh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.smart0.xyz/gtbcclfbvh.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtbfmrxtup.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gtiovyjkuo.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtifvbnith.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.52xcode.cn/gtqrkvervc.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtzqerdttw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jiagoushi.top/gtfpueivgg.html

[R76] 使用临时文件
来源：http://hz.kuanghao11.cn/gtquysusvj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtrreccvpg.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtcqytnxri.html

read -rp "请输入: " ans
来源：http://hz.pycfn.com/gtsaancewk.html

[R78] 交互式菜单
来源：http://hz.yvedp.cn/gtaiogfcjy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuanzx.com/gtyrhkwyxi.html

[R79] 解析命令行选项
来源：http://hz.feifeiyinyue.top/gtkzwkicch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hammf.cn/gtdkwpeqzf.html

[R80] 查看脚本执行耗时
来源：http://hz.zycfv.cn/gtwxilsmdc.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtbvzdpdky.html

================================================================================
来源：http://hz.bjfxy.top/gtgpuvisvx.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtbjyzlwjs.html

================================================================================
来源：http://hz.yuxming.cn/gtrkxxpzbd.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gttuuhvrvo.html

#include <stdio.h>
来源：http://hz.shuidangran.top/gtuehnkccz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gotoacloud.top/gtfphqdasn.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtkxngnlwi.html

int a = 10; printf("%d\n", a);
来源：http://hz.yvedp.cn/gtqdviufmg.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtrsjonroq.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtcfrxmmrg.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtpruyrzsv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtrlwvtegh.html

[S05] C：字符串长度
来源：http://hz.9152youxi.cn/gtslghbwsj.html

strlen(s)
来源：http://hz.yangfankeji.com/gtoftaultz.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtwekcndxo.html

strcmp(a, b) == 0
来源：http://hz.havefunace.top/gtpbcnaovj.html

[S07] C：数组遍历求和
来源：http://hz.cqqwz.cn/gthnoizsct.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhongyouzk.top/gtbyibawbo.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gtbfgqftmu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtilvghqzp.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtuoayammj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gtxxdgwvon.html

[S10] C：指针与解引用
来源：http://hz.yanxiufei.cn/gtqocijbgf.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gtprrzbact.html

[S11] C：逐行读文件
来源：http://hz.jyoumei.cn/gttxxabdkm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtjshvbtcr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jlsjyb.cn/gtnbxujkul.html

fclose(f);
来源：http://hz.havefunace.top/gtzjrgptkp.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtwajnqejo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtbxphrryh.html

[S13] C：宏定义
来源：http://hz.xuetiantiany.cn/gttqjylumc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtaxpvpglj.html

[S14] C：枚举
来源：http://hz.havefunace.top/gtudaerpym.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigufen.top/gthjmgdajo.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtwxwpvqcn.html

(double) a / b
来源：http://hz.tianlin.xyz/gtjrpfbbvu.html

[S16] C：位操作置位
来源：http://hz.shangyingyoupin.top/gtscsvuibb.html

x |= (1 << 3);
来源：http://hz.dianchejie.cn/gtdtbjbnvq.html

[S17] C：安全拼接字符串
来源：http://hz.hysaishi.cn/gtadmwjnzs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hysaishi.cn/gtcykjuewe.html

[S18] C：命令行参数
来源：http://hz.xinyue.icu/gtuumcyfps.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtjlbtvrsh.html

[S19] C：快速排序
来源：http://hz.kuanghao11.cn/gtjzzgxynu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtooqsghjx.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gtqhhaghiw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtwswxoqvj.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtmlcnzsgc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shzxlz.cn/gtuyegtuzv.html

[S22] C：字符串转数字
来源：http://hz.xylfe.cn/gtzhcurnyg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cashguo.top/gtkmqfisgl.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtjbqxztun.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hammf.cn/gtrwivakry.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtfloscjcm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yangfankeji.com/gtyauptetl.html

[S25] C：内存拷贝
来源：http://hz.meibo888.top/gtaamhryou.html

memcpy(dst, src, n);
来源：http://hz.shangyingyoupin.top/gtaikwkpjd.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtjwaijpvp.html

memset(a, 0, sizeof a);
来源：http://hz.hfpthk.cn/gtmwggkdwk.html

[S27] C：定义常量
来源：http://hz.yuanzhike.top/gtvqfnryxj.html

const double PI = 3.14159;
来源：http://hz.ivvv.top/gtqzqimgob.html

[S28] C：静态变量
来源：http://hz.hnqzz.top/gtmdtdswsx.html

static int counter = 0;
来源：http://hz.jinghuilouyu.cn/gtqiovybui.html

[S29] C：变参函数
来源：http://hz.yj20258.top/gtzsjhkonp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtvprzbvhk.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gtghahggiq.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtcwntzcur.html

#define X_H
来源：http://hz.xylfe.cn/gtkhhcwrsz.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtrryslzau.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gththszlnu.html

#include <iostream>
来源：http://hz.gaohongyu789.top/gtgrmgjlwz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fengsongda.top/gtykpeescv.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtbsbcrqrd.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtiwtwuiqe.html

[S33] C++：vector 增删
来源：http://hz.52xcode.cn/gtimdxqacf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenzaomai.com/gtkabazbed.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtrffvilsv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.mhx1999.top/gtyradpmuw.html

[S35] C++：map
来源：http://hz.hongshengwenyu.top/gtzifzsydq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtkcwuexed.html

[S36] C++：unordered_map
来源：http://hz.chenzaomai.com/gtmyjidhpz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtbzljmmok.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtpptfajia.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtkkpgybbx.html

[S38] C++：排序
来源：http://hz.gaohongyu789.top/gteijbkamn.html

std::sort(v.begin(), v.end());
来源：http://hz.9152youxi.cn/gtqyhjfmxk.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gthbyaretd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.haohaochexian.top/gtexuuelyu.html

[S40] C++：查找元素
来源：http://hz.jinqigfzy.top/gtegjxparx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.pycfn.com/gtrqvwirry.html

[S41] C++：类与构造函数
来源：http://hz.birdmap.top/gtcfwkzgzq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gotoacloud.top/gtmsgjrtyv.html

[S42] C++：继承与虚函数
来源：http://hz.shuidangran.top/gtkmchyinv.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtkniipkiq.html

[S43] C++：智能指针
来源：http://hz.gzhubu.top/gtgfatjjkx.html

auto p = std::make_unique<int>(5);
来源：http://hz.fengsongda.top/gthlsngxlc.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtgknjxiqc.html

void inc(int &x) { ++x; }
来源：http://hz.iojbl.cn/gtqejkzqfs.html

[S45] C++：lambda
来源：http://hz.cheryme.top/gtoeeoyeaj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtayprsuge.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtpwjkvanu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hywenlv.cn/gtgrswglrh.html

[S47] C++：结构化绑定遍历
来源：http://hz.yanxiufei.cn/gtutvkrceq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yonumen.top/gtmvieauab.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtirlaydfw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jyoumei.cn/gtlfhnxczf.html

while (std::getline(in, line)) { }
来源：http://hz.hysaishi.cn/gtkxwgijqr.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gtzdruknoe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.svipenyu.cn/gthpsqfrdq.html

[S50] C++：格式化数字
来源：http://hz.dianchejie.cn/gtqiwrmkuy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pengpengdd.cyou/gtnjgwmrun.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gtcdmhnvpx.html

static_cast<double>(a) / b
来源：http://hz.cucudq.cn/gtiibapzig.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtfgbepojt.html

int size() const noexcept { return n_; }
来源：http://hz.yonumen.top/gtxpqpaidu.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtvmbkogso.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtqvyxcldt.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtjywqzwps.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.meibo888.top/gtqtuakaat.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gttwunrpoc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.vqdsnc.cn/gtcqqkihqa.html

[S56] C++：optional
来源：http://hz.daxiang520.top/gtkrniohbq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gtnhxllssu.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtdgrbmpzy.html

constexpr int N = 10;
来源：http://hz.hfpthk.cn/gtaxzsrlgu.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gttgfvsxoy.html

namespace ns { int f() { return 1; } }
来源：http://hz.jiagoushi.top/gtgoevtcsf.html

[S59] C++：静态断言
来源：http://hz.meibo888.top/gtdidquqfl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gtpupkvlst.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtamrhigxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pengpengdd.cyou/gtdewhqlqv.html

================================================================================
来源：http://hz.jyoumei.cn/gtbqjxyhzo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jlsjyb.cn/gtlijifayv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzkdceqre.html

[T01] Kotlin：Hello World
来源：http://hz.ehwqpu.com/gtewmdtxod.html

println("Hello")
来源：http://hz.zhoulong.xyz/gthsmscurl.html

[T02] Kotlin：变量
来源：http://hz.aizwys.cn/gteswpwqmg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daxiang520.top/gtvnvgeknu.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtosxgvgbo.html

"值: $b"
来源：http://hz.ivvv.top/gtzpntrcpf.html

[T04] Kotlin：空安全
来源：http://hz.cheryme.top/gtmqhkxsbd.html

val n: String? = null;  n?.length
来源：http://hz.meibo888.top/gtqnjqafne.html

[T05] Kotlin：when 表达式
来源：http://hz.guowangkeji.top/gtujatblgc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.feifeiyinyue.top/gtnpjcqota.html

[T06] Kotlin：集合映射
来源：http://hz.yuanzhike.top/gtnlzckclp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.bjfxy.top/gtmxxxwisn.html

[T07] Kotlin：集合过滤
来源：http://hz.sweek.top/gtjwgpruvo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guowangkeji.top/gtbyncjasj.html

[T08] Kotlin：数据类
来源：http://hz.yanxiufei.cn/gtvfgscqta.html

data class User(val name: String, val age: Int)
来源：http://hz.zhixingplan.top/gtnrxbvwap.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gtneluayvj.html

fun String.exclaim() = this + "!"
来源：http://hz.ydzc1.top/gtbzhqesuf.html

[T10] Kotlin：默认参数
来源：http://hz.52xcode.cn/gtbqsrowpm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gtfakzljto.html

[T11] Kotlin：协程
来源：http://hz.ywan-chungtsiang.top/gthpqnjhiq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tian-w.cn/gtpeaipvpq.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gtrlaqacqm.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj202588.top/gtstvfyyuq.html

[T13] Kotlin：只读 Map
来源：http://hz.gaohongyu789.top/gtiphppfuy.html

val m = mapOf("a" to 1)
来源：http://hz.havefunace.top/gtppshjwtv.html

[T14] Kotlin：循环
来源：http://hz.bjfxy.top/gtnfzrvhwo.html

for (i in 1..10) println(i)
来源：http://hz.aibaodan.cn/gtgomvglpu.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gtuoniecxc.html

interface Shape { fun area(): Double }
来源：http://hz.snrcjt.cn/gtxbtmmepb.html

[T16] Swift：Hello World
来源：http://hz.cqqwz.cn/gtbzhnzzai.html

print("Hello")
来源：http://hz.jyoumei.cn/gtvwtcsdnp.html

[T17] Swift：变量与常量
来源：http://hz.yangfankeji.com/gtdgbwvlfn.html

var a = 1;  let b = 2
来源：http://hz.svipenyu.cn/gttgpjxdac.html

[T18] Swift：字符串插值
来源：http://hz.jlsjyb.cn/gtojdawrum.html

"值: \(b)"
来源：http://hz.snrcjt.cn/gtghnjrlsy.html

[T19] Swift：可选绑定
来源：http://hz.ywan-chungtsiang.top/gtmckzlels.html

if let n = opt { print(n) }
来源：http://hz.gotoacloud.top/gtydcaizgz.html

[T20] Swift：数组操作
来源：http://hz.zhoulong.xyz/gttbftatwg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.birdmap.top/gthdgepyqe.html

[T21] Swift：遍历
来源：http://hz.iojbl.cn/gtxxnumsem.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtsswksdid.html

[T22] Swift：字典
来源：http://hz.birdmap.top/gtcgtrkhot.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zdqjudy.top/gttmzvhxsm.html

[T23] Swift：函数
来源：http://hz.guannengcc.top/gtyjyebzqr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhijiandao.cn/gtgqplpaak.html

[T24] Swift：闭包
来源：http://hz.316326.xyz/gtemdozhvu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.quarkkingdee.top/gtzewqruxb.html

[T25] Swift：结构体
来源：http://hz.zhiwuduotai.top/gtvkyozrjr.html

struct P { var x: Int }
来源：http://hz.hammf.cn/gthelqszcw.html

[T26] Swift：类与重写
来源：http://hz.hywenlv.cn/gtqxnmaafo.html

class A: Base { override func f() {} }
来源：http://hz.dianchejie.cn/gtnigqezls.html

[T27] Swift：错误处理
来源：http://hz.c1oappe.top/gtipuiujzw.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtnscfmlub.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtimpvdiuy.html

enum Color { case red, green }
来源：http://hz.xziqi.cn/gtgmemfqmh.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangkeji.top/gtzfpkvjzf.html

guard let x = opt else { return }
来源：http://hz.fzhhl.top/gtowajtftb.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gtlpztwpcn.html

protocol Shape { func area() -> Double }
来源：http://hz.316326.xyz/gthwgygwxr.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtqxvooxgx.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtljyfctwn.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gtknelnxvk.html

local a = 1
来源：http://hz.tian-w.cn/gtloxbcpjc.html

[T33] Lua：表（数组）
来源：http://hz.9152youxi.cn/gtvwazxorw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnqzz.top/gthrlzpnds.html

[T34] Lua：遍历表
来源：http://hz.redwolf501.top/gtnrltcodu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gtjhukrjlm.html

[T35] Lua：字典表
来源：http://hz.yuxming.cn/gtobgikyqa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jqgufenzy.top/gtwlqyjliu.html

[T36] Lua：函数
来源：http://hz.daxiang520.top/gtnbevqekc.html

function add(a, b) return a + b end
来源：http://hz.tian-w.cn/gtiinvocpr.html

[T37] Lua：字符串拼接
来源：http://hz.gogol.net.cn/gtdsxujefn.html

"a" .. "b"
来源：http://hz.fengsongda.top/gtatpkqmgg.html

[T38] Lua：条件
来源：http://hz.jinghuilouyu.cn/gtxymagrbt.html

if x > 0 then print("正") end
来源：http://hz.9152youxi.cn/gtkywdnkht.html

[T39] Lua：模式匹配
来源：http://hz.jqgfzy.top/gtznnksizf.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtulscvmzt.html

[T40] Lua：元表
来源：http://hz.ybcxt.top/gtsgwaafvf.html

setmetatable({}, { __index = base })
来源：http://hz.gaohongyu789.top/gtuhltkquh.html

[T41] Perl：Hello World
来源：http://hz.nanxinkj.top/gtsgetyyxm.html

print "Hello\n";
来源：http://hz.zdqjudy.top/gtstevhomb.html

[T42] Perl：变量类型
来源：http://hz.feifeiyinyue.top/gtiayrriwe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gtqizrmpnf.html

[T43] Perl：字符串插值
来源：http://hz.52xcode.cn/gtwddoqwhr.html

"值: $a"
来源：http://hz.gotoacloud.top/gturyeubph.html

[T44] Perl：条件
来源：http://hz.guannengcc.top/gtghftmcyn.html

if ($a > 0) { print "正"; }
来源：http://hz.hnqzz.top/gtkdypjghj.html

[T45] Perl：数组遍历
来源：http://hz.zhiwuduotai.top/gtlpjiuyoh.html

for my $x (@arr) { print $x; }
来源：http://hz.haohaochexian.top/gtoakvssgf.html

[T46] Perl：哈希操作
来源：http://hz.pycfn.com/gtyqdmbnao.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258888.top/gtfsewoxzj.html

[T47] Perl：正则捕获
来源：http://hz.jinghuilouyu.cn/gtmiojfnim.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydzc1.top/gthvtvfjst.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtjkosrjpr.html

$s =~ s/old/new/g;
来源：http://hz.hywenlv.cn/gtqizeppaf.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gtwlvxhcxj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.wangdashe.top/gtbepgzarn.html

[T50] Perl：逐行读文件
来源：http://hz.316326.xyz/gtujxydxfy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shangyingyoupin.top/gtvlnvvvgu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.c1oappe.top/gtebsatdmh.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gtqhfjauqt.html

println("Hello")
来源：http://hz.ppjwa.cn/gtwbjwtaav.html

[T52] Scala：变量
来源：http://hz.hywenlv.cn/gtyokscrua.html

val a = 1;  var b = 2
来源：http://hz.hnqzz.top/gtdbxbtwax.html

[T53] Scala：字符串插值
来源：http://hz.sweek.top/gtxyeiqpnh.html

s"值: $b"
来源：http://hz.guowangkeji.top/gtylllwthd.html

[T54] Scala：集合映射
来源：http://hz.haohaochexian.top/gttvkwrzqq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtcrkparee.html

[T55] Scala：集合过滤
来源：http://hz.gaohongyu789.top/gtwlbwcbws.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ppjwa.cn/gtzgmivxhf.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtzvihkenu.html

case class User(name: String, age: Int)
来源：http://hz.iojbl.cn/gtjyruanuq.html

[T57] Scala：模式匹配
来源：http://hz.yuxming.cn/gtfrtjwjol.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinyuanbaomall.cn/gtdnuqremm.html

[T58] Scala：函数定义
来源：http://hz.jiagoushi.top/gtdiobfeel.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtafwitpfd.html

[T59] Scala：循环
来源：http://hz.redwolf501.top/gtzyjxtson.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtihhevezi.html

[T60] Scala：折叠
来源：http://hz.jinyuanbaomall.cn/gtpnugkwdf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.fzhhl.top/gtlnqbfsgb.html

================================================================================
来源：http://hz.tian-w.cn/gtfrdpiqkp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydzc1.top/gtrteynfum.html

================================================================================
来源：http://hz.ehwqpu.com/gtwvaknivv.html

[U01] Py：创建虚拟环境
来源：http://hz.ydzc1.top/gtsksatbnq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.snrcjt.cn/gtzwqdalmh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydjk.org.cn/gtmqjvfeif.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.daxiang520.top/gtrusnimzd.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gtikumikky.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinghuilouyu.cn/gteoigpuhj.html

[U04] Py：变量调试打印
来源：http://hz.gzhubu.top/gtnnozmhdg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yangfankeji.com/gtrnjuhkvp.html

[U05] Py：列表去重且保序
来源：http://hz.yangfankeji.com/gtxhpqqztk.html

list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gthzbwosct.html

[U06] Py：合并两个字典
来源：http://hz.jinqigfzy.top/gtdszesxbg.html

{**a, **b}
来源：http://hz.zycfv.cn/gtybwbkbsg.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gtkxmqlxff.html

{v: k for k, v in d.items()}
来源：http://hz.ydjk.org.cn/gtpatitaws.html

[U08] Py：展平二维列表
来源：http://hz.aibaodan.cn/gtnptnbnfa.html

[y for x in nested for y in x]
来源：http://hz.snrcjt.cn/gtkfbghjej.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangkeji.top/gtpvsyqasw.html

max(d, key=d.get)
来源：http://hz.hysaishi.cn/gtkoadlwvv.html

[U10] Py：按值排序字典
来源：http://hz.shanyushiyangtech.top/gtlvaurzri.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sxryk.cn/gtasmwthsf.html


<!-- 参考信息 -->