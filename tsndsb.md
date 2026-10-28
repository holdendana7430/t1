代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gtiovrktlr.html

[R70] 时间戳与互转
来源：http://hz.gotoacloud.top/gtjwgptvwv.html

date +%s;  date -d @1700000000
来源：http://hz.guowangkeji.top/gtxxzwrcxl.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtigqjnuzc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sysykeji.top/gtdwegbakm.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtyzewhcqh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtehonnqvn.html

[R73] 分割大日志
来源：http://hz.0kj1m.cn/gtqrngusmc.html

split -l 1000 big.log part_
来源：http://hz.yonumen.top/gtjkpwtdje.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtamlwrlpz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtbjesqmmw.html

[R75] 导出环境变量
来源：http://hz.pycfn.com/gtkegeliqk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtqpsbeeep.html

[R76] 使用临时文件
来源：http://hz.52xcode.cn/gtjhlktdoj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxinkj.top/gtznqfozlm.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gthdbvutei.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtalohfupo.html

[R78] 交互式菜单
来源：http://hz.hnqzz.top/gtawbjybdp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtcvahuutf.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtrtjdqjpb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtaifpgwrw.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtsosxywia.html

time ./run.sh
来源：http://hz.smart0.xyz/gtnsiqncln.html

================================================================================
来源：http://hz.redwolf501.top/gtlyjdeubs.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtttebfiml.html

================================================================================
来源：http://hz.ydzc1.top/gtporjsvuf.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gthziqnkdr.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtdoudfpin.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtrohljtpu.html

[S02] C：变量与格式化输出
来源：http://hz.fengsongda.top/gtcmfwflaf.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangdashe.top/gtgwwupotl.html

[S03] C：读入整数
来源：http://hz.smart0.xyz/gtyheyoycd.html

int x; scanf("%d", &x);
来源：http://hz.gotoacloud.top/gtfqlaqmkc.html

[S04] C：字符串复制
来源：http://hz.zhiwuduotai.top/gtyeftksqu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yueranfly.top/gtuldavkjb.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtyipinkox.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gtkvwmfzpp.html

[S06] C：字符串比较
来源：http://hz.zhixingplan.top/gtdopnutsb.html

strcmp(a, b) == 0
来源：http://hz.smart0.xyz/gtzzsupwth.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtizsmgoyq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgfzy.top/gtwhkwxxug.html

[S08] C：动态内存分配与释放
来源：http://hz.yonumen.top/gtxohjitmp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtwdojkagh.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtwbjndreu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gtlkdlxuwv.html

[S10] C：指针与解引用
来源：http://hz.iojbl.cn/gtsuhxwmck.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtdwhkallq.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtnzcjprrb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtnnvsvozy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gtbtqxewpy.html

fclose(f);
来源：http://hz.yuxming.cn/gtqzpcshsl.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtumdrzcry.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gtbusjvzbv.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gtjqwzsxpt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtrbjfydjt.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtabjwxene.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.mhx1999.top/gterccfjte.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtdzrzywmt.html

(double) a / b
来源：http://hz.aizwys.cn/gtiognnfvo.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtjxygxnxb.html

x |= (1 << 3);
来源：http://hz.shanyushiyangkeji.top/gtjsgbdhgm.html

[S17] C：安全拼接字符串
来源：http://hz.ydzc1.top/gtrqiwiwpw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhiwuduotai.top/gtmcoatghh.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gtscphemgb.html

int main(int argc, char **argv)
来源：http://hz.hysaishi.cn/gtdonvzvfy.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gtcrykhzrn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtxtmwwerp.html

[S20] C：二分查找
来源：http://hz.daxiang520.top/gtijfsheqy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtdgtcmaon.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtiapvanls.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtxfdzckqd.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtrvfoivxi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tian-w.cn/gthldhpfjo.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtebnmcjfi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tanke756.top/gtnlsktymv.html

