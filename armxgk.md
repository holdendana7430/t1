代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydzc1.top/gtpcxnkrfb.html

[R72] 等待端口就绪
来源：http://hz.sysykeji.top/gtjhhnqymg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dashuyun.cn/gtcupmratf.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtvlozjebi.html

split -l 1000 big.log part_
来源：http://hz.zhaomingkeji.xyz/gtqeqebtwy.html

[R74] 批量重命名
来源：http://hz.daria6918.cn/gttwmvoqvp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuanzhike.top/gtbdlzsmzc.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtauouqjip.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cqqwz.cn/gtoiikbssd.html

[R76] 使用临时文件
来源：http://hz.yonumen.top/gtwlfiumtz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tianlin.xyz/gtrzvnxakf.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtacqvalua.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtoiksclfp.html

[R78] 交互式菜单
来源：http://hz.xylfe.cn/gtvlpdtssq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gthhhnkbqu.html

[R79] 解析命令行选项
来源：http://hz.zhixingplan.top/gtaqzxmung.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.meibo888.top/gtqzvyojri.html

[R80] 查看脚本执行耗时
来源：http://hz.dashuyun.cn/gtutzmicji.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtuzqzlcsb.html

================================================================================
来源：http://hz.andypj.xyz/gtxjqmcolm.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtdsdrcdpg.html

================================================================================
来源：http://hz.ydzc1.top/gtxjhliojh.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtfpvbzzcv.html

#include <stdio.h>
来源：http://hz.jqgufenzy.top/gtenjlbouv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shzxlz.cn/gtmbcrhvtg.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtfejbulmm.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtjgohhuvr.html

[S03] C：读入整数
来源：http://hz.zhongyouzk.top/gtsafnttxf.html

int x; scanf("%d", &x);
来源：http://hz.yueranfly.top/gtenrodpjo.html

[S04] C：字符串复制
来源：http://hz.jinqigfzy.top/gtdtsbcchl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258.top/gtmpeqhbyq.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtxpgwvkza.html

strlen(s)
来源：http://hz.cqqwz.cn/gtiggxdbqu.html

[S06] C：字符串比较
来源：http://hz.cashguo.top/gtyaafusbd.html

strcmp(a, b) == 0
来源：http://hz.meibo888.top/gtkitpvzzw.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gtlkzhmbzp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.havefunace.top/gtppzkiprp.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gteybhznup.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtohubiggp.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gturiwvbkj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtjzddznzn.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtkwjnbbed.html

int *p = &a;  *p = 5;
来源：http://hz.daxiang520.top/gtivcppqil.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gtkjswkfad.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtfgrkdsqk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhiwuduotai.top/gtkfhpujwa.html

fclose(f);
来源：http://hz.shuidangran.top/gtpnfpkdcr.html

[S12] C：写文件
来源：http://hz.shanyushiyangtech.top/gtqggoxdbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.snrcjt.cn/gtidjnhfmz.html

[S13] C：宏定义
来源：http://hz.ybcxt.top/gtxskwphun.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gthfltnbzj.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtutqpxxed.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenjidiqi.icu/gtvbnanwfd.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtzbyudtdc.html

(double) a / b
来源：http://hz.zycfv.cn/gtpkeympre.html

[S16] C：位操作置位
来源：http://hz.yj20258888.top/gtgdifjfqi.html

x |= (1 << 3);
来源：http://hz.shanyushiyangtech.top/gtatcekfjq.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtzlorshgo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangshuangyany.cn/gteblxdkhu.html

[S18] C：命令行参数
来源：http://hz.c1oappe.top/gthjcdytst.html

int main(int argc, char **argv)
来源：http://hz.wangshuangyany.cn/gtosvzaiam.html

[S19] C：快速排序
来源：http://hz.ppjwa.cn/gtumqllwjd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtugzwwjbo.html

[S20] C：二分查找
来源：http://hz.yuxming.cn/gtgicrjibu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gtlfdooohw.html

[S21] C：字符类别判断
来源：http://hz.ydzc1.top/gtpocxgpkv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuanzx.com/gtvwgmjgnx.html

