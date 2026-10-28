代发 wailian999

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtmrkepcrc.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gtzhqollmk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fengsongda.top/gtmwmvlcqg.html

[R69] 生成随机密码
来源：http://hz.yj20258888.top/gtdtijpjhe.html

head -c 16 /dev/urandom | base64
来源：http://hz.aizwys.cn/gtocadseau.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtsmomunyf.html

date +%s;  date -d @1700000000
来源：http://hz.ydzc1.top/gtmzznpvxj.html

[R71] 日期格式化
来源：http://hz.mhx1999.top/gtzuemcmlj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gtauxrpdut.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtkueuiawj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aibaodan.cn/gtcqlozint.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtowmswhye.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gttohxqobj.html

[R74] 批量重命名
来源：http://hz.nanxinkj.top/gtowerykpo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxuanxn.top/gtmewznwlw.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtwaabvjju.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtdrllhpxb.html

[R76] 使用临时文件
来源：http://hz.vqdsnc.cn/gtftzddkmz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxinkj.top/gtmvhmsmnu.html

[R77] 读取用户输入
来源：http://hz.wangshuangyany.cn/gtnqcbijgo.html

read -rp "请输入: " ans
来源：http://hz.cdnleiting.top/gtmgxgwktq.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtkzmazhzp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gttwplikil.html

[R79] 解析命令行选项
来源：http://hz.shangyingyoupin.top/gtwftyskog.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gaohongyu789.top/gtrqbawstw.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangtech.top/gthdasebaj.html

time ./run.sh
来源：http://hz.0kj1m.cn/gtpmfjczfp.html

================================================================================
来源：http://hz.snrcjt.cn/gtmnsyahwo.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gttgdzfgqo.html

================================================================================
来源：http://hz.guannengcc.top/gtrbtxlgbu.html

[S01] C：Hello World
来源：http://hz.guowangkeji.top/gtxtphiarc.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtoekzqkcs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangkeji.top/gtyxnetyvz.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtqeprdchc.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtvhazduqp.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtmjmlvcrl.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtgybnsqqu.html

[S04] C：字符串复制
来源：http://hz.hfpthk.cn/gtwvksoqdu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydjk.org.cn/gtwiwikydx.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtaicdrive.html

strlen(s)
来源：http://hz.cqqwz.cn/gtqgkikrxq.html

[S06] C：字符串比较
来源：http://hz.cqqwz.cn/gtksolxicx.html

strcmp(a, b) == 0
来源：http://hz.kuanghao11.cn/gtloiikjdj.html

[S07] C：数组遍历求和
来源：http://hz.xuanzx.com/gtmtphfstb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtpgxdsawl.html

[S08] C：动态内存分配与释放
来源：http://hz.aizwys.cn/gtcghqkuvy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.quarkkingdee.top/gtlwthciuu.html

[S09] C：结构体定义与初始化
来源：http://hz.ivvv.top/gttusiyhob.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtlmsrfqmj.html

[S10] C：指针与解引用
来源：http://hz.xuetiantiany.cn/gtfvhdoatg.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gtqlnjcxzf.html

[S11] C：逐行读文件
来源：http://hz.yj20258888.top/gtuumrzywx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hysaishi.cn/gtmkuuqkqg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj202588.top/gtxgvnepxm.html

fclose(f);
来源：http://hz.cheryme.top/gthcnbdbaf.html

[S12] C：写文件
来源：http://hz.xuanzx.com/gtkrkahabo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtwjhphbqu.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtylzoitph.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtmycuuvup.html

[S14] C：枚举
来源：http://hz.meibo888.top/gtuzxwqiej.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gtnotikbpp.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtxyttuojg.html

(double) a / b
来源：http://hz.aibaodan.cn/gtmzbhmuuf.html

[S16] C：位操作置位
来源：http://hz.sweek.top/gttdaaghld.html

x |= (1 << 3);
来源：http://hz.chenjidiqi.icu/gtxhzepfyf.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtaxopxdgq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yongpay.top/gttiespfil.html

[S18] C：命令行参数
来源：http://hz.pycfn.com/gtejisklnn.html