[S24] C：获取本地时间
来源：http://hz.jinghuilouyu.cn/gtvbprhvor.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sysykeji.top/gtdynfeadq.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangkeji.top/gtjfwivaks.html

memcpy(dst, src, n);
来源：http://hz.yueranfly.top/gtbmgfbgtc.html

[S26] C：内存清零
来源：http://hz.ppjwa.cn/gtzrfltccc.html

memset(a, 0, sizeof a);
来源：http://hz.yangfankeji.com/gthlxmeijz.html

[S27] C：定义常量
来源：http://hz.bjfxy.top/gttemvlzeh.html

const double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gthxenaebx.html

[S28] C：静态变量
来源：http://hz.yonumen.top/gtvydkmaop.html

static int counter = 0;
来源：http://hz.redwolf501.top/gtcoeqogra.html

[S29] C：变参函数
来源：http://hz.tanke756.top/gtnrnofefw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtjfmfoexu.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtujnmackp.html

#ifndef X_H
来源：http://hz.dianchejie.cn/gtpbwszqic.html

#define X_H
来源：http://hz.aizwys.cn/gtshadixdm.html

#endif
来源：http://hz.jinqigfzy.top/gtjfudwkub.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtthmzfkbl.html

#include <iostream>
来源：http://hz.guowangkeji.top/gtarqvhfnc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tianlin.xyz/gtzdmrftbw.html

[S32] C++：字符串
来源：http://hz.9152youxi.cn/gtdnrhttac.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtqyppngca.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtvfffsxmj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtvvrjxxdu.html

[S34] C++：遍历 vector
来源：http://hz.guannengcc.top/gtsbluliyp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ppjwa.cn/gtysukkylo.html

[S35] C++：map
来源：http://hz.gzhubu.top/gtkqndxjef.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtrgteoylc.html

[S36] C++：unordered_map
来源：http://hz.jqgfzy.top/gtocofskqm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtzzmpmlns.html

[S37] C++：set
来源：http://hz.nanxuanxn.top/gtfomxcdxh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtciaedbrm.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtpvjqlelx.html

std::sort(v.begin(), v.end());
来源：http://hz.bjfxy.top/gtaankcwjl.html

[S39] C++：自定义比较器排序
来源：http://hz.hnxiangtu.top/gtwkwrncgs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtvidfetsw.html

[S40] C++：查找元素
来源：http://hz.zhoulong.xyz/gtkeukhutv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tianlin.xyz/gtvdtiykce.html

[S41] C++：类与构造函数
来源：http://hz.yj20258888.top/gtwvmulohh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtakcyfbti.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gtweiaixru.html

class B : public Base { public: void f() override {} };
来源：http://hz.daria6918.cn/gtngwngkbv.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gtavexzfgn.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtjuowwxip.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtmlongaec.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtwfpgbqja.html

[S45] C++：lambda
来源：http://hz.dianchejie.cn/gtazrfvddy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gttwnyzvov.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gtibksqunl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gttdwpfdzs.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydjk.org.cn/gtsqprdwbv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yanxiufei.cn/gtrzlzamei.html

[S48] C++：逐行读文件
来源：http://hz.hnqzz.top/gtkqpfclaf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinyuanbaomall.cn/gtriqyotzt.html

while (std::getline(in, line)) { }
来源：http://hz.zhengqikj.top/gtdljhgnif.html

[S49] C++：写文件
来源：http://hz.yonumen.top/gtjttohsnj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tanke756.top/gtiwcabfum.html

[S50] C++：格式化数字
来源：http://hz.hfpthk.cn/gtlfduqnid.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dianchejie.cn/gtdgzehxzs.html

[S51] C++：显式类型转换
来源：http://hz.jinqigufen.top/gtujjiqoou.html

static_cast<double>(a) / b
来源：http://hz.pycfn.com/gthtnvkkrd.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangkeji.top/gtkpfsaxup.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtvvsbrlxf.html

