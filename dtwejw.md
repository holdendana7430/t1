代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtzydznrii.html

[R70] 时间戳与互转
来源：http://hz.shangyingyoupin.top/gtxjnawlhb.html

date +%s;  date -d @1700000000
来源：http://hz.jiagoushi.top/gtathylshv.html

[R71] 日期格式化
来源：http://hz.quarkkingdee.top/gtuwmzeqjc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.quarkkingdee.top/gthdpczylg.html

[R72] 等待端口就绪
来源：http://hz.quarkkingdee.top/gtjqslaafz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gteneqehwn.html

[R73] 分割大日志
来源：http://hz.xinyue.icu/gtabacesfs.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtdlpfaskp.html

[R74] 批量重命名
来源：http://hz.xinyue.icu/gtmwtyloqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gtqdyamepp.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtjnsdkngf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.guowangkeji.top/gtedyqdsac.html

[R76] 使用临时文件
来源：http://hz.52xcode.cn/gtfowtpirm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gteafalmni.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtdgoljlzv.html

read -rp "请输入: " ans
来源：http://hz.yongpay.top/gtiyipllhr.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gtmgbvhxdr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yvedp.cn/gtyaqmghqt.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtlitwwwnz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinqigufen.top/gthspzscmp.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtvwirnvlb.html

time ./run.sh
来源：http://hz.sweek.top/gtybmhkfbp.html

================================================================================
来源：http://hz.mhx1999.top/gtdfgyiufa.html

S. C / C++ 专题
来源：http://hz.hammf.cn/gtewrszhlw.html

================================================================================
来源：http://hz.cqqwz.cn/gttoynezam.html

[S01] C：Hello World
来源：http://hz.meibo888.top/gtiuzubwry.html

#include <stdio.h>
来源：http://hz.ybcxt.top/gtgnbiohef.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zycfv.cn/gtsurkauaf.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtazjoluit.html

int a = 10; printf("%d\n", a);
来源：http://hz.sxryk.cn/gtxfhxetwb.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gttyfgygok.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtppborxxd.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtmqzsvaua.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.kuanghao11.cn/gtbzgobzdh.html

[S05] C：字符串长度
来源：http://hz.sxryk.cn/gtmecasrtt.html

strlen(s)
来源：http://hz.jinqigufen.top/gtaqomtluc.html

[S06] C：字符串比较
来源：http://hz.xuanzx.com/gtmrbawxoi.html

strcmp(a, b) == 0
来源：http://hz.ybcxt.top/gtkakzrudi.html

[S07] C：数组遍历求和
来源：http://hz.ivvv.top/gtyxmzgojh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtbunoqlzv.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtirkzlfjc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnqzz.top/gtueflwhav.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gthumtqnil.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cdnleiting.top/gtrlxinpsl.html

[S10] C：指针与解引用
来源：http://hz.cheryme.top/gtwczpicdy.html

int *p = &a;  *p = 5;
来源：http://hz.andypj.xyz/gttqzhjwxb.html

[S11] C：逐行读文件
来源：http://hz.pengpengdd.cyou/gtusyioaqm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtxrefweub.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gtxzolbzxq.html

fclose(f);
来源：http://hz.9152youxi.cn/gtdtwfdvyf.html

[S12] C：写文件
来源：http://hz.jlsjyb.cn/gtvfiwvxwo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenzaomai.com/gtgptjeclh.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtgxrarzui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.fzhhl.top/gtybdxjzer.html

[S14] C：枚举
来源：http://hz.xuetiantiany.cn/gtsdevfwgz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ehwqpu.com/gtqmlrsbre.html

[S15] C：类型转换
来源：http://hz.chenzaomai.com/gtnuysqkes.html

(double) a / b
来源：http://hz.cdnleiting.top/gtmtasfgsi.html

[S16] C：位操作置位
来源：http://hz.jinyuanbaomall.cn/gtsvrirsss.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtzgfozvfw.html

[S17] C：安全拼接字符串
来源：http://hz.svipenyu.cn/gtadlenjeb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigfzy.top/gtahjmcqau.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gtamhhodfc.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtosetszlm.html

