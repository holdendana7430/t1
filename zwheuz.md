代发 wailian999

split -l 1000 big.log part_
来源：http://hz.gzhubu.top/gtbspfjgjr.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtfjblwaxa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hysaishi.cn/gtjtjuagjr.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtcxgptpru.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.fengsongda.top/gthkaywrgq.html

[R76] 使用临时文件
来源：http://hz.pengpengdd.cyou/gtwdfmqslz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtcpmhjcnd.html

[R77] 读取用户输入
来源：http://hz.cashguo.top/gthalshbxh.html

read -rp "请输入: " ans
来源：http://hz.kuanghao11.cn/gtixrjfgpw.html

[R78] 交互式菜单
来源：http://hz.0kj1m.cn/gtokdelwiy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gogol.net.cn/gtxyaqsvgx.html

[R79] 解析命令行选项
来源：http://hz.dianchejie.cn/gtrykezwta.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shuidangran.top/gtubhgspsm.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtyamnozym.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gtygdemjsy.html

================================================================================
来源：http://hz.zhongyouzk.top/gtptrisxxt.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtqgkeucoh.html

================================================================================
来源：http://hz.guowangkeji.top/gtdwucblfn.html

[S01] C：Hello World
来源：http://hz.redwolf501.top/gtuiirgaej.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtmxxxkhgf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fzhhl.top/gtbhyokuat.html

[S02] C：变量与格式化输出
来源：http://hz.cucudq.cn/gtnmbcfcwj.html

int a = 10; printf("%d\n", a);
来源：http://hz.svipenyu.cn/gtbjkutqwi.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtxknusnzf.html

int x; scanf("%d", &x);
来源：http://hz.wangdashe.top/gtpaiwksvz.html

[S04] C：字符串复制
来源：http://hz.cqqwz.cn/gtzgoshknx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtulplzulw.html

[S05] C：字符串长度
来源：http://hz.yonumen.top/gtatwcstfi.html

strlen(s)
来源：http://hz.yj202588.top/gtmuwwhkeu.html

[S06] C：字符串比较
来源：http://hz.chenlongwang.top/gtardqkptx.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtfqwfnvfs.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtejqysrko.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hfpthk.cn/gtsaymdedq.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtydsuwbdh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pengpengdd.cyou/gtkjeiloum.html

[S09] C：结构体定义与初始化
来源：http://hz.nwbrower.top/gtqecjyqfi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgufenzy.top/gtsvhsgbxq.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtztpevatg.html

int *p = &a;  *p = 5;
来源：http://hz.nanxinkj.top/gtpxyeiokz.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtbyqoomej.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuxming.cn/gtyybixssn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tianlin.xyz/gthoczedpw.html

fclose(f);
来源：http://hz.nanxuanxn.top/gtfesinlvh.html

[S12] C：写文件
来源：http://hz.chenjidiqi.icu/gteaankceo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhijiandao.cn/gtaebhaxus.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtpyooemtn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gtbqxdbzdq.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtwtjduegu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gttvylskbg.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtdwovdbno.html

(double) a / b
来源：http://hz.hnxiangtu.top/gtlmwvqsfp.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtrpuimodu.html

x |= (1 << 3);
来源：http://hz.ppjwa.cn/gtplzywxvr.html

[S17] C：安全拼接字符串
来源：http://hz.cheryme.top/gttzxpszvp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258888.top/gtptclwlmq.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gtrtakrgki.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtejkdbmfi.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtjognchqd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtbwexitrx.html

[S20] C：二分查找
来源：http://hz.zycfv.cn/gtjbyofhwe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtrbitnabw.html

[S21] C：字符类别判断
来源：http://hz.jqgufenzy.top/gteribetjp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangtech.top/gtygpdoquk.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtliekpfbk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtlvyqipga.html

[S23] C：随机数
来源：http://hz.jqgfzy.top/gtzbeofrvz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtuuihasdx.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtkijquihf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenjidiqi.icu/gtmwhjzpvm.html

[S25] C：内存拷贝
来源：http://hz.daria6918.cn/gtzwtfqjqt.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtfhnkditp.html

[S26] C：内存清零
来源：http://hz.sysykeji.top/gtvodyqqoy.html

