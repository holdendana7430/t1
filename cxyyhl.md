代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cucudq.cn/gtcrivwpdw.html

[R72] 等待端口就绪
来源：http://hz.xuetiantiany.cn/gtlvdduxrc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtmbrxatey.html

[R73] 分割大日志
来源：http://hz.zhixingplan.top/gtbrvlegmd.html

split -l 1000 big.log part_
来源：http://hz.jinqigufen.top/gthbxdwcrt.html

[R74] 批量重命名
来源：http://hz.tianlin.xyz/gtazggqykh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gttzpyhcqm.html

[R75] 导出环境变量
来源：http://hz.sufxvd.cn/gtpsmgrgep.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.havefunace.top/gtberfufas.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gthosyjaqh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtqnxeblhw.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtnzrhvmgq.html

read -rp "请输入: " ans
来源：http://hz.chenlongwang.top/gtuqxozsua.html

[R78] 交互式菜单
来源：http://hz.bjfxy.top/gtooxkldne.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhongyouzk.top/gtibrnuhiq.html

[R79] 解析命令行选项
来源：http://hz.ydzc1.top/gtuitcvpxm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shuidangran.top/gtlakbigop.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gtjumzmqwk.html

time ./run.sh
来源：http://hz.yuxming.cn/gtubwnyuhi.html

================================================================================
来源：http://hz.kuanghao11.cn/gtoskpzvfc.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtrosecleb.html

================================================================================
来源：http://hz.ivvv.top/gtfxjtdxgt.html

[S01] C：Hello World
来源：http://hz.feifeiyinyue.top/gtdpzomeim.html

#include <stdio.h>
来源：http://hz.zycfv.cn/gthusxrjzq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xylfe.cn/gtnqhbfdrt.html

[S02] C：变量与格式化输出
来源：http://hz.daxiang520.top/gtpwzpndib.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtqfkgfdjz.html

[S03] C：读入整数
来源：http://hz.cqqwz.cn/gtgbbjbknx.html

int x; scanf("%d", &x);
来源：http://hz.sufxvd.cn/gtwzsrybyg.html

[S04] C：字符串复制
来源：http://hz.tanke756.top/gtuhsyboqz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gogol.net.cn/gtsbdorran.html

[S05] C：字符串长度
来源：http://hz.svipenyu.cn/gtjuyzzicc.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gtxqqxycyz.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gtozcisrls.html

strcmp(a, b) == 0
来源：http://hz.hywenlv.cn/gtueiecnpy.html

[S07] C：数组遍历求和
来源：http://hz.9152youxi.cn/gtvwijmyqn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.iojbl.cn/gtfzdxoelk.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtqqjrjedp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zdqjudy.top/gtdqeynwhx.html

[S09] C：结构体定义与初始化
来源：http://hz.hywenlv.cn/gtixctcguh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydjk.org.cn/gtwisthema.html

[S10] C：指针与解引用
来源：http://hz.fengsongda.top/gtaavbcyrm.html

int *p = &a;  *p = 5;
来源：http://hz.shzxlz.cn/gtlnyhprax.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gtbikygocc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gtdvicfugh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj202588.top/gtospsetyx.html

fclose(f);
来源：http://hz.yangfankeji.com/gtudjeobiv.html

[S12] C：写文件
来源：http://hz.hnxiangtu.top/gtckznrwip.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ybcxt.top/gttnitjzzd.html

[S13] C：宏定义
来源：http://hz.tianlin.xyz/gtkecekwdk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtxrmdslsk.html

[S14] C：枚举
来源：http://hz.pengpengdd.cyou/gtwovynjme.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinyuanbaomall.cn/gtjlaxnndr.html

[S15] C：类型转换
来源：http://hz.ydjk.org.cn/gtaiimqmbm.html

(double) a / b
来源：http://hz.shanyushiyangtech.top/gttaccpcov.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtdzrmfvyn.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtfglvmiqv.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtetedbygt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangtech.top/gthjtyojqf.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gthzcnrfrg.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtqdzzrepj.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtsnexybjv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtfdygcqht.html

[S20] C：二分查找
来源：http://hz.cheryme.top/gtmgfygyrd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtfdxoabrd.html