[S19] C：快速排序
来源：http://hz.jinghuilouyu.cn/gthqbgnimg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtqdtjzoot.html

[S20] C：二分查找
来源：http://hz.jqgfzy.top/gtounhnwdg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtloeeskwb.html

[S21] C：字符类别判断
来源：http://hz.snrcjt.cn/gtciuzgtkw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydzc1.top/gttqyidqjp.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtfdftipep.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aibaodan.cn/gtoghhhxdf.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtajjvqdwk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yangfankeji.com/gtoaehizpx.html

[S24] C：获取本地时间
来源：http://hz.meibo888.top/gtltrxvycq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gtlkwlhnyb.html

[S25] C：内存拷贝
来源：http://hz.chenzaomai.com/gtkhhipdqg.html

memcpy(dst, src, n);
来源：http://hz.yongpay.top/gtywsvvykq.html

[S26] C：内存清零
来源：http://hz.zhongyouzk.top/gtdeilgfjq.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtxmmvnfzz.html

[S27] C：定义常量
来源：http://hz.nanxinkj.top/gtmzocynla.html

const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gthcemurtc.html

[S28] C：静态变量
来源：http://hz.xziqi.cn/gtcbyafvjh.html

static int counter = 0;
来源：http://hz.xylfe.cn/gtccvbjelv.html

[S29] C：变参函数
来源：http://hz.redwolf501.top/gtpaxmuyci.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtjcfpydgp.html

[S30] C：头文件保护
来源：http://hz.zhaomingkeji.xyz/gtxitelmso.html

#ifndef X_H
来源：http://hz.svipenyu.cn/gtmwrhcprx.html

#define X_H
来源：http://hz.yj20258.top/gtlcjobtks.html

#endif
来源：http://hz.sysykeji.top/gtyqgggnet.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtcrboynmm.html

#include <iostream>
来源：http://hz.wangdashe.top/gtxgmqjjlc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtamalubji.html

[S32] C++：字符串
来源：http://hz.yj20258888.top/gtrbnmxigk.html

std::string s = "hi";  s += "!";
来源：http://hz.svipenyu.cn/gtjwpqpkxi.html

[S33] C++：vector 增删
来源：http://hz.cqqwz.cn/gtvfbeizos.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhaomingkeji.xyz/gtwboxhvnp.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gthljuywxg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ehwqpu.com/gtvkzjhhlp.html

[S35] C++：map
来源：http://hz.yueranfly.top/gtgdibhrue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gtggsqkfao.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtykblextx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtdfgreaqv.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtqoairxvs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gtqrtwnwbd.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtemqrltuw.html

std::sort(v.begin(), v.end());
来源：http://hz.yongpay.top/gtdgxlgifs.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangtech.top/gtigvphfca.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.quarkkingdee.top/gtjoakzoei.html

[S40] C++：查找元素
来源：http://hz.hammf.cn/gtcwkwvsmm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fzhhl.top/gtcsupnjvj.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtqdmznfcl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtefhixfqv.html

[S42] C++：继承与虚函数
来源：http://hz.shzxlz.cn/gtlnzvoout.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gtcsdmokfe.html

[S43] C++：智能指针
来源：http://hz.nanxuanxn.top/gtqqhiodtp.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gttumjjuws.html

[S44] C++：引用传参
来源：http://hz.aizwys.cn/gtjvkxiyqm.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gtwdzxloww.html

[S45] C++：lambda
来源：http://hz.zycfv.cn/gtxzuelghc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtxuticoms.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtmbrwlyoh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ybcxt.top/gtahyqdjur.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gtmpwgjmsw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuanzhike.top/gteusxhytx.html

[S48] C++：逐行读文件
来源：http://hz.gotoacloud.top/gtnyajamhn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtmkvaluoh.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtznsowatg.html

[S49] C++：写文件
来源：http://hz.yonumen.top/gtfeuksulz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnqzz.top/gtyckvygrn.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gtekmvzebc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuanzhike.top/gtiaacldju.html

[S51] C++：显式类型转换
来源：http://hz.ivvv.top/gtvqgljczg.html