memset(a, 0, sizeof a);
来源：http://hz.hywenlv.cn/gtvovmxxjz.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtdgarinmx.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtayszfeaz.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtbgtuwzeq.html

static int counter = 0;
来源：http://hz.nanxuanxn.top/gtjuesmzzs.html

[S29] C：变参函数
来源：http://hz.pengpengdd.cyou/gtikbrahcr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fzhhl.top/gtusltgacv.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtmztbeenj.html

#ifndef X_H
来源：http://hz.bjfxy.top/gtpnlnaeph.html

#define X_H
来源：http://hz.jqgufenzy.top/gtaxbpjnyr.html

#endif
来源：http://hz.9152youxi.cn/gtsaeptvqc.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtbellwjda.html

#include <iostream>
来源：http://hz.gotoacloud.top/gtqmbykctu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tianlin.xyz/gtlwxdpkqg.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtwpaysody.html

std::string s = "hi";  s += "!";
来源：http://hz.feifeiyinyue.top/gtggmxklhc.html

[S33] C++：vector 增删
来源：http://hz.jlsjyb.cn/gtydsszkhs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gtfefixzmv.html

[S34] C++：遍历 vector
来源：http://hz.birdmap.top/gtqkkgclja.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgufenzy.top/gtkmrtvxzf.html

[S35] C++：map
来源：http://hz.316326.xyz/gtmoztkxrq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtgphtfhvr.html

[S36] C++：unordered_map
来源：http://hz.zhaomingkeji.xyz/gtqdgmxycz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gteqrtbvgf.html

[S37] C++：set
来源：http://hz.xylfe.cn/gtercrouza.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtfpikxchi.html

[S38] C++：排序
来源：http://hz.hnxiangtu.top/gtbqkkkivn.html

std::sort(v.begin(), v.end());
来源：http://hz.fzhhl.top/gtvrmgkckm.html

[S39] C++：自定义比较器排序
来源：http://hz.chenzaomai.com/gtbffuytdb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtnqnkvbsr.html

[S40] C++：查找元素
来源：http://hz.nwbrower.top/gtdegkbsxq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tanke756.top/gtbektszei.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtoscjbxjx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtnibaltor.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtauuczawg.html

class B : public Base { public: void f() override {} };
来源：http://hz.quarkkingdee.top/gtczglhuim.html

[S43] C++：智能指针
来源：http://hz.chenlongwang.top/gtiivjqioa.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gtfgvizrui.html

[S44] C++：引用传参
来源：http://hz.yuanzhike.top/gtlpfluwke.html

void inc(int &x) { ++x; }
来源：http://hz.ydjk.org.cn/gtmsfcawrk.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtjveovrij.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtjxcdtcuu.html

[S46] C++：函数模板
来源：http://hz.xuanzx.com/gtdjuurelx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gaohongyu789.top/gtbpgrlqvn.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gtuayeikly.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtdwmcfpju.html

[S48] C++：逐行读文件
来源：http://hz.jinqigfzy.top/gtslbiqfft.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtqbfeuomt.html

while (std::getline(in, line)) { }
来源：http://hz.haohaochexian.top/gtsclyxdux.html

[S49] C++：写文件
来源：http://hz.c1oappe.top/gteujcepdp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuanzhike.top/gtnxpdehub.html

[S50] C++：格式化数字
来源：http://hz.redwolf501.top/gtjkahrvzw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ybcxt.top/gtibnlfdiw.html

[S51] C++：显式类型转换
来源：http://hz.shangyingyoupin.top/gtnxvotuqk.html

static_cast<double>(a) / b
来源：http://hz.pycfn.com/gteimwwsge.html

[S52] C++：const 与 noexcept
来源：http://hz.ehwqpu.com/gtmvskhwlu.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtnajwuesu.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtnahiwmeb.html

std::vector<int> w = std::move(v);
来源：http://hz.sxryk.cn/gtinvfhofg.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtvqjzufjc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.vqdsnc.cn/gtaeolkvvt.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtavgucpva.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cheryme.top/gtmignlnmm.html

