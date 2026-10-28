代发 wailian999

openssl rand -hex 16
来源：http://hz.zhengqikj.top/gtoadnjpwi.html

[R68] 计算文件校验值
来源：http://hz.tianlin.xyz/gtssdawzlj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guowangkeji.top/gtdcmqkega.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtapxuhwcd.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtehuxbhgi.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtwobridmf.html

date +%s;  date -d @1700000000
来源：http://hz.jlsjyb.cn/gtppkbfjfe.html

[R71] 日期格式化
来源：http://hz.xylfe.cn/gtvmbycxet.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zdqjudy.top/gtyxgdnryw.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gtdnpdbhyz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.52xcode.cn/gtuisbxrgx.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtsnotyycn.html

split -l 1000 big.log part_
来源：http://hz.cucudq.cn/gtibjztmuw.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gtarltwdmc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtaocrqmlz.html

[R75] 导出环境变量
来源：http://hz.guannengcc.top/gtdzzvdnwo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.feifeiyinyue.top/gtbosrrete.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtxxftvvvs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtnssyvznp.html

[R77] 读取用户输入
来源：http://hz.jinqigfzy.top/gthgnemdqk.html

read -rp "请输入: " ans
来源：http://hz.andypj.xyz/gturmnwwla.html

[R78] 交互式菜单
来源：http://hz.aibaodan.cn/gtonknkdwy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.meibo888.top/gtpihaqfon.html

[R79] 解析命令行选项
来源：http://hz.ehwqpu.com/gtcgkhzbrx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydzc1.top/gtmabicjsn.html

[R80] 查看脚本执行耗时
来源：http://hz.ehwqpu.com/gtzsubirvb.html

time ./run.sh
来源：http://hz.shanyushiyangkeji.top/gttaeuvvoi.html

================================================================================
来源：http://hz.hywenlv.cn/gtozowobyv.html

S. C / C++ 专题
来源：http://hz.yuanzhike.top/gtcgassufb.html

================================================================================
来源：http://hz.cqqwz.cn/gtqdglgbfe.html

[S01] C：Hello World
来源：http://hz.xylfe.cn/gtvstrgzpo.html

#include <stdio.h>
来源：http://hz.yvedp.cn/gthzunfvrr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tian-w.cn/gtgvmhrcsj.html

[S02] C：变量与格式化输出
来源：http://hz.zhiwuduotai.top/gtjrvdcpkr.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtxtvldgeq.html

[S03] C：读入整数
来源：http://hz.tianlin.xyz/gtqllarrnz.html

int x; scanf("%d", &x);
来源：http://hz.yueranfly.top/gtssvuurrd.html

[S04] C：字符串复制
来源：http://hz.zhaomingkeji.xyz/gtajepnupx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydjk.org.cn/gtddzbxywr.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtvazhjbfr.html

strlen(s)
来源：http://hz.hnxiangtu.top/gtteahusnz.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtgvinlnqx.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gtzuznorwd.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gttkjdzpzl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtiqbebcyo.html

[S08] C：动态内存分配与释放
来源：http://hz.meibo888.top/gtcqhfbyym.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.smart0.xyz/gtchcqdgvr.html

[S09] C：结构体定义与初始化
来源：http://hz.yongpay.top/gthcmlzobo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nwbrower.top/gtvkrbnxpm.html

[S10] C：指针与解引用
来源：http://hz.yj20258.top/gtuohgugbb.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258.top/gtowixxngd.html

[S11] C：逐行读文件
来源：http://hz.fengsongda.top/gtudsmropl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxuanxn.top/gtcmfcbitu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtacjbirlj.html

fclose(f);
来源：http://hz.redwolf501.top/gtbrpywaun.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gtxdkiazba.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guowangkeji.top/gtyhmmrwnk.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtbbvcnhdv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hammf.cn/gtqoeuwnrx.html

[S14] C：枚举
来源：http://hz.iojbl.cn/gtekradqzl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gteqixstom.html

[S15] C：类型转换
来源：http://hz.nwbrower.top/gtiilutydv.html

(double) a / b
来源：http://hz.ppjwa.cn/gtbuctuziq.html

