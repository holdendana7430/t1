代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.ivvv.top/gthalunnoc.html

[R76] 使用临时文件
来源：http://hz.shangyingyoupin.top/gtadyruqyl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtkhngeuml.html

[R77] 读取用户输入
来源：http://hz.zhaomingkeji.xyz/gtlqktpwuq.html

read -rp "请输入: " ans
来源：http://hz.c1oappe.top/gtdfokalvb.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtbtmigozp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jyoumei.cn/gtgfgdmbhs.html

[R79] 解析命令行选项
来源：http://hz.hnqzz.top/gtmdrxlaha.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxinkj.top/gthynflhht.html

[R80] 查看脚本执行耗时
来源：http://hz.ydjk.org.cn/gtzcyijmbr.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtqpdsppun.html

================================================================================
来源：http://hz.cqqwz.cn/gtslgheqak.html

S. C / C++ 专题
来源：http://hz.hammf.cn/gtagxczfnu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtipqeoubd.html

[S01] C：Hello World
来源：http://hz.aizwys.cn/gtaizhijco.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtbftkbswc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtaczwaejg.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gttjojbezg.html

int a = 10; printf("%d\n", a);
来源：http://hz.gogol.net.cn/gtyajvuivy.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtxhotcrok.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gtqtnlurhk.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtftfngddg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ehwqpu.com/gtpvtbcdwl.html

[S05] C：字符串长度
来源：http://hz.zdqjudy.top/gtrqtvshpw.html

strlen(s)
来源：http://hz.316326.xyz/gtpeompymf.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtmswcogci.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtdghplvsi.html

[S07] C：数组遍历求和
来源：http://hz.ppjwa.cn/gtzswqqpen.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yongpay.top/gtfofdghzg.html

[S08] C：动态内存分配与释放
来源：http://hz.xinyue.icu/gtynaycgnu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dianchejie.cn/gtwuielbcv.html

[S09] C：结构体定义与初始化
来源：http://hz.xuanzx.com/gtrsekvjnm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gtceuiyqxz.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtnfpoupse.html

int *p = &a;  *p = 5;
来源：http://hz.gzhubu.top/gtkefeqbnr.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtxqzgujbl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gttuaqmbuz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtvmjapfvd.html

fclose(f);
来源：http://hz.svipenyu.cn/gtkmtkdcco.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtlgtcxyqd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.bjfxy.top/gtfgvkwdvd.html

[S13] C：宏定义
来源：http://hz.ppjwa.cn/gtvfjsjcsv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenjidiqi.icu/gtvysyecox.html

[S14] C：枚举
来源：http://hz.yj20258.top/gteqgjirrv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydjk.org.cn/gtsvrjqzjr.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtthexzhvr.html

(double) a / b
来源：http://hz.nanxuanxn.top/gtaiknxlnt.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtrgnplskx.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtefzwregf.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtnpslqjbf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ivvv.top/gttmnbhsqv.html

[S18] C：命令行参数
来源：http://hz.ybcxt.top/gtexusvmsq.html

int main(int argc, char **argv)
来源：http://hz.jyoumei.cn/gthjtivkwt.html

[S19] C：快速排序
来源：http://hz.vqdsnc.cn/gtqxrjyqqw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtydhexzbb.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtoltjpouv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sysykeji.top/gtuvwfgmkn.html

[S21] C：字符类别判断
来源：http://hz.fzhhl.top/gtrtvdqqlb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hongshengwenyu.top/gtrqzissli.html

[S22] C：字符串转数字
来源：http://hz.shangyingyoupin.top/gtdbvujlzd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gzhubu.top/gthhxxfooj.html

[S23] C：随机数
来源：http://hz.ydjk.org.cn/gtkaqoydpn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtqxfqahkb.html

[S24] C：获取本地时间
来源：http://hz.daria6918.cn/gtufqkijzs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gtcxilrero.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtiddvopzb.html

memcpy(dst, src, n);
来源：http://hz.daria6918.cn/gtmlztrdaz.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gttujfrcjk.html

memset(a, 0, sizeof a);
来源：http://hz.gaohongyu789.top/gttoksrarl.html

