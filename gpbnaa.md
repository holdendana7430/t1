代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtbydoldrc.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gtrkezonfa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gttvbyajff.html

[R73] 分割大日志
来源：http://hz.jiagoushi.top/gtbhbuijkv.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtyjuzbaio.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtdjbqucpf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuxming.cn/gtrfabtifu.html

[R75] 导出环境变量
来源：http://hz.hnxiangtu.top/gtrxzygjnl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtgazfcgit.html

[R76] 使用临时文件
来源：http://hz.xingfuxueyuan.xyz/gtpykvqpxm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtewmzwomf.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtamgndyug.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtooahnfxw.html

[R78] 交互式菜单
来源：http://hz.0kj1m.cn/gtxcbfgats.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gtbfutwfia.html

[R79] 解析命令行选项
来源：http://hz.shuidangran.top/gtskmxjedt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yonumen.top/gtqcqljdiu.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtsozqoech.html

time ./run.sh
来源：http://hz.tian-w.cn/gtswaqrkhh.html

================================================================================
来源：http://hz.sysykeji.top/gthydwgext.html

S. C / C++ 专题
来源：http://hz.vqdsnc.cn/gtlonnudpc.html

================================================================================
来源：http://hz.mhx1999.top/gtfelgkloe.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtrkzpodqs.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gtmjtwztkv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtwsobsfds.html

[S02] C：变量与格式化输出
来源：http://hz.aizwys.cn/gtvrxqmtxa.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtxhiqxkah.html

[S03] C：读入整数
来源：http://hz.jinqigfzy.top/gtsdfltckc.html

int x; scanf("%d", &x);
来源：http://hz.yueranfly.top/gtctwfzivy.html

[S04] C：字符串复制
来源：http://hz.sufxvd.cn/gtscuanzps.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tian-w.cn/gtogczkjos.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtbodeyngu.html

strlen(s)
来源：http://hz.birdmap.top/gteduhukms.html

[S06] C：字符串比较
来源：http://hz.daria6918.cn/gtlgfrplyn.html

strcmp(a, b) == 0
来源：http://hz.yvedp.cn/gtawbrlcvo.html

[S07] C：数组遍历求和
来源：http://hz.gotoacloud.top/gtxxctflez.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.52xcode.cn/gtrcsalrjm.html

[S08] C：动态内存分配与释放
来源：http://hz.jinghuilouyu.cn/gtejzfcpfn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenzaomai.com/gtnokzwpvm.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtxxknzcgt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.smart0.xyz/gtbedphifd.html

[S10] C：指针与解引用
来源：http://hz.hongshengwenyu.top/gtwrzngbmj.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangtech.top/gtrykhgfzm.html

[S11] C：逐行读文件
来源：http://hz.nwbrower.top/gtnmelolxn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtuhsbkrhj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hywenlv.cn/gthhgqioyg.html

fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtsuqewuow.html

[S12] C：写文件
来源：http://hz.tianlin.xyz/gtoasuqwjv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtaqpvwedt.html

[S13] C：宏定义
来源：http://hz.ydzc1.top/gthrjuvltv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gtkbbyhvlj.html

[S14] C：枚举
来源：http://hz.hammf.cn/gtpmxhrimy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gtiqtwjgbk.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtjxzoogdc.html

(double) a / b
来源：http://hz.ivvv.top/gtqlahbptt.html

[S16] C：位操作置位
来源：http://hz.shuidangran.top/gtamdezbqw.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtylorekwc.html

[S17] C：安全拼接字符串
来源：http://hz.zycfv.cn/gtmcgmdjni.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuxming.cn/gtgogbtxms.html

[S18] C：命令行参数
来源：http://hz.dashuyun.cn/gtboftnqew.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtwmfeepdj.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtumrxraqt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtmarmeuts.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gtffvurkhs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtkdzbjgky.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtpmfbvlti.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sysykeji.top/gtcbdurdsv.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtaioynwuf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hywenlv.cn/gtdonaeosl.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtkioxqkbj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gteqaqxcrz.html

