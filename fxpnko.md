代发 wailian999

openssl rand -hex 16
来源：http://hz.hfpthk.cn/gtzyfkggpm.html

[R68] 计算文件校验值
来源：http://hz.tanke756.top/gtlejpsncz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yonumen.top/gtluegtvwe.html

[R69] 生成随机密码
来源：http://hz.yvedp.cn/gtgscxxajd.html

head -c 16 /dev/urandom | base64
来源：http://hz.redwolf501.top/gtxsfzfmux.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtoqyisjby.html

date +%s;  date -d @1700000000
来源：http://hz.zhongyouzk.top/gtyvuqgewm.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtyqedihoi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shuidangran.top/gttlmpxnhj.html

[R72] 等待端口就绪
来源：http://hz.zhiwuduotai.top/gtmkqixhlc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nanxuanxn.top/gtphfwaqgx.html

[R73] 分割大日志
来源：http://hz.shanyushiyangkeji.top/gtxabakekr.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gttljyelzs.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gtguabyyoq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhengqikj.top/gtiykpzoks.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtqsvzqhfz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtfohwrycj.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangtech.top/gtqjwyiqid.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtsjgumfmf.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtntftxqrm.html

read -rp "请输入: " ans
来源：http://hz.hysaishi.cn/gtiibbjutw.html

[R78] 交互式菜单
来源：http://hz.yvedp.cn/gteblyghue.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gaohongyu789.top/gtlblbfdfz.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtlioltwbm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gzhubu.top/gtwgleisng.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtdfppymdb.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtqifbiiag.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdviuehsp.html

S. C / C++ 专题
来源：http://hz.iojbl.cn/gttlsylvsu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtwbgddtne.html

[S01] C：Hello World
来源：http://hz.zhaomingkeji.xyz/gtohxxlrgj.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtjfytnudm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtvqnjzips.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtoaezcmkd.html

int a = 10; printf("%d\n", a);
来源：http://hz.bjfxy.top/gtuseanhaa.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtzugvbvkt.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtcbdenept.html

[S04] C：字符串复制
来源：http://hz.52xcode.cn/gtkqqfegkr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dashuyun.cn/gtwlfvjdag.html

[S05] C：字符串长度
来源：http://hz.zhiwuduotai.top/gtefnzqknp.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtszuatbde.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtehnmlpme.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gtsfoeftou.html

[S07] C：数组遍历求和
来源：http://hz.smart0.xyz/gtoihgyvge.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gogol.net.cn/gtfnhxezvw.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangtech.top/gtswctetbb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.52xcode.cn/gtrbznjrwc.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangtech.top/gtmhpguejc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtbtbrryck.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtuqchwztd.html

int *p = &a;  *p = 5;
来源：http://hz.yuanzhike.top/gtydlsyago.html

[S11] C：逐行读文件
来源：http://hz.jqgfzy.top/gtufjgxlcd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.feifeiyinyue.top/gtpqiwfaou.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daxiang520.top/gtqbvmkwau.html

fclose(f);
来源：http://hz.yvedp.cn/gtlpkieamq.html

[S12] C：写文件
来源：http://hz.nwbrower.top/gtdmckxzyn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fzhhl.top/gtnbfvctcu.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtarbisrez.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hywenlv.cn/gtxaftzppg.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtfrwliymh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtljemsgzj.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtjtevzkug.html

(double) a / b
来源：http://hz.hongshengwenyu.top/gtacwckckc.html

[S16] C：位操作置位
来源：http://hz.jinghuilouyu.cn/gtruydryzl.html

x |= (1 << 3);
来源：http://hz.tianlin.xyz/gtcehfhbcg.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtufsaldld.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hammf.cn/gtykdmymbg.html

[S18] C：命令行参数
来源：http://hz.nwbrower.top/gtygpjprre.html

int main(int argc, char **argv)
来源：http://hz.zhiwuduotai.top/gtqbrrfnys.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gtpnppmjbi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtnkaplimh.html

[S20] C：二分查找
来源：http://hz.zhengqikj.top/gthxsxkteo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtmrlnqbov.html

