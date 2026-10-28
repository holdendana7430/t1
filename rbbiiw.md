代发 wailian999

split -l 1000 big.log part_
来源：http://hz.shanyushiyangtech.top/gtmrwgohye.html

[R74] 批量重命名
来源：http://hz.tian-w.cn/gtuznpreyd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuxming.cn/gtjxuqvaft.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtcrkoahpg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtcjinqvag.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtuivelwny.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtubynxuhz.html

[R77] 读取用户输入
来源：http://hz.sufxvd.cn/gtyyeibbfn.html

read -rp "请输入: " ans
来源：http://hz.ivvv.top/gtvqdivczy.html

[R78] 交互式菜单
来源：http://hz.yj202588.top/gttnvjjrul.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhoulong.xyz/gtpvuvwvwv.html

[R79] 解析命令行选项
来源：http://hz.svipenyu.cn/gtqfayybqt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aibaodan.cn/gtlnmpphya.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtcomqedhx.html

time ./run.sh
来源：http://hz.jinghuilouyu.cn/gtwkrxcujr.html

================================================================================
来源：http://hz.xylfe.cn/gtpwuobqlo.html

S. C / C++ 专题
来源：http://hz.yuxming.cn/gtliccqjcn.html

================================================================================
来源：http://hz.52xcode.cn/gtvxdqtkud.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gtcjyphejv.html

#include <stdio.h>
来源：http://hz.jinyuanbaomall.cn/gtsezhpcfb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtyoibqcnn.html

[S02] C：变量与格式化输出
来源：http://hz.jiagoushi.top/gtmxudxsxs.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gtwxjwgqwl.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtftzauuuc.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtfhsibjnn.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtmsczhazn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtjkcjdllx.html

[S05] C：字符串长度
来源：http://hz.fengsongda.top/gtbgxszwqm.html

strlen(s)
来源：http://hz.gaohongyu789.top/gtwfyjlqfz.html

[S06] C：字符串比较
来源：http://hz.gzhubu.top/gtffoswnnb.html

strcmp(a, b) == 0
来源：http://hz.aizwys.cn/gtqpvurmdw.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gtujdomkqv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cqqwz.cn/gtjeuyttbr.html

[S08] C：动态内存分配与释放
来源：http://hz.ywan-chungtsiang.top/gtgdlqttbv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zdqjudy.top/gtszdfaqbb.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gtkgddyago.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtfcqrqpnr.html

[S10] C：指针与解引用
来源：http://hz.sufxvd.cn/gtpfwkinjh.html

int *p = &a;  *p = 5;
来源：http://hz.vqdsnc.cn/gtkftnbqpi.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtnivrwynw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangtech.top/gtsxlgcqap.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.iojbl.cn/gtnvrgujmc.html

fclose(f);
来源：http://hz.redwolf501.top/gtvjzwubnx.html

[S12] C：写文件
来源：http://hz.gaohongyu789.top/gtsokzbdrq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tianlin.xyz/gthboukann.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtxaxmfduv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtlcizbjft.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtsaiqvblx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gtxelbnobt.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtoojxagxv.html

(double) a / b
来源：http://hz.pengpengdd.cyou/gtwowufnio.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtxniznjmg.html

x |= (1 << 3);
来源：http://hz.ybcxt.top/gtsufibxmi.html

[S17] C：安全拼接字符串
来源：http://hz.xuanzx.com/gtabokmdji.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangtech.top/gtcckrskbm.html

[S18] C：命令行参数
来源：http://hz.nanxinkj.top/gtlaspniyz.html

int main(int argc, char **argv)
来源：http://hz.yangfankeji.com/gtelgjhpxj.html

[S19] C：快速排序
来源：http://hz.bjfxy.top/gtywawjqni.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtxxlorrpi.html

[S20] C：二分查找
来源：http://hz.jinyuanbaomall.cn/gtrnznaruk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtmsyxamvn.html

[S21] C：字符类别判断
来源：http://hz.ppjwa.cn/gtufuafmek.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenjidiqi.icu/gtpuvyqcmu.html

[S22] C：字符串转数字
来源：http://hz.cqqwz.cn/gtfrqmmovw.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtpggxjphu.html

