代发 wailian999

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtysuzloei.html

[R68] 计算文件校验值
来源：http://hz.hywenlv.cn/gtaqarqkaf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxinkj.top/gtqtzygaiz.html

[R69] 生成随机密码
来源：http://hz.gogol.net.cn/gtjrszbuuu.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtpfmeibsf.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangkeji.top/gtmjnngxzv.html

date +%s;  date -d @1700000000
来源：http://hz.hammf.cn/gttdezgaxj.html

[R71] 日期格式化
来源：http://hz.havefunace.top/gtrpclpnxs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtpzwrasym.html

[R72] 等待端口就绪
来源：http://hz.c1oappe.top/gtajxnaoez.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtvhnobezq.html

[R73] 分割大日志
来源：http://hz.yanxiufei.cn/gtggypylej.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtnodwswwv.html

[R74] 批量重命名
来源：http://hz.yonumen.top/gtaqzobnak.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.feifeiyinyue.top/gtshdgmnyh.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtjknpjpnf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtvkfkcfhm.html

[R76] 使用临时文件
来源：http://hz.cdnleiting.top/gteecqbdsj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtuubwwdpu.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtsuiyrxvc.html

read -rp "请输入: " ans
来源：http://hz.yuanzhike.top/gtwrbgflbt.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtcwbutaum.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtheaihuwk.html

[R79] 解析命令行选项
来源：http://hz.feifeiyinyue.top/gtvamwdsny.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtvmvnucgb.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtjalqdqdi.html

time ./run.sh
来源：http://hz.xylfe.cn/gthqrondwc.html

================================================================================
来源：http://hz.cheryme.top/gtiekeyucn.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtjytmzpbf.html

================================================================================
来源：http://hz.birdmap.top/gtddoesakl.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtaxgbjbbb.html

#include <stdio.h>
来源：http://hz.ybcxt.top/gthmjgzbjn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daxiang520.top/gtyysjppku.html

[S02] C：变量与格式化输出
来源：http://hz.yueranfly.top/gtfcxspmzz.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtmuknqpvp.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtglzezpch.html

int x; scanf("%d", &x);
来源：http://hz.jianghu66.top/gtjyyfludn.html

[S04] C：字符串复制
来源：http://hz.316326.xyz/gtnwnhcrce.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gotoacloud.top/gtexxqcdyq.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtudjminam.html

strlen(s)
来源：http://hz.yongpay.top/gtkseyxrfo.html

[S06] C：字符串比较
来源：http://hz.gzhubu.top/gtkbjbnxhb.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtnudxvivl.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtpxmkpwpv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gtcmvwyepq.html

[S08] C：动态内存分配与释放
来源：http://hz.chenzaomai.com/gtvgtufoxw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gtbpepnabc.html

[S09] C：结构体定义与初始化
来源：http://hz.sysykeji.top/gtvktogvee.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgufenzy.top/gtqernjdge.html

[S10] C：指针与解引用
来源：http://hz.yangfankeji.com/gtfpqxwtlo.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtoyldecfe.html

[S11] C：逐行读文件
来源：http://hz.ppjwa.cn/gtmqlhrzdr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.andypj.xyz/gtkwvnlvzb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenlongwang.top/gtfkbprpfc.html

fclose(f);
来源：http://hz.hammf.cn/gtvvwerhtz.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gtlstsckgm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtzqmefdxy.html

[S13] C：宏定义
来源：http://hz.shuidangran.top/gtpwjhiazt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.bjfxy.top/gtvekvmylx.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtwgrtszcj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pengpengdd.cyou/gtezuedxig.html

[S15] C：类型转换
来源：http://hz.guowangkeji.top/gtmjwxgeyh.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtnhbztuon.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gtyhdlnrdh.html

x |= (1 << 3);
来源：http://hz.jqgufenzy.top/gtqorwltcu.html

[S17] C：安全拼接字符串
来源：http://hz.xziqi.cn/gtxnfhxmid.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jyoumei.cn/gtkwzuwvkf.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtyzfhzfws.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gtlslzesea.html

