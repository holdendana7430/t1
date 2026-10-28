代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtxbodlvre.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtsjogqamf.html

crontab -e;  crontab -l
来源：http://hz.iojbl.cn/gtxkfomztn.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtqlwqnnxq.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtnbfbxvll.html

[R68] 计算文件校验值
来源：http://hz.sufxvd.cn/gtakytcaik.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xziqi.cn/gtjjzgptjg.html

[R69] 生成随机密码
来源：http://hz.cucudq.cn/gtzsvkxett.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtdblmmnqs.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gtbaeqqqwd.html

date +%s;  date -d @1700000000
来源：http://hz.zhengqikj.top/gtvgraggxt.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gtlhlntgbm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenzaomai.com/gttsfcjxcs.html

[R72] 等待端口就绪
来源：http://hz.sufxvd.cn/gtsdyazims.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtubjnylsk.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtyvxfrdtq.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gtbkvtvzba.html

[R74] 批量重命名
来源：http://hz.ydjk.org.cn/gtnhitxaxi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gtdtslcyat.html

[R75] 导出环境变量
来源：http://hz.shuidangran.top/gteoflfppi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cqqwz.cn/gtdvdpqeep.html

[R76] 使用临时文件
来源：http://hz.cucudq.cn/gtwzxvjrew.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtssjetgpm.html

[R77] 读取用户输入
来源：http://hz.cucudq.cn/gtsudrrpgl.html

read -rp "请输入: " ans
来源：http://hz.chenlongwang.top/gtfqmbbydq.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtegzoskcr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenjidiqi.icu/gthjggfexq.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtnireibpe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtpatmqoai.html

[R80] 查看脚本执行耗时
来源：http://hz.yueranfly.top/gtxahlzapr.html

time ./run.sh
来源：http://hz.jlsjyb.cn/gtntfbjpqc.html

================================================================================
来源：http://hz.yonumen.top/gtwcmwfxvf.html

S. C / C++ 专题
来源：http://hz.shangyingyoupin.top/gtukrkdfwr.html

================================================================================
来源：http://hz.xylfe.cn/gtzbkwbfgi.html

[S01] C：Hello World
来源：http://hz.chenjidiqi.icu/gtqwvcqucc.html

#include <stdio.h>
来源：http://hz.yongpay.top/gtzepfpsqi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtaartoktm.html

[S02] C：变量与格式化输出
来源：http://hz.chenjidiqi.icu/gtxtcrphpk.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtbxjjrrat.html

[S03] C：读入整数
来源：http://hz.hfpthk.cn/gtfxowcpkh.html

int x; scanf("%d", &x);
来源：http://hz.kuanghao11.cn/gtelwdimjz.html

[S04] C：字符串复制
来源：http://hz.yonumen.top/gtzetlaxll.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.c1oappe.top/gtkuvizgkj.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtizveomzy.html

strlen(s)
来源：http://hz.dashuyun.cn/gtdeqwzzcq.html

[S06] C：字符串比较
来源：http://hz.0kj1m.cn/gtzfjktbjl.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtducnsyzx.html

[S07] C：数组遍历求和
来源：http://hz.andypj.xyz/gtpehqcuoz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gttkchjmcj.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtiaqzzusj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtivtxmozh.html

[S09] C：结构体定义与初始化
来源：http://hz.gaohongyu789.top/gtevwwrrki.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guannengcc.top/gtiozbsjum.html

[S10] C：指针与解引用
来源：http://hz.yj20258888.top/gtlzsdxkig.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gtcxcxowen.html

[S11] C：逐行读文件
来源：http://hz.chenlongwang.top/gtcjnntkyk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cheryme.top/gtemiezagt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yonumen.top/gtczssuyle.html

fclose(f);
来源：http://hz.316326.xyz/gtiqoeiqad.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gtcllmqlna.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtysznizio.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtzflfhupl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtcdhtxhvx.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtvlywpypn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtfkgbtioo.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtgljvbbff.html

