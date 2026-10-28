代发 wailian999

openssl rand -hex 16
来源：http://hz.zhiwuduotai.top/gtvxusxrdq.html

[R68] 计算文件校验值
来源：http://hz.fengsongda.top/gtilaxsiap.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gtnxxyicff.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gtfzbvixiv.html

head -c 16 /dev/urandom | base64
来源：http://hz.zycfv.cn/gtkkkmkwxp.html

[R70] 时间戳与互转
来源：http://hz.smart0.xyz/gtpvkdydbu.html

date +%s;  date -d @1700000000
来源：http://hz.gogol.net.cn/gtlhidesuq.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtjakazygg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhijiandao.cn/gtfidyctew.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtxwipfaub.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtmythwmpd.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gteqzvvdrg.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtucsguteo.html

[R74] 批量重命名
来源：http://hz.xziqi.cn/gtgjdlfuyt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtuwwypwvg.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtkclndjwd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtjvbwzaht.html

[R76] 使用临时文件
来源：http://hz.c1oappe.top/gtcsrvdmqv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtacruqskc.html

[R77] 读取用户输入
来源：http://hz.yuxming.cn/gtvgvncemw.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gtpjkexnga.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gttzywkcwc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gtadzbtydw.html

[R79] 解析命令行选项
来源：http://hz.guannengcc.top/gteepevaln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guannengcc.top/gtznmuqoii.html

[R80] 查看脚本执行耗时
来源：http://hz.yongpay.top/gtblyhpmyu.html

time ./run.sh
来源：http://hz.yvedp.cn/gtdsnifiur.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpxewjblr.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtqfjrgnfr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjbuyzdnp.html

[S01] C：Hello World
来源：http://hz.yj20258.top/gtmdwtigyz.html

#include <stdio.h>
来源：http://hz.tanke756.top/gtjfgfybkt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenlongwang.top/gtugomgkum.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtlxqqakls.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gtzksrmydn.html

[S03] C：读入整数
来源：http://hz.sysykeji.top/gtpvqafpen.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtrpyzhvom.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtbbuvtakl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtnpjqpigr.html

[S05] C：字符串长度
来源：http://hz.iojbl.cn/gtlgiteuda.html

strlen(s)
来源：http://hz.yj20258.top/gtsgzcwqfg.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtmdxlghkz.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtbodyuzrd.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtfefqjcgx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shzxlz.cn/gtikmrbvju.html

[S08] C：动态内存分配与释放
来源：http://hz.sxryk.cn/gtajzniual.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtopmdlgtc.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtdwqgryrt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tian-w.cn/gtyuaszrql.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtohezgndy.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtuhxamgea.html

[S11] C：逐行读文件
来源：http://hz.yongpay.top/gtqyofigld.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.snrcjt.cn/gtjtkogvvz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.quarkkingdee.top/gtdulecbzk.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtvwqlxtat.html

[S12] C：写文件
来源：http://hz.wangshuangyany.cn/gtdjjtayuq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtwlivouhe.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtnruegwad.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhaomingkeji.xyz/gtkyfmeqia.html

[S14] C：枚举
来源：http://hz.yanxiufei.cn/gtkagsbowo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhixingplan.top/gtwteskreo.html

[S15] C：类型转换
来源：http://hz.feifeiyinyue.top/gtarwltvpx.html

(double) a / b
来源：http://hz.daxiang520.top/gtvhfkiwwf.html

[S16] C：位操作置位
来源：http://hz.yongpay.top/gttwjouyld.html

x |= (1 << 3);
来源：http://hz.gotoacloud.top/gtodxylews.html

[S17] C：安全拼接字符串
来源：http://hz.ybcxt.top/gtzrontdcf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtwkshgnhm.html

[S18] C：命令行参数
来源：http://hz.hysaishi.cn/gthsmllxhy.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtlxrfiiry.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gtmmzhkckb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fengsongda.top/gtudkbqimr.html