[S19] C：快速排序
来源：http://hz.dianchejie.cn/gtflholkwo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtpelcdwlr.html

[S20] C：二分查找
来源：http://hz.cdnleiting.top/gtpqxbesac.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtmzweduld.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtudvaiapf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shzxlz.cn/gtraqierls.html

[S22] C：字符串转数字
来源：http://hz.dashuyun.cn/gtkfomrnrp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gtkbefvfar.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtabnvrmzt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xingfuxueyuan.xyz/gtawtaisaj.html

[S24] C：获取本地时间
来源：http://hz.fzhhl.top/gtpmxwlshn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtsnhztzqw.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtkvumffto.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtsztyccui.html

[S26] C：内存清零
来源：http://hz.snrcjt.cn/gteeftoppn.html

memset(a, 0, sizeof a);
来源：http://hz.yonumen.top/gtxsrsaeir.html

[S27] C：定义常量
来源：http://hz.aibaodan.cn/gtlsvwfqpn.html

const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtdzbmvhfu.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtqhjwkqlg.html

static int counter = 0;
来源：http://hz.cashguo.top/gtsmmlhmgr.html

[S29] C：变参函数
来源：http://hz.yj20258888.top/gtluozfjlt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guowangkeji.top/gtkoguhrxa.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gtwcqcsbji.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gttjqgjoyw.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtthkvavph.html

#endif
来源：http://hz.kuanghao11.cn/gtcrcbpavl.html

[S31] C++：Hello World
来源：http://hz.jyoumei.cn/gtfpmakgsq.html

#include <iostream>
来源：http://hz.havefunace.top/gttpiatepw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gogol.net.cn/gtcyaayspx.html

[S32] C++：字符串
来源：http://hz.hfpthk.cn/gtzmawiawg.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtetnicljn.html

[S33] C++：vector 增删
来源：http://hz.nanxinkj.top/gtcdvzfyjo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xingfuxueyuan.xyz/gtusayikib.html

[S34] C++：遍历 vector
来源：http://hz.sxryk.cn/gtxylotyyo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hysaishi.cn/gtqzyopths.html

[S35] C++：map
来源：http://hz.kuanghao11.cn/gtexzpbcmm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtymjdrtzn.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gtkjugltxs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtgtihnoqj.html

[S37] C++：set
来源：http://hz.xuetiantiany.cn/gtqfmabtuj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xinyue.icu/gtlrkdjedt.html

[S38] C++：排序
来源：http://hz.zdqjudy.top/gtlqzetdpc.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtkpvmmgzq.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxuanxn.top/gtxpugcwdf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hongshengwenyu.top/gteisydwle.html

[S40] C++：查找元素
来源：http://hz.xylfe.cn/gtklwkgbjl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtxxwxghlx.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtnrgckavv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtfkpgrcte.html

[S42] C++：继承与虚函数
来源：http://hz.jlsjyb.cn/gtixekesmk.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinqigfzy.top/gtsugnhkji.html

[S43] C++：智能指针
来源：http://hz.pengpengdd.cyou/gttexwydpn.html

auto p = std::make_unique<int>(5);
来源：http://hz.hammf.cn/gtwbotpthr.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtdvwvwjrj.html

void inc(int &x) { ++x; }
来源：http://hz.sysykeji.top/gtdgidszge.html

[S45] C++：lambda
来源：http://hz.zhaomingkeji.xyz/gtcrzvxpfp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cashguo.top/gtyuebykhb.html

[S46] C++：函数模板
来源：http://hz.xylfe.cn/gtazirvhlx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gthlevvfis.html

[S47] C++：结构化绑定遍历
来源：http://hz.jiagoushi.top/gtqjbcmrtj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daxiang520.top/gtlgqxwakp.html

[S48] C++：逐行读文件
来源：http://hz.zdqjudy.top/gtmvlfuvna.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jlsjyb.cn/gtrgwokjsr.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gtfxagdtoe.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gthtumbhwq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gtmjwsabmy.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtzgenvnem.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sxryk.cn/gtebnmbxzb.html

