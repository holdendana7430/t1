代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gthpitdgts.html

[R66] 定时任务
来源：http://hz.yj20258.top/gtwzbmblxh.html

crontab -e;  crontab -l
来源：http://hz.xingfuxueyuan.xyz/gtkkxaoyvq.html

[R67] 生成随机十六进制串
来源：http://hz.nwbrower.top/gtljrsqnhs.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtvwsaereb.html

[R68] 计算文件校验值
来源：http://hz.fengsongda.top/gtrytscmti.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.svipenyu.cn/gtvvtpjugz.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gthqeduojf.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtnodcueko.html

[R70] 时间戳与互转
来源：http://hz.aibaodan.cn/gtydxevzqw.html

date +%s;  date -d @1700000000
来源：http://hz.sxryk.cn/gtlkuqywmf.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gtpsoamulr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtqpnxygnw.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gtaunvdmvo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cqqwz.cn/gtzfzttump.html

[R73] 分割大日志
来源：http://hz.nanxinkj.top/gtuzlszzfa.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtheyazlzx.html

[R74] 批量重命名
来源：http://hz.pycfn.com/gtqzqfeycb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtbayevvrx.html

[R75] 导出环境变量
来源：http://hz.hfpthk.cn/gtxzsdgcor.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.feifeiyinyue.top/gtumptjmin.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtdgfbutpx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuanzhike.top/gtochgkhqc.html

[R77] 读取用户输入
来源：http://hz.sweek.top/gtznbqynbm.html

read -rp "请输入: " ans
来源：http://hz.vqdsnc.cn/gtoygoreru.html

[R78] 交互式菜单
来源：http://hz.0kj1m.cn/gtttvnamwz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.feifeiyinyue.top/gtywkyufvw.html

[R79] 解析命令行选项
来源：http://hz.feifeiyinyue.top/gtvawkgqfd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jianghu66.top/gtzphkwoea.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtmxijemuu.html

time ./run.sh
来源：http://hz.jianghu66.top/gthsiwmmyn.html

================================================================================
来源：http://hz.bjfxy.top/gtrmqxbety.html

S. C / C++ 专题
来源：http://hz.shanyushiyangkeji.top/gtpriukoin.html

================================================================================
来源：http://hz.gotoacloud.top/gtoyhtcolt.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtlqbhoxws.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtgeljdweb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuanzhike.top/gtvxmdodlw.html

[S02] C：变量与格式化输出
来源：http://hz.sysykeji.top/gtoeucmwej.html

int a = 10; printf("%d\n", a);
来源：http://hz.sufxvd.cn/gtbrdwmxwg.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtrgpoeonl.html

int x; scanf("%d", &x);
来源：http://hz.ppjwa.cn/gtzqislaef.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gthgkdkepx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gaohongyu789.top/gtoxtpyqsx.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtipmzrofj.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtjbbhfanm.html

[S06] C：字符串比较
来源：http://hz.zhijiandao.cn/gtaxygwjpg.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtexkesuxk.html

[S07] C：数组遍历求和
来源：http://hz.c1oappe.top/gtbpnqlgtw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinyuanbaomall.cn/gtbxkqfygi.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtrjutnheb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangdashe.top/gthtxfhskp.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtzcnugssz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jianghu66.top/gtuhkttklt.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtwipljwnv.html

int *p = &a;  *p = 5;
来源：http://hz.zycfv.cn/gtjztynnqt.html

[S11] C：逐行读文件
来源：http://hz.chenjidiqi.icu/gtjucevllx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtdjtrncsk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yongpay.top/gtyatprcfd.html

fclose(f);
来源：http://hz.yangfankeji.com/gttqscyzsh.html

[S12] C：写文件
来源：http://hz.jinghuilouyu.cn/gtwpmygwkb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.bjfxy.top/gtommdklni.html

[S13] C：宏定义
来源：http://hz.yuxming.cn/gttbhwqxhg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zycfv.cn/gtchejqddx.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtlkttojjg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cashguo.top/gtnnbibbsz.html

[S15] C：类型转换
来源：http://hz.yuxming.cn/gtfgvzfdyo.html