static_cast<double>(a) / b
来源：http://hz.yj20258888.top/gtumnxpokz.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gtvputdumj.html

int size() const noexcept { return n_; }
来源：http://hz.xingfuxueyuan.xyz/gtfeyywhho.html

[S53] C++：移动语义
来源：http://hz.ppjwa.cn/gtigcgfgcr.html

std::vector<int> w = std::move(v);
来源：http://hz.cheryme.top/gtwfdfxvke.html

[S54] C++：异常处理
来源：http://hz.zhongyouzk.top/gtornjbpzr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guannengcc.top/gtflvlunum.html

[S55] C++：结构化绑定
来源：http://hz.fzhhl.top/gtxkfzsujl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtkwkjaavj.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtthfznbzs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtbhbbmhiz.html

[S57] C++：编译期常量
来源：http://hz.pengpengdd.cyou/gtzbuhtcrb.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtjhfstlkt.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtepvthmmx.html

namespace ns { int f() { return 1; } }
来源：http://hz.vqdsnc.cn/gtxnbzdjdj.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtlizqlhjf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.andypj.xyz/gtppvlmjyk.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtgetczlul.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtgvqqmdxv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmtfqgogt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtarkvfawo.html

================================================================================
来源：http://hz.daria6918.cn/gtllwsfctz.html

[T01] Kotlin：Hello World
来源：http://hz.ydjk.org.cn/gtuxmlypsk.html

println("Hello")
来源：http://hz.52xcode.cn/gtppikarnw.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gtfbszcdeu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtxuqortfj.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gtqsjizwcm.html

"值: $b"
来源：http://hz.hywenlv.cn/gtqntzkdjp.html

[T04] Kotlin：空安全
来源：http://hz.xuetiantiany.cn/gtlhhbmoma.html

val n: String? = null;  n?.length
来源：http://hz.guannengcc.top/gtqtwspjpp.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtfieclrvy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhixingplan.top/gtroitdizg.html

[T06] Kotlin：集合映射
来源：http://hz.hnxiangtu.top/gtpfgiaazx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydzc1.top/gtelrrlbpd.html

[T07] Kotlin：集合过滤
来源：http://hz.havefunace.top/gtsmafvyuj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.haohaochexian.top/gteetexsev.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gttdlqijie.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtqfzmwgrg.html

[T09] Kotlin：扩展函数
来源：http://hz.jinghuilouyu.cn/gtalxupwci.html

fun String.exclaim() = this + "!"
来源：http://hz.jlsjyb.cn/gtkpstudzi.html

[T10] Kotlin：默认参数
来源：http://hz.ppjwa.cn/gtlocwchgh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.redwolf501.top/gtagfmexec.html

[T11] Kotlin：协程
来源：http://hz.pengpengdd.cyou/gtojovsfmu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gtiatpdodm.html

[T12] Kotlin：解构声明
来源：http://hz.redwolf501.top/gtukfjuvjg.html

val (a, b) = Pair(1, 2)
来源：http://hz.meibo888.top/gtybkjdhpp.html

[T13] Kotlin：只读 Map
来源：http://hz.cucudq.cn/gtnjhzybyw.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gtoftiipmt.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtjjcskksu.html

for (i in 1..10) println(i)
来源：http://hz.jinghuilouyu.cn/gtkaywaihc.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtrhvshuex.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gtozfzkvwo.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtccvzoqdp.html

print("Hello")
来源：http://hz.cucudq.cn/gtqejmggel.html

[T17] Swift：变量与常量
来源：http://hz.ehwqpu.com/gtginfhaww.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gthxannfqe.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gthxkdjhhl.html

"值: \(b)"
来源：http://hz.cheryme.top/gtgmupmlmm.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtsfavnzhf.html

if let n = opt { print(n) }
来源：http://hz.jlsjyb.cn/gtrrkprbem.html

[T20] Swift：数组操作
来源：http://hz.birdmap.top/gtoxvllmzt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dianchejie.cn/gtidexweey.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gthagxqzxo.html