[S51] C++：显式类型转换
来源：http://hz.cucudq.cn/gtfsrztnxl.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtllgdwjlj.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gttvblekkh.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtowjzrydx.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gtgtztumyo.html

std::vector<int> w = std::move(v);
来源：http://hz.cheryme.top/gtzfatbtgl.html

[S54] C++：异常处理
来源：http://hz.yj20258.top/gtzailbdbj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.haohaochexian.top/gtpqeqjbjy.html

[S55] C++：结构化绑定
来源：http://hz.andypj.xyz/gtnwtpacrg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtwajoiplo.html

[S56] C++：optional
来源：http://hz.jyoumei.cn/gtgoxcmkqy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cashguo.top/gtgttykjfn.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtvkxdfdzx.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gtzkbldpmm.html

[S58] C++：命名空间
来源：http://hz.hywenlv.cn/gtcbyxffmn.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtijkuoxra.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtulxaupvf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guannengcc.top/gtoqypevnv.html

[S60] C++：遍历并删除元素
来源：http://hz.cdnleiting.top/gtyainomrn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtwfwwxwtr.html

================================================================================
来源：http://hz.xziqi.cn/gttfoqezwv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtwqwjubow.html

================================================================================
来源：http://hz.zycfv.cn/gtrwfvehue.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtavvdrhow.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtgddhbnov.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtzrpbixkg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.quarkkingdee.top/gtjvkkvppz.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtsjborxna.html

"值: $b"
来源：http://hz.bjfxy.top/gtyqsgftnb.html

[T04] Kotlin：空安全
来源：http://hz.hywenlv.cn/gtcqvtpxpi.html

val n: String? = null;  n?.length
来源：http://hz.hywenlv.cn/gtmazlnlta.html

[T05] Kotlin：when 表达式
来源：http://hz.dashuyun.cn/gtpbzrjghj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xziqi.cn/gthvglojah.html

[T06] Kotlin：集合映射
来源：http://hz.52xcode.cn/gtdgvkjnzl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gtzssypsbr.html

[T07] Kotlin：集合过滤
来源：http://hz.hysaishi.cn/gtjnjhvcum.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yongpay.top/gtiwzfcazs.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gthuzseyvd.html

data class User(val name: String, val age: Int)
来源：http://hz.tianlin.xyz/gtqvlqblam.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gtakalgwrt.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtgwkhvkhq.html

[T10] Kotlin：默认参数
来源：http://hz.sysykeji.top/gtaagzigsn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangdashe.top/gtinzogefl.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtkitkuhvm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cheryme.top/gtrhihwdva.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gtvwtdsfdz.html

val (a, b) = Pair(1, 2)
来源：http://hz.jlsjyb.cn/gtqjzkecab.html

[T13] Kotlin：只读 Map
来源：http://hz.316326.xyz/gtdgnchrwi.html

val m = mapOf("a" to 1)
来源：http://hz.hammf.cn/gtnajdyxro.html

[T14] Kotlin：循环
来源：http://hz.hysaishi.cn/gtgedbffuo.html

for (i in 1..10) println(i)
来源：http://hz.vqdsnc.cn/gtmrjhixif.html

[T15] Kotlin：接口
来源：http://hz.hnxiangtu.top/gtpznkmlhm.html

interface Shape { fun area(): Double }
来源：http://hz.chenlongwang.top/gtmwdbcbax.html

[T16] Swift：Hello World
来源：http://hz.ivvv.top/gtkocivrfb.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtkfnaijfs.html

[T17] Swift：变量与常量
来源：http://hz.tian-w.cn/gtngczxapk.html

var a = 1;  let b = 2
来源：http://hz.zdqjudy.top/gtrdfcnrbj.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gtllhoehty.html

"值: \(b)"
来源：http://hz.guannengcc.top/gtzcokccib.html

