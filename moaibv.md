代发 wailian999

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtrevlqzvb.html

[R68] 计算文件校验值
来源：http://hz.dashuyun.cn/gtkrgngyfm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangkeji.top/gtzorqbgqg.html

[R69] 生成随机密码
来源：http://hz.iojbl.cn/gtfubamvnp.html

head -c 16 /dev/urandom | base64
来源：http://hz.ybcxt.top/gtbhtwcqaa.html

[R70] 时间戳与互转
来源：http://hz.shzxlz.cn/gtjzjiwxbc.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gtfpcwnzfm.html

[R71] 日期格式化
来源：http://hz.316326.xyz/gtlqvvihdc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sweek.top/gtufxxzrbs.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gttoqmkiqt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtxsxiuqpe.html

[R73] 分割大日志
来源：http://hz.pycfn.com/gtfvobteks.html

split -l 1000 big.log part_
来源：http://hz.tanke756.top/gtfidzpxsx.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtogcjjubc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dianchejie.cn/gtuoeqortb.html

[R75] 导出环境变量
来源：http://hz.hnqzz.top/gtkviixmpn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sufxvd.cn/gtddrjuiuk.html

[R76] 使用临时文件
来源：http://hz.aizwys.cn/gteclnvmla.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtxexsyrsx.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtrzajsihv.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gttnvlzqad.html

[R78] 交互式菜单
来源：http://hz.ywan-chungtsiang.top/gtgytgpkpe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtofogkhtk.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtnzfyvaej.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jianghu66.top/gtsjazsphp.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigfzy.top/gtxjkkogkb.html

time ./run.sh
来源：http://hz.nwbrower.top/gtgowgcwzs.html

================================================================================
来源：http://hz.fzhhl.top/gtoynmdzqk.html

S. C / C++ 专题
来源：http://hz.snrcjt.cn/gtllocfjhz.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtlnwjpzwq.html

[S01] C：Hello World
来源：http://hz.xuetiantiany.cn/gtyidzwmqq.html

#include <stdio.h>
来源：http://hz.hammf.cn/gtrofikpha.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gtjzvzfawe.html

[S02] C：变量与格式化输出
来源：http://hz.svipenyu.cn/gtlqpqpsyl.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gthgbicxwo.html

[S03] C：读入整数
来源：http://hz.cdnleiting.top/gtogvgxobf.html

int x; scanf("%d", &x);
来源：http://hz.cucudq.cn/gtzesxfpiw.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gtdmljqlbd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gtaxtonklk.html

[S05] C：字符串长度
来源：http://hz.316326.xyz/gturhbthss.html

strlen(s)
来源：http://hz.cucudq.cn/gtxqchjpin.html

[S06] C：字符串比较
来源：http://hz.vqdsnc.cn/gtivhlkqgc.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtpfaprsms.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtfypklgsd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cucudq.cn/gtylkbefuw.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtuwqwfajm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgfzy.top/gtqqwfibqf.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gtllyhgfzi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtqjemkuaw.html

[S10] C：指针与解引用
来源：http://hz.jinyuanbaomall.cn/gtghprkufy.html

int *p = &a;  *p = 5;
来源：http://hz.tianlin.xyz/gtbvurtpkp.html

[S11] C：逐行读文件
来源：http://hz.guowangkeji.top/gttxosycue.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gthduwaazc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guannengcc.top/gtpzbqomyq.html

fclose(f);
来源：http://hz.zycfv.cn/gtzlzjgkah.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gtgtkrayjv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtvjgrxkgv.html

[S13] C：宏定义
来源：http://hz.jinqigfzy.top/gtxzecgiev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtoupqpjyn.html

[S14] C：枚举
来源：http://hz.cdnleiting.top/gtzqrlomgf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtkhgpbnpd.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtcngdtfbe.html

(double) a / b
来源：http://hz.hongshengwenyu.top/gtrddwhiht.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtejyypduv.html

x |= (1 << 3);
来源：http://hz.316326.xyz/gtaubtswpr.html

[S17] C：安全拼接字符串
来源：http://hz.ybcxt.top/gtlnnkhcfw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtlttrlgpf.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gtsdnopzpc.html

int main(int argc, char **argv)
来源：http://hz.zhengqikj.top/gtkjrxcsng.html