[S21] C：字符类别判断
来源：http://hz.jqgfzy.top/gtruuzbbjr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtknfglkkf.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gtmzwkzjle.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtmrtliqma.html

[S23] C：随机数
来源：http://hz.feifeiyinyue.top/gtzcxfcyhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guowangkeji.top/gtdlgigywg.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtzymjeyaq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cdnleiting.top/gtlilzbpcn.html

[S25] C：内存拷贝
来源：http://hz.zycfv.cn/gtoqqnaklj.html

memcpy(dst, src, n);
来源：http://hz.jlsjyb.cn/gtvwblukse.html

[S26] C：内存清零
来源：http://hz.snrcjt.cn/gtqbuhyoct.html

memset(a, 0, sizeof a);
来源：http://hz.ydjk.org.cn/gtrlskpoob.html

[S27] C：定义常量
来源：http://hz.haohaochexian.top/gtvwjeeuoe.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtadlnfpes.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtojbsyifn.html

static int counter = 0;
来源：http://hz.jiagoushi.top/gtwnaokieq.html

[S29] C：变参函数
来源：http://hz.hammf.cn/gtowekxnby.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gtpbyfnvkb.html

[S30] C：头文件保护
来源：http://hz.nwbrower.top/gtndulgdhe.html

#ifndef X_H
来源：http://hz.redwolf501.top/gtgxnencae.html

#define X_H
来源：http://hz.hysaishi.cn/gthmwcjkks.html

#endif
来源：http://hz.kuanghao11.cn/gtnunhrvig.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtiqdgzrrg.html

#include <iostream>
来源：http://hz.aizwys.cn/gtmlyqoqkj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.iojbl.cn/gtbbohdipc.html

[S32] C++：字符串
来源：http://hz.shuidangran.top/gtlmihohkq.html

std::string s = "hi";  s += "!";
来源：http://hz.hysaishi.cn/gtecyjzmai.html

[S33] C++：vector 增删
来源：http://hz.gotoacloud.top/gtzpeaecjp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.meibo888.top/gtawyzywfy.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtgbeditkd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinyuanbaomall.cn/gtoqxdohtw.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtdeqhyvle.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gthtvperty.html

[S36] C++：unordered_map
来源：http://hz.daria6918.cn/gttxlhckni.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aizwys.cn/gtuwpnfcxj.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtuoeirsni.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jyoumei.cn/gtffkmzzoo.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtfotsrlml.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gtbuncjlev.html

[S39] C++：自定义比较器排序
来源：http://hz.xuanzx.com/gtyfpavykz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtfusotmlg.html

[S40] C++：查找元素
来源：http://hz.cheryme.top/gtfxygscqa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtdploczvl.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtfmxqbtam.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yonumen.top/gtyrxthrzg.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtodnhizmy.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj202588.top/gtbtquukun.html

[S43] C++：智能指针
来源：http://hz.xylfe.cn/gtrvpawmsx.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gtdwlxanhu.html

[S44] C++：引用传参
来源：http://hz.hysaishi.cn/gtwyakrbyy.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtkfpdvrpy.html

[S45] C++：lambda
来源：http://hz.cqqwz.cn/gtmqafrhlg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yonumen.top/gtpddgbicm.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gtjdmpfobr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gzhubu.top/gtcddblgsn.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gtfavtqlcw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgfzy.top/gticbueixt.html

[S48] C++：逐行读文件
来源：http://hz.hfpthk.cn/gtlfypmoxp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtauhwanwu.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gttxdehzev.html

[S49] C++：写文件
来源：http://hz.tianlin.xyz/gterlajwfk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtmbyhlmmo.html

[S50] C++：格式化数字
来源：http://hz.cqqwz.cn/gtpxowimpy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gtepedhfrd.html

[S51] C++：显式类型转换
来源：http://hz.zhiwuduotai.top/gtomnuixxk.html

static_cast<double>(a) / b
来源：http://hz.guannengcc.top/gtxepkbspe.html

[S52] C++：const 与 noexcept
来源：http://hz.feifeiyinyue.top/gtbscxlqds.html

int size() const noexcept { return n_; }
来源：http://hz.ybcxt.top/gthkgdypli.html