[S22] C：字符串转数字
来源：http://hz.cheryme.top/gtluudwhda.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtmngyljnk.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtvidznbnw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangkeji.top/gtxyxwrizu.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gtdxupbobt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtgqtrxkjg.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtugpcwehy.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtxfoxgypo.html

[S26] C：内存清零
来源：http://hz.jinqigufen.top/gtfsghokuq.html

memset(a, 0, sizeof a);
来源：http://hz.hnqzz.top/gtaftiayrt.html

[S27] C：定义常量
来源：http://hz.jinqigufen.top/gtigrmtalc.html

const double PI = 3.14159;
来源：http://hz.hammf.cn/gthkvgucye.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gtxuqrpqrr.html

static int counter = 0;
来源：http://hz.svipenyu.cn/gttwifxdtx.html

[S29] C：变参函数
来源：http://hz.ywan-chungtsiang.top/gtknexlsgo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigufen.top/gtnxjrnblg.html

[S30] C：头文件保护
来源：http://hz.hnxiangtu.top/gtqhmdgghi.html

#ifndef X_H
来源：http://hz.yj20258888.top/gtwjeieigq.html

#define X_H
来源：http://hz.guowangkeji.top/gtxukbjwzt.html

#endif
来源：http://hz.shanyushiyangtech.top/gttemkzaxd.html

[S31] C++：Hello World
来源：http://hz.chenjidiqi.icu/gtbgttkvxo.html

#include <iostream>
来源：http://hz.meibo888.top/gtdezdpcki.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cdnleiting.top/gteegusixn.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtvhfubaio.html

std::string s = "hi";  s += "!";
来源：http://hz.sysykeji.top/gtkttikepq.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtpdeucvde.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtsuxuwory.html

[S34] C++：遍历 vector
来源：http://hz.ivvv.top/gtjvwrxldy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hfpthk.cn/gtunjvbfmg.html

[S35] C++：map
来源：http://hz.yonumen.top/gtjwswfopy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtzdsprske.html

[S36] C++：unordered_map
来源：http://hz.havefunace.top/gtnklriyvp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtoauvzctc.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtixzklepk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cqqwz.cn/gtbtczotwg.html

[S38] C++：排序
来源：http://hz.sxryk.cn/gteqlarlhf.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtipeqltgf.html

[S39] C++：自定义比较器排序
来源：http://hz.zdqjudy.top/gtyxyxorqz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.316326.xyz/gtlrdctfhs.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtlffuosro.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ywan-chungtsiang.top/gtxdinbcrh.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtzxvofwdl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xingfuxueyuan.xyz/gtwqbfnked.html

[S42] C++：继承与虚函数
来源：http://hz.hongshengwenyu.top/gtdfgexuvd.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhixingplan.top/gtnjeitbdd.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtyyyedbgz.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuxming.cn/gtqpfbexss.html

[S44] C++：引用传参
来源：http://hz.tian-w.cn/gtdfkhvhzs.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtoegwqdkk.html

[S45] C++：lambda
来源：http://hz.hnxiangtu.top/gtbttkxvnw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jyoumei.cn/gtjvnyksym.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtfbgqhmmp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xingfuxueyuan.xyz/gtgkzbhvpj.html

[S47] C++：结构化绑定遍历
来源：http://hz.yanxiufei.cn/gtfxitgwrp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtihykigzg.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gtgixyjkmz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xinyue.icu/gteghvvhgr.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtfijqaevm.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtjxyasyrs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zdqjudy.top/gtqykxvjla.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtxmezmfvy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhiwuduotai.top/gtwspingbj.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gtclrodubh.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtdhlagigw.html

[S52] C++：const 与 noexcept
来源：http://hz.shuidangran.top/gtrqbujcmw.html

int size() const noexcept { return n_; }
来源：http://hz.cheryme.top/gtgttufrbt.html

[S53] C++：移动语义
来源：http://hz.jinyuanbaomall.cn/gtuhqylyaw.html

std::vector<int> w = std::move(v);
来源：http://hz.hywenlv.cn/gtpirytdrw.html