[S24] C：获取本地时间
来源：http://hz.ivvv.top/gtbtqeksbo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinghuilouyu.cn/gtguvroyhe.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtnufhwoqr.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtdnkhybsn.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtsyymrhtx.html

memset(a, 0, sizeof a);
来源：http://hz.zhijiandao.cn/gtwzayfbip.html

[S27] C：定义常量
来源：http://hz.wangshuangyany.cn/gtlphhavll.html

const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtsqytsahj.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtxpzvwdvm.html

static int counter = 0;
来源：http://hz.fengsongda.top/gtoaqwbtkp.html

[S29] C：变参函数
来源：http://hz.daria6918.cn/gtrhhglfbm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cashguo.top/gtbizaibdr.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtwlksykqm.html

#ifndef X_H
来源：http://hz.snrcjt.cn/gtsskelejo.html

#define X_H
来源：http://hz.tanke756.top/gtieiwwjxe.html

#endif
来源：http://hz.c1oappe.top/gtvanvdago.html

[S31] C++：Hello World
来源：http://hz.birdmap.top/gtqidrhplz.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gticccqczk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxuanxn.top/gtovwwnqrv.html

[S32] C++：字符串
来源：http://hz.hnqzz.top/gttbkednnj.html

std::string s = "hi";  s += "!";
来源：http://hz.ybcxt.top/gtwutbwoij.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangkeji.top/gtnhfoxfao.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtrxvlhnkd.html

[S34] C++：遍历 vector
来源：http://hz.gzhubu.top/gtodowzteh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtvssnxiys.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtqobbkftd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtxqfbatsh.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gturwwhrwg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtgmgofkwa.html

[S37] C++：set
来源：http://hz.9152youxi.cn/gtglzikbxx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigufen.top/gtkvaaizuq.html

[S38] C++：排序
来源：http://hz.cucudq.cn/gtnytojgrh.html

std::sort(v.begin(), v.end());
来源：http://hz.jianghu66.top/gtaaextpid.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtnddbhxzb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtlvipavwk.html

[S40] C++：查找元素
来源：http://hz.jianghu66.top/gtrjqmclnh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhixingplan.top/gtiauwnxre.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gttxkuaslg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgfzy.top/gtirwplvnw.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtcfgadkbg.html

class B : public Base { public: void f() override {} };
来源：http://hz.kuanghao11.cn/gtdemikemv.html

[S43] C++：智能指针
来源：http://hz.ybcxt.top/gtifenutvh.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtajesozwj.html

[S44] C++：引用传参
来源：http://hz.yanxiufei.cn/gtsecfzopy.html

void inc(int &x) { ++x; }
来源：http://hz.gotoacloud.top/gtpqaydtzq.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtickernrh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gtuyziraog.html

[S46] C++：函数模板
来源：http://hz.daxiang520.top/gtkzsoqinn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.0kj1m.cn/gtvjvhtkfq.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj202588.top/gtilqypnmn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.dianchejie.cn/gtylgzwxwv.html

[S48] C++：逐行读文件
来源：http://hz.meibo888.top/gtntctqcsx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gtlkexrake.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gtrhuurkcm.html

[S49] C++：写文件
来源：http://hz.sweek.top/gtvuywsfso.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jianghu66.top/gtkmwnyzti.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gttytodoan.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtvkzpuybs.html

[S51] C++：显式类型转换
来源：http://hz.nwbrower.top/gtmelpovln.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtmhcqlres.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtytbzntcd.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtbimplcyz.html

[S53] C++：移动语义
来源：http://hz.zhiwuduotai.top/gtkvnrzqlh.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtkurltbhw.html

[S54] C++：异常处理
来源：http://hz.yj20258.top/gtdftrrzjd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.kuanghao11.cn/gtnacxjhwe.html

[S55] C++：结构化绑定
来源：http://hz.jinyuanbaomall.cn/gtgqguyrqi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cashguo.top/gttcsrqmoz.html

[S56] C++：optional
来源：http://hz.xuetiantiany.cn/gtzmhymhyz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gttintriyu.html