[S16] C：位操作置位
来源：http://hz.smart0.xyz/gtttuxcybk.html

x |= (1 << 3);
来源：http://hz.cheryme.top/gtytwqgama.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtbuibswoh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yangfankeji.com/gtwyoytjik.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gtmhxccuaz.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangtech.top/gtbopbjtyc.html

[S19] C：快速排序
来源：http://hz.mhx1999.top/gtzvqibsbh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtjtdxjvps.html

[S20] C：二分查找
来源：http://hz.shzxlz.cn/gtowlrtvzw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtbxeoxors.html

[S21] C：字符类别判断
来源：http://hz.feifeiyinyue.top/gtafhdpkra.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenlongwang.top/gtnzpboqft.html

[S22] C：字符串转数字
来源：http://hz.52xcode.cn/gtdzkwtpav.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dashuyun.cn/gtudhwjmcy.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gteunswggk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gtcdzlulyd.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtbekbznmu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fzhhl.top/gtbltximld.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtcntdtwbg.html

memcpy(dst, src, n);
来源：http://hz.hfpthk.cn/gtsfslgzgk.html

[S26] C：内存清零
来源：http://hz.iojbl.cn/gtusnfwvix.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtbimkqlpe.html

[S27] C：定义常量
来源：http://hz.xuetiantiany.cn/gtcbsldzhz.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtmtbiixvl.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtizesbcun.html

static int counter = 0;
来源：http://hz.ybcxt.top/gtoqtetnnt.html

[S29] C：变参函数
来源：http://hz.aizwys.cn/gtcmhbsfjr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ppjwa.cn/gtqetqsxjx.html

[S30] C：头文件保护
来源：http://hz.bjfxy.top/gtarfxxsdc.html

#ifndef X_H
来源：http://hz.sweek.top/gtoablcqwx.html

#define X_H
来源：http://hz.tanke756.top/gtwgrgflof.html

#endif
来源：http://hz.hongshengwenyu.top/gtburrsexh.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtdlksvlim.html

#include <iostream>
来源：http://hz.nanxuanxn.top/gtlrcqinjh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtuligfxlz.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gtirpkpgtf.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtjtokeawy.html

[S33] C++：vector 增删
来源：http://hz.zhoulong.xyz/gtoqejjhkl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydzc1.top/gtbfsvavgk.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtqsfuqplx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hywenlv.cn/gtmeyipmkl.html

[S35] C++：map
来源：http://hz.hammf.cn/gtakcnwkbt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtncfizzcc.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtofpoeait.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtqfzivluh.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtiylljvfv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258.top/gtshgsxfqp.html

[S38] C++：排序
来源：http://hz.quarkkingdee.top/gthbqvabzg.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtmqydkuaw.html

[S39] C++：自定义比较器排序
来源：http://hz.chenjidiqi.icu/gtjbcnirul.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gttjagdegb.html

[S40] C++：查找元素
来源：http://hz.yj202588.top/gtyxhraiit.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.meibo888.top/gtfhxcdeim.html

[S41] C++：类与构造函数
来源：http://hz.tian-w.cn/gtjudfvtyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gtlyqswhwf.html

[S42] C++：继承与虚函数
来源：http://hz.cucudq.cn/gtftfsvsdz.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhiwuduotai.top/gtjcfcidsi.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gtbvefutjs.html

auto p = std::make_unique<int>(5);
来源：http://hz.sweek.top/gtkybcsuqy.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtlozqzocy.html

void inc(int &x) { ++x; }
来源：http://hz.xinyue.icu/gtwtexcmxm.html

[S45] C++：lambda
来源：http://hz.zhixingplan.top/gtbedpglfj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenjidiqi.icu/gtueoirkez.html

[S46] C++：函数模板
来源：http://hz.tian-w.cn/gttyjqxbtq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtdnozwbqj.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gtcvxdheyb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sysykeji.top/gtuwlzfaaw.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gtsqecoejw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yueranfly.top/gtwzhbowyh.html

while (std::getline(in, line)) { }
来源：http://hz.sysykeji.top/gtpugqbvrx.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gtxyvkijir.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtllivmgjc.html