[S54] C++：异常处理
来源：http://hz.chenzaomai.com/gteeecirks.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ivvv.top/gtcpwgfmpl.html

[S55] C++：结构化绑定
来源：http://hz.jinghuilouyu.cn/gtrztlyoax.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gtpohjxusf.html

[S56] C++：optional
来源：http://hz.gogol.net.cn/gtwbytxaub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhijiandao.cn/gtvfwgljwo.html

[S57] C++：编译期常量
来源：http://hz.cqqwz.cn/gtdtgfhcxp.html

constexpr int N = 10;
来源：http://hz.chenjidiqi.icu/gtomxvymyf.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gthvvaxzdm.html

namespace ns { int f() { return 1; } }
来源：http://hz.iojbl.cn/gtkpvzicrt.html

[S59] C++：静态断言
来源：http://hz.yj20258888.top/gtaqvyvahf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtdjalwdxc.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtypsyzdus.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtlchvnlzl.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgtxzyrmg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtpfvobfjo.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttovthrwk.html

[T01] Kotlin：Hello World
来源：http://hz.52xcode.cn/gtipcsfmwz.html

println("Hello")
来源：http://hz.birdmap.top/gtrkcfyzdy.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gthxqksrzx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fengsongda.top/gtervfoxtl.html

[T03] Kotlin：字符串模板
来源：http://hz.cheryme.top/gtznyojzoq.html

"值: $b"
来源：http://hz.hnqzz.top/gttzfsndjy.html

[T04] Kotlin：空安全
来源：http://hz.yuanzhike.top/gtgpxlgdif.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtlwlfvcly.html

[T05] Kotlin：when 表达式
来源：http://hz.smart0.xyz/gtakxtpgvu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtndiwngvt.html

[T06] Kotlin：集合映射
来源：http://hz.yueranfly.top/gtldunxgje.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtnvkyyice.html

[T07] Kotlin：集合过滤
来源：http://hz.zhoulong.xyz/gtwbtplqvh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nwbrower.top/gtaezvyait.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtgbgwqjbj.html

data class User(val name: String, val age: Int)
来源：http://hz.tian-w.cn/gttarpxblj.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxuanxn.top/gtdvoztdfb.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258.top/gtqjqbovji.html

[T10] Kotlin：默认参数
来源：http://hz.chenzaomai.com/gtozmfkwjo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuxming.cn/gtabgaccst.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtbincrugz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenjidiqi.icu/gtfbuqviji.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gtpsufneit.html

val (a, b) = Pair(1, 2)
来源：http://hz.aizwys.cn/gtyzjqcpsq.html

[T13] Kotlin：只读 Map
来源：http://hz.sufxvd.cn/gtdkfystkl.html

val m = mapOf("a" to 1)
来源：http://hz.xuetiantiany.cn/gtjxxwyyvh.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gtugggpntk.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtjhmswobt.html

[T15] Kotlin：接口
来源：http://hz.hnxiangtu.top/gttamprbph.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gtifayhjmy.html

[T16] Swift：Hello World
来源：http://hz.daxiang520.top/gtesjaztku.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtoqznfxfl.html

[T17] Swift：变量与常量
来源：http://hz.yuxming.cn/gtjozqlbai.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtspzxzuil.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtfephmhmu.html

"值: \(b)"
来源：http://hz.shanyushiyangtech.top/gtyjikzcmo.html

[T19] Swift：可选绑定
来源：http://hz.smart0.xyz/gtogmfihta.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gtvbjvdyge.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangkeji.top/gtdtvxxkfx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.c1oappe.top/gthzlmuvkk.html

[T21] Swift：遍历
来源：http://hz.hysaishi.cn/gtdwkdfyuo.html

for x in a { print(x) }
来源：http://hz.yonumen.top/gtegcxtgcl.html

[T22] Swift：字典
来源：http://hz.hywenlv.cn/gtneshyjqf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.52xcode.cn/gtppambkvb.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtxppxrshr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.316326.xyz/gtcpxlfdcq.html

[T24] Swift：闭包
来源：http://hz.meibo888.top/gtsajohnhb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhengqikj.top/gtqfttzhzi.html