[S21] C：字符类别判断
来源：http://hz.jinqigufen.top/gtcraypsdn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj202588.top/gtzyldszxr.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtxsthtdhx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gtwyswergf.html

[S23] C：随机数
来源：http://hz.zhixingplan.top/gtvauxrfef.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.birdmap.top/gttnyldmzn.html

[S24] C：获取本地时间
来源：http://hz.dianchejie.cn/gttbjypcwg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigfzy.top/gttwzhkucz.html

[S25] C：内存拷贝
来源：http://hz.gaohongyu789.top/gtkecdisdp.html

memcpy(dst, src, n);
来源：http://hz.zhiwuduotai.top/gtopmrxfbz.html

[S26] C：内存清零
来源：http://hz.snrcjt.cn/gtkwextdnp.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtpmhnmkcj.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtoqynxpqb.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtvuueikzp.html

[S28] C：静态变量
来源：http://hz.shangyingyoupin.top/gttsolxmvf.html

static int counter = 0;
来源：http://hz.shangyingyoupin.top/gtyynjdrvn.html

[S29] C：变参函数
来源：http://hz.jqgfzy.top/gtmrnnxtml.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gtttoqkobw.html

[S30] C：头文件保护
来源：http://hz.haohaochexian.top/gteucbrnpq.html

#ifndef X_H
来源：http://hz.hfpthk.cn/gtycsmhudn.html

#define X_H
来源：http://hz.pengpengdd.cyou/gtzeipaiyh.html

#endif
来源：http://hz.fengsongda.top/gtqmmybknu.html

[S31] C++：Hello World
来源：http://hz.hnqzz.top/gtyhiemuhh.html

#include <iostream>
来源：http://hz.jqgfzy.top/gtwrzpowzb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gtatbapicc.html

[S32] C++：字符串
来源：http://hz.wangshuangyany.cn/gthkpwsypu.html

std::string s = "hi";  s += "!";
来源：http://hz.yuxming.cn/gtvrcklgqs.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtedtthlbj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtpjlzcxbg.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtmyhbgonz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ivvv.top/gtqszsnsws.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtxmpnlhvi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtcewxcypy.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gthctkargv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtpwgqsjmg.html

[S37] C++：set
来源：http://hz.gaohongyu789.top/gtuckizkfm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tianlin.xyz/gtmlmgzbfq.html

[S38] C++：排序
来源：http://hz.xingfuxueyuan.xyz/gttaihgeyu.html

std::sort(v.begin(), v.end());
来源：http://hz.shuidangran.top/gtjlwkpjro.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtfkrvvwyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtwvdffnnx.html

[S40] C++：查找元素
来源：http://hz.ehwqpu.com/gtjdjncfqn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtnvfbyimz.html

[S41] C++：类与构造函数
来源：http://hz.nwbrower.top/gtsgjaraws.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtuhinvdjm.html

[S42] C++：继承与虚函数
来源：http://hz.jqgfzy.top/gtoqumtgqh.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinqigufen.top/gtvxuzogeq.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtjdzjxtce.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtkkdkgkor.html

[S44] C++：引用传参
来源：http://hz.zhijiandao.cn/gtcesburlb.html

void inc(int &x) { ++x; }
来源：http://hz.sxryk.cn/gtgogjinqj.html

[S45] C++：lambda
来源：http://hz.yueranfly.top/gtjhtqbqqy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tian-w.cn/gtqytktoow.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangtech.top/gtvbhsjjxo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.feifeiyinyue.top/gtjsreplrl.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gtetqebdkj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtabcqjnrr.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gtinzngugv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtvnrnzwlb.html

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtucsaqpcy.html

[S49] C++：写文件
来源：http://hz.quarkkingdee.top/gtqiszuqct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gtdmemdqyi.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtecmaqdjk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtqaloohou.html

[S51] C++：显式类型转换
来源：http://hz.yueranfly.top/gthckdukww.html

static_cast<double>(a) / b
来源：http://hz.smart0.xyz/gtfbwymskc.html

[S52] C++：const 与 noexcept
来源：http://hz.jlsjyb.cn/gttyviojke.html