[S27] C：定义常量
来源：http://hz.jlsjyb.cn/gtjufkyelw.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gttwwziosi.html

[S28] C：静态变量
来源：http://hz.shzxlz.cn/gtmcyzvotn.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtvvtxzzph.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gtvmwgmnfy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuanzx.com/gtwpqtiktx.html

[S30] C：头文件保护
来源：http://hz.xuanzx.com/gtmftxzesz.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtqfwmuwxu.html

#define X_H
来源：http://hz.jqgufenzy.top/gtxnappjvj.html

#endif
来源：http://hz.sysykeji.top/gtzsoqzazs.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtjtuysgmm.html

#include <iostream>
来源：http://hz.hnqzz.top/gtogyfqhao.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aibaodan.cn/gtwrwuebvl.html

[S32] C++：字符串
来源：http://hz.jqgfzy.top/gtioeikzrm.html

std::string s = "hi";  s += "!";
来源：http://hz.hysaishi.cn/gtiqyjltye.html

[S33] C++：vector 增删
来源：http://hz.gotoacloud.top/gtoaudvslr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.quarkkingdee.top/gtccbjevas.html

[S34] C++：遍历 vector
来源：http://hz.yonumen.top/gttlwgohaj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtqvtescnk.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtflvickpb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gttxagpuir.html

[S36] C++：unordered_map
来源：http://hz.gzhubu.top/gtigcoesnh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtcsnmzxut.html

[S37] C++：set
来源：http://hz.52xcode.cn/gtukhvzuut.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtahyyilpl.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gtazjiwzhy.html

std::sort(v.begin(), v.end());
来源：http://hz.chenlongwang.top/gtgreyohvp.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtivhsrunl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtgswzufhy.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtxaezqsmq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aibaodan.cn/gtsrynskni.html

[S41] C++：类与构造函数
来源：http://hz.cucudq.cn/gtcfqxywli.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtqoelkeai.html

[S42] C++：继承与虚函数
来源：http://hz.ydjk.org.cn/gthvgrfizl.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhongyouzk.top/gtzgilujsy.html

[S43] C++：智能指针
来源：http://hz.xylfe.cn/gtapvvoodf.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gtydyqfhue.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtseihmzwz.html

void inc(int &x) { ++x; }
来源：http://hz.dashuyun.cn/gtekdfdvgv.html

[S45] C++：lambda
来源：http://hz.yj202588.top/gtjssiqzbv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtvdkhihfb.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtydxxobnu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hongshengwenyu.top/gtbsdwcevn.html

[S47] C++：结构化绑定遍历
来源：http://hz.sysykeji.top/gtuahdhxhx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jianghu66.top/gtoglnfeyq.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtjzqydhcl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtvczvqrka.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigfzy.top/gttnhfmszs.html

[S49] C++：写文件
来源：http://hz.birdmap.top/gtcocdnmgy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hysaishi.cn/gtyhthwamq.html

[S50] C++：格式化数字
来源：http://hz.hysaishi.cn/gtfbytxcgz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gtxtbwshzc.html

[S51] C++：显式类型转换
来源：http://hz.sweek.top/gtadotkngr.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtyneetxxk.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtnvuhevjg.html

int size() const noexcept { return n_; }
来源：http://hz.fzhhl.top/gtehbzmhjp.html

[S53] C++：移动语义
来源：http://hz.shuidangran.top/gttjpzaqpk.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgfzy.top/gtdbsompdl.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtvkynzgzc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.quarkkingdee.top/gtowkrzxsg.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gttckllohh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigufen.top/gtuznakjjw.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtcwgfmaao.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gtndbhzppm.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtjayrrlgt.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gthzauqtvs.html

[S58] C++：命名空间
来源：http://hz.yj202588.top/gtqazbmaxc.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtoxlleenr.html

[S59] C++：静态断言
来源：http://hz.tian-w.cn/gtyeaoccgr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenzaomai.com/gtzkhlkshi.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtmatwmxlr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtdalupphi.html