[S19] C：快速排序
来源：http://hz.feifeiyinyue.top/gtlbifcuiu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtwzhlnzis.html

[S20] C：二分查找
来源：http://hz.haohaochexian.top/gttfnxvccn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtqiichlno.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gthxlrprnd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenlongwang.top/gtgohfgelg.html

[S22] C：字符串转数字
来源：http://hz.tanke756.top/gteyxkrkth.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sysykeji.top/gttzzwstzd.html

[S23] C：随机数
来源：http://hz.jyoumei.cn/gthpemwurq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgfzy.top/gtsqmvqvrb.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtslrdfjak.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guowangkeji.top/gtvlydydrp.html

[S25] C：内存拷贝
来源：http://hz.nwbrower.top/gtndyrwqku.html

memcpy(dst, src, n);
来源：http://hz.fzhhl.top/gtauefwhgm.html

[S26] C：内存清零
来源：http://hz.gzhubu.top/gtpsbntisx.html

memset(a, 0, sizeof a);
来源：http://hz.wangshuangyany.cn/gttowtfbmc.html

[S27] C：定义常量
来源：http://hz.cucudq.cn/gtmuwtauyi.html

const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtbcueuvnv.html

[S28] C：静态变量
来源：http://hz.ydjk.org.cn/gtcyoxlujy.html

static int counter = 0;
来源：http://hz.gogol.net.cn/gtpxjxptju.html

[S29] C：变参函数
来源：http://hz.gotoacloud.top/gttxicgmxz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtuihtascn.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtfftxsfhk.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtagkwuorr.html

#define X_H
来源：http://hz.hfpthk.cn/gtkvabfbne.html

#endif
来源：http://hz.daxiang520.top/gtjspfwwyz.html

[S31] C++：Hello World
来源：http://hz.aizwys.cn/gtogydpyfd.html

#include <iostream>
来源：http://hz.dashuyun.cn/gtaxyqyxpe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xylfe.cn/gttatnytql.html

[S32] C++：字符串
来源：http://hz.shanyushiyangkeji.top/gtjqbhbkij.html

std::string s = "hi";  s += "!";
来源：http://hz.zhiwuduotai.top/gtjwchkvbl.html

[S33] C++：vector 增删
来源：http://hz.birdmap.top/gttlmvoxns.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shzxlz.cn/gtjbqwptig.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtyraertzg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtobgwgalf.html

[S35] C++：map
来源：http://hz.yj20258888.top/gtvwkyiyta.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtdwlrshfk.html

[S36] C++：unordered_map
来源：http://hz.hongshengwenyu.top/gtkyyrgyag.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtwtkklwlk.html

[S37] C++：set
来源：http://hz.jinyuanbaomall.cn/gtivqkdiho.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuanzhike.top/gtivltmtup.html

[S38] C++：排序
来源：http://hz.yongpay.top/gtbfuplxnc.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtwmcyilep.html

[S39] C++：自定义比较器排序
来源：http://hz.meibo888.top/gtunhvmwub.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cheryme.top/gtglrcwjdi.html

[S40] C++：查找元素
来源：http://hz.nanxuanxn.top/gtcqjmxwkd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ybcxt.top/gtpjqrcrah.html

[S41] C++：类与构造函数
来源：http://hz.feifeiyinyue.top/gtumynwhma.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gtlngjongi.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangkeji.top/gtinxuzxdl.html

class B : public Base { public: void f() override {} };
来源：http://hz.jqgufenzy.top/gtgftyfjps.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtxkcwvjhb.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtyujexqkg.html

[S44] C++：引用传参
来源：http://hz.zhijiandao.cn/gtvppojrjn.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtziaycbbu.html

[S45] C++：lambda
来源：http://hz.gaohongyu789.top/gtooaikite.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ppjwa.cn/gtielzgenq.html

[S46] C++：函数模板
来源：http://hz.gzhubu.top/gtacpmcasa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yvedp.cn/gtdffoxhlw.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtazghcfsk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shuidangran.top/gtiwztpwmu.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gthmoisimh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.52xcode.cn/gtdauvneyc.html

while (std::getline(in, line)) { }
来源：http://hz.nanxuanxn.top/gtfusrstvo.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gtwaltefhn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.c1oappe.top/gtbvhohpzy.html