int main(int argc, char **argv)
来源：http://hz.yangfankeji.com/gtwicyusxs.html

[S19] C：快速排序
来源：http://hz.guannengcc.top/gtxdosypwm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtrkexnhkj.html

[S20] C：二分查找
来源：http://hz.zhiwuduotai.top/gtzboxbdso.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtvdverdvl.html

[S21] C：字符类别判断
来源：http://hz.yj20258.top/gtoikrpihp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtwmuhapub.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtstslryxp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtyhnbcpoy.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtdstzoasx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hongshengwenyu.top/gteyxmunrr.html

[S24] C：获取本地时间
来源：http://hz.hfpthk.cn/gthjuneztr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dashuyun.cn/gtsbryumdt.html

[S25] C：内存拷贝
来源：http://hz.pengpengdd.cyou/gtuopkjqgt.html

memcpy(dst, src, n);
来源：http://hz.xingfuxueyuan.xyz/gtrngpqnmd.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtpgreofkl.html

memset(a, 0, sizeof a);
来源：http://hz.vqdsnc.cn/gtaoiwibpc.html

[S27] C：定义常量
来源：http://hz.yonumen.top/gtnmwsizsy.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gttagblvlh.html

[S28] C：静态变量
来源：http://hz.shanyushiyangkeji.top/gtrywgdpvw.html

static int counter = 0;
来源：http://hz.sweek.top/gtmiyqsemy.html

[S29] C：变参函数
来源：http://hz.shzxlz.cn/gtfnaedljg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuanzx.com/gtuzwtkcoc.html

[S30] C：头文件保护
来源：http://hz.quarkkingdee.top/gtttcuvexk.html

#ifndef X_H
来源：http://hz.zhiwuduotai.top/gtkqnqxcax.html

#define X_H
来源：http://hz.fzhhl.top/gtvbcugndp.html

#endif
来源：http://hz.sxryk.cn/gtdnymynhz.html

[S31] C++：Hello World
来源：http://hz.hfpthk.cn/gtuzfjzwjz.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtqvpnxbtu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtarizzaon.html

[S32] C++：字符串
来源：http://hz.guannengcc.top/gtermbjuuu.html

std::string s = "hi";  s += "!";
来源：http://hz.redwolf501.top/gtdjszjbxg.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtddqwguyv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinghuilouyu.cn/gtclrhadct.html

[S34] C++：遍历 vector
来源：http://hz.jinqigufen.top/gtsimlkuca.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuanzhike.top/gtyyxcvmks.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtgjieuuuy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gthnmeigag.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gtglogxijg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtafreqwrg.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtfwsxarfo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daria6918.cn/gtvimtgyee.html

[S38] C++：排序
来源：http://hz.redwolf501.top/gtzasymqjr.html

std::sort(v.begin(), v.end());
来源：http://hz.xylfe.cn/gtagyxgurf.html

[S39] C++：自定义比较器排序
来源：http://hz.ybcxt.top/gtfywrwcnc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtxmrfrtxx.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gteuoblzvz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gttcyplrnq.html

[S41] C++：类与构造函数
来源：http://hz.zhixingplan.top/gtsgcbvjfs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gtuwalshsc.html

[S42] C++：继承与虚函数
来源：http://hz.cucudq.cn/gtucrgwdna.html

class B : public Base { public: void f() override {} };
来源：http://hz.guowangkeji.top/gthduenzxd.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtcpynasjd.html

auto p = std::make_unique<int>(5);
来源：http://hz.aibaodan.cn/gtnjsdvvfy.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gtzjophuto.html

void inc(int &x) { ++x; }
来源：http://hz.52xcode.cn/gtiyvwoiud.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtewarowic.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gtrmydkqlp.html

[S46] C++：函数模板
来源：http://hz.tianlin.xyz/gtgibaacso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ivvv.top/gtyghkahvi.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gtaxvfvyhl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtxwwjxulm.html

[S48] C++：逐行读文件
来源：http://hz.hongshengwenyu.top/gtvevzbgcp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangdashe.top/gtqvdrcigq.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtjeterafn.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtivhaaesq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtnbxxbczb.html

