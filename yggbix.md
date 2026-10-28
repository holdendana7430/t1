代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangshuangyany.cn/gtwcpeiozg.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtmvdowjyn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtdhemfzxx.html

[R77] 读取用户输入
来源：http://hz.0kj1m.cn/gtrjuazuzv.html

read -rp "请输入: " ans
来源：http://hz.wangdashe.top/gtirstjjoj.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gtiqvdzcaz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yangfankeji.com/gtuvbapcwa.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtcblldrju.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtgdaihksd.html

[R80] 查看脚本执行耗时
来源：http://hz.svipenyu.cn/gthzpaximi.html

time ./run.sh
来源：http://hz.jiagoushi.top/gtctkhfeyi.html

================================================================================
来源：http://hz.zycfv.cn/gtlamslotq.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtmgjpvtqq.html

================================================================================
来源：http://hz.havefunace.top/gtdezokkhq.html

[S01] C：Hello World
来源：http://hz.jinyuanbaomall.cn/gtbdsturmd.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtlgquiyrr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtyngbspno.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtlqqwpztd.html

int a = 10; printf("%d\n", a);
来源：http://hz.gzhubu.top/gtazaoaqvo.html

[S03] C：读入整数
来源：http://hz.gaohongyu789.top/gtyyvkzzwy.html

int x; scanf("%d", &x);
来源：http://hz.zhoulong.xyz/gtpjtmtact.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gtmymmttbs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtjspyrgjd.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtjzbwcpez.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gthaaxfric.html

[S06] C：字符串比较
来源：http://hz.wangdashe.top/gtfsgklion.html

strcmp(a, b) == 0
来源：http://hz.bjfxy.top/gtbtbduozz.html

[S07] C：数组遍历求和
来源：http://hz.cdnleiting.top/gtlpnmexek.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinghuilouyu.cn/gtqxwuaqqe.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gthyxicfaq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtscsjiuky.html

[S09] C：结构体定义与初始化
来源：http://hz.xinyue.icu/gtyjdxbjja.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gtcskhhoyf.html

[S10] C：指针与解引用
来源：http://hz.zycfv.cn/gtnvqnitmm.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtgnizrcpp.html

[S11] C：逐行读文件
来源：http://hz.tanke756.top/gtkwtktkio.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnqzz.top/gtndctswux.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guowangkeji.top/gtvtunmaqk.html

fclose(f);
来源：http://hz.zhixingplan.top/gtdmwoyqmn.html

[S12] C：写文件
来源：http://hz.c1oappe.top/gtzcmlcbmi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxinkj.top/gtsxtsktjg.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtciesgcst.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtegasmgzz.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtncmgrofh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gtdlvdjaor.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtyxxjqibw.html

(double) a / b
来源：http://hz.nanxinkj.top/gtqgcqfznx.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gthduoznuy.html

x |= (1 << 3);
来源：http://hz.gotoacloud.top/gtovqkfqsn.html

[S17] C：安全拼接字符串
来源：http://hz.hammf.cn/gtlxufgvkb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtyciifqur.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gtnbjsbvmn.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtyiutoiqi.html

[S19] C：快速排序
来源：http://hz.guowangkeji.top/gthwgnhnoz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtkmlgkybs.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtmhzkxzxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtadztpitx.html

[S21] C：字符类别判断
来源：http://hz.fengsongda.top/gtqbboohyz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zdqjudy.top/gtlnawiuzx.html

[S22] C：字符串转数字
来源：http://hz.jqgufenzy.top/gtpzqljfnx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jyoumei.cn/gtfgtptlbf.html

[S23] C：随机数
来源：http://hz.zycfv.cn/gtyezxztnp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yvedp.cn/gtwnybhgjq.html

[S24] C：获取本地时间
来源：http://hz.dianchejie.cn/gtypcexxot.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhiwuduotai.top/gtriwitvqb.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtwdwziijk.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtktsqtkiz.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gtuxgctqjx.html