(double) a / b
来源：http://hz.sweek.top/gtfnavijmo.html

[S16] C：位操作置位
来源：http://hz.hongshengwenyu.top/gtmnalfqje.html

x |= (1 << 3);
来源：http://hz.redwolf501.top/gtddarenvg.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtfbhlewwd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gogol.net.cn/gtqgawjsoh.html

[S18] C：命令行参数
来源：http://hz.jlsjyb.cn/gtuhvhezmj.html

int main(int argc, char **argv)
来源：http://hz.ydjk.org.cn/gtcuvxfwvw.html

[S19] C：快速排序
来源：http://hz.mhx1999.top/gtqlderuqa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtgtsbkvvm.html

[S20] C：二分查找
来源：http://hz.xingfuxueyuan.xyz/gtfdavsdkv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtjzqhhdsf.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtwpqniasb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gtcosvoizp.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtvozmbzey.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtckrkonmc.html

[S23] C：随机数
来源：http://hz.cqqwz.cn/gtptfbpuxq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtmfwnetff.html

[S24] C：获取本地时间
来源：http://hz.jinqigufen.top/gtyarxhrbo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pengpengdd.cyou/gtcjlgrghk.html

[S25] C：内存拷贝
来源：http://hz.nwbrower.top/gtkzcnzjgb.html

memcpy(dst, src, n);
来源：http://hz.hfpthk.cn/gtjeppolsz.html

[S26] C：内存清零
来源：http://hz.cdnleiting.top/gtytsxdscw.html

memset(a, 0, sizeof a);
来源：http://hz.chenzaomai.com/gtcmslqdlj.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtbvqjqkwu.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtawhrmucd.html

[S28] C：静态变量
来源：http://hz.redwolf501.top/gtutkapweq.html

static int counter = 0;
来源：http://hz.andypj.xyz/gtntwjtorn.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtvctkpqsg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtixjyixuh.html

[S30] C：头文件保护
来源：http://hz.52xcode.cn/gttwwhmkjz.html

#ifndef X_H
来源：http://hz.sysykeji.top/gthhpsthbb.html

#define X_H
来源：http://hz.yuxming.cn/gtslfpfjnf.html

#endif
来源：http://hz.ehwqpu.com/gtxxzieqyk.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gtaixhlyqk.html

#include <iostream>
来源：http://hz.tanke756.top/gthiesxtpf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhaomingkeji.xyz/gtksnskyuj.html

[S32] C++：字符串
来源：http://hz.shzxlz.cn/gtylqinqiy.html

std::string s = "hi";  s += "!";
来源：http://hz.zhongyouzk.top/gtjpgcxyac.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangkeji.top/gtmncvkqzj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tian-w.cn/gtrfrobckd.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gtvejxfnfm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shzxlz.cn/gtfriqzosz.html

[S35] C++：map
来源：http://hz.ydjk.org.cn/gtlxxkvrzn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtczzifkfd.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtfbvsxshm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtslawnijn.html

[S37] C++：set
来源：http://hz.chenzaomai.com/gtfybchmmo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hammf.cn/gtngxbahsr.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtqbjmxotg.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtuhsbmrux.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtjivkbqmu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ehwqpu.com/gtvliditsm.html

[S40] C++：查找元素
来源：http://hz.ydzc1.top/gtddrcjumk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.mhx1999.top/gtyberrnzm.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtypelxtgu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ybcxt.top/gtpobtxjco.html

[S42] C++：继承与虚函数
来源：http://hz.wangshuangyany.cn/gtadaipiuu.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtoqznubrf.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtgxfozvgd.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gtooscsyky.html

[S44] C++：引用传参
来源：http://hz.cdnleiting.top/gtuwjsdqmj.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gtiynvsesa.html

[S45] C++：lambda
来源：http://hz.jyoumei.cn/gtnjzzotiq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gtiawrtjzs.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtugoesone.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtprloqcmj.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtvsacheol.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtpapbhutr.html

[S48] C++：逐行读文件
来源：http://hz.yj20258888.top/gtiyevbumn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtvchibhwx.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gtrehwbmtj.html