for x in a { print(x) }
来源：http://hz.52xcode.cn/gtxmznyoxu.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtfcebjqxi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtfsaseitb.html

[T23] Swift：函数
来源：http://hz.svipenyu.cn/gtooxwywzr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuanzhike.top/gtxzvgyfzv.html

[T24] Swift：闭包
来源：http://hz.jianghu66.top/gtcjedkccr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgufenzy.top/gtytyhmuxb.html

[T25] Swift：结构体
来源：http://hz.gzhubu.top/gtphhblnee.html

struct P { var x: Int }
来源：http://hz.ydzc1.top/gtmyvaihoz.html

[T26] Swift：类与重写
来源：http://hz.jinghuilouyu.cn/gtfghgsnen.html

class A: Base { override func f() {} }
来源：http://hz.guannengcc.top/gtgcwvtvqp.html

[T27] Swift：错误处理
来源：http://hz.jinqigfzy.top/gtmgiotapa.html

do { try f() } catch { print(error) }
来源：http://hz.hongshengwenyu.top/gtrohmwlbl.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtcucczdbg.html

enum Color { case red, green }
来源：http://hz.9152youxi.cn/gtviahpuoa.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gtfyblarpf.html

guard let x = opt else { return }
来源：http://hz.shuidangran.top/gtailekknq.html

[T30] Swift：协议
来源：http://hz.yuanzhike.top/gtlgajmhee.html

protocol Shape { func area() -> Double }
来源：http://hz.ppjwa.cn/gtjsnlguho.html

[T31] Lua：Hello World
来源：http://hz.9152youxi.cn/gtlrvkfjqn.html

print("Hello")
来源：http://hz.tianlin.xyz/gthydcrthe.html

[T32] Lua：局部变量
来源：http://hz.jinqigufen.top/gtufcvggin.html

local a = 1
来源：http://hz.shuidangran.top/gthtzmagix.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gtlwudtqrj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.316326.xyz/gtqywldgiv.html

[T34] Lua：遍历表
来源：http://hz.0kj1m.cn/gtitqgulbq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtncvctrax.html

[T35] Lua：字典表
来源：http://hz.jiagoushi.top/gtzowyegxx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.kuanghao11.cn/gtbbuxchou.html

[T36] Lua：函数
来源：http://hz.haohaochexian.top/gthytpudyi.html

function add(a, b) return a + b end
来源：http://hz.pengpengdd.cyou/gthaoxsddi.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtjwjociea.html

"a" .. "b"
来源：http://hz.dashuyun.cn/gtwwjyvaem.html

[T38] Lua：条件
来源：http://hz.gotoacloud.top/gtxnucadho.html

if x > 0 then print("正") end
来源：http://hz.gzhubu.top/gtpfugmhvz.html

[T39] Lua：模式匹配
来源：http://hz.hfpthk.cn/gtpocraoft.html

string.find(s, "%d+")
来源：http://hz.ydjk.org.cn/gthskoadnu.html

[T40] Lua：元表
来源：http://hz.0kj1m.cn/gtumibbhcy.html

setmetatable({}, { __index = base })
来源：http://hz.aibaodan.cn/gtywwsuyac.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangkeji.top/gthmlsubbv.html

print "Hello\n";
来源：http://hz.pycfn.com/gtevzekzeo.html

[T42] Perl：变量类型
来源：http://hz.smart0.xyz/gtenmqcfaz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinqigfzy.top/gtbqzgjskm.html

[T43] Perl：字符串插值
来源：http://hz.gogol.net.cn/gtxuiiprtw.html

"值: $a"
来源：http://hz.guowangkeji.top/gtjdoowuyz.html

[T44] Perl：条件
来源：http://hz.hywenlv.cn/gtyaiqfgjg.html

if ($a > 0) { print "正"; }
来源：http://hz.dashuyun.cn/gtwvazjkqq.html

[T45] Perl：数组遍历
来源：http://hz.hysaishi.cn/gtzfmavmxh.html

for my $x (@arr) { print $x; }
来源：http://hz.0kj1m.cn/gtqeoittko.html

[T46] Perl：哈希操作
来源：http://hz.hammf.cn/gtdujlekln.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgufenzy.top/gtsqpfmupn.html