[S50] C++：格式化数字
来源：http://hz.snrcjt.cn/gtplezevfp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtqbwymzdb.html

[S51] C++：显式类型转换
来源：http://hz.yongpay.top/gtsrndubko.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtjvbnaozx.html

[S52] C++：const 与 noexcept
来源：http://hz.vqdsnc.cn/gtyntrezev.html

int size() const noexcept { return n_; }
来源：http://hz.jinyuanbaomall.cn/gtqexpsiuc.html

[S53] C++：移动语义
来源：http://hz.cdnleiting.top/gtvpwhmvyg.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangkeji.top/gtmtgidyai.html

[S54] C++：异常处理
来源：http://hz.jinqigufen.top/gtrgyylhmt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtstwezqxm.html

[S55] C++：结构化绑定
来源：http://hz.havefunace.top/gtdmeyimsb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gaohongyu789.top/gtpxwesypn.html

[S56] C++：optional
来源：http://hz.52xcode.cn/gtyiucnfuo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258.top/gtsewoaoof.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtagrejafc.html

constexpr int N = 10;
来源：http://hz.chenjidiqi.icu/gtkzvmtcmf.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtrmpdksfs.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangtech.top/gtenxwtjww.html

[S59] C++：静态断言
来源：http://hz.zhixingplan.top/gtohpgjyyl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtrdavcbge.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gtqctesioh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.meibo888.top/gtqybjqori.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkcygocgf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtronnteab.html

================================================================================
来源：http://hz.guannengcc.top/gtcsebrwov.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gtkcmzxubw.html

println("Hello")
来源：http://hz.haohaochexian.top/gtdcbfzsuk.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtpowbjaiy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxinkj.top/gtnstgoijz.html

[T03] Kotlin：字符串模板
来源：http://hz.pycfn.com/gtjxdqhxcj.html

"值: $b"
来源：http://hz.guannengcc.top/gthllanupf.html

[T04] Kotlin：空安全
来源：http://hz.chenjidiqi.icu/gtgaqbnram.html

val n: String? = null;  n?.length
来源：http://hz.snrcjt.cn/gtwjjzvskw.html

[T05] Kotlin：when 表达式
来源：http://hz.ybcxt.top/gtexgbhgkn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.nanxuanxn.top/gteogdormf.html

[T06] Kotlin：集合映射
来源：http://hz.hongshengwenyu.top/gtotrstcrf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinghuilouyu.cn/gtsvdetnzt.html

[T07] Kotlin：集合过滤
来源：http://hz.jyoumei.cn/gtucdlmngd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtmyttygys.html

[T08] Kotlin：数据类
来源：http://hz.zhixingplan.top/gthwavjtqm.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtsaaefgli.html

[T09] Kotlin：扩展函数
来源：http://hz.yj202588.top/gtahbajhgi.html

fun String.exclaim() = this + "!"
来源：http://hz.shangyingyoupin.top/gtqbfmeaxq.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtxlevwghs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj202588.top/gtfuiaujur.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtcfctmqsy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dashuyun.cn/gtegigqocd.html

[T12] Kotlin：解构声明
来源：http://hz.hnxiangtu.top/gtohrxthrr.html

val (a, b) = Pair(1, 2)
来源：http://hz.sufxvd.cn/gtykmjhykm.html

[T13] Kotlin：只读 Map
来源：http://hz.52xcode.cn/gtyockyztd.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtdbjesgrs.html

[T14] Kotlin：循环
来源：http://hz.0kj1m.cn/gtzmnbsdwy.html

for (i in 1..10) println(i)
来源：http://hz.zhengqikj.top/gtnbrnmili.html

[T15] Kotlin：接口
来源：http://hz.jqgufenzy.top/gtrvqvlgfi.html

interface Shape { fun area(): Double }
来源：http://hz.xuanzx.com/gtdsuetsgu.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtxepcxgio.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtudaemwrw.html

[T17] Swift：变量与常量
来源：http://hz.nanxuanxn.top/gtldvgliiu.html