[S20] C：二分查找
来源：http://hz.guowangkeji.top/gtedixqstf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtzraryvop.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtumyggdee.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtubezdveh.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gtzeeiwoas.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.snrcjt.cn/gtgydatmvu.html

[S23] C：随机数
来源：http://hz.jinqigfzy.top/gtyoucjkgu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shuidangran.top/gtgjdwvjzf.html

[S24] C：获取本地时间
来源：http://hz.jinghuilouyu.cn/gtxphbefti.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.iojbl.cn/gticnespqr.html

[S25] C：内存拷贝
来源：http://hz.birdmap.top/gtfhbinhjl.html

memcpy(dst, src, n);
来源：http://hz.iojbl.cn/gtczhqfteh.html

[S26] C：内存清零
来源：http://hz.ivvv.top/gtucymcyzj.html

memset(a, 0, sizeof a);
来源：http://hz.kuanghao11.cn/gtsxwxtzjp.html

[S27] C：定义常量
来源：http://hz.yj20258.top/gttlrlukap.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtyaktjpmb.html

[S28] C：静态变量
来源：http://hz.wangdashe.top/gtkqjfvraw.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtoymhmkyj.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gtvllbnbcg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtcnythiwi.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtzpimvuir.html

#ifndef X_H
来源：http://hz.zhaomingkeji.xyz/gtrkqbzvvq.html

#define X_H
来源：http://hz.ydzc1.top/gtpqirqszr.html

#endif
来源：http://hz.hysaishi.cn/gtvkomvjfo.html

[S31] C++：Hello World
来源：http://hz.gogol.net.cn/gtpfygsmex.html

#include <iostream>
来源：http://hz.gogol.net.cn/gtwxvfsfnr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gtsswazqur.html

[S32] C++：字符串
来源：http://hz.jiagoushi.top/gtjakwwcrz.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtxvnxhwlg.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtvmxcmvjz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yvedp.cn/gtmhqrxved.html

[S34] C++：遍历 vector
来源：http://hz.daxiang520.top/gtwgzwddsh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jiagoushi.top/gtxryyavax.html

[S35] C++：map
来源：http://hz.sufxvd.cn/gtfaqyfjes.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtlcqkoirq.html

[S36] C++：unordered_map
来源：http://hz.wangdashe.top/gtowdgqszv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtezsratsg.html

[S37] C++：set
来源：http://hz.ivvv.top/gtgrepklli.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ehwqpu.com/gtgfhkxfba.html

[S38] C++：排序
来源：http://hz.zhaomingkeji.xyz/gttznviwio.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtiejmgdem.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtrlecftmp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgfzy.top/gttkzgptbq.html

[S40] C++：查找元素
来源：http://hz.yj202588.top/gtoqjzoxxl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gtcbgmtxbu.html

[S41] C++：类与构造函数
来源：http://hz.guannengcc.top/gtagijxkcp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuanzx.com/gtjeznuxoq.html

[S42] C++：继承与虚函数
来源：http://hz.xuetiantiany.cn/gtekpbosob.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydzc1.top/gtcjbyphth.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gthwhzgawx.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinghuilouyu.cn/gtiqktwbjh.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gtojesszzh.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtlullsbsr.html

[S45] C++：lambda
来源：http://hz.ydjk.org.cn/gtncqacnei.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cashguo.top/gthtcohhni.html

[S46] C++：函数模板
来源：http://hz.hammf.cn/gtxflwuikx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.birdmap.top/gtzcksjwyi.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtqnjyoqhp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.kuanghao11.cn/gtftrmutum.html

[S48] C++：逐行读文件
来源：http://hz.sysykeji.top/gteoqmcwbm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nwbrower.top/gttridtjuh.html

while (std::getline(in, line)) { }
来源：http://hz.redwolf501.top/gtqtwfyvht.html

[S49] C++：写文件
来源：http://hz.mhx1999.top/gtljqshyct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhengqikj.top/gtuwmujnaf.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtzkmxivke.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangshuangyany.cn/gtinohtemf.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtllreozde.html