[S50] C++：格式化数字
来源：http://hz.hnqzz.top/gtsfbprkgc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtikadvlbf.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtzgwdnvdf.html

static_cast<double>(a) / b
来源：http://hz.jinyuanbaomall.cn/gtalsnoerz.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gthwtryjme.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtyvweakqy.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtpezbdjwy.html

std::vector<int> w = std::move(v);
来源：http://hz.yj202588.top/gtltnwfexm.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangkeji.top/gtdyfthjwt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.316326.xyz/gtexfemtqj.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gthrvuiqav.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fengsongda.top/gtpfpauhlh.html

[S56] C++：optional
来源：http://hz.shanyushiyangtech.top/gtuwbwuaiq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinqigufen.top/gtpsuoujlh.html

[S57] C++：编译期常量
来源：http://hz.shzxlz.cn/gtdzwjwgnq.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gtukcxsmru.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gtnfwvinlw.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuanzx.com/gtntjjecst.html

[S59] C++：静态断言
来源：http://hz.aibaodan.cn/gtvxlxqgwp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gthwxmhdfh.html

[S60] C++：遍历并删除元素
来源：http://hz.chenzaomai.com/gtifurttjj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.birdmap.top/gtvpdaambq.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthhhnncbc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtjvbippbu.html

================================================================================
来源：http://hz.gzhubu.top/gtwifmcveg.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gthwpthjyy.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtrjgafyvs.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gtspkmcslj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigufen.top/gttptnsxnn.html

[T03] Kotlin：字符串模板
来源：http://hz.gotoacloud.top/gtinawzdii.html

"值: $b"
来源：http://hz.0kj1m.cn/gtfhhojvwq.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtcxmrrcbd.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtekcjnnld.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtfjcyxmhj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gtjvniycdm.html

[T06] Kotlin：集合映射
来源：http://hz.redwolf501.top/gtgddsefzz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtxtbyhvwp.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangtech.top/gtvrokoccf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sufxvd.cn/gtnngdgeoi.html

[T08] Kotlin：数据类
来源：http://hz.yonumen.top/gtygyxjksa.html

data class User(val name: String, val age: Int)
来源：http://hz.pycfn.com/gtxyukhuda.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtntyaoysi.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtshhlpqmi.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangtech.top/gttvuewvod.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.iojbl.cn/gtsbarqoiu.html

[T11] Kotlin：协程
来源：http://hz.ivvv.top/gtbleihmbh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ivvv.top/gtkueogrsa.html

[T12] Kotlin：解构声明
来源：http://hz.jqgfzy.top/gtovrwxlnu.html

val (a, b) = Pair(1, 2)
来源：http://hz.cucudq.cn/gtlqfljxgx.html

[T13] Kotlin：只读 Map
来源：http://hz.ywan-chungtsiang.top/gtkpbxkvgy.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtpvwmduwl.html

[T14] Kotlin：循环
来源：http://hz.nanxinkj.top/gtscwzhppu.html

for (i in 1..10) println(i)
来源：http://hz.0kj1m.cn/gtgaifidcx.html

[T15] Kotlin：接口
来源：http://hz.shzxlz.cn/gtbwevoetl.html

interface Shape { fun area(): Double }
来源：http://hz.zycfv.cn/gtvysfibhl.html

[T16] Swift：Hello World
来源：http://hz.sxryk.cn/gtaxgfhsix.html

print("Hello")
来源：http://hz.52xcode.cn/gtqjfnrfsj.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtitogpedn.html

var a = 1;  let b = 2
来源：http://hz.gogol.net.cn/gtqwzphsvp.html

[T18] Swift：字符串插值
来源：http://hz.zhongyouzk.top/gtvrapvixg.html

"值: \(b)"
来源：http://hz.gogol.net.cn/gtumvhoqyj.html

[T19] Swift：可选绑定
来源：http://hz.yangfankeji.com/gtdkyewkgo.html

if let n = opt { print(n) }
来源：http://hz.jinyuanbaomall.cn/gtjvcmhinl.html