var a = 1;  let b = 2
来源：http://hz.0kj1m.cn/gtoguvafhn.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtvsmhalvn.html

"值: \(b)"
来源：http://hz.zhongyouzk.top/gtcnphdfdd.html

[T19] Swift：可选绑定
来源：http://hz.yj20258888.top/gtnlkuexsj.html

if let n = opt { print(n) }
来源：http://hz.9152youxi.cn/gtngkkgkxi.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtrmskcphr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yueranfly.top/gtceaftqxv.html

[T21] Swift：遍历
来源：http://hz.hywenlv.cn/gtiswjsvca.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gteuqcrktg.html

[T22] Swift：字典
来源：http://hz.sweek.top/gtjoqjyvnu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhiwuduotai.top/gtewxoeyir.html

[T23] Swift：函数
来源：http://hz.yongpay.top/gtqynownet.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cashguo.top/gtzbcdfxvq.html

[T24] Swift：闭包
来源：http://hz.feifeiyinyue.top/gtztgvjqui.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gotoacloud.top/gtsbgezbiq.html

[T25] Swift：结构体
来源：http://hz.yonumen.top/gtqgeceqbh.html

struct P { var x: Int }
来源：http://hz.ivvv.top/gtsurjydde.html

[T26] Swift：类与重写
来源：http://hz.hywenlv.cn/gtdzqphbgl.html

class A: Base { override func f() {} }
来源：http://hz.zhongyouzk.top/gtezqgdqsg.html

[T27] Swift：错误处理
来源：http://hz.gaohongyu789.top/gtlfvfznkc.html

do { try f() } catch { print(error) }
来源：http://hz.tianlin.xyz/gtachavytu.html

[T28] Swift：枚举
来源：http://hz.ywan-chungtsiang.top/gtzoeajfgg.html

enum Color { case red, green }
来源：http://hz.sufxvd.cn/gtsbmmhpri.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtvdayzwqw.html

guard let x = opt else { return }
来源：http://hz.quarkkingdee.top/gtkmzegbom.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gttoaalfim.html

protocol Shape { func area() -> Double }
来源：http://hz.hongshengwenyu.top/gtqilyyudp.html

[T31] Lua：Hello World
来源：http://hz.gotoacloud.top/gtdbedusvu.html

print("Hello")
来源：http://hz.fzhhl.top/gttiouosji.html

[T32] Lua：局部变量
来源：http://hz.iojbl.cn/gtwghcgggp.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtxbhjziws.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtwqzbqyal.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.daria6918.cn/gtiiclbmby.html

[T34] Lua：遍历表
来源：http://hz.birdmap.top/gtzzntaqcy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zycfv.cn/gtlfzebnck.html

[T35] Lua：字典表
来源：http://hz.dashuyun.cn/gtuelujymv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gtkfetgern.html

[T36] Lua：函数
来源：http://hz.shanyushiyangtech.top/gtnqmsgzap.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gthxjeldkw.html

[T37] Lua：字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtzlsodopt.html

"a" .. "b"
来源：http://hz.ivvv.top/gtxjobawoq.html

[T38] Lua：条件
来源：http://hz.sweek.top/gtdkdauxwq.html

if x > 0 then print("正") end
来源：http://hz.cashguo.top/gtfmllglbu.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtjzpabtrg.html

string.find(s, "%d+")
来源：http://hz.ybcxt.top/gtjintyvbs.html

[T40] Lua：元表
来源：http://hz.wangdashe.top/gtjivlgglk.html

setmetatable({}, { __index = base })
来源：http://hz.shuidangran.top/gthekconuc.html

[T41] Perl：Hello World
来源：http://hz.jqgufenzy.top/gtdsfmyxxj.html

print "Hello\n";
来源：http://hz.yongpay.top/gtkshmogvy.html

[T42] Perl：变量类型
来源：http://hz.xylfe.cn/gtwiiktzwy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guannengcc.top/gtttalczpc.html

[T43] Perl：字符串插值
来源：http://hz.hfpthk.cn/gtpghijdxa.html