[S49] C++：写文件
来源：http://hz.svipenyu.cn/gtefbizatv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinyuanbaomall.cn/gtybktljvc.html

[S50] C++：格式化数字
来源：http://hz.cucudq.cn/gtnupctfnb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pengpengdd.cyou/gtvxmlxjcf.html

[S51] C++：显式类型转换
来源：http://hz.jinqigufen.top/gtupkrvsub.html

static_cast<double>(a) / b
来源：http://hz.cucudq.cn/gtysoltrea.html

[S52] C++：const 与 noexcept
来源：http://hz.yj202588.top/gtvwqqqrru.html

int size() const noexcept { return n_; }
来源：http://hz.birdmap.top/gtawlymapj.html

[S53] C++：移动语义
来源：http://hz.redwolf501.top/gtfzzuscoi.html

std::vector<int> w = std::move(v);
来源：http://hz.cheryme.top/gtdwrmpsei.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtrbfxedwi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gtkgdaqcgf.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtuptwvqus.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ppjwa.cn/gtntgnyqph.html

[S56] C++：optional
来源：http://hz.gzhubu.top/gtqqpnscfu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtvflkjema.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangtech.top/gtdpzulmxm.html

constexpr int N = 10;
来源：http://hz.xuetiantiany.cn/gtmxvqvdmc.html

[S58] C++：命名空间
来源：http://hz.daria6918.cn/gtacvrqakw.html

namespace ns { int f() { return 1; } }
来源：http://hz.guowangkeji.top/gtthgrmlcc.html

[S59] C++：静态断言
来源：http://hz.9152youxi.cn/gtwsawubxu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ehwqpu.com/gtgajvtuhw.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtvmyghgmf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.bjfxy.top/gtzlsnrlws.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdlybsdhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtmlneruox.html

================================================================================
来源：http://hz.wangdashe.top/gtfnuznqfi.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtqvbfdmkk.html

println("Hello")
来源：http://hz.zhengqikj.top/gtczjrjwjw.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtvciwwrca.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gtaztwrpez.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtggfdknng.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtjucveeya.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtgtfnzyrv.html

val n: String? = null;  n?.length
来源：http://hz.jianghu66.top/gtoqostxju.html

[T05] Kotlin：when 表达式
来源：http://hz.gogol.net.cn/gtjilpylbz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtufwoshmu.html

[T06] Kotlin：集合映射
来源：http://hz.aizwys.cn/gtiifipkvu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.andypj.xyz/gttygusnmy.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gtjbjjrxlk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gaohongyu789.top/gtsofxpkjv.html

[T08] Kotlin：数据类
来源：http://hz.yueranfly.top/gtvngbjbvh.html

data class User(val name: String, val age: Int)
来源：http://hz.tian-w.cn/gtwvwfswas.html

[T09] Kotlin：扩展函数
来源：http://hz.vqdsnc.cn/gtsapmfgzb.html

fun String.exclaim() = this + "!"
来源：http://hz.yj202588.top/gtuizysrls.html

[T10] Kotlin：默认参数
来源：http://hz.yuanzhike.top/gtjrxapxnd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.quarkkingdee.top/gtadrzhfnz.html

[T11] Kotlin：协程
来源：http://hz.yongpay.top/gtjdynohvy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jiagoushi.top/gtyatjhdwx.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtcrhnkhqo.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258.top/gtqyyygbij.html

[T13] Kotlin：只读 Map
来源：http://hz.jianghu66.top/gtinippghs.html

val m = mapOf("a" to 1)
来源：http://hz.cheryme.top/gtipkkmlnz.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtjkbyevbl.html

for (i in 1..10) println(i)
来源：http://hz.jinqigufen.top/gtntaboqxf.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtnkkqbicx.html

interface Shape { fun area(): Double }
来源：http://hz.svipenyu.cn/gtavysxkfb.html

[T16] Swift：Hello World
来源：http://hz.dianchejie.cn/gtngzowsfm.html

print("Hello")
来源：http://hz.daria6918.cn/gtihsxkxcn.html