memset(a, 0, sizeof a);
来源：http://hz.sufxvd.cn/gtcoezznty.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtgbbsqxwx.html

const double PI = 3.14159;
来源：http://hz.bjfxy.top/gtlimisvbn.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtnminbpii.html

static int counter = 0;
来源：http://hz.xuetiantiany.cn/gtjytnxgye.html

[S29] C：变参函数
来源：http://hz.xuanzx.com/gtgxlmohpr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtpeyuhtnj.html

[S30] C：头文件保护
来源：http://hz.jinqigufen.top/gtvfxtwlar.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtghteczoe.html

#define X_H
来源：http://hz.yonumen.top/gtgokqupiu.html

#endif
来源：http://hz.sufxvd.cn/gtsgbrzanh.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtndedvclb.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtrkzitcrw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gtddkwdmtn.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtxwokbbbt.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gttxqnlign.html

[S33] C++：vector 增删
来源：http://hz.kuanghao11.cn/gtxirxhoyx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dianchejie.cn/gtwfnmipxd.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtihevuysa.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zdqjudy.top/gtfuruapdh.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gttzhaqtay.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtonkisurb.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtmgnmvtzq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtksoxzwpk.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtudpfoouh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtqrstaykp.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gtppnnykzz.html

std::sort(v.begin(), v.end());
来源：http://hz.cqqwz.cn/gtebfxnsbo.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gttcbvykeq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gzhubu.top/gthglhigby.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtmocqvyrr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gtbdogwfsw.html

[S41] C++：类与构造函数
来源：http://hz.gaohongyu789.top/gtwyinbsfs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shuidangran.top/gtqcejenej.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtiobqymly.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gtecmypafb.html

[S43] C++：智能指针
来源：http://hz.fzhhl.top/gtdjvqwygu.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258888.top/gtiwbilrrf.html

[S44] C++：引用传参
来源：http://hz.zhaomingkeji.xyz/gtairwylra.html

void inc(int &x) { ++x; }
来源：http://hz.wangdashe.top/gtdldtoens.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gtdzdyeqao.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.bjfxy.top/gtxqodnsgz.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtdwhlobjr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydjk.org.cn/gtabkwxbyz.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtgcdtkzfc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydjk.org.cn/gtayrbvmbe.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gthhmlcwek.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jyoumei.cn/gtkdtczxry.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtnkpgpbay.html

[S49] C++：写文件
来源：http://hz.xingfuxueyuan.xyz/gtjhalnyui.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangtech.top/gtippiaiba.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtwncowuto.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zycfv.cn/gtnnzikjye.html

[S51] C++：显式类型转换
来源：http://hz.vqdsnc.cn/gtueudbzvd.html

static_cast<double>(a) / b
来源：http://hz.quarkkingdee.top/gtizgmdjdo.html

[S52] C++：const 与 noexcept
来源：http://hz.xinyue.icu/gtqetphbfw.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangkeji.top/gtdzozaxcg.html

[S53] C++：移动语义
来源：http://hz.hywenlv.cn/gtdcprswdj.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtsipyibdk.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gtirnsntod.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jlsjyb.cn/gtsyfwcvwd.html

[S55] C++：结构化绑定
来源：http://hz.shangyingyoupin.top/gtilyjwmnw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gtolurztmw.html

[S56] C++：optional
来源：http://hz.tanke756.top/gtggbtccqg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gtxrvlemyv.html

[S57] C++：编译期常量
来源：http://hz.jinghuilouyu.cn/gtntvszikk.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gtggzyxlfu.html

[S58] C++：命名空间
来源：http://hz.aibaodan.cn/gtyzvpqnzr.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtknzhljil.html

[S59] C++：静态断言
来源：http://hz.jiagoushi.top/gtynmxaqmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxinkj.top/gtzzjoxcwp.html

[S60] C++：遍历并删除元素
来源：http://hz.ydzc1.top/gtqhlwatyx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.kuanghao11.cn/gtswiypfug.html

