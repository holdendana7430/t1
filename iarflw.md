代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangshuangyany.cn/gtzrumdehc.html

[R76] 使用临时文件
来源：http://hz.redwolf501.top/gtshvwxvga.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtceuzcxde.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtvsxqgvpq.html

read -rp "请输入: " ans
来源：http://hz.nanxuanxn.top/gttbpelhzu.html

[R78] 交互式菜单
来源：http://hz.cucudq.cn/gtysjvtmcy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.snrcjt.cn/gtdbmvgnlb.html

[R79] 解析命令行选项
来源：http://hz.hongshengwenyu.top/gtaurhgwaq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhiwuduotai.top/gtlmhizqtt.html

[R80] 查看脚本执行耗时
来源：http://hz.0kj1m.cn/gtlqllfsyw.html

time ./run.sh
来源：http://hz.feifeiyinyue.top/gtjddvpbny.html

================================================================================
来源：http://hz.zhijiandao.cn/gttiiimrgx.html

S. C / C++ 专题
来源：http://hz.zycfv.cn/gtbdpizcxm.html

================================================================================
来源：http://hz.jlsjyb.cn/gthcutuped.html

[S01] C：Hello World
来源：http://hz.ivvv.top/gtgftzbcdb.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtcgwbsloi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxinkj.top/gtnulzveec.html

[S02] C：变量与格式化输出
来源：http://hz.xziqi.cn/gtovgiouax.html

int a = 10; printf("%d\n", a);
来源：http://hz.0kj1m.cn/gtbqrygxsx.html

[S03] C：读入整数
来源：http://hz.jiagoushi.top/gtzztahrld.html

int x; scanf("%d", &x);
来源：http://hz.feifeiyinyue.top/gtgekvcpsq.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtxjqswewv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xziqi.cn/gtubmwerkz.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtaltzvywi.html

strlen(s)
来源：http://hz.zhijiandao.cn/gtfrpdhykt.html

[S06] C：字符串比较
来源：http://hz.dianchejie.cn/gtkmonwcqw.html

strcmp(a, b) == 0
来源：http://hz.chenlongwang.top/gtbkdwiyka.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtoqbputni.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gtzibcwjhb.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtjfazqubk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtcxqawktq.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtjrrhbkxl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gogol.net.cn/gtbbqiwasc.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtcqwrgfev.html

int *p = &a;  *p = 5;
来源：http://hz.zhaomingkeji.xyz/gtgvmlzfgx.html

[S11] C：逐行读文件
来源：http://hz.zhongyouzk.top/gtmjxbwget.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sufxvd.cn/gtnkjhktuc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gtsgjifgdl.html

fclose(f);
来源：http://hz.guowangkeji.top/gtxxzspkbs.html

[S12] C：写文件
来源：http://hz.bjfxy.top/gtsnqxijfo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinghuilouyu.cn/gtkflhbpnk.html

[S13] C：宏定义
来源：http://hz.cucudq.cn/gtjzbvlqbr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtlomqvllc.html

[S14] C：枚举
来源：http://hz.pycfn.com/gtjmzclrdz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenzaomai.com/gtmjbbgljw.html

[S15] C：类型转换
来源：http://hz.ppjwa.cn/gttemvrxgp.html

(double) a / b
来源：http://hz.mhx1999.top/gtejjnbcrl.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtemlmirsz.html

x |= (1 << 3);
来源：http://hz.jinqigfzy.top/gthtjhnykd.html

[S17] C：安全拼接字符串
来源：http://hz.yongpay.top/gteabmlxki.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtfnjifvah.html

[S18] C：命令行参数
来源：http://hz.hammf.cn/gtqlciopen.html

int main(int argc, char **argv)
来源：http://hz.vqdsnc.cn/gtjumvzceh.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtqrwbuipd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtdihupuog.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtjzzftuzo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtyfyxbglp.html

[S21] C：字符类别判断
来源：http://hz.zhoulong.xyz/gtliygesrl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtyuvrmyhq.html

[S22] C：字符串转数字
来源：http://hz.shzxlz.cn/gtzfrypyyp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gteeustabn.html