[S23] C：随机数
来源：http://hz.zhiwuduotai.top/gtdvxolyux.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj202588.top/gtzwxtzwlz.html

[S24] C：获取本地时间
来源：http://hz.fzhhl.top/gtgpvprvli.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtseusjcdu.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtmczbnfai.html

memcpy(dst, src, n);
来源：http://hz.jlsjyb.cn/gtythlutrt.html

[S26] C：内存清零
来源：http://hz.hnxiangtu.top/gtrpkbpgnt.html

memset(a, 0, sizeof a);
来源：http://hz.quarkkingdee.top/gtzkqhrmfw.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtctiirich.html

const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtvateiazv.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtkymqqkvd.html

static int counter = 0;
来源：http://hz.hongshengwenyu.top/gtlwrcfazb.html

[S29] C：变参函数
来源：http://hz.svipenyu.cn/gtxnwglvkf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtfnqvfqmg.html

[S30] C：头文件保护
来源：http://hz.havefunace.top/gtxqcvjzfg.html

#ifndef X_H
来源：http://hz.yanxiufei.cn/gtavgncvub.html

#define X_H
来源：http://hz.yj20258888.top/gtijfzjagf.html

#endif
来源：http://hz.hywenlv.cn/gtjpduntzj.html

[S31] C++：Hello World
来源：http://hz.xuetiantiany.cn/gtwyqmxwer.html

#include <iostream>
来源：http://hz.jinghuilouyu.cn/gtjqurgmqx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtderhgxfm.html

[S32] C++：字符串
来源：http://hz.zhoulong.xyz/gtdnlinsed.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtbaekdhys.html

[S33] C++：vector 增删
来源：http://hz.sweek.top/gtwaycrmkr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinghuilouyu.cn/gthaircfui.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gthekoiyfl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ppjwa.cn/gtqwjupcnz.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gtvpqxnrzl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtuvmexsxa.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtcacnewzt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtniwoprso.html

[S37] C++：set
来源：http://hz.yj20258.top/gtiiorgabe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.vqdsnc.cn/gtekqnakaz.html

[S38] C++：排序
来源：http://hz.haohaochexian.top/gtmiydtwbf.html

std::sort(v.begin(), v.end());
来源：http://hz.daxiang520.top/gtdyiwyxqq.html

[S39] C++：自定义比较器排序
来源：http://hz.jinyuanbaomall.cn/gtcydbigdc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aibaodan.cn/gtnfffdmzz.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtnpunlduz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jlsjyb.cn/gtazmxdive.html

[S41] C++：类与构造函数
来源：http://hz.nanxuanxn.top/gtflqtxdts.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtjyragqyw.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gtkadupfah.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gtcmdnswhq.html

[S43] C++：智能指针
来源：http://hz.cqqwz.cn/gtapbfypqz.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gtdyqldbkn.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtajskyzel.html

void inc(int &x) { ++x; }
来源：http://hz.iojbl.cn/gtjfzitqzq.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtctchthim.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gttqpplwek.html

[S46] C++：函数模板
来源：http://hz.hnqzz.top/gttcgsyovt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yonumen.top/gtjnduhfxj.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gtlbqfszmh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cheryme.top/gtespdthmz.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gtilsqedju.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtnpclrett.html

while (std::getline(in, line)) { }
来源：http://hz.yvedp.cn/gtueqezmea.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtohobmcgi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtwnwffjst.html

[S50] C++：格式化数字
来源：http://hz.ivvv.top/gtkhfrfctn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aizwys.cn/gtipthorgz.html

[S51] C++：显式类型转换
来源：http://hz.xuetiantiany.cn/gtasbvwmvt.html

static_cast<double>(a) / b
来源：http://hz.jinyuanbaomall.cn/gtdjkiiuua.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtoeeatnyd.html

int size() const noexcept { return n_; }
来源：http://hz.tanke756.top/gtdtnvhopg.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtpqwbhccq.html

std::vector<int> w = std::move(v);
来源：http://hz.zhongyouzk.top/gtwijpiigy.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtcocgsvlh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtzvfdblsb.html