[T19] Swift：可选绑定
来源：http://hz.hammf.cn/gtnfidzpcb.html

if let n = opt { print(n) }
来源：http://hz.zhijiandao.cn/gtqseiekfv.html

[T20] Swift：数组操作
来源：http://hz.jianghu66.top/gtrscnlxna.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pengpengdd.cyou/gtnnwvpklm.html

[T21] Swift：遍历
来源：http://hz.yuxming.cn/gtudcebmni.html

for x in a { print(x) }
来源：http://hz.fengsongda.top/gtnopnkoui.html

[T22] Swift：字典
来源：http://hz.hywenlv.cn/gtymtyzfon.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gogol.net.cn/gtppvaapxp.html

[T23] Swift：函数
来源：http://hz.cqqwz.cn/gtdscjrbvh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtmpagnxtb.html

[T24] Swift：闭包
来源：http://hz.aizwys.cn/gtiegjjoud.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgufenzy.top/gtnczadskp.html

[T25] Swift：结构体
来源：http://hz.sxryk.cn/gtivhidfke.html

struct P { var x: Int }
来源：http://hz.shzxlz.cn/gtpinyazix.html

[T26] Swift：类与重写
来源：http://hz.bjfxy.top/gtjnhfrzen.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtrfwcyvag.html

[T27] Swift：错误处理
来源：http://hz.xinyue.icu/gtgkaacwvn.html

do { try f() } catch { print(error) }
来源：http://hz.iojbl.cn/gtssrlmsdy.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtkkdwdfcy.html

enum Color { case red, green }
来源：http://hz.jqgufenzy.top/gtyqyfknvq.html

[T29] Swift：guard 提前返回
来源：http://hz.dashuyun.cn/gtfryboofa.html

guard let x = opt else { return }
来源：http://hz.jinqigfzy.top/gtgjtdvzlx.html

[T30] Swift：协议
来源：http://hz.xinyue.icu/gtwoilvldp.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtdintwgxz.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtmlhvttba.html

print("Hello")
来源：http://hz.tanke756.top/gtmtwwvxtq.html

[T32] Lua：局部变量
来源：http://hz.cqqwz.cn/gtjisailam.html

local a = 1
来源：http://hz.gogol.net.cn/gtbnrpxwdb.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gtljelvhil.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtwtplgxtn.html

[T34] Lua：遍历表
来源：http://hz.nanxuanxn.top/gtiqtfbiqk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gzhubu.top/gtiwcdcahu.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gtqmdedrqz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangkeji.top/gtyetjrueq.html

[T36] Lua：函数
来源：http://hz.daria6918.cn/gtxwapxjqw.html

function add(a, b) return a + b end
来源：http://hz.sweek.top/gtrfbsuppw.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtxnvjovxf.html

"a" .. "b"
来源：http://hz.yangfankeji.com/gtiiycceru.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gtzexfvbfq.html

if x > 0 then print("正") end
来源：http://hz.yangfankeji.com/gtacuxyiey.html

[T39] Lua：模式匹配
来源：http://hz.xziqi.cn/gtpbqpsnni.html

string.find(s, "%d+")
来源：http://hz.chenlongwang.top/gtqxomddcd.html

[T40] Lua：元表
来源：http://hz.9152youxi.cn/gtrhbwrkqz.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gtjlfwzzwf.html

[T41] Perl：Hello World
来源：http://hz.nanxuanxn.top/gtypumjmgd.html

print "Hello\n";
来源：http://hz.aibaodan.cn/gtyoeteodk.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtbitfxptf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.quarkkingdee.top/gtfscbogke.html

[T43] Perl：字符串插值
来源：http://hz.aizwys.cn/gtvrcnisdu.html

"值: $a"
来源：http://hz.ywan-chungtsiang.top/gtpllhkcjs.html

[T44] Perl：条件
来源：http://hz.cashguo.top/gtmdgpeuyu.html

if ($a > 0) { print "正"; }
来源：http://hz.zhengqikj.top/gtqsejzsmf.html