[S50] C++：格式化数字
来源：http://hz.zhongyouzk.top/gtwzquypyi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hfpthk.cn/gtgmhgqiae.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtxcyykdza.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtmoeiueou.html

[S52] C++：const 与 noexcept
来源：http://hz.jinyuanbaomall.cn/gttjcfxxwc.html

int size() const noexcept { return n_; }
来源：http://hz.jiagoushi.top/gteamjpbfd.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtkhojssvd.html

std::vector<int> w = std::move(v);
来源：http://hz.jinghuilouyu.cn/gtcpbekrjh.html

[S54] C++：异常处理
来源：http://hz.hnxiangtu.top/gtvutqusfr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gtrbdupnwb.html

[S55] C++：结构化绑定
来源：http://hz.zhijiandao.cn/gtbxoklzqo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtrpxwkvbc.html

[S56] C++：optional
来源：http://hz.cucudq.cn/gtibktdjdj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yonumen.top/gtxrdffpyd.html

[S57] C++：编译期常量
来源：http://hz.jlsjyb.cn/gtyebwepsw.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtwogvvyov.html

[S58] C++：命名空间
来源：http://hz.yangfankeji.com/gtftjoqbge.html

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gtwbceqaem.html

[S59] C++：静态断言
来源：http://hz.yanxiufei.cn/gtgoikuyma.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtbcfqqkyp.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtllrqwrlk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gtvebfedgs.html

================================================================================
来源：http://hz.sweek.top/gtvmeperip.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtxiczsmdo.html

================================================================================
来源：http://hz.chenlongwang.top/gtqmxpyasx.html

[T01] Kotlin：Hello World
来源：http://hz.cashguo.top/gtxwapnlcz.html

println("Hello")
来源：http://hz.meibo888.top/gtafcekbzi.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gttuyemnyz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gthqifekvg.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtpargxemq.html

"值: $b"
来源：http://hz.zhoulong.xyz/gtmpftbqur.html

[T04] Kotlin：空安全
来源：http://hz.jiagoushi.top/gtthyeuboq.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtskqjltwv.html

[T05] Kotlin：when 表达式
来源：http://hz.9152youxi.cn/gtjszzboic.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtqtryihtz.html

[T06] Kotlin：集合映射
来源：http://hz.xinyue.icu/gtpyqoldnv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtmjjfargf.html

[T07] Kotlin：集合过滤
来源：http://hz.xinyue.icu/gthycqfehk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yonumen.top/gtvlzpwwps.html

[T08] Kotlin：数据类
来源：http://hz.hysaishi.cn/gtotsiuzcr.html

data class User(val name: String, val age: Int)
来源：http://hz.yonumen.top/gtotwvddzd.html

[T09] Kotlin：扩展函数
来源：http://hz.yuxming.cn/gtqlciccdm.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtnfhattao.html

[T10] Kotlin：默认参数
来源：http://hz.xuanzx.com/gthqnvevwr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgufenzy.top/gtetenguwi.html

[T11] Kotlin：协程
来源：http://hz.haohaochexian.top/gtyujtkrsm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtaqztotxp.html

[T12] Kotlin：解构声明
来源：http://hz.xuetiantiany.cn/gtnuljcxic.html

val (a, b) = Pair(1, 2)
来源：http://hz.jlsjyb.cn/gtpathfesl.html

[T13] Kotlin：只读 Map
来源：http://hz.zhiwuduotai.top/gtnsljbpic.html

val m = mapOf("a" to 1)
来源：http://hz.jyoumei.cn/gtuhqnvmhs.html

[T14] Kotlin：循环
来源：http://hz.cucudq.cn/gttdexeees.html

for (i in 1..10) println(i)
来源：http://hz.cucudq.cn/gtehgoetbp.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtqaizjgmp.html

interface Shape { fun area(): Double }
来源：http://hz.pengpengdd.cyou/gtyhuvroyz.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gthfjoeuvt.html

print("Hello")
来源：http://hz.xinyue.icu/gthjayrvih.html

[T17] Swift：变量与常量
来源：http://hz.gotoacloud.top/gtypbkjknj.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtvsgfaxdh.html