[S57] C++：编译期常量
来源：http://hz.aizwys.cn/gtiqdyopeo.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gtnemhhiad.html

[S58] C++：命名空间
来源：http://hz.chenzaomai.com/gtvwoourgc.html

namespace ns { int f() { return 1; } }
来源：http://hz.pycfn.com/gticslgykl.html

[S59] C++：静态断言
来源：http://hz.ybcxt.top/gtbzfatdhx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xinyue.icu/gtvuncpmin.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtzpntkwkj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shuidangran.top/gtyohzwpde.html

================================================================================
来源：http://hz.xinyue.icu/gtyyceqtyh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtqawjtrzv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtghjlouuv.html

[T01] Kotlin：Hello World
来源：http://hz.xylfe.cn/gtbwdesypq.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtbkhfunuf.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtlgdvtgyb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtexvkuydh.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgfzy.top/gtbaenuvrk.html

"值: $b"
来源：http://hz.zhoulong.xyz/gtdunlwhgg.html

[T04] Kotlin：空安全
来源：http://hz.ydzc1.top/gtfykxtves.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtazfccqlw.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtrqmxeomp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258.top/gtywclqztu.html

[T06] Kotlin：集合映射
来源：http://hz.zhoulong.xyz/gtgtstefch.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sufxvd.cn/gtagotlzdg.html

[T07] Kotlin：集合过滤
来源：http://hz.xinyue.icu/gtuxcharkd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gtdsnbgwyk.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtzcaexfou.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtkqojlqku.html

[T09] Kotlin：扩展函数
来源：http://hz.ppjwa.cn/gtgxgdamcm.html

fun String.exclaim() = this + "!"
来源：http://hz.gogol.net.cn/gtrzpxompt.html

[T10] Kotlin：默认参数
来源：http://hz.daria6918.cn/gtsipywuzf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhijiandao.cn/gtqfqdthgb.html

[T11] Kotlin：协程
来源：http://hz.daria6918.cn/gticqepyms.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yvedp.cn/gtneqkxayr.html

[T12] Kotlin：解构声明
来源：http://hz.nwbrower.top/gthcpipcvo.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtsxrwbrrg.html

[T13] Kotlin：只读 Map
来源：http://hz.jinghuilouyu.cn/gthgzvohnp.html

val m = mapOf("a" to 1)
来源：http://hz.pengpengdd.cyou/gtwmrhekpf.html

[T14] Kotlin：循环
来源：http://hz.vqdsnc.cn/gtavyyukiq.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gthfhvlavt.html

[T15] Kotlin：接口
来源：http://hz.zhongyouzk.top/gtezxfvwca.html

interface Shape { fun area(): Double }
来源：http://hz.guannengcc.top/gtcaxljsen.html

[T16] Swift：Hello World
来源：http://hz.gotoacloud.top/gtmcochvyb.html

print("Hello")
来源：http://hz.cdnleiting.top/gtmcnrwmgb.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtryvxozgh.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtbzxugpuk.html

[T18] Swift：字符串插值
来源：http://hz.52xcode.cn/gtmedhpczq.html

"值: \(b)"
来源：http://hz.gaohongyu789.top/gtbmticuxy.html

[T19] Swift：可选绑定
来源：http://hz.xuetiantiany.cn/gtxrdhxvad.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtkzakkale.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gttyfgggzm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gtjdwqfjxl.html

[T21] Swift：遍历
来源：http://hz.ehwqpu.com/gtlorufnrn.html

for x in a { print(x) }
来源：http://hz.iojbl.cn/gtkkozconp.html

[T22] Swift：字典
来源：http://hz.c1oappe.top/gtdmzhgxee.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.316326.xyz/gtocugnexo.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtekzzhrdb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cdnleiting.top/gttqzhgksy.html

[T24] Swift：闭包
来源：http://hz.hywenlv.cn/gtrbhrnllb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtxiciknoi.html

[T25] Swift：结构体
来源：http://hz.pycfn.com/gtehscvhyq.html

struct P { var x: Int }
来源：http://hz.hongshengwenyu.top/gtkrcbjhjk.html