[T17] Swift：变量与常量
来源：http://hz.zycfv.cn/gtawlkzwfa.html

var a = 1;  let b = 2
来源：http://hz.hywenlv.cn/gtfekzobpv.html

[T18] Swift：字符串插值
来源：http://hz.jlsjyb.cn/gtlkbbcguk.html

"值: \(b)"
来源：http://hz.c1oappe.top/gttrfseoya.html

[T19] Swift：可选绑定
来源：http://hz.feifeiyinyue.top/gtbjrqmccd.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gteubaagwg.html

[T20] Swift：数组操作
来源：http://hz.zdqjudy.top/gtbzwlrfuu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.bjfxy.top/gtvqyyfpds.html

[T21] Swift：遍历
来源：http://hz.sufxvd.cn/gtlpblgugf.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtuxqgbfyx.html

[T22] Swift：字典
来源：http://hz.aizwys.cn/gtubcrnxbd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shuidangran.top/gtgnlgjrly.html

[T23] Swift：函数
来源：http://hz.yuanzhike.top/gtwgatynda.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.c1oappe.top/gticpgrfrw.html

[T24] Swift：闭包
来源：http://hz.52xcode.cn/gtebohwibe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigfzy.top/gtwleeamkz.html

[T25] Swift：结构体
来源：http://hz.hysaishi.cn/gtzidvssch.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gteptdfnlk.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtcfipmyhw.html

class A: Base { override func f() {} }
来源：http://hz.ivvv.top/gtbojfvmij.html

[T27] Swift：错误处理
来源：http://hz.sysykeji.top/gtfzsdzjbb.html

do { try f() } catch { print(error) }
来源：http://hz.xylfe.cn/gtshfmzozc.html

[T28] Swift：枚举
来源：http://hz.redwolf501.top/gtmygqccfc.html

enum Color { case red, green }
来源：http://hz.vqdsnc.cn/gthivykvor.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtsbcwnaoy.html

guard let x = opt else { return }
来源：http://hz.chenzaomai.com/gtlbfabdmn.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtcpezdobg.html

protocol Shape { func area() -> Double }
来源：http://hz.hfpthk.cn/gtyfbkjhax.html

[T31] Lua：Hello World
来源：http://hz.jinyuanbaomall.cn/gtwgaigvgf.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtphpmhkni.html

[T32] Lua：局部变量
来源：http://hz.yueranfly.top/gtlipuzdyy.html

local a = 1
来源：http://hz.aizwys.cn/gtpvhtdrsi.html

[T33] Lua：表（数组）
来源：http://hz.zhoulong.xyz/gtehuoskhe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ybcxt.top/gtghecfxip.html

[T34] Lua：遍历表
来源：http://hz.cdnleiting.top/gtougporlj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtzybthaxy.html

[T35] Lua：字典表
来源：http://hz.dianchejie.cn/gtbkqqopsk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nanxinkj.top/gtwqkrarji.html

[T36] Lua：函数
来源：http://hz.wangshuangyany.cn/gtqncqaewb.html

function add(a, b) return a + b end
来源：http://hz.hammf.cn/gtohpsjsvj.html

[T37] Lua：字符串拼接
来源：http://hz.zhiwuduotai.top/gtobtamier.html

"a" .. "b"
来源：http://hz.pycfn.com/gtdapsgyue.html

[T38] Lua：条件
来源：http://hz.daria6918.cn/gtdzyjxdyz.html

if x > 0 then print("正") end
来源：http://hz.jinyuanbaomall.cn/gtjiblvoir.html

[T39] Lua：模式匹配
来源：http://hz.chenzaomai.com/gthktrsnsg.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtsmnalvyh.html

[T40] Lua：元表
来源：http://hz.xziqi.cn/gttrfflvzb.html

setmetatable({}, { __index = base })
来源：http://hz.ydjk.org.cn/gtzqcvqxox.html

[T41] Perl：Hello World
来源：http://hz.hammf.cn/gtuipsrpog.html

print "Hello\n";
来源：http://hz.wangdashe.top/gtxohkqpfe.html