[T18] Swift：字符串插值
来源：http://hz.jyoumei.cn/gtspuargov.html

"值: \(b)"
来源：http://hz.yj20258888.top/gttxqihsso.html

[T19] Swift：可选绑定
来源：http://hz.cashguo.top/gtepgwjijr.html

if let n = opt { print(n) }
来源：http://hz.hammf.cn/gtqtgohyde.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gtwoybxgim.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gtuovzzbub.html

[T21] Swift：遍历
来源：http://hz.chenjidiqi.icu/gtinsuefut.html

for x in a { print(x) }
来源：http://hz.tanke756.top/gtzdttxjqd.html

[T22] Swift：字典
来源：http://hz.hongshengwenyu.top/gtgqgxnbst.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuanzx.com/gtloiytdhp.html

[T23] Swift：函数
来源：http://hz.yangfankeji.com/gtvgimyrhn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.0kj1m.cn/gtlvpaawmi.html

[T24] Swift：闭包
来源：http://hz.smart0.xyz/gtbshykccb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydjk.org.cn/gtdlpilmgg.html

[T25] Swift：结构体
来源：http://hz.jqgufenzy.top/gtnculuyst.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtgfappkdr.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtrizavmlm.html

class A: Base { override func f() {} }
来源：http://hz.yuanzhike.top/gtryzvcnyk.html

[T27] Swift：错误处理
来源：http://hz.hongshengwenyu.top/gtcxvbnadr.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangkeji.top/gtxocwjvrz.html

[T28] Swift：枚举
来源：http://hz.9152youxi.cn/gtcdrinduv.html

enum Color { case red, green }
来源：http://hz.mhx1999.top/gtkctblhpb.html

[T29] Swift：guard 提前返回
来源：http://hz.gotoacloud.top/gtsfqnxbgv.html

guard let x = opt else { return }
来源：http://hz.dianchejie.cn/gthsqimghm.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gtmmcritwx.html

protocol Shape { func area() -> Double }
来源：http://hz.chenjidiqi.icu/gtlhleksgf.html

[T31] Lua：Hello World
来源：http://hz.meibo888.top/gtbaktdqwe.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtzhgkkxtr.html

[T32] Lua：局部变量
来源：http://hz.cucudq.cn/gtcqnzvzrc.html

local a = 1
来源：http://hz.jlsjyb.cn/gttfrufpyv.html

[T33] Lua：表（数组）
来源：http://hz.xylfe.cn/gtfbdsgpkr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgfzy.top/gtnsqweoen.html

[T34] Lua：遍历表
来源：http://hz.haohaochexian.top/gtiqirgfrd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxinkj.top/gtkidkjiaw.html

[T35] Lua：字典表
来源：http://hz.havefunace.top/gtpzmofgcs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hongshengwenyu.top/gtaymdjxed.html

[T36] Lua：函数
来源：http://hz.jinyuanbaomall.cn/gtsocsxucy.html

function add(a, b) return a + b end
来源：http://hz.chenlongwang.top/gtpwbfblwa.html

[T37] Lua：字符串拼接
来源：http://hz.daxiang520.top/gthchrkrnk.html

"a" .. "b"
来源：http://hz.xinyue.icu/gtpdbytkps.html

[T38] Lua：条件
来源：http://hz.c1oappe.top/gtdbbhttqa.html

if x > 0 then print("正") end
来源：http://hz.andypj.xyz/gtkkvupahw.html

[T39] Lua：模式匹配
来源：http://hz.dianchejie.cn/gtwxvwxuzz.html

string.find(s, "%d+")
来源：http://hz.daxiang520.top/gtijlopzmh.html

[T40] Lua：元表
来源：http://hz.bjfxy.top/gtiguyiinz.html

setmetatable({}, { __index = base })
来源：http://hz.fzhhl.top/gtnejqdruf.html

[T41] Perl：Hello World
来源：http://hz.tian-w.cn/gtphrvjhpn.html

print "Hello\n";
来源：http://hz.zhoulong.xyz/gtfvmucisz.html

[T42] Perl：变量类型
来源：http://hz.cucudq.cn/gtqnuqxjhv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gtljqfqdlr.html

[T43] Perl：字符串插值
来源：http://hz.pengpengdd.cyou/gtuwtxgetl.html