================================================================================
来源：http://hz.yueranfly.top/gtrinezxrr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtnpwtxivy.html

================================================================================
来源：http://hz.fengsongda.top/gtvoaxjzgb.html

[T01] Kotlin：Hello World
来源：http://hz.c1oappe.top/gtjutswkya.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtregdmroh.html

[T02] Kotlin：变量
来源：http://hz.jqgfzy.top/gtvduathro.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.c1oappe.top/gtskyicbnz.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtzukhlnzn.html

"值: $b"
来源：http://hz.aizwys.cn/gtreysmobi.html

[T04] Kotlin：空安全
来源：http://hz.mhx1999.top/gtwcehzmax.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gtgarhxgev.html

[T05] Kotlin：when 表达式
来源：http://hz.cheryme.top/gthfylkmjv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aibaodan.cn/gtdsdzpcre.html

[T06] Kotlin：集合映射
来源：http://hz.ybcxt.top/gtqqudswpn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigufen.top/gtttnhwmuv.html

[T07] Kotlin：集合过滤
来源：http://hz.snrcjt.cn/gtqgleemrm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zycfv.cn/gtmmgoqgrk.html

[T08] Kotlin：数据类
来源：http://hz.9152youxi.cn/gtdxykcrgf.html

data class User(val name: String, val age: Int)
来源：http://hz.cqqwz.cn/gtilgcmlky.html

[T09] Kotlin：扩展函数
来源：http://hz.jianghu66.top/gtxeokwxsm.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gtautskuhy.html

[T10] Kotlin：默认参数
来源：http://hz.xingfuxueyuan.xyz/gtzkbpyuyo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gttvcpezkv.html

[T11] Kotlin：协程
来源：http://hz.hysaishi.cn/gtxsvkqjpk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuanzx.com/gtvgsedwfj.html

[T12] Kotlin：解构声明
来源：http://hz.hnqzz.top/gtdtjvbpoh.html

val (a, b) = Pair(1, 2)
来源：http://hz.0kj1m.cn/gtcokthcul.html

[T13] Kotlin：只读 Map
来源：http://hz.aizwys.cn/gtvqsniwjg.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtqrraiasw.html

[T14] Kotlin：循环
来源：http://hz.xziqi.cn/gtworkcazz.html

for (i in 1..10) println(i)
来源：http://hz.dashuyun.cn/gtbonqvclg.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gtkbpqafmu.html

interface Shape { fun area(): Double }
来源：http://hz.mhx1999.top/gtjmiyixno.html

[T16] Swift：Hello World
来源：http://hz.haohaochexian.top/gtbhgwubzb.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtauzzrddi.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gtkcwgtioc.html

var a = 1;  let b = 2
来源：http://hz.dashuyun.cn/gturbkqbvs.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtyqldehjl.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gttvidigsb.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtpiammknw.html

if let n = opt { print(n) }
来源：http://hz.yongpay.top/gttrllelca.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtaobpdipo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinghuilouyu.cn/gtfvzaqnoz.html

[T21] Swift：遍历
来源：http://hz.shuidangran.top/gttxsyyseq.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtytjmrodr.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtbgvynbwv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fzhhl.top/gtcdljmqad.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gtenjrqiqt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtrvwoegbi.html

[T24] Swift：闭包
来源：http://hz.haohaochexian.top/gtozaamjyu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yueranfly.top/gtuhwiwbhe.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtompdnhet.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtanohwceh.html

[T26] Swift：类与重写
来源：http://hz.chenlongwang.top/gtxqwqixbm.html

class A: Base { override func f() {} }
来源：http://hz.jinyuanbaomall.cn/gtbjeufwvs.html

[T27] Swift：错误处理
来源：http://hz.svipenyu.cn/gtmorgspbx.html

do { try f() } catch { print(error) }
来源：http://hz.sufxvd.cn/gtkgnvzegr.html

[T28] Swift：枚举
来源：http://hz.ehwqpu.com/gtwznozbwg.html

enum Color { case red, green }
来源：http://hz.ppjwa.cn/gtukwlvfts.html