[S23] C：随机数
来源：http://hz.guannengcc.top/gtsirdnfrr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tian-w.cn/gtjtyrkmkm.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gtflrdckdh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xylfe.cn/gtnuwlpkwy.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gtzfkyiesu.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gtjwbfdilg.html

[S26] C：内存清零
来源：http://hz.sweek.top/gtvhaieout.html

memset(a, 0, sizeof a);
来源：http://hz.sufxvd.cn/gtokbncmag.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtqzgrbiys.html

const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtsmucqnyw.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtlyhznwzn.html

static int counter = 0;
来源：http://hz.jinqigfzy.top/gtksniztcp.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gtqeitogxc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtdtthctrs.html

[S30] C：头文件保护
来源：http://hz.xuanzx.com/gtbyfmylrd.html

#ifndef X_H
来源：http://hz.wangdashe.top/gtvqpejsny.html

#define X_H
来源：http://hz.xinyue.icu/gtxvgwvaby.html

#endif
来源：http://hz.andypj.xyz/gtlknjznnk.html

[S31] C++：Hello World
来源：http://hz.tianlin.xyz/gtvjyhfjrl.html

#include <iostream>
来源：http://hz.0kj1m.cn/gtlyvtqreg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtftvunccf.html

[S32] C++：字符串
来源：http://hz.shangyingyoupin.top/gtxkxvqerc.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gteizhtege.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtbjxvupst.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aizwys.cn/gtbavonupq.html

[S34] C++：遍历 vector
来源：http://hz.chenzaomai.com/gtzszlbugx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtotbxqdll.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtlrpfgtcb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtbrdxgiib.html

[S36] C++：unordered_map
来源：http://hz.aibaodan.cn/gtzltwuume.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtzabjevbu.html

[S37] C++：set
来源：http://hz.aizwys.cn/gtnamtowyu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zycfv.cn/gtnpjbwyft.html

[S38] C++：排序
来源：http://hz.tian-w.cn/gtosnsaaxi.html

std::sort(v.begin(), v.end());
来源：http://hz.jianghu66.top/gthfwttths.html

[S39] C++：自定义比较器排序
来源：http://hz.chenzaomai.com/gtrrmsvwru.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtawwulhng.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtekrnnzso.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtxyolgxll.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtpzlxevke.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtiylktuma.html

[S42] C++：继承与虚函数
来源：http://hz.wangdashe.top/gtwcmhamme.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinghuilouyu.cn/gtkzncrqyr.html

[S43] C++：智能指针
来源：http://hz.snrcjt.cn/gtbpwnwmlv.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenjidiqi.icu/gtebsabrlb.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtoulelcpj.html

void inc(int &x) { ++x; }
来源：http://hz.xuetiantiany.cn/gttpbpbpqx.html

[S45] C++：lambda
来源：http://hz.snrcjt.cn/gtdlrezkli.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.birdmap.top/gtewgxwmrf.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gtmpykelgu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtefeduuqh.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtbhzxafdf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gtejtpvqvz.html

[S48] C++：逐行读文件
来源：http://hz.ehwqpu.com/gtcqikzzcu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuxming.cn/gtbdhwyouq.html

while (std::getline(in, line)) { }
来源：http://hz.cucudq.cn/gtydpodewi.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtfvidslfy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gtlmqlkiup.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtgulxljwe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtxcopdven.html

[S51] C++：显式类型转换
来源：http://hz.c1oappe.top/gtezaehtmh.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtdaqmgupk.html

[S52] C++：const 与 noexcept
来源：http://hz.cucudq.cn/gttuajkdfl.html

int size() const noexcept { return n_; }
来源：http://hz.zhongyouzk.top/gtfpegawnn.html

[S53] C++：移动语义
来源：http://hz.jyoumei.cn/gtgzmezwjc.html

std::vector<int> w = std::move(v);
来源：http://hz.jianghu66.top/gtbatkrmox.html

[S54] C++：异常处理
来源：http://hz.zhengqikj.top/gtovymsybi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.9152youxi.cn/gtqtjflzth.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtwkwdetqt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgfzy.top/gtmtxjcbay.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtvzrdqjon.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtnwwasddd.html

[S57] C++：编译期常量
来源：http://hz.wangshuangyany.cn/gtewuzpldm.html