[S55] C++：结构化绑定
来源：http://hz.dianchejie.cn/gtttqcdzvh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtuxxqrbtw.html

[S56] C++：optional
来源：http://hz.wangshuangyany.cn/gtuxkhaech.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.52xcode.cn/gtkrappqfn.html

[S57] C++：编译期常量
来源：http://hz.feifeiyinyue.top/gtgsflggeq.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gtacrzsfgf.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtxjuzqiik.html

namespace ns { int f() { return 1; } }
来源：http://hz.meibo888.top/gtdjrywffa.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtndcnlmvu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gthjpthajj.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gtujbhuyjc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtxhwpjvga.html

================================================================================
来源：http://hz.jianghu66.top/gtvfreirtu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtadjmgqre.html

================================================================================
来源：http://hz.316326.xyz/gtgvsykpxd.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gtufqbisfp.html

println("Hello")
来源：http://hz.xziqi.cn/gtbrhzruov.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtyaxopqfw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnxiangtu.top/gtjdwxbuml.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gtiinspfmr.html

"值: $b"
来源：http://hz.jinqigfzy.top/gtyoofxlnn.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtpstwqbtt.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtdovicdnd.html

[T05] Kotlin：when 表达式
来源：http://hz.birdmap.top/gtnjjruqgg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gtgomnlupn.html

[T06] Kotlin：集合映射
来源：http://hz.jinqigfzy.top/gtahlxweye.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gttfmksdej.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gtivbevctq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhiwuduotai.top/gtmmwwvsqp.html

[T08] Kotlin：数据类
来源：http://hz.yueranfly.top/gtcrqgfwvt.html

data class User(val name: String, val age: Int)
来源：http://hz.ppjwa.cn/gtpudkgqqn.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtnwpjslws.html

fun String.exclaim() = this + "!"
来源：http://hz.jlsjyb.cn/gtnhrwwkic.html

[T10] Kotlin：默认参数
来源：http://hz.aibaodan.cn/gtvadqxzim.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fengsongda.top/gtocrtvazr.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtiyywvdli.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangshuangyany.cn/gtlxwyngxe.html

[T12] Kotlin：解构声明
来源：http://hz.shangyingyoupin.top/gtnpikdnaq.html

val (a, b) = Pair(1, 2)
来源：http://hz.feifeiyinyue.top/gtglsztpgw.html

[T13] Kotlin：只读 Map
来源：http://hz.hnqzz.top/gtnoijyzei.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gthfpykcpv.html

[T14] Kotlin：循环
来源：http://hz.yj20258.top/gtchqgooaw.html

for (i in 1..10) println(i)
来源：http://hz.fengsongda.top/gtpnzvqbjd.html

[T15] Kotlin：接口
来源：http://hz.sxryk.cn/gtcznbqdac.html

interface Shape { fun area(): Double }
来源：http://hz.ydzc1.top/gtrryjzfpf.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtzdttdufo.html

print("Hello")
来源：http://hz.ybcxt.top/gtktzqralw.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtarndcxxa.html

var a = 1;  let b = 2
来源：http://hz.ydjk.org.cn/gtodnoshqe.html

[T18] Swift：字符串插值
来源：http://hz.yj20258888.top/gtibrkrxqj.html

"值: \(b)"
来源：http://hz.quarkkingdee.top/gtwhbbkzau.html

[T19] Swift：可选绑定
来源：http://hz.gotoacloud.top/gteagxhekg.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtmmvbdsbd.html

[T20] Swift：数组操作
来源：http://hz.andypj.xyz/gtckoeyhrr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgufenzy.top/gtpbhnkryh.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtwhzkevlb.html

for x in a { print(x) }
来源：http://hz.quarkkingdee.top/gtcsrvlfnq.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gttanbxhmv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sysykeji.top/gtcreitwpd.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtiejjzpui.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xylfe.cn/gthkzegddp.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtdswgjayk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hywenlv.cn/gtmgzrjyfo.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtqbbkizge.html

struct P { var x: Int }
来源：http://hz.svipenyu.cn/gtnootmbvr.html