[T25] Swift：结构体
来源：http://hz.jinqigfzy.top/gtthnhuydc.html

struct P { var x: Int }
来源：http://hz.ywan-chungtsiang.top/gtoyltayfz.html

[T26] Swift：类与重写
来源：http://hz.jinghuilouyu.cn/gtvngdonei.html

class A: Base { override func f() {} }
来源：http://hz.0kj1m.cn/gtnantzlid.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtdahhaemp.html

do { try f() } catch { print(error) }
来源：http://hz.ehwqpu.com/gtjjuforjh.html

[T28] Swift：枚举
来源：http://hz.nanxuanxn.top/gtbhstclzs.html

enum Color { case red, green }
来源：http://hz.svipenyu.cn/gtzrhykxdz.html

[T29] Swift：guard 提前返回
来源：http://hz.9152youxi.cn/gtfwdwyrgw.html

guard let x = opt else { return }
来源：http://hz.yonumen.top/gtoyswzgbw.html

[T30] Swift：协议
来源：http://hz.9152youxi.cn/gtkxkpuqay.html

protocol Shape { func area() -> Double }
来源：http://hz.xuanzx.com/gtxywmptdj.html

[T31] Lua：Hello World
来源：http://hz.chenzaomai.com/gtkforloym.html

print("Hello")
来源：http://hz.sweek.top/gtftqlntth.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gthrgjugxo.html

local a = 1
来源：http://hz.gaohongyu789.top/gtbwdpwoon.html

[T33] Lua：表（数组）
来源：http://hz.feifeiyinyue.top/gtejocliui.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuetiantiany.cn/gtdpgyyjvp.html

[T34] Lua：遍历表
来源：http://hz.ybcxt.top/gtpwlarvuc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hfpthk.cn/gtxbzayedn.html

[T35] Lua：字典表
来源：http://hz.ppjwa.cn/gtbbpytkfx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gogol.net.cn/gtgtkmmbfc.html

[T36] Lua：函数
来源：http://hz.dianchejie.cn/gtnqmopvtd.html

function add(a, b) return a + b end
来源：http://hz.shzxlz.cn/gtdsscwhyq.html

[T37] Lua：字符串拼接
来源：http://hz.zhixingplan.top/gtahrdyrkb.html

"a" .. "b"
来源：http://hz.hnxiangtu.top/gtanjwycjv.html

[T38] Lua：条件
来源：http://hz.yj202588.top/gtizselpiw.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gtfkwrnkhn.html

[T39] Lua：模式匹配
来源：http://hz.hfpthk.cn/gtuocxrazz.html

string.find(s, "%d+")
来源：http://hz.zhengqikj.top/gtgqoxzsxf.html

[T40] Lua：元表
来源：http://hz.snrcjt.cn/gtzilrvjtf.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigufen.top/gtprxdqoaa.html

[T41] Perl：Hello World
来源：http://hz.ehwqpu.com/gtlyniqnup.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtgoiskeke.html

[T42] Perl：变量类型
来源：http://hz.jinqigfzy.top/gtogzzktow.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtwzwbxkvv.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtgupmeiws.html

"值: $a"
来源：http://hz.ybcxt.top/gttbwjvlka.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtnlnvjzer.html

if ($a > 0) { print "正"; }
来源：http://hz.cqqwz.cn/gtvxkaubjy.html

[T45] Perl：数组遍历
来源：http://hz.jiagoushi.top/gtdnjdzlwi.html

for my $x (@arr) { print $x; }
来源：http://hz.aibaodan.cn/gtbtwhtyha.html

[T46] Perl：哈希操作
来源：http://hz.hongshengwenyu.top/gtitfavjez.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.havefunace.top/gtbhzwkcep.html

[T47] Perl：正则捕获
来源：http://hz.zhoulong.xyz/gtpwkjjwkt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtuuooxoba.html

[T48] Perl：正则替换
来源：http://hz.xingfuxueyuan.xyz/gteuhysddl.html

$s =~ s/old/new/g;
来源：http://hz.zdqjudy.top/gtreuqtwnu.html