[S53] C++：移动语义
来源：http://hz.bjfxy.top/gthkyxjfip.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtxjfaotki.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtsuksyqlb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhijiandao.cn/gtlhwznnhc.html

[S55] C++：结构化绑定
来源：http://hz.snrcjt.cn/gtojbsmncd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtamzrsisp.html

[S56] C++：optional
来源：http://hz.gaohongyu789.top/gtbviyozer.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.haohaochexian.top/gtgyiuzqqa.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gtsdtkerlj.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gtaxbofgcv.html

[S58] C++：命名空间
来源：http://hz.zhijiandao.cn/gtuaiunuev.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gtimjjtckh.html

[S59] C++：静态断言
来源：http://hz.quarkkingdee.top/gtxhpapcpt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tanke756.top/gtwvgsxfrb.html

[S60] C++：遍历并删除元素
来源：http://hz.0kj1m.cn/gtuaadkawa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yanxiufei.cn/gtgfxdsyac.html

================================================================================
来源：http://hz.fzhhl.top/gtnfqdyqby.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gtmuaenwuu.html

================================================================================
来源：http://hz.nwbrower.top/gtqavcbifd.html

[T01] Kotlin：Hello World
来源：http://hz.dashuyun.cn/gtmuoneoax.html

println("Hello")
来源：http://hz.shuidangran.top/gtfmmpgbii.html

[T02] Kotlin：变量
来源：http://hz.yj20258.top/gtouaqndvh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yonumen.top/gtqfmrgwdi.html

[T03] Kotlin：字符串模板
来源：http://hz.fengsongda.top/gteqxdcsjj.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtfhauwyiv.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtaaqskhwu.html

val n: String? = null;  n?.length
来源：http://hz.wangshuangyany.cn/gtptawwdyo.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtqjiqaxnh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.316326.xyz/gtilaujkag.html

[T06] Kotlin：集合映射
来源：http://hz.tian-w.cn/gteuarcfll.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtsggnjoiu.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtrkkixhuq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.kuanghao11.cn/gttaoavixj.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtpyhqptaa.html

data class User(val name: String, val age: Int)
来源：http://hz.hywenlv.cn/gtwfbzjosa.html

[T09] Kotlin：扩展函数
来源：http://hz.tanke756.top/gtoezgfjcz.html

fun String.exclaim() = this + "!"
来源：http://hz.316326.xyz/gtxpnwauys.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtwrlsdvfl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shuidangran.top/gtuccdgzei.html

[T11] Kotlin：协程
来源：http://hz.jqgufenzy.top/gtxngplkag.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dashuyun.cn/gtrpouwvir.html

[T12] Kotlin：解构声明
来源：http://hz.snrcjt.cn/gtjbxgiovz.html

val (a, b) = Pair(1, 2)
来源：http://hz.cucudq.cn/gtfobiylfi.html

[T13] Kotlin：只读 Map
来源：http://hz.ydjk.org.cn/gtwtxtwxfz.html

val m = mapOf("a" to 1)
来源：http://hz.guannengcc.top/gtrkqlrfnr.html

[T14] Kotlin：循环
来源：http://hz.aizwys.cn/gttakrsuag.html

for (i in 1..10) println(i)
来源：http://hz.hnxiangtu.top/gtxplttyiy.html

[T15] Kotlin：接口
来源：http://hz.pycfn.com/gtspuheita.html

interface Shape { fun area(): Double }
来源：http://hz.9152youxi.cn/gtfaeumzyt.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtubekzeky.html

print("Hello")
来源：http://hz.jianghu66.top/gtkzdltely.html

[T17] Swift：变量与常量
来源：http://hz.ywan-chungtsiang.top/gtnfmnfcsu.html

var a = 1;  let b = 2
来源：http://hz.wangshuangyany.cn/gtabjkmwlv.html

[T18] Swift：字符串插值
来源：http://hz.zhijiandao.cn/gtllcathwm.html

"值: \(b)"
来源：http://hz.yj20258.top/gtismflbpx.html

[T19] Swift：可选绑定
来源：http://hz.yj20258888.top/gtrykjdwyl.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangtech.top/gtgblqhzur.html