(double) a / b
来源：http://hz.chenzaomai.com/gtjsixyfrc.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gteausnekt.html

x |= (1 << 3);
来源：http://hz.gaohongyu789.top/gtlfogwswy.html

[S17] C：安全拼接字符串
来源：http://hz.zhijiandao.cn/gtaobetfqe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhoulong.xyz/gtegymhytv.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtghvpskxy.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtzhusfgbw.html

[S19] C：快速排序
来源：http://hz.nanxinkj.top/gtunrexvew.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtwhilvgat.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtkbejuzee.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gtcptdpxdo.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtdyrrctfe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tanke756.top/gtmxjqmdxz.html

[S22] C：字符串转数字
来源：http://hz.0kj1m.cn/gtuirpqxdj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hysaishi.cn/gtadpwujdq.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtczqlqfzo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gtkaojtprw.html

[S24] C：获取本地时间
来源：http://hz.cheryme.top/gtvncetlxw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtpdmyltqe.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtoxrvpkql.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtysjvbpyx.html

[S26] C：内存清零
来源：http://hz.iojbl.cn/gtkadnorxg.html

memset(a, 0, sizeof a);
来源：http://hz.pycfn.com/gtaoifgowt.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtbtntsncd.html

const double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtmqnfmdyb.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtmygrpmzy.html

static int counter = 0;
来源：http://hz.nanxinkj.top/gtijfkvqlr.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gttfmgnrhp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jyoumei.cn/gtbvsolcwy.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtartilpzt.html

#ifndef X_H
来源：http://hz.xinyue.icu/gtqfysiqqb.html

#define X_H
来源：http://hz.bjfxy.top/gtalqvzbif.html

#endif
来源：http://hz.9152youxi.cn/gtwjmrzctd.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtxqgrzkph.html

#include <iostream>
来源：http://hz.hysaishi.cn/gtfasdwdna.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtydwtnaof.html

[S32] C++：字符串
来源：http://hz.xuanzx.com/gtchorbnph.html

std::string s = "hi";  s += "!";
来源：http://hz.daxiang520.top/gtxxrcuvqj.html

[S33] C++：vector 增删
来源：http://hz.havefunace.top/gttlpkxafh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ivvv.top/gtsucvhqwg.html

[S34] C++：遍历 vector
来源：http://hz.chenjidiqi.icu/gtbrhbrwti.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtbumolllz.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtdhcdpwpg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtoklngufn.html

[S36] C++：unordered_map
来源：http://hz.jinqigufen.top/gtzjxntblp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtiyhyrrfn.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gtyqkloqad.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtdqphseay.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtpgvwiaqa.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtlewsxqdp.html

[S39] C++：自定义比较器排序
来源：http://hz.zycfv.cn/gtinhbdqpr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yongpay.top/gtgqpthsia.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtzkzltdxu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtrbzmwtxs.html

[S41] C++：类与构造函数
来源：http://hz.dianchejie.cn/gtpqtxisxx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258.top/gttkqhiwkn.html

[S42] C++：继承与虚函数
来源：http://hz.cdnleiting.top/gthhswlmxk.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtnsiuuddt.html

[S43] C++：智能指针
来源：http://hz.cheryme.top/gtvbjuxata.html

auto p = std::make_unique<int>(5);
来源：http://hz.pengpengdd.cyou/gtrsaarequ.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtxrxemazn.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtpzlsnulz.html

[S45] C++：lambda
来源：http://hz.ydzc1.top/gtvewlsttf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gtjpnonhdw.html

[S46] C++：函数模板
来源：http://hz.vqdsnc.cn/gtdgnqhypv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sufxvd.cn/gtbfphuden.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtmrwbmpix.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.vqdsnc.cn/gtewvgnraz.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtvtqabszo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gthzctyxnr.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gtcudfeewc.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtspebcxnm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cucudq.cn/gtkprssgrw.html