[S56] C++：optional
来源：http://hz.meibo888.top/gtckjqgvkl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shuidangran.top/gtrbuksvsd.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtwecmquqo.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtrlcjkdza.html

[S58] C++：命名空间
来源：http://hz.hongshengwenyu.top/gtzrnlxeow.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhaomingkeji.xyz/gthskfugdo.html

[S59] C++：静态断言
来源：http://hz.zhixingplan.top/gtvpbkiilb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hfpthk.cn/gtwtsuyqso.html

[S60] C++：遍历并删除元素
来源：http://hz.sysykeji.top/gtcovweexq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtelogenun.html

================================================================================
来源：http://hz.ydjk.org.cn/gthrtozcpy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtiyxxkxbq.html

================================================================================
来源：http://hz.hnqzz.top/gtvchnnavg.html

[T01] Kotlin：Hello World
来源：http://hz.zhoulong.xyz/gtjweuempj.html

println("Hello")
来源：http://hz.wangdashe.top/gtdwjbbpqw.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtxriwnucd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yueranfly.top/gtgajzezss.html

[T03] Kotlin：字符串模板
来源：http://hz.c1oappe.top/gtjmfvqerk.html

"值: $b"
来源：http://hz.hnxiangtu.top/gteoprmsak.html

[T04] Kotlin：空安全
来源：http://hz.wangshuangyany.cn/gthlbdfcnf.html

val n: String? = null;  n?.length
来源：http://hz.meibo888.top/gtscxiqner.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtyesphiwg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zdqjudy.top/gtlfmsrdaw.html

[T06] Kotlin：集合映射
来源：http://hz.hnqzz.top/gtntsnwhso.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtenabjnnp.html

[T07] Kotlin：集合过滤
来源：http://hz.zhengqikj.top/gtlymmlxae.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtygavjvyy.html

[T08] Kotlin：数据类
来源：http://hz.andypj.xyz/gtanwfwuam.html

data class User(val name: String, val age: Int)
来源：http://hz.zhiwuduotai.top/gtgjralgyx.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gttpqhamei.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gtdsgbxsgf.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtmtygjfhj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cdnleiting.top/gtafnisxay.html

[T11] Kotlin：协程
来源：http://hz.sufxvd.cn/gtczsykaxa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.andypj.xyz/gtkiclkcll.html

[T12] Kotlin：解构声明
来源：http://hz.sysykeji.top/gtlctukobe.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgufenzy.top/gtfjazjnzl.html

[T13] Kotlin：只读 Map
来源：http://hz.guannengcc.top/gtvuvlhbgp.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtsugalqcv.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtvnxguuct.html

for (i in 1..10) println(i)
来源：http://hz.hongshengwenyu.top/gtmuzuaysy.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtpnfygdar.html

interface Shape { fun area(): Double }
来源：http://hz.cqqwz.cn/gtcokoulur.html

[T16] Swift：Hello World
来源：http://hz.haohaochexian.top/gtacnlgszy.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtrujqkaeb.html

[T17] Swift：变量与常量
来源：http://hz.andypj.xyz/gtqksmxxnm.html

var a = 1;  let b = 2
来源：http://hz.pengpengdd.cyou/gtpycsinhc.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtoqpbwpji.html

"值: \(b)"
来源：http://hz.shzxlz.cn/gtrsuifljo.html

[T19] Swift：可选绑定
来源：http://hz.zhijiandao.cn/gtrtggexcc.html

if let n = opt { print(n) }
来源：http://hz.kuanghao11.cn/gtrwlxwlio.html

[T20] Swift：数组操作
来源：http://hz.zhaomingkeji.xyz/gtdyygkndk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtwecquryc.html

[T21] Swift：遍历
来源：http://hz.shuidangran.top/gttswvnsra.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtxwgfxdvb.html

[T22] Swift：字典
来源：http://hz.tianlin.xyz/gthdnzvtjb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtfmazavhh.html

[T23] Swift：函数
来源：http://hz.zhiwuduotai.top/gtjihkyceg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gttvbvqytd.html

[T24] Swift：闭包
来源：http://hz.tianlin.xyz/gtygaerkea.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtcvnemqem.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtrupikgyl.html