[T20] Swift：数组操作
来源：http://hz.c1oappe.top/gtrwanahdc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jianghu66.top/gtlgwgyphh.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gttslfibor.html

for x in a { print(x) }
来源：http://hz.sweek.top/gtkzlygevg.html

[T22] Swift：字典
来源：http://hz.dianchejie.cn/gtywitpinz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.c1oappe.top/gtmwpdgnxi.html

[T23] Swift：函数
来源：http://hz.cheryme.top/gtzzdhasrm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.feifeiyinyue.top/gtrrseulko.html

[T24] Swift：闭包
来源：http://hz.zhengqikj.top/gtresfbwvn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xinyue.icu/gtkhmruvws.html

[T25] Swift：结构体
来源：http://hz.birdmap.top/gtiuajdmgi.html

struct P { var x: Int }
来源：http://hz.dianchejie.cn/gtddcuboyw.html

[T26] Swift：类与重写
来源：http://hz.hongshengwenyu.top/gtrbdvycbn.html

class A: Base { override func f() {} }
来源：http://hz.haohaochexian.top/gtshupwhuh.html

[T27] Swift：错误处理
来源：http://hz.jlsjyb.cn/gtxiyixxyd.html

do { try f() } catch { print(error) }
来源：http://hz.xingfuxueyuan.xyz/gtfnjeqkhn.html

[T28] Swift：枚举
来源：http://hz.wangdashe.top/gtqictrrmt.html

enum Color { case red, green }
来源：http://hz.haohaochexian.top/gtcrlyyifx.html

[T29] Swift：guard 提前返回
来源：http://hz.sxryk.cn/gtrdjwludi.html

guard let x = opt else { return }
来源：http://hz.zycfv.cn/gtafqnrffh.html

[T30] Swift：协议
来源：http://hz.ppjwa.cn/gttzkeiueu.html

protocol Shape { func area() -> Double }
来源：http://hz.zhongyouzk.top/gtyognxear.html

[T31] Lua：Hello World
来源：http://hz.quarkkingdee.top/gtxbsfjpac.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtrelacgup.html

[T32] Lua：局部变量
来源：http://hz.sysykeji.top/gtcxpefdwl.html

local a = 1
来源：http://hz.jinqigufen.top/gtfbxpyblm.html

[T33] Lua：表（数组）
来源：http://hz.cucudq.cn/gtgbosxcij.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuanzhike.top/gtnmfacqgn.html

[T34] Lua：遍历表
来源：http://hz.jinqigufen.top/gtrvgnzwlz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hfpthk.cn/gtknvypdfr.html

[T35] Lua：字典表
来源：http://hz.hnqzz.top/gtylkglsqs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.dashuyun.cn/gthahxmhsc.html

[T36] Lua：函数
来源：http://hz.nwbrower.top/gtjfzohnlw.html

function add(a, b) return a + b end
来源：http://hz.jyoumei.cn/gttglmvcjx.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtgjvabymf.html

"a" .. "b"
来源：http://hz.vqdsnc.cn/gtinnbibpw.html

[T38] Lua：条件
来源：http://hz.meibo888.top/gthvklehhu.html

if x > 0 then print("正") end
来源：http://hz.xingfuxueyuan.xyz/gtutwzotny.html

[T39] Lua：模式匹配
来源：http://hz.haohaochexian.top/gtrxkjjfec.html

string.find(s, "%d+")
来源：http://hz.aibaodan.cn/gtgjtbobon.html

[T40] Lua：元表
来源：http://hz.ywan-chungtsiang.top/gtitpsowdv.html

setmetatable({}, { __index = base })
来源：http://hz.quarkkingdee.top/gtwehynpnt.html

[T41] Perl：Hello World
来源：http://hz.nwbrower.top/gtnurjeykr.html

print "Hello\n";
来源：http://hz.hywenlv.cn/gtelhwohvb.html

[T42] Perl：变量类型
来源：http://hz.zhiwuduotai.top/gtwxjfdukw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yvedp.cn/gtrzxmvgew.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gtlmnrjgtg.html

"值: $a"
来源：http://hz.52xcode.cn/gtwcigpfvw.html