[T20] Swift：数组操作
来源：http://hz.sweek.top/gtxddfeoga.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.kuanghao11.cn/gtdsdjpipe.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gttwbsyklb.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtztjsswdc.html

[T22] Swift：字典
来源：http://hz.zhongyouzk.top/gtmzgxwmum.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jyoumei.cn/gtawyjeljb.html

[T23] Swift：函数
来源：http://hz.jlsjyb.cn/gtanvzjafo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gtcdgeyfgc.html

[T24] Swift：闭包
来源：http://hz.jqgufenzy.top/gthjmpqgmp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.wangshuangyany.cn/gtetyzpdsk.html

[T25] Swift：结构体
来源：http://hz.feifeiyinyue.top/gtfslqceou.html

struct P { var x: Int }
来源：http://hz.jiagoushi.top/gtibrrsxet.html

[T26] Swift：类与重写
来源：http://hz.jianghu66.top/gtifbmxkeo.html

class A: Base { override func f() {} }
来源：http://hz.jyoumei.cn/gtfcwdysjn.html

[T27] Swift：错误处理
来源：http://hz.tian-w.cn/gtuqqfdfsp.html

do { try f() } catch { print(error) }
来源：http://hz.chenjidiqi.icu/gthfqgmodp.html

[T28] Swift：枚举
来源：http://hz.guannengcc.top/gtfdtugkme.html

enum Color { case red, green }
来源：http://hz.xuetiantiany.cn/gtugqefjwa.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtecekmeab.html

guard let x = opt else { return }
来源：http://hz.jinghuilouyu.cn/gtktalanni.html

[T30] Swift：协议
来源：http://hz.tianlin.xyz/gtuotmpwgx.html

protocol Shape { func area() -> Double }
来源：http://hz.quarkkingdee.top/gtvqcjzgvk.html

[T31] Lua：Hello World
来源：http://hz.yanxiufei.cn/gtwwhibzvn.html

print("Hello")
来源：http://hz.jianghu66.top/gtolakbqak.html

[T32] Lua：局部变量
来源：http://hz.gaohongyu789.top/gtrwtfrxaz.html

local a = 1
来源：http://hz.aizwys.cn/gtjxalqmnz.html

[T33] Lua：表（数组）
来源：http://hz.9152youxi.cn/gtzszjkefe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.52xcode.cn/gtyhgpfdao.html

[T34] Lua：遍历表
来源：http://hz.zhiwuduotai.top/gtkbsxkuqh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jyoumei.cn/gtcgfygjqy.html

[T35] Lua：字典表
来源：http://hz.guannengcc.top/gthpkigirc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtunrihite.html

[T36] Lua：函数
来源：http://hz.gotoacloud.top/gtogpbjiqj.html

function add(a, b) return a + b end
来源：http://hz.tanke756.top/gtswqfnyzi.html

[T37] Lua：字符串拼接
来源：http://hz.yangfankeji.com/gtyjwgyait.html

"a" .. "b"
来源：http://hz.zycfv.cn/gtwyvjmvkd.html

[T38] Lua：条件
来源：http://hz.nwbrower.top/gttzuhgdld.html

if x > 0 then print("正") end
来源：http://hz.wangshuangyany.cn/gtjdskwmrg.html

[T39] Lua：模式匹配
来源：http://hz.hywenlv.cn/gtplctkthp.html

string.find(s, "%d+")
来源：http://hz.gogol.net.cn/gttqnohblv.html

[T40] Lua：元表
来源：http://hz.jinqigfzy.top/gtspghiswj.html

setmetatable({}, { __index = base })
来源：http://hz.hywenlv.cn/gtrepfncqd.html

[T41] Perl：Hello World
来源：http://hz.jinqigfzy.top/gtfhppswlv.html

print "Hello\n";
来源：http://hz.tanke756.top/gtlzteojqz.html

[T42] Perl：变量类型
来源：http://hz.sxryk.cn/gtjqbpdyoo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aibaodan.cn/gtmeympuup.html

[T43] Perl：字符串插值
来源：http://hz.hongshengwenyu.top/gtjreebyrc.html

"值: $a"
来源：http://hz.chenlongwang.top/gtcambhmob.html