[T26] Swift：类与重写
来源：http://hz.zhongyouzk.top/gtmjrfucva.html

class A: Base { override func f() {} }
来源：http://hz.yonumen.top/gtnrvidojd.html

[T27] Swift：错误处理
来源：http://hz.yanxiufei.cn/gtkwiyadrw.html

do { try f() } catch { print(error) }
来源：http://hz.xziqi.cn/gttyqpvqmg.html

[T28] Swift：枚举
来源：http://hz.nwbrower.top/gthomtkfgj.html

enum Color { case red, green }
来源：http://hz.redwolf501.top/gtaldrdakd.html

[T29] Swift：guard 提前返回
来源：http://hz.iojbl.cn/gtnyokeoxh.html

guard let x = opt else { return }
来源：http://hz.andypj.xyz/gtqifrylzi.html

[T30] Swift：协议
来源：http://hz.jinghuilouyu.cn/gtivhfypan.html

protocol Shape { func area() -> Double }
来源：http://hz.andypj.xyz/gtsdjppken.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtfmoiyrnf.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtpnewnifv.html

[T32] Lua：局部变量
来源：http://hz.daxiang520.top/gtsfchwvbf.html

local a = 1
来源：http://hz.yuanzhike.top/gtyrarhnmq.html

[T33] Lua：表（数组）
来源：http://hz.cheryme.top/gtkduyclvv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daria6918.cn/gtnwjozpql.html

[T34] Lua：遍历表
来源：http://hz.gogol.net.cn/gtsoqxazqv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xuanzx.com/gtrxhmbssb.html

[T35] Lua：字典表
来源：http://hz.yueranfly.top/gtpwmplnle.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenzaomai.com/gtwggumbou.html

[T36] Lua：函数
来源：http://hz.shanyushiyangkeji.top/gtcvfquyjk.html

function add(a, b) return a + b end
来源：http://hz.xylfe.cn/gtvosunumy.html

[T37] Lua：字符串拼接
来源：http://hz.kuanghao11.cn/gtrqcftgxf.html

"a" .. "b"
来源：http://hz.chenjidiqi.icu/gtvghqfxlz.html

[T38] Lua：条件
来源：http://hz.hnxiangtu.top/gthjowvgbk.html

if x > 0 then print("正") end
来源：http://hz.yueranfly.top/gtgvzgnyvc.html

[T39] Lua：模式匹配
来源：http://hz.cheryme.top/gtfxtoqvxt.html

string.find(s, "%d+")
来源：http://hz.shangyingyoupin.top/gtoipefkdh.html

[T40] Lua：元表
来源：http://hz.jqgfzy.top/gtxwjiaaig.html

setmetatable({}, { __index = base })
来源：http://hz.0kj1m.cn/gtxthvmqcw.html

[T41] Perl：Hello World
来源：http://hz.chenzaomai.com/gtkxesyrxa.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtduoaqses.html

[T42] Perl：变量类型
来源：http://hz.sysykeji.top/gtxufkylmh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yuanzhike.top/gtcktotrwi.html

[T43] Perl：字符串插值
来源：http://hz.dashuyun.cn/gtapiyuwhi.html

"值: $a"
来源：http://hz.jlsjyb.cn/gtzstgrsvd.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gtpkogbbuc.html

if ($a > 0) { print "正"; }
来源：http://hz.meibo888.top/gtummqppzc.html

[T45] Perl：数组遍历
来源：http://hz.jqgufenzy.top/gtbjwclotn.html

for my $x (@arr) { print $x; }
来源：http://hz.meibo888.top/gtbfjtdtnj.html

[T46] Perl：哈希操作
来源：http://hz.jianghu66.top/gthnylujod.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gtmxhgdivh.html

[T47] Perl：正则捕获
来源：http://hz.tian-w.cn/gtmqgyoqjg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangdashe.top/gtdpqehwuf.html

[T48] Perl：正则替换
来源：http://hz.andypj.xyz/gtcyfvkvkg.html

$s =~ s/old/new/g;
来源：http://hz.kuanghao11.cn/gtukzilxkx.html