[T26] Swift：类与重写
来源：http://hz.yangfankeji.com/gtivgypszp.html

class A: Base { override func f() {} }
来源：http://hz.pycfn.com/gtudqyfrgc.html

[T27] Swift：错误处理
来源：http://hz.yongpay.top/gteeukhohx.html

do { try f() } catch { print(error) }
来源：http://hz.jqgfzy.top/gtwlrdyoyz.html

[T28] Swift：枚举
来源：http://hz.zhongyouzk.top/gthxesxwdj.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtjcecroxz.html

[T29] Swift：guard 提前返回
来源：http://hz.havefunace.top/gtafnmleiz.html

guard let x = opt else { return }
来源：http://hz.jinqigufen.top/gtclnbfvzw.html

[T30] Swift：协议
来源：http://hz.mhx1999.top/gtqzsuncba.html

protocol Shape { func area() -> Double }
来源：http://hz.haohaochexian.top/gtzzqxckja.html

[T31] Lua：Hello World
来源：http://hz.zdqjudy.top/gtflkmxzoz.html

print("Hello")
来源：http://hz.bjfxy.top/gtcbjljush.html

[T32] Lua：局部变量
来源：http://hz.tanke756.top/gtigbbomgo.html

local a = 1
来源：http://hz.zycfv.cn/gtovgukkwj.html

[T33] Lua：表（数组）
来源：http://hz.zhiwuduotai.top/gttrgmbalm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnxiangtu.top/gtgtfqxcfd.html

[T34] Lua：遍历表
来源：http://hz.xuetiantiany.cn/gtcjuqvsxg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj20258.top/gtcbdvpesx.html

[T35] Lua：字典表
来源：http://hz.xinyue.icu/gtvfnabery.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuetiantiany.cn/gttjlajpgq.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtffyamgqf.html

function add(a, b) return a + b end
来源：http://hz.jinqigfzy.top/gtgkxugasf.html

[T37] Lua：字符串拼接
来源：http://hz.shzxlz.cn/gtuutgfqaa.html

"a" .. "b"
来源：http://hz.meibo888.top/gtnhtwebgo.html

[T38] Lua：条件
来源：http://hz.xuetiantiany.cn/gtkkprazos.html

if x > 0 then print("正") end
来源：http://hz.zhiwuduotai.top/gtnrmyscrs.html

[T39] Lua：模式匹配
来源：http://hz.xuanzx.com/gtqxytziyd.html

string.find(s, "%d+")
来源：http://hz.daxiang520.top/gtomqrghgq.html

[T40] Lua：元表
来源：http://hz.hfpthk.cn/gtohutwdop.html

setmetatable({}, { __index = base })
来源：http://hz.haohaochexian.top/gtnxsfekyf.html

[T41] Perl：Hello World
来源：http://hz.jinyuanbaomall.cn/gtsdmaryyl.html

print "Hello\n";
来源：http://hz.hongshengwenyu.top/gtvjbwywzu.html

[T42] Perl：变量类型
来源：http://hz.sxryk.cn/gteqaihfrl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxuanxn.top/gteaoxozqf.html

[T43] Perl：字符串插值
来源：http://hz.tianlin.xyz/gtjcafikdo.html

"值: $a"
来源：http://hz.jiagoushi.top/gtfvwxigrz.html

[T44] Perl：条件
来源：http://hz.yj20258888.top/gtbotcrbmg.html

if ($a > 0) { print "正"; }
来源：http://hz.zhongyouzk.top/gtrjomxyud.html

[T45] Perl：数组遍历
来源：http://hz.sweek.top/gtrxrgeoog.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gttzjrfbec.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gtxngovpmj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tian-w.cn/gtoztmurkv.html

[T47] Perl：正则捕获
来源：http://hz.jinghuilouyu.cn/gtlaqrhffg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinghuilouyu.cn/gtwcqmyzuh.html

[T48] Perl：正则替换
来源：http://hz.gzhubu.top/gtvvwgfgzd.html

$s =~ s/old/new/g;
来源：http://hz.nwbrower.top/gtyovywlek.html