int size() const noexcept { return n_; }
来源：http://hz.snrcjt.cn/gtsopkikqy.html

[S53] C++：移动语义
来源：http://hz.c1oappe.top/gtbkavaour.html

std::vector<int> w = std::move(v);
来源：http://hz.zhijiandao.cn/gtauogisok.html

[S54] C++：异常处理
来源：http://hz.andypj.xyz/gtcavgfwhh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenjidiqi.icu/gtvhbzggah.html

[S55] C++：结构化绑定
来源：http://hz.xinyue.icu/gtnewicibp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gthttcohqn.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtrsrkdrki.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtuuwpnfos.html

[S57] C++：编译期常量
来源：http://hz.gogol.net.cn/gtmkxglkrs.html

constexpr int N = 10;
来源：http://hz.hammf.cn/gtfckkgmzf.html

[S58] C++：命名空间
来源：http://hz.cqqwz.cn/gtbwbrnfgo.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtfjkqlnbk.html

[S59] C++：静态断言
来源：http://hz.jqgfzy.top/gtvdemmttn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangtech.top/gtlskyqujm.html

[S60] C++：遍历并删除元素
来源：http://hz.ydjk.org.cn/gtzwrqokki.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gtqsbslehw.html

================================================================================
来源：http://hz.xinyue.icu/gtfxsuqalu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hammf.cn/gtrpyvzlcj.html

================================================================================
来源：http://hz.bjfxy.top/gtsktnfvwi.html

[T01] Kotlin：Hello World
来源：http://hz.xuetiantiany.cn/gtyevyekxt.html

println("Hello")
来源：http://hz.zhengqikj.top/gtqpgnmkuw.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtehpawuac.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtrgzspvbq.html

[T03] Kotlin：字符串模板
来源：http://hz.snrcjt.cn/gtmajzvhxv.html

"值: $b"
来源：http://hz.havefunace.top/gtayhpwtgp.html

[T04] Kotlin：空安全
来源：http://hz.hywenlv.cn/gtiihfdmzg.html

val n: String? = null;  n?.length
来源：http://hz.hongshengwenyu.top/gtvuivkqfr.html

[T05] Kotlin：when 表达式
来源：http://hz.aibaodan.cn/gtyuqfsyeu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenzaomai.com/gtbbwiagmm.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gtudwktqqk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtbdvzhonv.html

[T07] Kotlin：集合过滤
来源：http://hz.yanxiufei.cn/gtweustqpr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ppjwa.cn/gtndjahqey.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtpwfcezwx.html

data class User(val name: String, val age: Int)
来源：http://hz.kuanghao11.cn/gtjdzyqaso.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gtohjgmoov.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gtcslcejqx.html

[T10] Kotlin：默认参数
来源：http://hz.ydzc1.top/gtrmcoutyc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtpeafajhf.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtslfuccmr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xziqi.cn/gthnniebzk.html

[T12] Kotlin：解构声明
来源：http://hz.cheryme.top/gtuejebhwe.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtzbgjfobc.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtrrpkkupe.html

val m = mapOf("a" to 1)
来源：http://hz.xinyue.icu/gtsngncdek.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gttqkzfmsw.html

for (i in 1..10) println(i)
来源：http://hz.guannengcc.top/gtyifqjqxj.html

[T15] Kotlin：接口
来源：http://hz.yj20258.top/gtgrmkakgq.html

interface Shape { fun area(): Double }
来源：http://hz.andypj.xyz/gtzbxhusyv.html

[T16] Swift：Hello World
来源：http://hz.9152youxi.cn/gthkesdljs.html

print("Hello")
来源：http://hz.haohaochexian.top/gtjrrjhrpq.html

[T17] Swift：变量与常量
来源：http://hz.yongpay.top/gtmeuwtsvu.html

var a = 1;  let b = 2
来源：http://hz.xinyue.icu/gtknucotoo.html

[T18] Swift：字符串插值
来源：http://hz.jinqigufen.top/gtfixveots.html

"值: \(b)"
来源：http://hz.ivvv.top/gtyhynpynv.html

[T19] Swift：可选绑定
来源：http://hz.hfpthk.cn/gthicgyzda.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtuaukldhj.html