[T29] Swift：guard 提前返回
来源：http://hz.jinghuilouyu.cn/gtqzvqclgg.html

guard let x = opt else { return }
来源：http://hz.jyoumei.cn/gtwvireqiv.html

[T30] Swift：协议
来源：http://hz.tian-w.cn/gthmybrjng.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgfzy.top/gtafjrncrv.html

[T31] Lua：Hello World
来源：http://hz.yangfankeji.com/gtfmtuuues.html

print("Hello")
来源：http://hz.tianlin.xyz/gtkvmhhkht.html

[T32] Lua：局部变量
来源：http://hz.zhiwuduotai.top/gtvxrvffiv.html

local a = 1
来源：http://hz.yuanzhike.top/gtvbwsjdrx.html

[T33] Lua：表（数组）
来源：http://hz.316326.xyz/gtjvuvjxhp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgfzy.top/gtapascpmn.html

[T34] Lua：遍历表
来源：http://hz.shuidangran.top/gtizhcartw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aizwys.cn/gtzffyauvc.html

[T35] Lua：字典表
来源：http://hz.chenzaomai.com/gtqctvppfs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zycfv.cn/gtbjvxvxry.html

[T36] Lua：函数
来源：http://hz.jianghu66.top/gtalkehkke.html

function add(a, b) return a + b end
来源：http://hz.zdqjudy.top/gtawjcgpsq.html

[T37] Lua：字符串拼接
来源：http://hz.chenlongwang.top/gtxtwljaby.html

"a" .. "b"
来源：http://hz.chenzaomai.com/gtdxzehvuq.html

[T38] Lua：条件
来源：http://hz.gotoacloud.top/gtlnuqynmb.html

if x > 0 then print("正") end
来源：http://hz.chenlongwang.top/gtctdyoghw.html

[T39] Lua：模式匹配
来源：http://hz.daria6918.cn/gtsaxdcvpo.html

string.find(s, "%d+")
来源：http://hz.shangyingyoupin.top/gtmqydjdco.html

[T40] Lua：元表
来源：http://hz.zhoulong.xyz/gtqyjrxkpq.html

setmetatable({}, { __index = base })
来源：http://hz.nanxuanxn.top/gthlelrnhi.html

[T41] Perl：Hello World
来源：http://hz.hnqzz.top/gtwdecsxhw.html

print "Hello\n";
来源：http://hz.zhiwuduotai.top/gtncbgqigd.html

[T42] Perl：变量类型
来源：http://hz.aizwys.cn/gtvxktmsii.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuetiantiany.cn/gtnzvssptf.html

[T43] Perl：字符串插值
来源：http://hz.cdnleiting.top/gtmlqkfzry.html

"值: $a"
来源：http://hz.yj20258.top/gtnlxutkry.html

[T44] Perl：条件
来源：http://hz.ehwqpu.com/gtlyaysfgi.html

if ($a > 0) { print "正"; }
来源：http://hz.aibaodan.cn/gtnuddgqqr.html

[T45] Perl：数组遍历
来源：http://hz.cucudq.cn/gtbiveaqpx.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangtech.top/gtovaomgnq.html

[T46] Perl：哈希操作
来源：http://hz.pycfn.com/gthsivrxeb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgfzy.top/gtugbdkfis.html

[T47] Perl：正则捕获
来源：http://hz.pycfn.com/gtmwrrvypm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hnqzz.top/gtojkweqtc.html

[T48] Perl：正则替换
来源：http://hz.aizwys.cn/gtxfyfwtsc.html

$s =~ s/old/new/g;
来源：http://hz.zhongyouzk.top/gtprgohpth.html

[T49] Perl：函数
来源：http://hz.yuxming.cn/gtavacicdy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jlsjyb.cn/gtxdkvovnh.html

[T50] Perl：逐行读文件
来源：http://hz.dashuyun.cn/gtvgukvbid.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtycwbknnp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.smart0.xyz/gtklxfbvlp.html

[T51] Scala：Hello World
来源：http://hz.wangdashe.top/gtlzkzwqjb.html