[T49] Perl：函数
来源：http://hz.c1oappe.top/gtvwqajzpn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.0kj1m.cn/gtezpgnram.html

[T50] Perl：逐行读文件
来源：http://hz.xylfe.cn/gtvpjsrtle.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtudgrmwrp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gthxrvwljn.html

[T51] Scala：Hello World
来源：http://hz.quarkkingdee.top/gtunicxshh.html

println("Hello")
来源：http://hz.aibaodan.cn/gtervrhhys.html

[T52] Scala：变量
来源：http://hz.chenzaomai.com/gtlbnizbcz.html

val a = 1;  var b = 2
来源：http://hz.zhoulong.xyz/gtyhvvehfl.html

[T53] Scala：字符串插值
来源：http://hz.andypj.xyz/gtqzntqqto.html

s"值: $b"
来源：http://hz.ydjk.org.cn/gtjhogancb.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtmizbguem.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.52xcode.cn/gttgiohxln.html

[T55] Scala：集合过滤
来源：http://hz.yangfankeji.com/gtsqvzkazw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangtech.top/gtrmxhxilb.html

[T56] Scala：样例类
来源：http://hz.hnqzz.top/gtdeozuoxi.html

case class User(name: String, age: Int)
来源：http://hz.daria6918.cn/gtwnbuzfui.html

[T57] Scala：模式匹配
来源：http://hz.xinyue.icu/gtwwxxsbzj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hfpthk.cn/gtopgwslrr.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtesdffsfh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tanke756.top/gtnktntean.html

[T59] Scala：循环
来源：http://hz.chenzaomai.com/gtzlhudfqs.html

for (i <- 1 to 10) println(i)
来源：http://hz.yanxiufei.cn/gtigzbjzxe.html

[T60] Scala：折叠
来源：http://hz.xylfe.cn/gtnxpzqhga.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.birdmap.top/gteztukoqh.html

================================================================================
来源：http://hz.52xcode.cn/gttkndxepr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.guannengcc.top/gtpndcpfjn.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzsjzvqbe.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangkeji.top/gtbwidfgjf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ybcxt.top/gtvnjipmtc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtjbcwghzm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sysykeji.top/gtxdbfdlmh.html

[U03] Py：加载 .env 配置
来源：http://hz.aizwys.cn/gtctjqnmzf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydzc1.top/gtpoawbvvy.html

[U04] Py：变量调试打印
来源：http://hz.yuxming.cn/gtrpdujfkb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.daria6918.cn/gtpbiahzkr.html

[U05] Py：列表去重且保序
来源：http://hz.yuxming.cn/gteputujhz.html

list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gtogpcdbyp.html

[U06] Py：合并两个字典
来源：http://hz.ivvv.top/gttewyvkxc.html

{**a, **b}
来源：http://hz.yueranfly.top/gteaibzqpa.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtqlraihka.html

{v: k for k, v in d.items()}
来源：http://hz.ivvv.top/gtwplebdxx.html

[U08] Py：展平二维列表
来源：http://hz.9152youxi.cn/gtrrbwcteo.html

[y for x in nested for y in x]
来源：http://hz.zhoulong.xyz/gtexchptdk.html

[U09] Py：字典取最大值的键
来源：http://hz.quarkkingdee.top/gtasudxdex.html

max(d, key=d.get)
来源：http://hz.aibaodan.cn/gtrpyrcbyd.html

[U10] Py：按值排序字典
来源：http://hz.pengpengdd.cyou/gtheuxkzel.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gogol.net.cn/gtzvthtomd.html

[U11] Py：生成器表达式
来源：http://hz.ydjk.org.cn/gtptwuouue.html

(x * 2 for x in arr)
来源：http://hz.shzxlz.cn/gtjinyerpq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxuanxn.top/gtvhpbsbiw.html

Counter(arr).most_common(3)
来源：http://hz.snrcjt.cn/gtefhplggc.html

[U13] Py：固定长度队列
来源：http://hz.cashguo.top/gteuvhtmjt.html

deque(maxlen=10)
来源：http://hz.ppjwa.cn/gthwhukrfy.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtjynrxnkx.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtflmhfarh.html


<!-- 参考信息 -->