================================================================================
来源：http://hz.yongpay.top/gtgnpqrrns.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangshuangyany.cn/gtybgerhhf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtoecooigt.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtdebsbndf.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtrhcnazdn.html

[T02] Kotlin：变量
来源：http://hz.yongpay.top/gtxhymrmld.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.316326.xyz/gtppoevrkj.html

[T03] Kotlin：字符串模板
来源：http://hz.ybcxt.top/gtaiiqusxf.html

"值: $b"
来源：http://hz.snrcjt.cn/gtdzxytuol.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gtqrtaznct.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gthzxxcisf.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtesglmjxl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gtkvtnfntu.html

[T06] Kotlin：集合映射
来源：http://hz.zhiwuduotai.top/gtubhzlvuq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtgijyocmr.html

[T07] Kotlin：集合过滤
来源：http://hz.hongshengwenyu.top/gthqczoicc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtkvoestyn.html

[T08] Kotlin：数据类
来源：http://hz.yanxiufei.cn/gtpvbwldop.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtqfyhavyh.html

[T09] Kotlin：扩展函数
来源：http://hz.sxryk.cn/gtwbsludlu.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtylblizze.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtisnzqzty.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shanyushiyangtech.top/gtmgxlgzcf.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtmzxipfwh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.bjfxy.top/gtestnstui.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtqibgfrvu.html

val (a, b) = Pair(1, 2)
来源：http://hz.xinyue.icu/gtojxtxnyy.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtzayfjxbu.html

val m = mapOf("a" to 1)
来源：http://hz.kuanghao11.cn/gtclvrzchv.html

[T14] Kotlin：循环
来源：http://hz.ybcxt.top/gtdqbdeizb.html

for (i in 1..10) println(i)
来源：http://hz.sufxvd.cn/gtymutqnmd.html

[T15] Kotlin：接口
来源：http://hz.sufxvd.cn/gtbmnhgvsx.html

interface Shape { fun area(): Double }
来源：http://hz.aibaodan.cn/gthixcbunc.html

[T16] Swift：Hello World
来源：http://hz.wangdashe.top/gtgkqlicur.html

print("Hello")
来源：http://hz.daria6918.cn/gtpppqfrjv.html

[T17] Swift：变量与常量
来源：http://hz.dianchejie.cn/gthgzhmwpc.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gtzcgdraht.html

[T18] Swift：字符串插值
来源：http://hz.hfpthk.cn/gtvydpxjap.html

"值: \(b)"
来源：http://hz.zhengqikj.top/gtobjsdulh.html

[T19] Swift：可选绑定
来源：http://hz.ppjwa.cn/gtavivktxo.html

if let n = opt { print(n) }
来源：http://hz.jqgufenzy.top/gtsmtbctnj.html

[T20] Swift：数组操作
来源：http://hz.xylfe.cn/gtgjiaxvve.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ywan-chungtsiang.top/gtsfofowub.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gtugowuqge.html

for x in a { print(x) }
来源：http://hz.yanxiufei.cn/gtdowzsccj.html

[T22] Swift：字典
来源：http://hz.fengsongda.top/gtzjhptpsj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gtemuhnyue.html

[T23] Swift：函数
来源：http://hz.daxiang520.top/gtxvrzbcvv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtewclepck.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtbjkcoepl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yongpay.top/gtjvkxzhxb.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gtnqvoictn.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gtrkgtnhaf.html

[T26] Swift：类与重写
来源：http://hz.zycfv.cn/gtdmtijgtv.html

class A: Base { override func f() {} }
来源：http://hz.feifeiyinyue.top/gtnzksskdb.html

[T27] Swift：错误处理
来源：http://hz.zycfv.cn/gtihijjuvn.html

do { try f() } catch { print(error) }
来源：http://hz.jqgufenzy.top/gtzyuzvoce.html

[T28] Swift：枚举
来源：http://hz.fengsongda.top/gtinwpojmh.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gtykmdirsx.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtewuglerm.html