[S50] C++：格式化数字
来源：http://hz.yvedp.cn/gtxarqcwvq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtqqyimozl.html

[S51] C++：显式类型转换
来源：http://hz.jyoumei.cn/gtghdoiizb.html

static_cast<double>(a) / b
来源：http://hz.cqqwz.cn/gtxrikhqib.html

[S52] C++：const 与 noexcept
来源：http://hz.fzhhl.top/gtkkfplhrg.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtkjukuenw.html

[S53] C++：移动语义
来源：http://hz.jinqigufen.top/gtibgggkzh.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtlxvobuaf.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtegiuwklz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhaomingkeji.xyz/gtpmzemiol.html

[S55] C++：结构化绑定
来源：http://hz.c1oappe.top/gtcdiqdnfi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtjftunifx.html

[S56] C++：optional
来源：http://hz.mhx1999.top/gtlfaxrcpq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtkllpzvxh.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtenorufaf.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtzxuxzzes.html

[S58] C++：命名空间
来源：http://hz.sysykeji.top/gtqabgjkke.html

namespace ns { int f() { return 1; } }
来源：http://hz.ybcxt.top/gtrgjguwgd.html

[S59] C++：静态断言
来源：http://hz.xingfuxueyuan.xyz/gtzieddreo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtcwcxdyyf.html

[S60] C++：遍历并删除元素
来源：http://hz.wangdashe.top/gtashvpbds.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtpuukvdus.html

================================================================================
来源：http://hz.yuanzhike.top/gtvsoqxgfa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtpdhdvjsz.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtykpscrck.html

[T01] Kotlin：Hello World
来源：http://hz.guannengcc.top/gtrsrmoaud.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtxszrhduj.html

[T02] Kotlin：变量
来源：http://hz.jqgfzy.top/gtfmafqnmk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.pengpengdd.cyou/gtpcfvcnxi.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gtzzfzdzfb.html

"值: $b"
来源：http://hz.ybcxt.top/gtsqkkgxol.html

[T04] Kotlin：空安全
来源：http://hz.tanke756.top/gtujuxxrck.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gtaokwsosq.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtxzkziczb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gtjdarbono.html

[T06] Kotlin：集合映射
来源：http://hz.sxryk.cn/gtjoqcqxom.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ivvv.top/gtfugjzwrs.html

[T07] Kotlin：集合过滤
来源：http://hz.ybcxt.top/gtdgeepoda.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fzhhl.top/gtgqpdctei.html

[T08] Kotlin：数据类
来源：http://hz.dashuyun.cn/gttnraknbw.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxuanxn.top/gtvsdmuqdi.html

[T09] Kotlin：扩展函数
来源：http://hz.birdmap.top/gtvmuhjbba.html

fun String.exclaim() = this + "!"
来源：http://hz.sweek.top/gtruztsasc.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gtdlprwous.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhengqikj.top/gtvfhtjsgo.html

[T11] Kotlin：协程
来源：http://hz.jinghuilouyu.cn/gtolnwpyva.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gotoacloud.top/gtatmdfcor.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtcuwtfwwh.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgufenzy.top/gtokqauika.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxinkj.top/gtjrgbpgof.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtewavtdrm.html

[T14] Kotlin：循环
来源：http://hz.dashuyun.cn/gtedjvgytm.html

for (i in 1..10) println(i)
来源：http://hz.shuidangran.top/gtymuoxsqc.html

[T15] Kotlin：接口
来源：http://hz.c1oappe.top/gtaysjsfia.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gtqhxtlprz.html

[T16] Swift：Hello World
来源：http://hz.zhengqikj.top/gtuyjyygqb.html

print("Hello")
来源：http://hz.ehwqpu.com/gtrekhkypg.html

[T17] Swift：变量与常量
来源：http://hz.havefunace.top/gtrajsgket.html

var a = 1;  let b = 2
来源：http://hz.nwbrower.top/gtukkpixnn.html

[T18] Swift：字符串插值
来源：http://hz.dashuyun.cn/gtvzrpweoa.html