static_cast<double>(a) / b
来源：http://hz.gogol.net.cn/gtobvqvtta.html

[S52] C++：const 与 noexcept
来源：http://hz.gzhubu.top/gtbwkjauib.html

int size() const noexcept { return n_; }
来源：http://hz.cheryme.top/gtylxzgiyj.html

[S53] C++：移动语义
来源：http://hz.cucudq.cn/gtfkuvsdme.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gteogukqmk.html

[S54] C++：异常处理
来源：http://hz.guannengcc.top/gtxhoiylab.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.meibo888.top/gtjxpnrydb.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtkvuoewab.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daria6918.cn/gtwvprkyqd.html

[S56] C++：optional
来源：http://hz.daxiang520.top/gtccgixvxl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuetiantiany.cn/gtvrdlbpmz.html

[S57] C++：编译期常量
来源：http://hz.ybcxt.top/gtkotoacdm.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtpwyjclnj.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gturvhcimi.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinghuilouyu.cn/gtyanndcze.html

[S59] C++：静态断言
来源：http://hz.gogol.net.cn/gtnjettzom.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtbyvnteam.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gtmsysqmlc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtfaoxrhww.html

================================================================================
来源：http://hz.cashguo.top/gtbxvoosav.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtlioycwxz.html

================================================================================
来源：http://hz.gotoacloud.top/gtwjhvuwjt.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtwjwkzrek.html

println("Hello")
来源：http://hz.mhx1999.top/gtiooewpiq.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gtijrewbup.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj202588.top/gtebyhwzou.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtponqbghv.html

"值: $b"
来源：http://hz.hysaishi.cn/gtunthjelm.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtmrspeqzc.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtpvchykss.html

[T05] Kotlin：when 表达式
来源：http://hz.vqdsnc.cn/gtsmtvnirj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gtkvacdhoo.html

[T06] Kotlin：集合映射
来源：http://hz.jqgufenzy.top/gtsfzzvchj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigfzy.top/gtglrlqryh.html

[T07] Kotlin：集合过滤
来源：http://hz.meibo888.top/gtfmdeccwj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gttjfevvml.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtisxdxoxl.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtdphlizhn.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangtech.top/gtbjjhhzar.html

fun String.exclaim() = this + "!"
来源：http://hz.tian-w.cn/gttghlfjpp.html

[T10] Kotlin：默认参数
来源：http://hz.daria6918.cn/gtsgoklert.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ywan-chungtsiang.top/gtpkqhgwcn.html

[T11] Kotlin：协程
来源：http://hz.zhengqikj.top/gtdvqrhupx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtrphpfdwh.html

[T12] Kotlin：解构声明
来源：http://hz.nanxinkj.top/gtdulwzoas.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtbmnypbks.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtsecgnodm.html

val m = mapOf("a" to 1)
来源：http://hz.jyoumei.cn/gtdvoasbqm.html

[T14] Kotlin：循环
来源：http://hz.yj20258.top/gtajmczgbo.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtfdmrodng.html

[T15] Kotlin：接口
来源：http://hz.yongpay.top/gtahgdkwwt.html

interface Shape { fun area(): Double }
来源：http://hz.redwolf501.top/gtkjfdglxu.html

[T16] Swift：Hello World
来源：http://hz.pycfn.com/gtudpfpfqi.html

print("Hello")
来源：http://hz.chenlongwang.top/gtuvvsqemg.html

[T17] Swift：变量与常量
来源：http://hz.wangshuangyany.cn/gtehbmgayk.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtzivrtvyk.html

[T18] Swift：字符串插值
来源：http://hz.52xcode.cn/gthojctdqs.html

"值: \(b)"
来源：http://hz.yongpay.top/gtbooiutkg.html

[T19] Swift：可选绑定
来源：http://hz.ybcxt.top/gtfvycijyy.html