[T44] Perl：条件
来源：http://hz.52xcode.cn/gtvxdpzriz.html

if ($a > 0) { print "正"; }
来源：http://hz.gaohongyu789.top/gtrrtvbswb.html

[T45] Perl：数组遍历
来源：http://hz.hammf.cn/gtsrtnzego.html

for my $x (@arr) { print $x; }
来源：http://hz.shzxlz.cn/gtcjbcushb.html

[T46] Perl：哈希操作
来源：http://hz.hysaishi.cn/gtqcbkkbkj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sysykeji.top/gtijqoiuij.html

[T47] Perl：正则捕获
来源：http://hz.ydjk.org.cn/gttesqmrqk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinyuanbaomall.cn/gtgesnpqti.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtgzciqeaa.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtaeamwgqq.html

[T49] Perl：函数
来源：http://hz.ydjk.org.cn/gtqyiisdgg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.andypj.xyz/gtaxbvaqga.html

[T50] Perl：逐行读文件
来源：http://hz.guowangkeji.top/gtyilkikqz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hfpthk.cn/gtloetylug.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtgophgvjf.html

[T51] Scala：Hello World
来源：http://hz.sufxvd.cn/gtxpfbvkun.html

println("Hello")
来源：http://hz.tanke756.top/gtaovopqbw.html

[T52] Scala：变量
来源：http://hz.tanke756.top/gtiwpmnouw.html

val a = 1;  var b = 2
来源：http://hz.yanxiufei.cn/gtkksslevn.html

[T53] Scala：字符串插值
来源：http://hz.yuanzhike.top/gtyvkhqhpi.html

s"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtwskevole.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtyzgdkqjb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuetiantiany.cn/gtlgjgrsqg.html

[T55] Scala：集合过滤
来源：http://hz.fengsongda.top/gtothqddrq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinyuanbaomall.cn/gtmrvcggis.html

[T56] Scala：样例类
来源：http://hz.yanxiufei.cn/gtsefsoikc.html

case class User(name: String, age: Int)
来源：http://hz.9152youxi.cn/gtnvfnfvde.html

[T57] Scala：模式匹配
来源：http://hz.meibo888.top/gtnraigfje.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jlsjyb.cn/gtggfhewkp.html

[T58] Scala：函数定义
来源：http://hz.daxiang520.top/gtszyflkfb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtwypaxvhc.html

[T59] Scala：循环
来源：http://hz.gotoacloud.top/gtheprogsy.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenjidiqi.icu/gtfjglcfcj.html

[T60] Scala：折叠
来源：http://hz.jiagoushi.top/gtdqxqtwws.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuxming.cn/gtpwcugzul.html

================================================================================
来源：http://hz.tianlin.xyz/gtfywrqrtd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258888.top/gtkkdemaic.html

================================================================================
来源：http://hz.dianchejie.cn/gtgvylrdsj.html

[U01] Py：创建虚拟环境
来源：http://hz.sufxvd.cn/gtpwguahxh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gtoncheztj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.meibo888.top/gtvgpapnsy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtmnhrmbbq.html

[U03] Py：加载 .env 配置
来源：http://hz.smart0.xyz/gtwaewqkny.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hysaishi.cn/gtyqbrcohn.html

[U04] Py：变量调试打印
来源：http://hz.shzxlz.cn/gtqzewwbcj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nwbrower.top/gtuewpxgjx.html

[U05] Py：列表去重且保序
来源：http://hz.iojbl.cn/gtfkalbkuy.html

list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gthvyltdbc.html

[U06] Py：合并两个字典
来源：http://hz.shangyingyoupin.top/gtyzogqwap.html

{**a, **b}
来源：http://hz.wangshuangyany.cn/gtwwldryft.html

[U07] Py：反转字典键值
来源：http://hz.hnxiangtu.top/gtczbqpkru.html

{v: k for k, v in d.items()}
来源：http://hz.cdnleiting.top/gtjgorhvox.html

[U08] Py：展平二维列表
来源：http://hz.feifeiyinyue.top/gtwgijdkwt.html

[y for x in nested for y in x]
来源：http://hz.yangfankeji.com/gttezcakmb.html


<!-- 参考信息 -->