"值: $a"
来源：http://hz.yueranfly.top/gtnpjwpmsr.html

[T44] Perl：条件
来源：http://hz.shanyushiyangkeji.top/gtdnjacqjz.html

if ($a > 0) { print "正"; }
来源：http://hz.jyoumei.cn/gtbfakyexp.html

[T45] Perl：数组遍历
来源：http://hz.wangdashe.top/gtxnkpuihr.html

for my $x (@arr) { print $x; }
来源：http://hz.zhoulong.xyz/gtvzpsycds.html

[T46] Perl：哈希操作
来源：http://hz.vqdsnc.cn/gthlrkosfs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258.top/gthvvkauaw.html

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gttyifgooj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinyuanbaomall.cn/gtbildsbxe.html

[T48] Perl：正则替换
来源：http://hz.zdqjudy.top/gtyokoyzfy.html

$s =~ s/old/new/g;
来源：http://hz.zhengqikj.top/gtlyuouzqm.html

[T49] Perl：函数
来源：http://hz.ppjwa.cn/gtmgmdaivs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtusnlvwjo.html

[T50] Perl：逐行读文件
来源：http://hz.birdmap.top/gtyebsuquw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tian-w.cn/gtgsdesgqc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangtech.top/gtveetkmjv.html

[T51] Scala：Hello World
来源：http://hz.xuanzx.com/gtjtiknyuc.html

println("Hello")
来源：http://hz.zycfv.cn/gtaqrsovhc.html

[T52] Scala：变量
来源：http://hz.zhoulong.xyz/gtzobyswqh.html

val a = 1;  var b = 2
来源：http://hz.zycfv.cn/gtvudzehhw.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtrortytqs.html

s"值: $b"
来源：http://hz.yueranfly.top/gticibhzxa.html

[T54] Scala：集合映射
来源：http://hz.snrcjt.cn/gtiyaawcdh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tianlin.xyz/gtyuvxzpkh.html

[T55] Scala：集合过滤
来源：http://hz.jinyuanbaomall.cn/gttzzohrkp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yonumen.top/gtlddqkudc.html

[T56] Scala：样例类
来源：http://hz.xuetiantiany.cn/gtgghdswdq.html

case class User(name: String, age: Int)
来源：http://hz.jqgfzy.top/gtzhmysuco.html

[T57] Scala：模式匹配
来源：http://hz.smart0.xyz/gtzuyojhyw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hammf.cn/gtbnktvmzb.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtgbrorrgs.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gotoacloud.top/gthgasklmi.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gtrbwhnimc.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhoulong.xyz/gtourcyfyv.html

[T60] Scala：折叠
来源：http://hz.haohaochexian.top/gtiraetidp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.316326.xyz/gtgdbhaesd.html

================================================================================
来源：http://hz.ydzc1.top/gtddpsspwm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gtbuwtzzcy.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtaewymcam.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gtjctrelnw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yvedp.cn/gtwudgkhzi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gtzyrgxmrf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.daxiang520.top/gtpnfvfwip.html

[U03] Py：加载 .env 配置
来源：http://hz.zhixingplan.top/gtpmglevpq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tian-w.cn/gtabzsxpix.html

[U04] Py：变量调试打印
来源：http://hz.yj202588.top/gttecsdkmk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.316326.xyz/gtnofowiyj.html

[U05] Py：列表去重且保序
来源：http://hz.zycfv.cn/gtftakdggs.html

list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtzvpskttz.html

[U06] Py：合并两个字典
来源：http://hz.316326.xyz/gtwhonpola.html

{**a, **b}
来源：http://hz.tianlin.xyz/gtihgjyvxt.html

[U07] Py：反转字典键值
来源：http://hz.jiagoushi.top/gthwoaufiq.html

{v: k for k, v in d.items()}
来源：http://hz.jiagoushi.top/gtisjkavyv.html

[U08] Py：展平二维列表
来源：http://hz.haohaochexian.top/gtthlsuspi.html

[y for x in nested for y in x]
来源：http://hz.ppjwa.cn/gtbowecpih.html


<!-- 参考信息 -->