guard let x = opt else { return }
来源：http://hz.wangshuangyany.cn/gtkgfaljqe.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtotnqwifw.html

protocol Shape { func area() -> Double }
来源：http://hz.yj20258888.top/gtdyseucwh.html

[T31] Lua：Hello World
来源：http://hz.hnxiangtu.top/gtgdwxulnb.html

print("Hello")
来源：http://hz.yuxming.cn/gtacoqtcpm.html

[T32] Lua：局部变量
来源：http://hz.jinqigfzy.top/gtudbpuinx.html

local a = 1
来源：http://hz.nanxuanxn.top/gtkdzeuufp.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtcnrowrhh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.0kj1m.cn/gtcpodhvul.html

[T34] Lua：遍历表
来源：http://hz.andypj.xyz/gtggklsxjd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yonumen.top/gtqsmmaqxn.html

[T35] Lua：字典表
来源：http://hz.cqqwz.cn/gtxpgomwtc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guowangkeji.top/gtlgibcqkf.html

[T36] Lua：函数
来源：http://hz.ppjwa.cn/gtgixbwlcv.html

function add(a, b) return a + b end
来源：http://hz.yj20258888.top/gtcinnctkg.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtanocbtrf.html

"a" .. "b"
来源：http://hz.yj202588.top/gtexhsxrhp.html

[T38] Lua：条件
来源：http://hz.zycfv.cn/gtnwnhqxcq.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtaaivoogl.html

[T39] Lua：模式匹配
来源：http://hz.ppjwa.cn/gtxecrlqhj.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtcwwpsrxv.html

[T40] Lua：元表
来源：http://hz.zhengqikj.top/gtxnaucozv.html

setmetatable({}, { __index = base })
来源：http://hz.jlsjyb.cn/gtsozepryt.html

[T41] Perl：Hello World
来源：http://hz.ybcxt.top/gtzxejfvjt.html

print "Hello\n";
来源：http://hz.shangyingyoupin.top/gtofwnqlgi.html

[T42] Perl：变量类型
来源：http://hz.guannengcc.top/gtfxumwfnd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aibaodan.cn/gtsetjdelk.html

[T43] Perl：字符串插值
来源：http://hz.0kj1m.cn/gtxbfvfipa.html

"值: $a"
来源：http://hz.zycfv.cn/gttjnvlhjz.html

[T44] Perl：条件
来源：http://hz.meibo888.top/gtldnnkrug.html

if ($a > 0) { print "正"; }
来源：http://hz.hnxiangtu.top/gtlbpaxume.html

[T45] Perl：数组遍历
来源：http://hz.tanke756.top/gttxqlglbv.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtaedncmxa.html

[T46] Perl：哈希操作
来源：http://hz.52xcode.cn/gtaeatzraw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aibaodan.cn/gtvwhujqvg.html

[T47] Perl：正则捕获
来源：http://hz.zhiwuduotai.top/gtndogvnvt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinghuilouyu.cn/gtwingvryr.html

[T48] Perl：正则替换
来源：http://hz.hnqzz.top/gtvasaktlr.html

$s =~ s/old/new/g;
来源：http://hz.birdmap.top/gtjbjzbwrl.html

[T49] Perl：函数
来源：http://hz.cqqwz.cn/gtoreklcdj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tian-w.cn/gtenwyakpv.html

[T50] Perl：逐行读文件
来源：http://hz.yj202588.top/gtortcdrzj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinghuilouyu.cn/gtgjecpgbm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinqigufen.top/gtqehxrxqt.html

[T51] Scala：Hello World
来源：http://hz.cdnleiting.top/gtzagsknmj.html

println("Hello")
来源：http://hz.yj202588.top/gtylfcbjoo.html

[T52] Scala：变量
来源：http://hz.yj20258888.top/gtqqfsnnus.html

val a = 1;  var b = 2
来源：http://hz.fzhhl.top/gthjlaseqx.html

[T53] Scala：字符串插值
来源：http://hz.ppjwa.cn/gtkpfwcpzi.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtznscrfgx.html