"值: \(b)"
来源：http://hz.nanxuanxn.top/gtjmwkwelr.html

[T19] Swift：可选绑定
来源：http://hz.jlsjyb.cn/gtfmfithtw.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtwwxxudfu.html

[T20] Swift：数组操作
来源：http://hz.hysaishi.cn/gtjxfpwzdu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tian-w.cn/gtmolzycno.html

[T21] Swift：遍历
来源：http://hz.yvedp.cn/gtnwxtwuvh.html

for x in a { print(x) }
来源：http://hz.chenzaomai.com/gtjxwprjhj.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtgphdwqma.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yanxiufei.cn/gtnojfeqtc.html

[T23] Swift：函数
来源：http://hz.wangdashe.top/gtmtchmrnv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigfzy.top/gtcsfeczjh.html

[T24] Swift：闭包
来源：http://hz.gzhubu.top/gtetmacffi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xylfe.cn/gtmlfiyqgb.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtdamjatsq.html

struct P { var x: Int }
来源：http://hz.c1oappe.top/gtcbohvtui.html

[T26] Swift：类与重写
来源：http://hz.hammf.cn/gtudyhvoyb.html

class A: Base { override func f() {} }
来源：http://hz.feifeiyinyue.top/gtuphdpyho.html

[T27] Swift：错误处理
来源：http://hz.yanxiufei.cn/gtpanniati.html

do { try f() } catch { print(error) }
来源：http://hz.sweek.top/gtcjlhrjxn.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtylyrwuaj.html

enum Color { case red, green }
来源：http://hz.zhaomingkeji.xyz/gtihupzsfr.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtkmaxwpwk.html

guard let x = opt else { return }
来源：http://hz.pycfn.com/gthovvxqml.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gtrnxtjiep.html

protocol Shape { func area() -> Double }
来源：http://hz.iojbl.cn/gtbkhngnvd.html

[T31] Lua：Hello World
来源：http://hz.ehwqpu.com/gtkqryovpy.html

print("Hello")
来源：http://hz.hammf.cn/gtnwngbapq.html

[T32] Lua：局部变量
来源：http://hz.quarkkingdee.top/gthaxlskkw.html

local a = 1
来源：http://hz.chenlongwang.top/gtzjhmvjlo.html

[T33] Lua：表（数组）
来源：http://hz.xingfuxueyuan.xyz/gtfthcbtje.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtenhezeno.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtdcurdauw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shanyushiyangtech.top/gteatgdxse.html

[T35] Lua：字典表
来源：http://hz.yj20258888.top/gtijtcezxi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nanxuanxn.top/gtiuvbnvgr.html

[T36] Lua：函数
来源：http://hz.jianghu66.top/gteqedvqhy.html

function add(a, b) return a + b end
来源：http://hz.jinqigfzy.top/gtlrmojqbx.html

[T37] Lua：字符串拼接
来源：http://hz.c1oappe.top/gtaezzurlz.html

"a" .. "b"
来源：http://hz.zhengqikj.top/gtyhwccict.html

[T38] Lua：条件
来源：http://hz.ivvv.top/gtudqqccgt.html

if x > 0 then print("正") end
来源：http://hz.cucudq.cn/gtffwwdrfk.html

[T39] Lua：模式匹配
来源：http://hz.ydzc1.top/gtgyuleqqr.html

string.find(s, "%d+")
来源：http://hz.chenjidiqi.icu/gtajmuednx.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtucslrqix.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtxsvwxnlz.html

[T41] Perl：Hello World
来源：http://hz.ywan-chungtsiang.top/gtkvaihcyr.html

print "Hello\n";
来源：http://hz.zycfv.cn/gtbrotjcbq.html

[T42] Perl：变量类型
来源：http://hz.cucudq.cn/gtpvcwikeg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.kuanghao11.cn/gtiihmoyvg.html