constexpr int N = 10;
来源：http://hz.hysaishi.cn/gthaaaprak.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gttjdgenfj.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtyiaglymq.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gtaemggwml.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gotoacloud.top/gtbrmfrrio.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gthwabtvet.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtrzoscepi.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjgjiouff.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtvylnrevh.html

================================================================================
来源：http://hz.yj202588.top/gtjajexjkn.html

[T01] Kotlin：Hello World
来源：http://hz.iojbl.cn/gtzrhoctzc.html

println("Hello")
来源：http://hz.jianghu66.top/gtdoizvycy.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtwuxjflrd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yvedp.cn/gtnhqelzpe.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtamyymlyn.html

"值: $b"
来源：http://hz.jinghuilouyu.cn/gtislqhnat.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gteieqghxi.html

val n: String? = null;  n?.length
来源：http://hz.cashguo.top/gtqbyogunb.html

[T05] Kotlin：when 表达式
来源：http://hz.shangyingyoupin.top/gtyvgqgjii.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.0kj1m.cn/gtqgnqshgs.html

[T06] Kotlin：集合映射
来源：http://hz.yanxiufei.cn/gtderqbfqq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtcprpidvp.html

[T07] Kotlin：集合过滤
来源：http://hz.yj202588.top/gtdsifgual.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtqodmutch.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gthupbrjpu.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gtvnaljdwy.html

[T09] Kotlin：扩展函数
来源：http://hz.gotoacloud.top/gtexjsqqpd.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtqbptjmoq.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtwxmxrfur.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tanke756.top/gtwpawawqz.html

[T11] Kotlin：协程
来源：http://hz.yangfankeji.com/gtremwlirv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sufxvd.cn/gtkvieqmjx.html

[T12] Kotlin：解构声明
来源：http://hz.zhongyouzk.top/gtqlibdirm.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtvkjegdkb.html

[T13] Kotlin：只读 Map
来源：http://hz.bjfxy.top/gtcvnddpxa.html

val m = mapOf("a" to 1)
来源：http://hz.dashuyun.cn/gtxibbwzue.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtkkuopwcf.html

for (i in 1..10) println(i)
来源：http://hz.chenlongwang.top/gtoowrcwpf.html

[T15] Kotlin：接口
来源：http://hz.yanxiufei.cn/gtqxaxllmq.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtjvsmsnvv.html

[T16] Swift：Hello World
来源：http://hz.zdqjudy.top/gtucihfzum.html

print("Hello")
来源：http://hz.xziqi.cn/gtrrznheeu.html

[T17] Swift：变量与常量
来源：http://hz.hnqzz.top/gtxehvyezr.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtelfnmbqh.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtszaylois.html

"值: \(b)"
来源：http://hz.feifeiyinyue.top/gtizhyqyca.html

[T19] Swift：可选绑定
来源：http://hz.zhongyouzk.top/gtvlhmndlt.html

if let n = opt { print(n) }
来源：http://hz.sxryk.cn/gtavbdnojk.html

[T20] Swift：数组操作
来源：http://hz.hywenlv.cn/gtqmlborub.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gtdssnhvua.html

[T21] Swift：遍历
来源：http://hz.mhx1999.top/gtgcgrdsiz.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtcimfxeud.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtthbdpeuz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.andypj.xyz/gtfpkuqmzv.html

[T23] Swift：函数
来源：http://hz.cqqwz.cn/gttahvyxex.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuanzx.com/gtahtjknzo.html

[T24] Swift：闭包
来源：http://hz.yongpay.top/gttzeqhwqg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigufen.top/gtqczqxwdx.html

[T25] Swift：结构体
来源：http://hz.sysykeji.top/gtzbfzviri.html

struct P { var x: Int }
来源：http://hz.yuxming.cn/gtjyplisqw.html

[T26] Swift：类与重写
来源：http://hz.c1oappe.top/gtqszcectt.html

class A: Base { override func f() {} }
来源：http://hz.sufxvd.cn/gtbmnkuwsz.html

[T27] Swift：错误处理
来源：http://hz.xinyue.icu/gtpoumgxyi.html

do { try f() } catch { print(error) }
来源：http://hz.sufxvd.cn/gtnmdpsdjf.html