[S53] C++：移动语义
来源：http://hz.gzhubu.top/gtfpofjipm.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtfailrlxt.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtdrlnencs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhijiandao.cn/gtznwozakc.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gtfhopyypg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtaflvrjos.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gthmkytwvh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtjbupxsrs.html

[S57] C++：编译期常量
来源：http://hz.zycfv.cn/gtvwrwwldy.html

constexpr int N = 10;
来源：http://hz.gotoacloud.top/gtakancauo.html

[S58] C++：命名空间
来源：http://hz.hongshengwenyu.top/gtyhsnrkbx.html

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gtcdwolmov.html

[S59] C++：静态断言
来源：http://hz.guannengcc.top/gtwgwgcqzi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nwbrower.top/gtgungzzmy.html

[S60] C++：遍历并删除元素
来源：http://hz.tian-w.cn/gtavolmkxa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gthecjxefx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtafghrwuf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gtgmxiyarl.html

================================================================================
来源：http://hz.aibaodan.cn/gtfwvrvqhc.html

[T01] Kotlin：Hello World
来源：http://hz.hammf.cn/gtqcpqmzft.html

println("Hello")
来源：http://hz.yj202588.top/gtcomdcvsr.html

[T02] Kotlin：变量
来源：http://hz.jlsjyb.cn/gtqvwfplxr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daria6918.cn/gtqhdpukvg.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxuanxn.top/gtmoyfnufw.html

"值: $b"
来源：http://hz.snrcjt.cn/gtdgqvspmi.html

[T04] Kotlin：空安全
来源：http://hz.zhoulong.xyz/gtefsmsstv.html

val n: String? = null;  n?.length
来源：http://hz.aibaodan.cn/gtpyxcesnx.html

[T05] Kotlin：when 表达式
来源：http://hz.quarkkingdee.top/gthiagfwdn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtbakaksma.html

[T06] Kotlin：集合映射
来源：http://hz.gotoacloud.top/gtmruckmxa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtuixdavyt.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangtech.top/gtuowkkhsp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258888.top/gtyazgmnzi.html

[T08] Kotlin：数据类
来源：http://hz.yj20258.top/gtgoecoucx.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtvcztdebo.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtpvdzhlwx.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtjhizgvgc.html

[T10] Kotlin：默认参数
来源：http://hz.jlsjyb.cn/gtykegetxu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtlpdqdlvb.html

[T11] Kotlin：协程
来源：http://hz.zhoulong.xyz/gtpmwjelzl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtwuqywjpu.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258.top/gteaqxwqjq.html

val (a, b) = Pair(1, 2)
来源：http://hz.andypj.xyz/gthyysrwqt.html

[T13] Kotlin：只读 Map
来源：http://hz.pengpengdd.cyou/gtxtbkmvek.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtnpeppxkf.html

[T14] Kotlin：循环
来源：http://hz.zhaomingkeji.xyz/gtinxjtnrz.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtnetqlsya.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtuniajxls.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gtuqworjnq.html

[T16] Swift：Hello World
来源：http://hz.haohaochexian.top/gtewltwjkd.html

print("Hello")
来源：http://hz.xziqi.cn/gtjydhjhro.html

[T17] Swift：变量与常量
来源：http://hz.iojbl.cn/gtxuzyuygo.html

var a = 1;  let b = 2
来源：http://hz.hongshengwenyu.top/gtpcphuwud.html

[T18] Swift：字符串插值
来源：http://hz.haohaochexian.top/gtnvrpgzva.html

"值: \(b)"
来源：http://hz.jyoumei.cn/gtkvytcxhz.html

[T19] Swift：可选绑定
来源：http://hz.52xcode.cn/gtqmhbvvig.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtbbclczum.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtlvbjxjbh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtrymckhua.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gtpsgkoghy.html

for x in a { print(x) }
来源：http://hz.c1oappe.top/gttzrrrzan.html