[T49] Perl：函数
来源：http://hz.kuanghao11.cn/gtnqhealoh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtxyzhcyfq.html

[T50] Perl：逐行读文件
来源：http://hz.nwbrower.top/gtnvqkzksy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtyfrhvlwg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenjidiqi.icu/gtcjtucztf.html

[T51] Scala：Hello World
来源：http://hz.yuanzhike.top/gtxmkyqesj.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtlyezhoeu.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtvailnqaz.html

val a = 1;  var b = 2
来源：http://hz.cdnleiting.top/gtsiieluco.html

[T53] Scala：字符串插值
来源：http://hz.cqqwz.cn/gteazbgvys.html

s"值: $b"
来源：http://hz.yanxiufei.cn/gttijglkid.html

[T54] Scala：集合映射
来源：http://hz.yongpay.top/gtlihjarox.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhoulong.xyz/gtkbkluviy.html

[T55] Scala：集合过滤
来源：http://hz.wangshuangyany.cn/gtjqjrputr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sxryk.cn/gtywqpthex.html

[T56] Scala：样例类
来源：http://hz.hysaishi.cn/gtyegsoeeg.html

case class User(name: String, age: Int)
来源：http://hz.xziqi.cn/gtqpfgnwfs.html

[T57] Scala：模式匹配
来源：http://hz.xuetiantiany.cn/gtqrvlovnd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtlpgvluap.html

[T58] Scala：函数定义
来源：http://hz.zhijiandao.cn/gtqghvokwg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hywenlv.cn/gtuylgrpjp.html

[T59] Scala：循环
来源：http://hz.fzhhl.top/gtakheoooz.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtjfmiafib.html

[T60] Scala：折叠
来源：http://hz.birdmap.top/gtfnmkecuv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yvedp.cn/gtcimzygaf.html

================================================================================
来源：http://hz.fengsongda.top/gtkttrfvma.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cashguo.top/gtwxdmnqlr.html

================================================================================
来源：http://hz.yongpay.top/gtethajvrx.html

[U01] Py：创建虚拟环境
来源：http://hz.aizwys.cn/gtqigzbimf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guannengcc.top/gtjblvlywn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cheryme.top/gtyzpbpqkj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.guannengcc.top/gtlnkauyjb.html

[U03] Py：加载 .env 配置
来源：http://hz.birdmap.top/gthqxgpisp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhijiandao.cn/gtymulsbfi.html

[U04] Py：变量调试打印
来源：http://hz.zhoulong.xyz/gtbvqmcwwj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xinyue.icu/gtmwxzpvgu.html

[U05] Py：列表去重且保序
来源：http://hz.jyoumei.cn/gtzevksvil.html

list(dict.fromkeys(arr))
来源：http://hz.ybcxt.top/gtlejbsmyc.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangtech.top/gtwnvevzui.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gtzvjbacwr.html

[U07] Py：反转字典键值
来源：http://hz.tanke756.top/gtdipvmfuz.html

{v: k for k, v in d.items()}
来源：http://hz.hfpthk.cn/gtabeqmwth.html

[U08] Py：展平二维列表
来源：http://hz.yj20258888.top/gtlpbkpxmj.html

[y for x in nested for y in x]
来源：http://hz.chenzaomai.com/gteqkaryxt.html

[U09] Py：字典取最大值的键
来源：http://hz.9152youxi.cn/gthnixnvrr.html

max(d, key=d.get)
来源：http://hz.0kj1m.cn/gtxkrriysp.html

[U10] Py：按值排序字典
来源：http://hz.daxiang520.top/gtrsdbihru.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinghuilouyu.cn/gtarbcoxld.html

[U11] Py：生成器表达式
来源：http://hz.316326.xyz/gtbdgvbhlr.html

(x * 2 for x in arr)
来源：http://hz.zycfv.cn/gtmjhitejk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jiagoushi.top/gtqxkfmhsa.html

Counter(arr).most_common(3)
来源：http://hz.kuanghao11.cn/gtytxvrrov.html


<!-- 参考信息 -->