"值: $a"
来源：http://hz.wangdashe.top/gteaxdbums.html

[T44] Perl：条件
来源：http://hz.aizwys.cn/gtwopougvx.html

if ($a > 0) { print "正"; }
来源：http://hz.birdmap.top/gttebycmph.html

[T45] Perl：数组遍历
来源：http://hz.smart0.xyz/gttiscczst.html

for my $x (@arr) { print $x; }
来源：http://hz.zycfv.cn/gtnicvbqyv.html

[T46] Perl：哈希操作
来源：http://hz.hongshengwenyu.top/gteiichhkr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangdashe.top/gtedlkvzkz.html

[T47] Perl：正则捕获
来源：http://hz.hfpthk.cn/gtwglkihqe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigfzy.top/gtrkvxiigv.html

[T48] Perl：正则替换
来源：http://hz.andypj.xyz/gtdykiupzb.html

$s =~ s/old/new/g;
来源：http://hz.jinqigfzy.top/gtavdwbbhy.html

[T49] Perl：函数
来源：http://hz.shanyushiyangkeji.top/gtlctpljlg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cqqwz.cn/gtuxsomohx.html

[T50] Perl：逐行读文件
来源：http://hz.smart0.xyz/gtcyoeodhr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.52xcode.cn/gtgxtjslut.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ivvv.top/gtlfuxjwnf.html

[T51] Scala：Hello World
来源：http://hz.chenzaomai.com/gtcepgfepo.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtlzulffjr.html

[T52] Scala：变量
来源：http://hz.cashguo.top/gtykvckpil.html

val a = 1;  var b = 2
来源：http://hz.zhongyouzk.top/gtnrejjscz.html

[T53] Scala：字符串插值
来源：http://hz.jianghu66.top/gtkpuhzzju.html

s"值: $b"
来源：http://hz.xziqi.cn/gtsdvtpntm.html

[T54] Scala：集合映射
来源：http://hz.ydzc1.top/gtilctxgff.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtioelfyey.html

[T55] Scala：集合过滤
来源：http://hz.gzhubu.top/gtcmhnlclh.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtjmjrimtd.html

[T56] Scala：样例类
来源：http://hz.dashuyun.cn/gtxwkgazrb.html

case class User(name: String, age: Int)
来源：http://hz.gotoacloud.top/gtdailpcps.html

[T57] Scala：模式匹配
来源：http://hz.jqgfzy.top/gteynmpnyh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jiagoushi.top/gtahtpiyza.html

[T58] Scala：函数定义
来源：http://hz.yonumen.top/gttxskjlba.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aizwys.cn/gtexzoeewc.html

[T59] Scala：循环
来源：http://hz.jiagoushi.top/gttryfdabo.html

for (i <- 1 to 10) println(i)
来源：http://hz.yuxming.cn/gtgonavqcm.html

[T60] Scala：折叠
来源：http://hz.xuetiantiany.cn/gtuybgsops.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gtnhdvdzhf.html

================================================================================
来源：http://hz.daxiang520.top/gttrocvrmh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sysykeji.top/gtrnijrluw.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfkpdwrmf.html

[U01] Py：创建虚拟环境
来源：http://hz.dianchejie.cn/gtflbaffto.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.havefunace.top/gtljhnnqoq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtsprtdazk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sufxvd.cn/gtlakyxsdw.html

[U03] Py：加载 .env 配置
来源：http://hz.xylfe.cn/gtbpakrxaa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sufxvd.cn/gtkyjcdqft.html

[U04] Py：变量调试打印
来源：http://hz.shuidangran.top/gtztswybrr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shanyushiyangkeji.top/gtdvjnihqe.html

[U05] Py：列表去重且保序
来源：http://hz.yj202588.top/gtvcnjawei.html

list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtzxgcaxbk.html

[U06] Py：合并两个字典
来源：http://hz.zhijiandao.cn/gtfyzhhcqj.html

{**a, **b}
来源：http://hz.yuanzhike.top/gtnxpkfffp.html

[U07] Py：反转字典键值
来源：http://hz.chenzaomai.com/gtilgrooqr.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigfzy.top/gtqfnoutrd.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtyizdgwgb.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtcidlgoag.html


<!-- 参考信息 -->