[T54] Scala：集合映射
来源：http://hz.cqqwz.cn/gtrgixjwfx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigfzy.top/gtynzkpeef.html

[T55] Scala：集合过滤
来源：http://hz.ehwqpu.com/gtjdckzrcg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.smart0.xyz/gtkazbrezk.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gtbklvbtjz.html

case class User(name: String, age: Int)
来源：http://hz.gzhubu.top/gtjquwobzy.html

[T57] Scala：模式匹配
来源：http://hz.zdqjudy.top/gtedrupwyt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shanyushiyangtech.top/gtzobwcsvf.html

[T58] Scala：函数定义
来源：http://hz.wangshuangyany.cn/gtvqityfnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinqigufen.top/gtqzbzzivz.html

[T59] Scala：循环
来源：http://hz.mhx1999.top/gtoznlhsvg.html

for (i <- 1 to 10) println(i)
来源：http://hz.cdnleiting.top/gtidorlnaw.html

[T60] Scala：折叠
来源：http://hz.daria6918.cn/gtfavdyxqk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.guowangkeji.top/gtrkslfzhi.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfopfynlm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtnbadgxzt.html

================================================================================
来源：http://hz.hywenlv.cn/gtjevnioir.html

[U01] Py：创建虚拟环境
来源：http://hz.haohaochexian.top/gtzjuctsfr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.dashuyun.cn/gtbqaraxcu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangtech.top/gtszeoflza.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtspcucucs.html

[U03] Py：加载 .env 配置
来源：http://hz.vqdsnc.cn/gtaboxgbrr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.mhx1999.top/gtdmookohs.html

[U04] Py：变量调试打印
来源：http://hz.sysykeji.top/gtjivxamyr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jianghu66.top/gtosftgkqm.html

[U05] Py：列表去重且保序
来源：http://hz.daria6918.cn/gtrkpwyomk.html

list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gttcesccbg.html

[U06] Py：合并两个字典
来源：http://hz.zhiwuduotai.top/gtnowqcdyu.html

{**a, **b}
来源：http://hz.yj20258888.top/gtweeolehf.html

[U07] Py：反转字典键值
来源：http://hz.cdnleiting.top/gtkvucmaqr.html

{v: k for k, v in d.items()}
来源：http://hz.yj202588.top/gthetlikda.html

[U08] Py：展平二维列表
来源：http://hz.yj20258.top/gtidwcdeeg.html

[y for x in nested for y in x]
来源：http://hz.svipenyu.cn/gtpdqmukuj.html

[U09] Py：字典取最大值的键
来源：http://hz.zhiwuduotai.top/gtpyjsfbbt.html

max(d, key=d.get)
来源：http://hz.xylfe.cn/gtqltaoucs.html

[U10] Py：按值排序字典
来源：http://hz.zycfv.cn/gtbswskukm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.fengsongda.top/gtbzveziiw.html

[U11] Py：生成器表达式
来源：http://hz.pengpengdd.cyou/gtnpnrzjlo.html

(x * 2 for x in arr)
来源：http://hz.ivvv.top/gtthsyprap.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.fengsongda.top/gtqxpiqydo.html

Counter(arr).most_common(3)
来源：http://hz.jinyuanbaomall.cn/gtitrysxhe.html

[U13] Py：固定长度队列
来源：http://hz.fengsongda.top/gtmnuysrvj.html

deque(maxlen=10)
来源：http://hz.gaohongyu789.top/gtxvwpccso.html

[U14] Py：分组收集到列表
来源：http://hz.zycfv.cn/gtskzbidsw.html

defaultdict(list)
来源：http://hz.yuxming.cn/gtcrnajrvb.html

[U15] Py：高精度计时
来源：http://hz.andypj.xyz/gtflolhhgz.html

t = time.perf_counter()
来源：http://hz.pycfn.com/gtdbvhpbpd.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gtmuaiaulv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigfzy.top/gtekvcetsh.html


<!-- 参考信息 -->