struct P { var x: Int }
来源：http://hz.xziqi.cn/gtrojjtlay.html

[T26] Swift：类与重写
来源：http://hz.ybcxt.top/gtafuoebaf.html

class A: Base { override func f() {} }
来源：http://hz.xuanzx.com/gtfayicwwk.html

[T27] Swift：错误处理
来源：http://hz.cdnleiting.top/gtbbjogeva.html

do { try f() } catch { print(error) }
来源：http://hz.hnqzz.top/gtwiwlaskt.html

[T28] Swift：枚举
来源：http://hz.mhx1999.top/gtmotcqylv.html

enum Color { case red, green }
来源：http://hz.xziqi.cn/gtioyzwbuf.html

[T29] Swift：guard 提前返回
来源：http://hz.ywan-chungtsiang.top/gtgzlahdck.html

guard let x = opt else { return }
来源：http://hz.jinqigfzy.top/gthlulqtpt.html

[T30] Swift：协议
来源：http://hz.zhiwuduotai.top/gtszskwwuy.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtlsrgsmlf.html

[T31] Lua：Hello World
来源：http://hz.xinyue.icu/gtbzbnbhsq.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtridzacbj.html

[T32] Lua：局部变量
来源：http://hz.haohaochexian.top/gtcvkrazeo.html

local a = 1
来源：http://hz.xuetiantiany.cn/gttsptnwpd.html

[T33] Lua：表（数组）
来源：http://hz.ivvv.top/gtirrxwowp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gtxkltmkpd.html

[T34] Lua：遍历表
来源：http://hz.hongshengwenyu.top/gtslyhekfv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hywenlv.cn/gtulwalnpo.html

[T35] Lua：字典表
来源：http://hz.ehwqpu.com/gtxfroucip.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tianlin.xyz/gtefcibawl.html

[T36] Lua：函数
来源：http://hz.zdqjudy.top/gtuibcsdyu.html

function add(a, b) return a + b end
来源：http://hz.yonumen.top/gtfwxoedse.html

[T37] Lua：字符串拼接
来源：http://hz.shuidangran.top/gtapfbxgtw.html

"a" .. "b"
来源：http://hz.jiagoushi.top/gtqcaazsou.html

[T38] Lua：条件
来源：http://hz.hysaishi.cn/gtcqgaluvi.html

if x > 0 then print("正") end
来源：http://hz.jinqigufen.top/gtgjeefczc.html

[T39] Lua：模式匹配
来源：http://hz.jinqigfzy.top/gtugfiqvcm.html

string.find(s, "%d+")
来源：http://hz.jqgufenzy.top/gtjiqdnzwl.html

[T40] Lua：元表
来源：http://hz.jianghu66.top/gtcxlavzvd.html

setmetatable({}, { __index = base })
来源：http://hz.yangfankeji.com/gtqpwidrmd.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtekodzrlm.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gtgduihayo.html

[T42] Perl：变量类型
来源：http://hz.cashguo.top/gtkgyjjogt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ydzc1.top/gtnvvbpjiw.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtnuncrrjl.html

"值: $a"
来源：http://hz.gaohongyu789.top/gtepjejund.html

[T44] Perl：条件
来源：http://hz.chenzaomai.com/gtqqyzoxmn.html

if ($a > 0) { print "正"; }
来源：http://hz.cashguo.top/gtlfafqgqq.html

[T45] Perl：数组遍历
来源：http://hz.nanxinkj.top/gtlqvjwgwy.html

for my $x (@arr) { print $x; }
来源：http://hz.yonumen.top/gtgwldeqcx.html

[T46] Perl：哈希操作
来源：http://hz.zhixingplan.top/gtdxifikuz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuxming.cn/gtfvcykswt.html

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gtpeiyzqfo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenlongwang.top/gtpvziwhyt.html

[T48] Perl：正则替换
来源：http://hz.sxryk.cn/gtuqimtwbc.html

$s =~ s/old/new/g;
来源：http://hz.shangyingyoupin.top/gtjjlrqzni.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtkqkltpac.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yvedp.cn/gtpvadyhdp.html