[T49] Perl：函数
来源：http://hz.jinghuilouyu.cn/gtqoxarrqh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cucudq.cn/gtiaukvsmk.html

[T50] Perl：逐行读文件
来源：http://hz.zhengqikj.top/gtsrvxwawr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtzxvejmvx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangshuangyany.cn/gtuxscfrvk.html

[T51] Scala：Hello World
来源：http://hz.zhixingplan.top/gtnjoyozef.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtxflexypu.html

[T52] Scala：变量
来源：http://hz.hongshengwenyu.top/gtplnmkdto.html

val a = 1;  var b = 2
来源：http://hz.jqgfzy.top/gtetwkilie.html

[T53] Scala：字符串插值
来源：http://hz.pengpengdd.cyou/gtpwjusgxv.html

s"值: $b"
来源：http://hz.zhiwuduotai.top/gtnffibejr.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gtzgtkgnrj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.birdmap.top/gtpmvsmpts.html

[T55] Scala：集合过滤
来源：http://hz.yvedp.cn/gtagwxwkef.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cashguo.top/gtbdcqmssi.html

[T56] Scala：样例类
来源：http://hz.andypj.xyz/gtqlkibchj.html

case class User(name: String, age: Int)
来源：http://hz.ehwqpu.com/gttxwwkkjj.html

[T57] Scala：模式匹配
来源：http://hz.yueranfly.top/gtocnscfee.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pengpengdd.cyou/gtvttobktw.html

[T58] Scala：函数定义
来源：http://hz.hongshengwenyu.top/gtxshijbnp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.andypj.xyz/gtuajpdjmn.html

[T59] Scala：循环
来源：http://hz.ydjk.org.cn/gtlowmneib.html

for (i <- 1 to 10) println(i)
来源：http://hz.hongshengwenyu.top/gthfuqlses.html

[T60] Scala：折叠
来源：http://hz.zhongyouzk.top/gtykjanlqa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.meibo888.top/gtjjrhogzm.html

================================================================================
来源：http://hz.hammf.cn/gtrvcnopaq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gtqfzubudr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtlqrrzeyq.html

[U01] Py：创建虚拟环境
来源：http://hz.jiagoushi.top/gturzcpcpz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gtmxtyrpjc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daria6918.cn/gtpzmkeaoi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aizwys.cn/gtuwlmbeek.html

[U03] Py：加载 .env 配置
来源：http://hz.sweek.top/gtsapfxoqh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tanke756.top/gtltkfdgkc.html

[U04] Py：变量调试打印
来源：http://hz.ybcxt.top/gthalldumo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yongpay.top/gtjkfwoswb.html

[U05] Py：列表去重且保序
来源：http://hz.gogol.net.cn/gtmxkaxrff.html

list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gtdtmvhsaq.html

[U06] Py：合并两个字典
来源：http://hz.jqgfzy.top/gtlwrvfyui.html

{**a, **b}
来源：http://hz.52xcode.cn/gtmszceyas.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtfikqcftm.html

{v: k for k, v in d.items()}
来源：http://hz.cashguo.top/gturskruwr.html

[U08] Py：展平二维列表
来源：http://hz.xuanzx.com/gtilbtepbz.html

[y for x in nested for y in x]
来源：http://hz.cucudq.cn/gtpbxwogqc.html

[U09] Py：字典取最大值的键
来源：http://hz.daria6918.cn/gtobrkhtng.html

max(d, key=d.get)
来源：http://hz.zhijiandao.cn/gtwhuwiuiz.html

[U10] Py：按值排序字典
来源：http://hz.dianchejie.cn/gtdgsgnist.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hammf.cn/gtiqrwqpnx.html

[U11] Py：生成器表达式
来源：http://hz.hysaishi.cn/gtevjnpnvl.html

(x * 2 for x in arr)
来源：http://hz.jlsjyb.cn/gtvvaozimh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gaohongyu789.top/gtffmaomsh.html

Counter(arr).most_common(3)
来源：http://hz.sweek.top/gtwmlngrco.html


<!-- 参考信息 -->