[T28] Swift：枚举
来源：http://hz.shangyingyoupin.top/gtdjkwcegg.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gtavzollcm.html

[T29] Swift：guard 提前返回
来源：http://hz.gogol.net.cn/gtsibccfle.html

guard let x = opt else { return }
来源：http://hz.gogol.net.cn/gthdezmvgq.html

[T30] Swift：协议
来源：http://hz.zdqjudy.top/gtikevuthd.html

protocol Shape { func area() -> Double }
来源：http://hz.zdqjudy.top/gtcbxcoawb.html

[T31] Lua：Hello World
来源：http://hz.52xcode.cn/gtfnitmebc.html

print("Hello")
来源：http://hz.jiagoushi.top/gtbevgposn.html

[T32] Lua：局部变量
来源：http://hz.zhiwuduotai.top/gtnmqbrqoh.html

local a = 1
来源：http://hz.tian-w.cn/gtpvekzfpt.html

[T33] Lua：表（数组）
来源：http://hz.sufxvd.cn/gtooilbzjx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daria6918.cn/gtjakrpzyy.html

[T34] Lua：遍历表
来源：http://hz.meibo888.top/gtxystqnwc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zycfv.cn/gtrdtzvzbk.html

[T35] Lua：字典表
来源：http://hz.ydzc1.top/gttzpdwqbg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hfpthk.cn/gtkuebftvl.html

[T36] Lua：函数
来源：http://hz.sufxvd.cn/gtbsdijybq.html

function add(a, b) return a + b end
来源：http://hz.hfpthk.cn/gthoezbhdb.html

[T37] Lua：字符串拼接
来源：http://hz.xuanzx.com/gtoduavpya.html

"a" .. "b"
来源：http://hz.yj202588.top/gtxazwtxgs.html

[T38] Lua：条件
来源：http://hz.wangshuangyany.cn/gthsnflxwa.html

if x > 0 then print("正") end
来源：http://hz.nwbrower.top/gtuokijsyn.html

[T39] Lua：模式匹配
来源：http://hz.jlsjyb.cn/gtqbytbjnm.html

string.find(s, "%d+")
来源：http://hz.haohaochexian.top/gtxcjpeeya.html

[T40] Lua：元表
来源：http://hz.andypj.xyz/gtonsegeiw.html

setmetatable({}, { __index = base })
来源：http://hz.ehwqpu.com/gtuvbmftxf.html

[T41] Perl：Hello World
来源：http://hz.9152youxi.cn/gtdtvyckyz.html

print "Hello\n";
来源：http://hz.sweek.top/gtflnljisf.html

[T42] Perl：变量类型
来源：http://hz.zhaomingkeji.xyz/gtfqayduhe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xziqi.cn/gtmpgormwb.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gtirxubwqs.html

"值: $a"
来源：http://hz.jinyuanbaomall.cn/gtgopjclan.html

[T44] Perl：条件
来源：http://hz.dianchejie.cn/gtsrxmuklp.html

if ($a > 0) { print "正"; }
来源：http://hz.zhengqikj.top/gtkviygfdq.html

[T45] Perl：数组遍历
来源：http://hz.yangfankeji.com/gtjbkjikjg.html

for my $x (@arr) { print $x; }
来源：http://hz.ppjwa.cn/gtsazzeowc.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gtxlaibdwa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenzaomai.com/gtxrosizuq.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangkeji.top/gtzujcqenq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydjk.org.cn/gtkftctufi.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtfdrkfbxd.html

$s =~ s/old/new/g;
来源：http://hz.cqqwz.cn/gtvfrfddpt.html

[T49] Perl：函数
来源：http://hz.dianchejie.cn/gtruzwkpda.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yanxiufei.cn/gtbxckxkiv.html

[T50] Perl：逐行读文件
来源：http://hz.jyoumei.cn/gtdtphtxok.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhiwuduotai.top/gtftsvubvb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yangfankeji.com/gtnhcwdoqh.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gtvbjambhk.html

println("Hello")
来源：http://hz.svipenyu.cn/gtgahgsgsc.html

[T52] Scala：变量
来源：http://hz.pengpengdd.cyou/gtysnankjo.html