[T22] Swift：字典
来源：http://hz.gzhubu.top/gtacphooko.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yongpay.top/gtxhgobwmi.html

[T23] Swift：函数
来源：http://hz.xuetiantiany.cn/gtcnebgzom.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gtmmdlffid.html

[T24] Swift：闭包
来源：http://hz.shangyingyoupin.top/gteviukeht.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tian-w.cn/gtkjurpgsu.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gtqqivjkxh.html

struct P { var x: Int }
来源：http://hz.xuanzx.com/gteykzgrso.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtufwyscsk.html

class A: Base { override func f() {} }
来源：http://hz.ppjwa.cn/gtlgzrroaa.html

[T27] Swift：错误处理
来源：http://hz.fzhhl.top/gtzmxlxmfh.html

do { try f() } catch { print(error) }
来源：http://hz.tanke756.top/gtpzkdyyzl.html

[T28] Swift：枚举
来源：http://hz.chenlongwang.top/gtmmifgthb.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtxmdebqpx.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gturualbqd.html

guard let x = opt else { return }
来源：http://hz.jinyuanbaomall.cn/gturfbsqkg.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtjvakxapt.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgufenzy.top/gtcfaoffzy.html

[T31] Lua：Hello World
来源：http://hz.wangshuangyany.cn/gturxltflb.html

print("Hello")
来源：http://hz.yueranfly.top/gtmaobpmen.html

[T32] Lua：局部变量
来源：http://hz.kuanghao11.cn/gtkrvjmsqh.html

local a = 1
来源：http://hz.shuidangran.top/gtynvbegdu.html

[T33] Lua：表（数组）
来源：http://hz.jinqigfzy.top/gtusrfykrg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hywenlv.cn/gtrqqwokzc.html

[T34] Lua：遍历表
来源：http://hz.hongshengwenyu.top/gtdjgbcgyl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aizwys.cn/gtvzsihlhw.html

[T35] Lua：字典表
来源：http://hz.bjfxy.top/gtxyspevsm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.redwolf501.top/gtkelegwli.html

[T36] Lua：函数
来源：http://hz.hongshengwenyu.top/gtvbggwhrg.html

function add(a, b) return a + b end
来源：http://hz.sxryk.cn/gtdshldkuw.html

[T37] Lua：字符串拼接
来源：http://hz.c1oappe.top/gtdeldvpla.html

"a" .. "b"
来源：http://hz.yj20258.top/gtlqjfsfti.html

[T38] Lua：条件
来源：http://hz.0kj1m.cn/gtjiusykbv.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangkeji.top/gtwezkrpse.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtubwcnodf.html

string.find(s, "%d+")
来源：http://hz.zhaomingkeji.xyz/gtgnqxejxf.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtaufedayc.html

setmetatable({}, { __index = base })
来源：http://hz.ehwqpu.com/gtrdvtpiyf.html

[T41] Perl：Hello World
来源：http://hz.hywenlv.cn/gtobnwyheh.html

print "Hello\n";
来源：http://hz.pengpengdd.cyou/gttfupynji.html

[T42] Perl：变量类型
来源：http://hz.tianlin.xyz/gtmujffzqn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.daria6918.cn/gtoznmdadh.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtevpfhnfd.html

"值: $a"
来源：http://hz.birdmap.top/gtvlzzaiki.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gtbcwrntxo.html

if ($a > 0) { print "正"; }
来源：http://hz.ydjk.org.cn/gtdmjkmkkl.html

[T45] Perl：数组遍历
来源：http://hz.c1oappe.top/gtmdbhweaz.html

for my $x (@arr) { print $x; }
来源：http://hz.pycfn.com/gtxnemcvar.html

[T46] Perl：哈希操作
来源：http://hz.cqqwz.cn/gtidxatnwk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.daria6918.cn/gtbshkjqqr.html