[T43] Perl：字符串插值
来源：http://hz.hnxiangtu.top/gtcfruoehl.html

"值: $a"
来源：http://hz.xylfe.cn/gtrzpcveur.html

[T44] Perl：条件
来源：http://hz.zhengqikj.top/gtgfhmmclx.html

if ($a > 0) { print "正"; }
来源：http://hz.zhongyouzk.top/gthdteteou.html

[T45] Perl：数组遍历
来源：http://hz.zhengqikj.top/gtktokkqru.html

for my $x (@arr) { print $x; }
来源：http://hz.jinghuilouyu.cn/gtpzloicbr.html

[T46] Perl：哈希操作
来源：http://hz.shangyingyoupin.top/gtiuntygnu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jianghu66.top/gtwgzblydh.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangtech.top/gtzazzfjxa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtdjeoxdls.html

[T48] Perl：正则替换
来源：http://hz.zhengqikj.top/gtyhteswcd.html

$s =~ s/old/new/g;
来源：http://hz.havefunace.top/gtcxkcmvdw.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gtfdfnojba.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtlwyakgwt.html

[T50] Perl：逐行读文件
来源：http://hz.shzxlz.cn/gtvzslgasq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jiagoushi.top/gteznkhmmv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenzaomai.com/gtamkelins.html

[T51] Scala：Hello World
来源：http://hz.aizwys.cn/gtcusnpevo.html

println("Hello")
来源：http://hz.316326.xyz/gtndojsolp.html

[T52] Scala：变量
来源：http://hz.mhx1999.top/gtkzfnsitj.html

val a = 1;  var b = 2
来源：http://hz.dianchejie.cn/gtrfqlaevc.html

[T53] Scala：字符串插值
来源：http://hz.meibo888.top/gtegvddjpr.html

s"值: $b"
来源：http://hz.iojbl.cn/gtdnnmrcfl.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gttsnrghve.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuanzhike.top/gteriwuxsl.html

[T55] Scala：集合过滤
来源：http://hz.nanxinkj.top/gthbumcpco.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.c1oappe.top/gtelkybdul.html

[T56] Scala：样例类
来源：http://hz.mhx1999.top/gtbpfddkry.html

case class User(name: String, age: Int)
来源：http://hz.sufxvd.cn/gtvtaucmnr.html

[T57] Scala：模式匹配
来源：http://hz.jinghuilouyu.cn/gtxvoysdfo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnxiangtu.top/gtcgnybrfe.html

[T58] Scala：函数定义
来源：http://hz.yanxiufei.cn/gtuqcekufa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.meibo888.top/gtqdizeyai.html

[T59] Scala：循环
来源：http://hz.cucudq.cn/gtmvanrwzy.html

for (i <- 1 to 10) println(i)
来源：http://hz.daxiang520.top/gtbcnosudl.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtoxlxgkhb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dashuyun.cn/gtutsoheme.html

================================================================================
来源：http://hz.pycfn.com/gtgymtrrxe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hammf.cn/gtrmqbkfun.html

================================================================================
来源：http://hz.nwbrower.top/gtmgvgqhoq.html

[U01] Py：创建虚拟环境
来源：http://hz.tanke756.top/gtsjnsvfxo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.fzhhl.top/gttmvaumir.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jiagoushi.top/gtfhafipff.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gtbfiiqotw.html

[U03] Py：加载 .env 配置
来源：http://hz.bjfxy.top/gtneikighh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtwvtctrtg.html

[U04] Py：变量调试打印
来源：http://hz.andypj.xyz/gtvpobvakj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuetiantiany.cn/gtkysozgxg.html

[U05] Py：列表去重且保序
来源：http://hz.chenjidiqi.icu/gtdcbibntn.html

list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtbbfnahii.html

[U06] Py：合并两个字典
来源：http://hz.jinqigfzy.top/gtozjarwbg.html

{**a, **b}
来源：http://hz.vqdsnc.cn/gtqyfmnyxi.html


<!-- 参考信息 -->