if let n = opt { print(n) }
来源：http://hz.zdqjudy.top/gtmvausceh.html

[T20] Swift：数组操作
来源：http://hz.ppjwa.cn/gtqnzdvssa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtmfpkwiad.html

[T21] Swift：遍历
来源：http://hz.pengpengdd.cyou/gtjprascnt.html

for x in a { print(x) }
来源：http://hz.yongpay.top/gtifizeujy.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtiyvmgnrf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtguogryvh.html

[T23] Swift：函数
来源：http://hz.hfpthk.cn/gthejfaltj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhiwuduotai.top/gtvgdvqhli.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gttjzvjsjy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.iojbl.cn/gtclexzqni.html

[T25] Swift：结构体
来源：http://hz.yongpay.top/gtduczfelu.html

struct P { var x: Int }
来源：http://hz.dianchejie.cn/gtzvxlswgg.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gtrlyzmuqw.html

class A: Base { override func f() {} }
来源：http://hz.nanxuanxn.top/gtqqaozgdw.html

[T27] Swift：错误处理
来源：http://hz.tanke756.top/gtchcilzzr.html

do { try f() } catch { print(error) }
来源：http://hz.jiagoushi.top/gtrbalcfnh.html

[T28] Swift：枚举
来源：http://hz.xylfe.cn/gtklxdsirk.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtbmwhbrmy.html

[T29] Swift：guard 提前返回
来源：http://hz.bjfxy.top/gttenjbmqz.html

guard let x = opt else { return }
来源：http://hz.hnxiangtu.top/gtnszwkfxj.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtuuxlqsyw.html

protocol Shape { func area() -> Double }
来源：http://hz.guannengcc.top/gthytylpvn.html

[T31] Lua：Hello World
来源：http://hz.aibaodan.cn/gtcjsypukh.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtgnsikzmn.html

[T32] Lua：局部变量
来源：http://hz.daxiang520.top/gtqrhsokgo.html

local a = 1
来源：http://hz.chenlongwang.top/gtrclobddh.html

[T33] Lua：表（数组）
来源：http://hz.haohaochexian.top/gtxgsrcdym.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhongyouzk.top/gtmrsomrci.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtpqrwhoae.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jianghu66.top/gtrbvdddzo.html

[T35] Lua：字典表
来源：http://hz.iojbl.cn/gtjfhiyxmy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xylfe.cn/gtdwouyvwa.html

[T36] Lua：函数
来源：http://hz.yuanzhike.top/gtnpdrjtri.html

function add(a, b) return a + b end
来源：http://hz.chenlongwang.top/gtuqkbwsdy.html

[T37] Lua：字符串拼接
来源：http://hz.tianlin.xyz/gtpuwbdggb.html

"a" .. "b"
来源：http://hz.jinqigufen.top/gteffpsgbo.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtpvasdkaz.html

if x > 0 then print("正") end
来源：http://hz.jyoumei.cn/gtrlmwhmwd.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtimqhursq.html

string.find(s, "%d+")
来源：http://hz.fzhhl.top/gtvvbfvhhi.html

[T40] Lua：元表
来源：http://hz.meibo888.top/gtjxytmydf.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtosuzcxzk.html

[T41] Perl：Hello World
来源：http://hz.jiagoushi.top/gtejtchhuk.html

print "Hello\n";
来源：http://hz.yonumen.top/gtuuklwyeu.html

[T42] Perl：变量类型
来源：http://hz.hnxiangtu.top/gtmfhgigom.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gogol.net.cn/gtpbwdnnea.html

[T43] Perl：字符串插值
来源：http://hz.52xcode.cn/gtwehzuqlp.html

"值: $a"
来源：http://hz.gotoacloud.top/gtqscmppqe.html

[T44] Perl：条件
来源：http://hz.mhx1999.top/gtoejoncfc.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangkeji.top/gtayrxxplo.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gtitjhrcxt.html

for my $x (@arr) { print $x; }
来源：http://hz.tian-w.cn/gtjnqvbenq.html