[T47] Perl：正则捕获
来源：http://hz.zhixingplan.top/gtfupexfyi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hfpthk.cn/gtexmzqhle.html

[T48] Perl：正则替换
来源：http://hz.jyoumei.cn/gtrtvmxggc.html

$s =~ s/old/new/g;
来源：http://hz.zycfv.cn/gtyxmmlpis.html

[T49] Perl：函数
来源：http://hz.chenzaomai.com/gtujgfxtpo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtoimehbzz.html

[T50] Perl：逐行读文件
来源：http://hz.havefunace.top/gtrqdvwucn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtbytimjxl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.quarkkingdee.top/gtufyytlkf.html

[T51] Scala：Hello World
来源：http://hz.nanxinkj.top/gtwergwzof.html

println("Hello")
来源：http://hz.aibaodan.cn/gtwobtyhhp.html

[T52] Scala：变量
来源：http://hz.ywan-chungtsiang.top/gtsbbffgow.html

val a = 1;  var b = 2
来源：http://hz.haohaochexian.top/gtogizgbbr.html

[T53] Scala：字符串插值
来源：http://hz.sweek.top/gtinhgbrpe.html

s"值: $b"
来源：http://hz.52xcode.cn/gtomkhykys.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtiqomosea.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gtfswktinh.html

[T55] Scala：集合过滤
来源：http://hz.hammf.cn/gtnxebiwen.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhoulong.xyz/gtqfydkxnl.html

[T56] Scala：样例类
来源：http://hz.iojbl.cn/gtjbnpdvys.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtvxjjuwyi.html

[T57] Scala：模式匹配
来源：http://hz.hongshengwenyu.top/gtneizmpkv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinqigufen.top/gtycdgfnzx.html

[T58] Scala：函数定义
来源：http://hz.cdnleiting.top/gtkozyxqvw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinghuilouyu.cn/gtpkqldabe.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gtsivnpyah.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuanzx.com/gttiupdmot.html

[T60] Scala：折叠
来源：http://hz.jlsjyb.cn/gtlsueumvy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.iojbl.cn/gtoacwpfgc.html

================================================================================
来源：http://hz.yvedp.cn/gtutktcmhw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtasmpmkcj.html

================================================================================
来源：http://hz.iojbl.cn/gtywrcvtdo.html

[U01] Py：创建虚拟环境
来源：http://hz.jyoumei.cn/gtzuvtminc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangtech.top/gtkmaioxut.html

[U02] Py：导出 / 安装依赖
来源：http://hz.smart0.xyz/gtvzljdkjr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtuhhkykfk.html

[U03] Py：加载 .env 配置
来源：http://hz.ybcxt.top/gtitbkpscn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yvedp.cn/gtiypbqnwi.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gtbdjzfndg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nwbrower.top/gtwztdxfjl.html

[U05] Py：列表去重且保序
来源：http://hz.havefunace.top/gtszmyzsib.html

list(dict.fromkeys(arr))
来源：http://hz.sweek.top/gtzxfjqboi.html

[U06] Py：合并两个字典
来源：http://hz.9152youxi.cn/gtnuwbcldn.html

{**a, **b}
来源：http://hz.yj20258888.top/gtivewwzjs.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gtcvyafdub.html

{v: k for k, v in d.items()}
来源：http://hz.ybcxt.top/gtiltvydjc.html

[U08] Py：展平二维列表
来源：http://hz.bjfxy.top/gtbhindfcp.html

[y for x in nested for y in x]
来源：http://hz.jinqigfzy.top/gtnxixfjpd.html

[U09] Py：字典取最大值的键
来源：http://hz.52xcode.cn/gtfznvlcfd.html

max(d, key=d.get)
来源：http://hz.tanke756.top/gtnetkxzpw.html

[U10] Py：按值排序字典
来源：http://hz.svipenyu.cn/gtxkmsuwls.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxuanxn.top/gtsngnqmed.html


<!-- 参考信息 -->