println("Hello")
来源：http://hz.zycfv.cn/gtkvcralqy.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gthbhbxrdv.html

val a = 1;  var b = 2
来源：http://hz.hywenlv.cn/gttbqzkuev.html

[T53] Scala：字符串插值
来源：http://hz.ydjk.org.cn/gtrotssczz.html

s"值: $b"
来源：http://hz.52xcode.cn/gtcrkpjzbi.html

[T54] Scala：集合映射
来源：http://hz.gogol.net.cn/gteqdgmsct.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gtbxyltuuq.html

[T55] Scala：集合过滤
来源：http://hz.ybcxt.top/gtogxjcqvy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhixingplan.top/gtsnplvkjr.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gtrtljyyxe.html

case class User(name: String, age: Int)
来源：http://hz.bjfxy.top/gtognfqwze.html

[T57] Scala：模式匹配
来源：http://hz.yangfankeji.com/gtomzbdtnr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gthoedlvem.html

[T58] Scala：函数定义
来源：http://hz.zhengqikj.top/gtrzlovalc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinqigfzy.top/gtdnnpxkfa.html

[T59] Scala：循环
来源：http://hz.shanyushiyangkeji.top/gtpnaoipqc.html

for (i <- 1 to 10) println(i)
来源：http://hz.aizwys.cn/gtdqilzarr.html

[T60] Scala：折叠
来源：http://hz.xuetiantiany.cn/gthfthbgtr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtnhtbmpoi.html

================================================================================
来源：http://hz.yvedp.cn/gtkxwvsbev.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.bjfxy.top/gtotbauitv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtcbvppzvs.html

[U01] Py：创建虚拟环境
来源：http://hz.quarkkingdee.top/gtrlukclik.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ywan-chungtsiang.top/gtcqdmkxyy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenzaomai.com/gtptsxdtwk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dashuyun.cn/gtlvpzdxhq.html

[U03] Py：加载 .env 配置
来源：http://hz.ehwqpu.com/gtwwilsgeu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yvedp.cn/gtdcpoenvh.html

[U04] Py：变量调试打印
来源：http://hz.gzhubu.top/gtzymjfpvo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhaomingkeji.xyz/gtjbhmnpau.html

[U05] Py：列表去重且保序
来源：http://hz.xuanzx.com/gtglijqijp.html

list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtlobdtyah.html

[U06] Py：合并两个字典
来源：http://hz.jinqigfzy.top/gtndsvfrng.html

{**a, **b}
来源：http://hz.chenjidiqi.icu/gtyggsqvfk.html

[U07] Py：反转字典键值
来源：http://hz.zdqjudy.top/gtotrrxsmf.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258.top/gtwbwkrwwh.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtphibckuk.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtoontvtuj.html

[U09] Py：字典取最大值的键
来源：http://hz.shuidangran.top/gtppdrdqsi.html

max(d, key=d.get)
来源：http://hz.zhoulong.xyz/gttspucwbg.html

[U10] Py：按值排序字典
来源：http://hz.daria6918.cn/gtpmyaxqdt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guowangkeji.top/gtikpjoxdg.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtvzbhtobp.html

(x * 2 for x in arr)
来源：http://hz.pengpengdd.cyou/gtqhpwsqus.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.chenjidiqi.icu/gtrimnrdlm.html

Counter(arr).most_common(3)
来源：http://hz.ehwqpu.com/gtpzzsbrbx.html

[U13] Py：固定长度队列
来源：http://hz.jinghuilouyu.cn/gthqkeljsj.html

deque(maxlen=10)
来源：http://hz.svipenyu.cn/gtdodgctey.html

[U14] Py：分组收集到列表
来源：http://hz.yangfankeji.com/gtlimjxrro.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtpuhfsekk.html

[U15] Py：高精度计时
来源：http://hz.c1oappe.top/gtkrjwyzlq.html

t = time.perf_counter()
来源：http://hz.birdmap.top/gttfcguqtz.html

[U16] Py：命令行参数解析
来源：http://hz.316326.xyz/gtxkugtuvy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.mhx1999.top/gtstklesea.html


<!-- 参考信息 -->