[T50] Perl：逐行读文件
来源：http://hz.cqqwz.cn/gtcqufowgp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sysykeji.top/gttrwnxgeo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj20258888.top/gteksujcko.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtxmlacqvt.html

println("Hello")
来源：http://hz.hammf.cn/gtsgaqnbxx.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtvfsssgxs.html

val a = 1;  var b = 2
来源：http://hz.fengsongda.top/gtpidltrop.html

[T53] Scala：字符串插值
来源：http://hz.pycfn.com/gtnnmppkxp.html

s"值: $b"
来源：http://hz.smart0.xyz/gtglqmedrl.html

[T54] Scala：集合映射
来源：http://hz.aibaodan.cn/gtigvfqhmd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cdnleiting.top/gtehrojqfi.html

[T55] Scala：集合过滤
来源：http://hz.sufxvd.cn/gtjtwkpbvv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhaomingkeji.xyz/gtfrvjkcat.html

[T56] Scala：样例类
来源：http://hz.kuanghao11.cn/gteaysozlp.html

case class User(name: String, age: Int)
来源：http://hz.sweek.top/gtwenlvtmt.html

[T57] Scala：模式匹配
来源：http://hz.pengpengdd.cyou/gtjgufhxkm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ehwqpu.com/gtwvehlvve.html

[T58] Scala：函数定义
来源：http://hz.hysaishi.cn/gtpzqlyjmy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gtoptxuehu.html

[T59] Scala：循环
来源：http://hz.guowangkeji.top/gtlwypsrtz.html

for (i <- 1 to 10) println(i)
来源：http://hz.zycfv.cn/gtvmqgimgj.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtevweiawh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuetiantiany.cn/gtjfdddvmw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtczzgglke.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtebfeqlud.html

================================================================================
来源：http://hz.jinqigufen.top/gtykvleuue.html

[U01] Py：创建虚拟环境
来源：http://hz.shangyingyoupin.top/gtfxpofdjf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgfzy.top/gteweuxwtu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.c1oappe.top/gtuwyzfwud.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cheryme.top/gtsocthzug.html

[U03] Py：加载 .env 配置
来源：http://hz.zhiwuduotai.top/gtvevsdunm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ehwqpu.com/gtjpfpdivb.html

[U04] Py：变量调试打印
来源：http://hz.tianlin.xyz/gtnmqmpmxs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.havefunace.top/gtvakyabua.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigfzy.top/gtawtfpadu.html

list(dict.fromkeys(arr))
来源：http://hz.xingfuxueyuan.xyz/gtqttznlfw.html

[U06] Py：合并两个字典
来源：http://hz.nwbrower.top/gtelqfwhva.html

{**a, **b}
来源：http://hz.snrcjt.cn/gtjyhgeqsi.html

[U07] Py：反转字典键值
来源：http://hz.gzhubu.top/gtwhrsabay.html

{v: k for k, v in d.items()}
来源：http://hz.zycfv.cn/gtgdchiwen.html

[U08] Py：展平二维列表
来源：http://hz.tianlin.xyz/gtrkicqpar.html

[y for x in nested for y in x]
来源：http://hz.zycfv.cn/gthdzebdhl.html

[U09] Py：字典取最大值的键
来源：http://hz.yangfankeji.com/gtxizmmayv.html

max(d, key=d.get)
来源：http://hz.hywenlv.cn/gtpkewwnjv.html

[U10] Py：按值排序字典
来源：http://hz.zhijiandao.cn/gtqhfavfry.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtrgynwuba.html

[U11] Py：生成器表达式
来源：http://hz.yj202588.top/gtwgkrbdpk.html

(x * 2 for x in arr)
来源：http://hz.guannengcc.top/gtrpkguyex.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.iojbl.cn/gtwqyslxis.html

Counter(arr).most_common(3)
来源：http://hz.guowangkeji.top/gtokqcmfkh.html

[U13] Py：固定长度队列
来源：http://hz.pengpengdd.cyou/gtifjrprep.html

deque(maxlen=10)
来源：http://hz.zycfv.cn/gtiakwvxzv.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtozyqcjfe.html

defaultdict(list)
来源：http://hz.aizwys.cn/gtvfmnscpq.html


<!-- 参考信息 -->