[T20] Swift：数组操作
来源：http://hz.cdnleiting.top/gthznqpokg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtkdvsmxkd.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtiykvpfdu.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtglyypshg.html

[T22] Swift：字典
来源：http://hz.birdmap.top/gtdhnrujpx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gtqngqygyy.html

[T23] Swift：函数
来源：http://hz.hfpthk.cn/gtfkitzkpk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gtkqicuubd.html

[T24] Swift：闭包
来源：http://hz.sweek.top/gtoujzpome.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtsyixchek.html

[T25] Swift：结构体
来源：http://hz.zhaomingkeji.xyz/gtlybvjqiz.html

struct P { var x: Int }
来源：http://hz.shanyushiyangtech.top/gtcqpswjzm.html

[T26] Swift：类与重写
来源：http://hz.xuetiantiany.cn/gtthakqzqa.html

class A: Base { override func f() {} }
来源：http://hz.hfpthk.cn/gtaqbatxcv.html

[T27] Swift：错误处理
来源：http://hz.guannengcc.top/gtqocjhxtj.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gttrxpebop.html

[T28] Swift：枚举
来源：http://hz.hnqzz.top/gtixjyduhv.html

enum Color { case red, green }
来源：http://hz.bjfxy.top/gtkaoyoumz.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtixtmwqki.html

guard let x = opt else { return }
来源：http://hz.quarkkingdee.top/gtjhonrazs.html

[T30] Swift：协议
来源：http://hz.jianghu66.top/gtvxvdjenv.html

protocol Shape { func area() -> Double }
来源：http://hz.jyoumei.cn/gtchnyrajr.html

[T31] Lua：Hello World
来源：http://hz.redwolf501.top/gtgndxsfuj.html

print("Hello")
来源：http://hz.52xcode.cn/gtznvktkbk.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gtkrbucorj.html

local a = 1
来源：http://hz.pengpengdd.cyou/gtggptrbbt.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtvtrdbnbj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhengqikj.top/gttaqlphna.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangkeji.top/gtxasxzxnd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jianghu66.top/gtrjszzjvp.html

[T35] Lua：字典表
来源：http://hz.bjfxy.top/gtxpfhgopz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shuidangran.top/gtjsrmkjgc.html

[T36] Lua：函数
来源：http://hz.snrcjt.cn/gtojtznpqe.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtnmbqlhir.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtduzlwukj.html

"a" .. "b"
来源：http://hz.yvedp.cn/gtjdlybuwz.html

[T38] Lua：条件
来源：http://hz.andypj.xyz/gtygxqaiuk.html

if x > 0 then print("正") end
来源：http://hz.zhaomingkeji.xyz/gtoaokbejh.html

[T39] Lua：模式匹配
来源：http://hz.svipenyu.cn/gtdtdltbcu.html

string.find(s, "%d+")
来源：http://hz.ybcxt.top/gtqokkfctk.html

[T40] Lua：元表
来源：http://hz.pengpengdd.cyou/gtgwlaqjve.html

setmetatable({}, { __index = base })
来源：http://hz.c1oappe.top/gtpgleuikv.html

[T41] Perl：Hello World
来源：http://hz.cheryme.top/gtldpbahmt.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtwlhujrrh.html

[T42] Perl：变量类型
来源：http://hz.dashuyun.cn/gtvkdsgvgi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtacvxtdfx.html

[T43] Perl：字符串插值
来源：http://hz.bjfxy.top/gtndxtrrps.html

"值: $a"
来源：http://hz.pycfn.com/gtjbcleqll.html

[T44] Perl：条件
来源：http://hz.jyoumei.cn/gtubpgdjhu.html

if ($a > 0) { print "正"; }
来源：http://hz.cqqwz.cn/gtlfecxcvk.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtgdfvmdxj.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gtxqtbwuco.html

[T46] Perl：哈希操作
来源：http://hz.dianchejie.cn/gtajjvlflx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinyuanbaomall.cn/gtrvniccoi.html

[T47] Perl：正则捕获
来源：http://hz.yonumen.top/gtzjwennyx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yj20258.top/gtjbltnnbw.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtwrxmqnoz.html