[T46] Perl：哈希操作
来源：http://hz.tianlin.xyz/gtyuixbleo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shuidangran.top/gtablowggp.html

[T47] Perl：正则捕获
来源：http://hz.xuetiantiany.cn/gtdiwkodvi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.tianlin.xyz/gtxjhbausu.html

[T48] Perl：正则替换
来源：http://hz.aibaodan.cn/gtgkiudriq.html

$s =~ s/old/new/g;
来源：http://hz.ydjk.org.cn/gtxnwbmeln.html

[T49] Perl：函数
来源：http://hz.shuidangran.top/gtwbgusids.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.birdmap.top/gttsmuoqeq.html

[T50] Perl：逐行读文件
来源：http://hz.hysaishi.cn/gtvjtxrzld.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tanke756.top/gtdvnrkdfd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gotoacloud.top/gtsjjrcasl.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtdawtfzxz.html

println("Hello")
来源：http://hz.bjfxy.top/gtqnicqcoz.html

[T52] Scala：变量
来源：http://hz.gaohongyu789.top/gtkhjvtuec.html

val a = 1;  var b = 2
来源：http://hz.nanxuanxn.top/gtdkzholea.html

[T53] Scala：字符串插值
来源：http://hz.316326.xyz/gtysbwgwdo.html

s"值: $b"
来源：http://hz.feifeiyinyue.top/gtegyvheaw.html

[T54] Scala：集合映射
来源：http://hz.tian-w.cn/gtsaumgegj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.c1oappe.top/gthqlpymxn.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gtffvpjfjt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ybcxt.top/gtnnyczrws.html

[T56] Scala：样例类
来源：http://hz.nanxuanxn.top/gteiumnoab.html

case class User(name: String, age: Int)
来源：http://hz.shanyushiyangtech.top/gtjuujezqz.html

[T57] Scala：模式匹配
来源：http://hz.snrcjt.cn/gtqutlghsu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guannengcc.top/gtnamgfazw.html

[T58] Scala：函数定义
来源：http://hz.yanxiufei.cn/gtjyvzvazv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xuetiantiany.cn/gtrhjtusxz.html

[T59] Scala：循环
来源：http://hz.xylfe.cn/gtdijeumlk.html

for (i <- 1 to 10) println(i)
来源：http://hz.xylfe.cn/gtpuzxmrwe.html

[T60] Scala：折叠
来源：http://hz.nanxuanxn.top/gthzzmvzhz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenlongwang.top/gtxxemobmb.html

================================================================================
来源：http://hz.kuanghao11.cn/gtcsqysany.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtjvdovsil.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqhojniyr.html

[U01] Py：创建虚拟环境
来源：http://hz.snrcjt.cn/gtrozscwmr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gtngtzttvh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.316326.xyz/gtbzuphqya.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jqgufenzy.top/gtzzxkvtui.html

[U03] Py：加载 .env 配置
来源：http://hz.snrcjt.cn/gtnmkdrzbe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtvzqdazfs.html

[U04] Py：变量调试打印
来源：http://hz.feifeiyinyue.top/gtdnhlbbsg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gtwixubfcv.html

[U05] Py：列表去重且保序
来源：http://hz.quarkkingdee.top/gtxbtqkveu.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtabjniivq.html

[U06] Py：合并两个字典
来源：http://hz.jinghuilouyu.cn/gtglyogfsc.html

{**a, **b}
来源：http://hz.yuanzhike.top/gtilczcgwx.html

[U07] Py：反转字典键值
来源：http://hz.chenlongwang.top/gtjdkpdpmv.html

{v: k for k, v in d.items()}
来源：http://hz.ivvv.top/gtosjabxxo.html

[U08] Py：展平二维列表
来源：http://hz.aizwys.cn/gtfaiqrtfn.html

[y for x in nested for y in x]
来源：http://hz.zdqjudy.top/gtiheckufx.html


<!-- 参考信息 -->