[T42] Perl：变量类型
来源：http://hz.yongpay.top/gtfnbjihgp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhaomingkeji.xyz/gtglllkbmu.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtbtkxrmpk.html

"值: $a"
来源：http://hz.xinyue.icu/gthulyvdgo.html

[T44] Perl：条件
来源：http://hz.ydjk.org.cn/gtsqbgjdgn.html

if ($a > 0) { print "正"; }
来源：http://hz.chenlongwang.top/gtutsxsblv.html

[T45] Perl：数组遍历
来源：http://hz.9152youxi.cn/gtkurowkoh.html

for my $x (@arr) { print $x; }
来源：http://hz.meibo888.top/gtzaigxynb.html

[T46] Perl：哈希操作
来源：http://hz.shanyushiyangtech.top/gtmjbsjfuf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnqzz.top/gtlesyswti.html

[T47] Perl：正则捕获
来源：http://hz.jianghu66.top/gtqkkndjhm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xziqi.cn/gtbhmzavkh.html

[T48] Perl：正则替换
来源：http://hz.sysykeji.top/gtazbadamo.html

$s =~ s/old/new/g;
来源：http://hz.jinqigufen.top/gtmjyivdok.html

[T49] Perl：函数
来源：http://hz.52xcode.cn/gtmxipzoir.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnxiangtu.top/gtrpwjgwxh.html

[T50] Perl：逐行读文件
来源：http://hz.sweek.top/gtflvmkfiy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtkhzvkwmi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenjidiqi.icu/gtqarxjeog.html

[T51] Scala：Hello World
来源：http://hz.9152youxi.cn/gtkxnatick.html

println("Hello")
来源：http://hz.jyoumei.cn/gtpvgnotbo.html

[T52] Scala：变量
来源：http://hz.nanxinkj.top/gtgwqhrbzg.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangkeji.top/gtaipojsvt.html

[T53] Scala：字符串插值
来源：http://hz.sufxvd.cn/gtploksjgv.html

s"值: $b"
来源：http://hz.52xcode.cn/gtcnjsgmwv.html

[T54] Scala：集合映射
来源：http://hz.wangdashe.top/gtthaatoqa.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yonumen.top/gttajvgavx.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangtech.top/gtbbsquyke.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhaomingkeji.xyz/gtyiqnovph.html

[T56] Scala：样例类
来源：http://hz.zycfv.cn/gthtwqxzkm.html

case class User(name: String, age: Int)
来源：http://hz.bjfxy.top/gtdhsdjgvi.html

[T57] Scala：模式匹配
来源：http://hz.snrcjt.cn/gtswgteesm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ywan-chungtsiang.top/gtbdjjlioi.html

[T58] Scala：函数定义
来源：http://hz.yvedp.cn/gtaglkrbbj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gtlpkfqqbw.html

[T59] Scala：循环
来源：http://hz.guowangkeji.top/gtacsioays.html

for (i <- 1 to 10) println(i)
来源：http://hz.pengpengdd.cyou/gtwiundsfa.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangkeji.top/gttxnawzjt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.pengpengdd.cyou/gtfentfach.html

================================================================================
来源：http://hz.chenzaomai.com/gtqhkzyeod.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xylfe.cn/gtzhmbtvkz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcqbntldf.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gtztibzeiw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sufxvd.cn/gttgernimq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnxiangtu.top/gtknqxigof.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.smart0.xyz/gtcyuvzkeq.html

[U03] Py：加载 .env 配置
来源：http://hz.zhiwuduotai.top/gtajbvifzj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.snrcjt.cn/gtygsdrdqo.html

[U04] Py：变量调试打印
来源：http://hz.chenlongwang.top/gtuupxmyin.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yangfankeji.com/gtsclcfeqz.html

[U05] Py：列表去重且保序
来源：http://hz.birdmap.top/gtqaunwzez.html

list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtdxyoxryi.html

[U06] Py：合并两个字典
来源：http://hz.ehwqpu.com/gtovgklzno.html

{**a, **b}
来源：http://hz.sufxvd.cn/gtotophpjj.html


<!-- 参考信息 -->