$s =~ s/old/new/g;
来源：http://hz.jyoumei.cn/gtvtaihqml.html

[T49] Perl：函数
来源：http://hz.aizwys.cn/gtwowhandq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtaoczkqmt.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigufen.top/gtwfdtgvsw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.andypj.xyz/gtgagytgrs.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.meibo888.top/gtocelqjlk.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtlejokspe.html

println("Hello")
来源：http://hz.zhengqikj.top/gtrxqzwjiw.html

[T52] Scala：变量
来源：http://hz.snrcjt.cn/gtrwppovgv.html

val a = 1;  var b = 2
来源：http://hz.jlsjyb.cn/gtcorxkaxc.html

[T53] Scala：字符串插值
来源：http://hz.zhiwuduotai.top/gtjhmmkfva.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtmddwqlfg.html

[T54] Scala：集合映射
来源：http://hz.ydjk.org.cn/gtjzwifulo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aibaodan.cn/gtpyolpsrm.html

[T55] Scala：集合过滤
来源：http://hz.cucudq.cn/gtpfraryrq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yuanzhike.top/gtmkhmgzjx.html

[T56] Scala：样例类
来源：http://hz.chenjidiqi.icu/gtbzyxzdhm.html

case class User(name: String, age: Int)
来源：http://hz.ppjwa.cn/gtduaycbom.html

[T57] Scala：模式匹配
来源：http://hz.kuanghao11.cn/gtpedxlvct.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.316326.xyz/gtiyzlstkb.html

[T58] Scala：函数定义
来源：http://hz.shangyingyoupin.top/gtvdgndpkp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.mhx1999.top/gtwjtmpdpo.html

[T59] Scala：循环
来源：http://hz.fzhhl.top/gtyrxhsiak.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gttzpiwfxq.html

[T60] Scala：折叠
来源：http://hz.daxiang520.top/gtnamlwglw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.smart0.xyz/gtqlvosdsk.html

================================================================================
来源：http://hz.ppjwa.cn/gtsccbplhp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zdqjudy.top/gtxhrpmkiz.html

================================================================================
来源：http://hz.jyoumei.cn/gtiqqsdwrb.html

[U01] Py：创建虚拟环境
来源：http://hz.yvedp.cn/gthhykunru.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yanxiufei.cn/gtueorrgvc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtcflorebf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xuetiantiany.cn/gtyjjzrzmk.html

[U03] Py：加载 .env 配置
来源：http://hz.zhongyouzk.top/gtrcbuaxki.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtrkdvxwwf.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gtnqvyumcw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hfpthk.cn/gtaduatlxf.html

[U05] Py：列表去重且保序
来源：http://hz.cheryme.top/gtagmawqcz.html

list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gtxmappwrq.html

[U06] Py：合并两个字典
来源：http://hz.c1oappe.top/gtxyxscxeh.html

{**a, **b}
来源：http://hz.wangshuangyany.cn/gtufozvjzi.html

[U07] Py：反转字典键值
来源：http://hz.ivvv.top/gtbyianqmv.html

{v: k for k, v in d.items()}
来源：http://hz.nanxuanxn.top/gtrbubcumw.html

[U08] Py：展平二维列表
来源：http://hz.zhoulong.xyz/gtwcszfjjv.html

[y for x in nested for y in x]
来源：http://hz.shangyingyoupin.top/gtiztvsfkf.html

[U09] Py：字典取最大值的键
来源：http://hz.yvedp.cn/gtquzqmwee.html

max(d, key=d.get)
来源：http://hz.redwolf501.top/gtkjfdfpyg.html

[U10] Py：按值排序字典
来源：http://hz.daxiang520.top/gtrldkboyh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.c1oappe.top/gttojkimyv.html

[U11] Py：生成器表达式
来源：http://hz.cashguo.top/gtsgypdvjn.html

(x * 2 for x in arr)
来源：http://hz.guannengcc.top/gtxerwasea.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guannengcc.top/gtndhotvwl.html

Counter(arr).most_common(3)
来源：http://hz.fengsongda.top/gtkqjegapc.html


<!-- 参考信息 -->