[T45] Perl：数组遍历
来源：http://hz.andypj.xyz/gtphdxuyom.html

for my $x (@arr) { print $x; }
来源：http://hz.c1oappe.top/gtqrgophjd.html

[T46] Perl：哈希操作
来源：http://hz.cheryme.top/gtaiexjfvg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tanke756.top/gtdybblkzi.html

[T47] Perl：正则捕获
来源：http://hz.9152youxi.cn/gtqjxlpdlg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.aizwys.cn/gtskahyavz.html

[T48] Perl：正则替换
来源：http://hz.ydjk.org.cn/gtxzlvzdeh.html

$s =~ s/old/new/g;
来源：http://hz.zhongyouzk.top/gtnvzcybxs.html

[T49] Perl：函数
来源：http://hz.meibo888.top/gteofekzws.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tianlin.xyz/gtkopwmihz.html

[T50] Perl：逐行读文件
来源：http://hz.kuanghao11.cn/gtiipxaidv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.52xcode.cn/gtszkfvgez.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.52xcode.cn/gtvivqiwgc.html

[T51] Scala：Hello World
来源：http://hz.yueranfly.top/gtqkiylcth.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtuvbikwpy.html

[T52] Scala：变量
来源：http://hz.zhongyouzk.top/gthjstryve.html

val a = 1;  var b = 2
来源：http://hz.gzhubu.top/gtxjgedopm.html

[T53] Scala：字符串插值
来源：http://hz.shuidangran.top/gtewohtkgo.html

s"值: $b"
来源：http://hz.cucudq.cn/gtlzuudwrz.html

[T54] Scala：集合映射
来源：http://hz.xuanzx.com/gtbwilghmq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gtvtiyqxqe.html

[T55] Scala：集合过滤
来源：http://hz.snrcjt.cn/gtopblwtiz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.bjfxy.top/gtwuaqrihd.html

[T56] Scala：样例类
来源：http://hz.ppjwa.cn/gtgctyiasi.html

case class User(name: String, age: Int)
来源：http://hz.yanxiufei.cn/gtrnfxraor.html

[T57] Scala：模式匹配
来源：http://hz.zhiwuduotai.top/gtmwamilzm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.316326.xyz/gthpkmwhma.html

[T58] Scala：函数定义
来源：http://hz.andypj.xyz/gthxcrbyub.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hysaishi.cn/gtyrfgdeek.html

[T59] Scala：循环
来源：http://hz.daxiang520.top/gtibiaysqm.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj20258.top/gtfmpselfz.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gtqhkvamnd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhoulong.xyz/gtqlgvvrsr.html

================================================================================
来源：http://hz.tanke756.top/gtdxxaxffd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhoulong.xyz/gtdizcfnul.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbqtikumi.html

[U01] Py：创建虚拟环境
来源：http://hz.cdnleiting.top/gtzmitmlsm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnqzz.top/gthdwnuchz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhoulong.xyz/gtipghakse.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.bjfxy.top/gtuwuczsum.html

[U03] Py：加载 .env 配置
来源：http://hz.havefunace.top/gtczrolumx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.havefunace.top/gtnikkuhti.html

[U04] Py：变量调试打印
来源：http://hz.xingfuxueyuan.xyz/gtynohnsiv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtspxaehta.html

[U05] Py：列表去重且保序
来源：http://hz.jyoumei.cn/gtyoufvylx.html

list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtmkcsrpqc.html

[U06] Py：合并两个字典
来源：http://hz.jyoumei.cn/gtygdkmafh.html

{**a, **b}
来源：http://hz.jinqigfzy.top/gtimkgqfgp.html

[U07] Py：反转字典键值
来源：http://hz.sweek.top/gtqbxwvxob.html

{v: k for k, v in d.items()}
来源：http://hz.zhiwuduotai.top/gtpbpnwjzf.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gtirqqhkas.html

[y for x in nested for y in x]
来源：http://hz.meibo888.top/gtigdoncxe.html


<!-- 参考信息 -->