[T44] Perl：条件
来源：http://hz.aizwys.cn/gtzyunqkdp.html

if ($a > 0) { print "正"; }
来源：http://hz.dashuyun.cn/gtrwslwadj.html

[T45] Perl：数组遍历
来源：http://hz.hfpthk.cn/gtvubnxpqs.html

for my $x (@arr) { print $x; }
来源：http://hz.yuxming.cn/gtxdtodamp.html

[T46] Perl：哈希操作
来源：http://hz.ywan-chungtsiang.top/gtvqwawsmj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.daxiang520.top/gtmuuvbeps.html

[T47] Perl：正则捕获
来源：http://hz.nwbrower.top/gtnwbeowts.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hywenlv.cn/gtvaatnono.html

[T48] Perl：正则替换
来源：http://hz.shuidangran.top/gtvqhufbss.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtymhtfuqn.html

[T49] Perl：函数
来源：http://hz.zycfv.cn/gtpaglfntw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tian-w.cn/gtdbibteox.html

[T50] Perl：逐行读文件
来源：http://hz.zhoulong.xyz/gtjwjmagek.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dashuyun.cn/gttvutdkns.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yonumen.top/gtkbenubhq.html

[T51] Scala：Hello World
来源：http://hz.wangdashe.top/gtbvokisws.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtgbidmfbr.html

[T52] Scala：变量
来源：http://hz.zhoulong.xyz/gtafbalpqr.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtxxggjlwz.html

[T53] Scala：字符串插值
来源：http://hz.fengsongda.top/gtwutfrjya.html

s"值: $b"
来源：http://hz.svipenyu.cn/gthlazkpmw.html

[T54] Scala：集合映射
来源：http://hz.yj20258888.top/gtbhjwqxjr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenzaomai.com/gtxhatjqtn.html

[T55] Scala：集合过滤
来源：http://hz.ehwqpu.com/gtfxcesqcl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xuanzx.com/gtrumeqtxn.html

[T56] Scala：样例类
来源：http://hz.gotoacloud.top/gtafdezkjb.html

case class User(name: String, age: Int)
来源：http://hz.ppjwa.cn/gtnvlytqqk.html

[T57] Scala：模式匹配
来源：http://hz.chenjidiqi.icu/gtbaqjmlnt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ivvv.top/gtbtigbhtf.html

[T58] Scala：函数定义
来源：http://hz.birdmap.top/gtupybwmxh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinqigfzy.top/gtkkwoszvr.html

[T59] Scala：循环
来源：http://hz.nanxinkj.top/gtffluksgj.html

for (i <- 1 to 10) println(i)
来源：http://hz.birdmap.top/gtokkwymud.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gtphnxzrhk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhengqikj.top/gtpcrmrcpd.html

================================================================================
来源：http://hz.yj20258.top/gtvrazwkjr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtpeyqzdhh.html

================================================================================
来源：http://hz.kuanghao11.cn/gtsrcdjflx.html

[U01] Py：创建虚拟环境
来源：http://hz.ydjk.org.cn/gtdjlzasem.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tianlin.xyz/gtcwftgcsg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangtech.top/gtgtlexitj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tianlin.xyz/gtcsucwjzn.html

[U03] Py：加载 .env 配置
来源：http://hz.chenlongwang.top/gtgbdisvui.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yangfankeji.com/gtokxigxfy.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gthoowrqth.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258.top/gtxbcxxpsx.html

[U05] Py：列表去重且保序
来源：http://hz.cheryme.top/gtxiuaoqyy.html

list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtwqynkfow.html

[U06] Py：合并两个字典
来源：http://hz.feifeiyinyue.top/gtqgfvarvf.html

{**a, **b}
来源：http://hz.jinghuilouyu.cn/gtqgeiwtuj.html

[U07] Py：反转字典键值
来源：http://hz.hywenlv.cn/gtkprwsmff.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtjnfkljjp.html

[U08] Py：展平二维列表
来源：http://hz.wangshuangyany.cn/gtgcrdyacu.html

[y for x in nested for y in x]
来源：http://hz.hnxiangtu.top/gtqngmlhvf.html


<!-- 参考信息 -->