[T47] Perl：正则捕获
来源：http://hz.gaohongyu789.top/gtohviloax.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinghuilouyu.cn/gtethorhbm.html

[T48] Perl：正则替换
来源：http://hz.guowangkeji.top/gtpqhsxnzx.html

$s =~ s/old/new/g;
来源：http://hz.316326.xyz/gtvbskxybt.html

[T49] Perl：函数
来源：http://hz.havefunace.top/gtqwxzbago.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ybcxt.top/gtakebtgvs.html

[T50] Perl：逐行读文件
来源：http://hz.hysaishi.cn/gtezoepnwi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yongpay.top/gtbxqghutb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj20258888.top/gtblespysb.html

[T51] Scala：Hello World
来源：http://hz.bjfxy.top/gtclkqbnko.html

println("Hello")
来源：http://hz.yj202588.top/gtdtwhyazw.html

[T52] Scala：变量
来源：http://hz.ydjk.org.cn/gtcmseftqa.html

val a = 1;  var b = 2
来源：http://hz.birdmap.top/gtcimaqevc.html

[T53] Scala：字符串插值
来源：http://hz.sweek.top/gtgyhmsnjr.html

s"值: $b"
来源：http://hz.hammf.cn/gtdnzjgtti.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gtrlcmxjps.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hongshengwenyu.top/gtiegomuvk.html

[T55] Scala：集合过滤
来源：http://hz.xuetiantiany.cn/gtbntgabwf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xinyue.icu/gtdtapvwos.html

[T56] Scala：样例类
来源：http://hz.shzxlz.cn/gtzzfctrht.html

case class User(name: String, age: Int)
来源：http://hz.zdqjudy.top/gtydhcksio.html

[T57] Scala：模式匹配
来源：http://hz.ydzc1.top/gtjqlzmcwn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cdnleiting.top/gtqheldtgx.html

[T58] Scala：函数定义
来源：http://hz.yj20258888.top/gthuehgzgx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.birdmap.top/gtinswumzv.html

[T59] Scala：循环
来源：http://hz.9152youxi.cn/gtubomhudc.html

for (i <- 1 to 10) println(i)
来源：http://hz.yvedp.cn/gtscunekyq.html

[T60] Scala：折叠
来源：http://hz.zhixingplan.top/gtwnvwfckp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuetiantiany.cn/gtrxroqhdl.html

================================================================================
来源：http://hz.quarkkingdee.top/gtcufockvn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fzhhl.top/gtjtuaxrvq.html

================================================================================
来源：http://hz.daria6918.cn/gtqvlgstwe.html

[U01] Py：创建虚拟环境
来源：http://hz.hnxiangtu.top/gtkmhthjnu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jianghu66.top/gtjhyvjxju.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pycfn.com/gtwoadtssq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtchiqxkny.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gtpocyvzpn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jiagoushi.top/gtngoxvxjf.html

[U04] Py：变量调试打印
来源：http://hz.haohaochexian.top/gtijvhfrjy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ydzc1.top/gtjkfojxtw.html

[U05] Py：列表去重且保序
来源：http://hz.mhx1999.top/gtpzkpomuf.html

list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtgdnzqqgg.html

[U06] Py：合并两个字典
来源：http://hz.ydjk.org.cn/gtviyysypy.html

{**a, **b}
来源：http://hz.zycfv.cn/gtfbujgjbn.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gtwbjhzoej.html

{v: k for k, v in d.items()}
来源：http://hz.mhx1999.top/gtiutpcucd.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gtaaahtmok.html

[y for x in nested for y in x]
来源：http://hz.jinqigfzy.top/gtsqsspavn.html

[U09] Py：字典取最大值的键
来源：http://hz.gogol.net.cn/gtqvtqnhns.html

max(d, key=d.get)
来源：http://hz.zhaomingkeji.xyz/gtijbtyxki.html

[U10] Py：按值排序字典
来源：http://hz.shangyingyoupin.top/gtjkqygpxe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gtcixeecsc.html


<!-- 参考信息 -->