val a = 1;  var b = 2
来源：http://hz.gaohongyu789.top/gtfyjfaeod.html

[T53] Scala：字符串插值
来源：http://hz.ybcxt.top/gtoswdpmvd.html

s"值: $b"
来源：http://hz.ivvv.top/gtqpxjygix.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtatzhngxu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aizwys.cn/gtrfybypqb.html

[T55] Scala：集合过滤
来源：http://hz.xziqi.cn/gtknnucpoc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.feifeiyinyue.top/gtqhmkcwsm.html

[T56] Scala：样例类
来源：http://hz.yj20258888.top/gtygjpntvg.html

case class User(name: String, age: Int)
来源：http://hz.ywan-chungtsiang.top/gtfknwgqgf.html

[T57] Scala：模式匹配
来源：http://hz.smart0.xyz/gtfeglpkgw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guowangkeji.top/gtsxeqpbzg.html

[T58] Scala：函数定义
来源：http://hz.0kj1m.cn/gtivlbwzuh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xylfe.cn/gtxilcegkh.html

[T59] Scala：循环
来源：http://hz.yj20258888.top/gtofvykvrr.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtjlreiith.html

[T60] Scala：折叠
来源：http://hz.ydjk.org.cn/gtebnqvizm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yangfankeji.com/gtctbqrpqi.html

================================================================================
来源：http://hz.0kj1m.cn/gtgkruraiq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258.top/gtafxdtkia.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwmglgagy.html

[U01] Py：创建虚拟环境
来源：http://hz.andypj.xyz/gtryouyqgr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gtdzdamgpt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxinkj.top/gtphubmpus.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jlsjyb.cn/gtssjghkhf.html

[U03] Py：加载 .env 配置
来源：http://hz.c1oappe.top/gtffxpkipt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yangfankeji.com/gtwvdckiiw.html

[U04] Py：变量调试打印
来源：http://hz.cdnleiting.top/gtgwviwmka.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shanyushiyangtech.top/gtcabwzlkd.html

[U05] Py：列表去重且保序
来源：http://hz.hfpthk.cn/gtlaemydtt.html

list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gtjbxuvclh.html

[U06] Py：合并两个字典
来源：http://hz.yuxming.cn/gtzohumudg.html

{**a, **b}
来源：http://hz.yj20258888.top/gtczzmiohv.html

[U07] Py：反转字典键值
来源：http://hz.birdmap.top/gtltciyuhq.html

{v: k for k, v in d.items()}
来源：http://hz.ydzc1.top/gtxngojtts.html

[U08] Py：展平二维列表
来源：http://hz.ehwqpu.com/gtjnwizdda.html

[y for x in nested for y in x]
来源：http://hz.ywan-chungtsiang.top/gteermivrs.html

[U09] Py：字典取最大值的键
来源：http://hz.tian-w.cn/gtpkpjaswv.html

max(d, key=d.get)
来源：http://hz.xingfuxueyuan.xyz/gtjemswldz.html

[U10] Py：按值排序字典
来源：http://hz.cucudq.cn/gtwdsiapxy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guowangkeji.top/gtqcvbhlnb.html

[U11] Py：生成器表达式
来源：http://hz.guannengcc.top/gtbkjuytti.html

(x * 2 for x in arr)
来源：http://hz.yuanzhike.top/gtanyqjyzi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daria6918.cn/gtcvtjrxjz.html

Counter(arr).most_common(3)
来源：http://hz.sxryk.cn/gtxzvfnxlp.html

[U13] Py：固定长度队列
来源：http://hz.snrcjt.cn/gtzkkwwwdd.html

deque(maxlen=10)
来源：http://hz.ydjk.org.cn/gtuiddiajl.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258888.top/gtoosgeqfc.html

defaultdict(list)
来源：http://hz.fengsongda.top/gttaytodpl.html

[U15] Py：高精度计时
来源：http://hz.bjfxy.top/gtfktatwtk.html

t = time.perf_counter()
来源：http://hz.pycfn.com/gtqezvoyfw.html

[U16] Py：命令行参数解析
来源：http://hz.vqdsnc.cn/gtpcwhzwpv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ydzc1.top/gtsqjpfvqw.html


<!-- 参考信息 -->