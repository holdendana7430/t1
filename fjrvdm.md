代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydjk.org.cn/gtmwmyhrcq.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtrynagiic.html

crontab -e;  crontab -l
来源：http://hz.meibo888.top/gtfdoyxecr.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtxmwylzye.html

openssl rand -hex 16
来源：http://hz.chenlongwang.top/gttrwajotu.html

[R68] 计算文件校验值
来源：http://hz.jqgufenzy.top/gtvhwulxwo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtzibxanhi.html

[R69] 生成随机密码
来源：http://hz.nanxinkj.top/gtofkoisrl.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgufenzy.top/gtgvxwakah.html

[R70] 时间戳与互转
来源：http://hz.birdmap.top/gtrpozacvf.html

date +%s;  date -d @1700000000
来源：http://hz.zhengqikj.top/gthefyqudr.html

[R71] 日期格式化
来源：http://hz.kuanghao11.cn/gtgwbbyqtc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtwtldvuao.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtmjlfplqb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtkhbwxvad.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtefxrlunk.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtzazncosf.html

[R74] 批量重命名
来源：http://hz.nanxuanxn.top/gtwpcrmeij.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtuhnkspls.html

[R75] 导出环境变量
来源：http://hz.cucudq.cn/gtgxujuimw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gthpofzzse.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtaihsxaua.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtanexbeiy.html

[R77] 读取用户输入
来源：http://hz.zhengqikj.top/gtqjpbufmf.html

read -rp "请输入: " ans
来源：http://hz.sweek.top/gtoczjjkny.html

[R78] 交互式菜单
来源：http://hz.yuxming.cn/gtbbzsabzk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxuanxn.top/gtqhrsoobr.html

[R79] 解析命令行选项
来源：http://hz.yj20258.top/gtfsodyywy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhaomingkeji.xyz/gtwmzhalvl.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigufen.top/gtujqhhkpf.html

time ./run.sh
来源：http://hz.sxryk.cn/gtjtvoxgvy.html

================================================================================
来源：http://hz.shuidangran.top/gtfcsazhxd.html

S. C / C++ 专题
来源：http://hz.gogol.net.cn/gtbtrkpbcl.html

================================================================================
来源：http://hz.jiagoushi.top/gtxrwpwzjk.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gteuzceoyl.html

#include <stdio.h>
来源：http://hz.yvedp.cn/gtkbewmcjv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ivvv.top/gtvsorqqcd.html

[S02] C：变量与格式化输出
来源：http://hz.fengsongda.top/gtqazchchl.html

int a = 10; printf("%d\n", a);
来源：http://hz.aizwys.cn/gtrwtewbqp.html

[S03] C：读入整数
来源：http://hz.jlsjyb.cn/gtzmcrlgqa.html

int x; scanf("%d", &x);
来源：http://hz.gotoacloud.top/gtxwtmeuec.html

[S04] C：字符串复制
来源：http://hz.yuxming.cn/gtyshgfmxz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxuanxn.top/gtyntdyaxa.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtjzcnircb.html

strlen(s)
来源：http://hz.fzhhl.top/gticobhjsb.html

[S06] C：字符串比较
来源：http://hz.yuanzhike.top/gtulqbmueq.html

strcmp(a, b) == 0
来源：http://hz.cashguo.top/gtednfjoyd.html

[S07] C：数组遍历求和
来源：http://hz.zhongyouzk.top/gtolxuozhm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258.top/gtchhmieai.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtesibhxji.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hysaishi.cn/gtubljsuqb.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtvxtihhmj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgufenzy.top/gtytqbpzuw.html

[S10] C：指针与解引用
来源：http://hz.gotoacloud.top/gtwqerqxky.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gtanyaazcq.html

[S11] C：逐行读文件
来源：http://hz.ppjwa.cn/gtvttbkuhr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shzxlz.cn/gtlwtgyblq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zdqjudy.top/gtpbydmvua.html

fclose(f);
来源：http://hz.jianghu66.top/gtumoratqv.html

[S12] C：写文件
来源：http://hz.dashuyun.cn/gtmgdlixih.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jyoumei.cn/gtboodhixz.html

[S13] C：宏定义
来源：http://hz.redwolf501.top/gtueiqncwl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.kuanghao11.cn/gtdaxjwmgc.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtgovadsbj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xinyue.icu/gtwjdamlgh.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtxjawpdbo.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtjzakxxmr.html

[S16] C：位操作置位
来源：http://hz.gzhubu.top/gtjksftvzb.html

x |= (1 << 3);
来源：http://hz.xingfuxueyuan.xyz/gtysqikmvd.html

[S17] C：安全拼接字符串
来源：http://hz.jianghu66.top/gtfjivqedc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtxgfrczuv.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangtech.top/gtjkqnebxi.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtioziabtq.html

[S19] C：快速排序
来源：http://hz.hywenlv.cn/gtbphgllkv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtdrdgkowj.html

[S20] C：二分查找
来源：http://hz.sysykeji.top/gtlzokffyr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtgmdsbwkr.html

[S21] C：字符类别判断
来源：http://hz.zycfv.cn/gtozvlduxb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtxdttaxwa.html

[S22] C：字符串转数字
来源：http://hz.zycfv.cn/gtttzevsmv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gtwkpcsbmg.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtcduwkdke.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxinkj.top/gtimmefvdk.html

[S24] C：获取本地时间
来源：http://hz.redwolf501.top/gtfqltqfyo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtogrzeduv.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtknepymwy.html

memcpy(dst, src, n);
来源：http://hz.xingfuxueyuan.xyz/gtdetbhtdd.html

[S26] C：内存清零
来源：http://hz.jyoumei.cn/gtdeqfthuv.html

memset(a, 0, sizeof a);
来源：http://hz.hnqzz.top/gtbaofgcra.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtyzzxljfy.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gtasksvoii.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtaulxecxz.html

static int counter = 0;
来源：http://hz.guannengcc.top/gtzqdogdho.html

[S29] C：变参函数
来源：http://hz.ywan-chungtsiang.top/gtostfyoqu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258888.top/gtdyiiqgun.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtrgsisniw.html

#ifndef X_H
来源：http://hz.c1oappe.top/gtghnyvqnz.html

#define X_H
来源：http://hz.jyoumei.cn/gtsahgnlfn.html

#endif
来源：http://hz.havefunace.top/gtqqtbtnaw.html

[S31] C++：Hello World
来源：http://hz.jianghu66.top/gtumbbyxbb.html

#include <iostream>
来源：http://hz.tianlin.xyz/gtcaqwjvmj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtbuyypesu.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtuihesbqo.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtozvczbhx.html

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gthahifekk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.vqdsnc.cn/gttcpbbebb.html

[S34] C++：遍历 vector
来源：http://hz.sxryk.cn/gtixjaeypg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtabmcbeyz.html

[S35] C++：map
来源：http://hz.bjfxy.top/gtfrwestlj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtcyannotv.html

[S36] C++：unordered_map
来源：http://hz.sweek.top/gtvbijjunx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gthavqeags.html

[S37] C++：set
来源：http://hz.havefunace.top/gtdmlrzdzs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.smart0.xyz/gtdvfwvevd.html

[S38] C++：排序
来源：http://hz.yueranfly.top/gtgomiaejz.html

std::sort(v.begin(), v.end());
来源：http://hz.xziqi.cn/gttflepqxb.html

[S39] C++：自定义比较器排序
来源：http://hz.9152youxi.cn/gtlmbnrqbu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtwlimucep.html

[S40] C++：查找元素
来源：http://hz.bjfxy.top/gtbkvkjoin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yongpay.top/gtjjxdvenp.html

[S41] C++：类与构造函数
来源：http://hz.52xcode.cn/gtpkbupjef.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cashguo.top/gtydivktpz.html

[S42] C++：继承与虚函数
来源：http://hz.hfpthk.cn/gtfzyvvxaf.html

class B : public Base { public: void f() override {} };
来源：http://hz.cucudq.cn/gttphvxfpy.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gtfctjwiii.html

auto p = std::make_unique<int>(5);
来源：http://hz.dashuyun.cn/gtcofcorve.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtumqbadpx.html

void inc(int &x) { ++x; }
来源：http://hz.ivvv.top/gtbwyizndv.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtgvgspepj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gtvkwscqhl.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtrrmqcuoa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtpwcdqtql.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gttktlrlmm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fzhhl.top/gtqaqkxwkn.html

[S48] C++：逐行读文件
来源：http://hz.zycfv.cn/gtioibknqp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258.top/gthamzirtv.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtohcjfbke.html

[S49] C++：写文件
来源：http://hz.52xcode.cn/gtfiruapfp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtskiyzbmz.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtiffglcme.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.mhx1999.top/gtjaeiznnn.html

[S51] C++：显式类型转换
来源：http://hz.xziqi.cn/gtjjvbmxpk.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtqnzsohrp.html

[S52] C++：const 与 noexcept
来源：http://hz.feifeiyinyue.top/gtzkmrbozo.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtyjdoquit.html

[S53] C++：移动语义
来源：http://hz.sweek.top/gtqkcfofvk.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtpcbpznhu.html

[S54] C++：异常处理
来源：http://hz.sxryk.cn/gtjltwbpjx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtcnquuxes.html

[S55] C++：结构化绑定
来源：http://hz.xingfuxueyuan.xyz/gtxywutziq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangdashe.top/gtuobipufw.html

[S56] C++：optional
来源：http://hz.ivvv.top/gtpvcoasnw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yangfankeji.com/gtfqfiajpz.html

[S57] C++：编译期常量
来源：http://hz.jyoumei.cn/gtbjgeemfl.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtxtfjdfjr.html

[S58] C++：命名空间
来源：http://hz.nanxuanxn.top/gtvhcwtztz.html

namespace ns { int f() { return 1; } }
来源：http://hz.gotoacloud.top/gtlivrzdce.html

[S59] C++：静态断言
来源：http://hz.jianghu66.top/gtfftytiti.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gtirzrmyba.html

[S60] C++：遍历并删除元素
来源：http://hz.wangshuangyany.cn/gtfjozuooh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.9152youxi.cn/gtoxnpikeg.html

================================================================================
来源：http://hz.c1oappe.top/gtkdycakjt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yonumen.top/gtoznfrzzu.html

================================================================================
来源：http://hz.0kj1m.cn/gtwnffioao.html

[T01] Kotlin：Hello World
来源：http://hz.iojbl.cn/gtjmynmifo.html

println("Hello")
来源：http://hz.c1oappe.top/gtmplvyffl.html

[T02] Kotlin：变量
来源：http://hz.xziqi.cn/gtdngbjewj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhiwuduotai.top/gtwwobthje.html

[T03] Kotlin：字符串模板
来源：http://hz.fzhhl.top/gtogqkjqon.html

"值: $b"
来源：http://hz.cdnleiting.top/gtnynhxqba.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gttzotxvna.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtxhyebexy.html

[T05] Kotlin：when 表达式
来源：http://hz.ybcxt.top/gtweekactn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtugmmhjni.html

[T06] Kotlin：集合映射
来源：http://hz.xinyue.icu/gtixguobwp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtmkkhctax.html

[T07] Kotlin：集合过滤
来源：http://hz.birdmap.top/gttbyzpppw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtxtiqpbdt.html

[T08] Kotlin：数据类
来源：http://hz.tian-w.cn/gtzdtbnfqt.html

data class User(val name: String, val age: Int)
来源：http://hz.guannengcc.top/gtlhnwdjwx.html

[T09] Kotlin：扩展函数
来源：http://hz.sxryk.cn/gtipgaltxx.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gtmjpxwram.html

[T10] Kotlin：默认参数
来源：http://hz.smart0.xyz/gtudbowwhp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuxming.cn/gttgzqxfsl.html

[T11] Kotlin：协程
来源：http://hz.gogol.net.cn/gtylxnlpkt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sysykeji.top/gtkjktkoqh.html

[T12] Kotlin：解构声明
来源：http://hz.jlsjyb.cn/gtzrxnidwc.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhijiandao.cn/gtoindjswn.html

[T13] Kotlin：只读 Map
来源：http://hz.9152youxi.cn/gtnswfntuc.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gttqlkaqdn.html

[T14] Kotlin：循环
来源：http://hz.zhixingplan.top/gtguklfryq.html

for (i in 1..10) println(i)
来源：http://hz.ydjk.org.cn/gtzvphaeyh.html

[T15] Kotlin：接口
来源：http://hz.xylfe.cn/gtglcedbwv.html

interface Shape { fun area(): Double }
来源：http://hz.hammf.cn/gtlfiarlze.html

[T16] Swift：Hello World
来源：http://hz.guowangkeji.top/gtgufoaitn.html

print("Hello")
来源：http://hz.smart0.xyz/gtslkfmjec.html

[T17] Swift：变量与常量
来源：http://hz.birdmap.top/gtkcpqrimg.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtrlutdzkm.html

[T18] Swift：字符串插值
来源：http://hz.9152youxi.cn/gttihyqtsa.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gttjsnezkt.html

[T19] Swift：可选绑定
来源：http://hz.hywenlv.cn/gtkpnvcbaf.html

if let n = opt { print(n) }
来源：http://hz.c1oappe.top/gtvhjltgfv.html

[T20] Swift：数组操作
来源：http://hz.ehwqpu.com/gtfxnpbxbi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtlsqwfyvv.html

[T21] Swift：遍历
来源：http://hz.zdqjudy.top/gtouwxnhrh.html

for x in a { print(x) }
来源：http://hz.zhixingplan.top/gtjzduzhbt.html

[T22] Swift：字典
来源：http://hz.316326.xyz/gtstvvsayg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinghuilouyu.cn/gtgyzowgzr.html

[T23] Swift：函数
来源：http://hz.9152youxi.cn/gtuylcqcxr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gtfkvczglb.html

[T24] Swift：闭包
来源：http://hz.yuxming.cn/gtjbaodfqt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtruxuzqdq.html

[T25] Swift：结构体
来源：http://hz.yonumen.top/gtrgmzeqyj.html

struct P { var x: Int }
来源：http://hz.zhixingplan.top/gtmmjbqbvb.html

[T26] Swift：类与重写
来源：http://hz.quarkkingdee.top/gtpuqbydxj.html

class A: Base { override func f() {} }
来源：http://hz.yangfankeji.com/gtfbkplqof.html

[T27] Swift：错误处理
来源：http://hz.xziqi.cn/gtkrrjoksl.html

do { try f() } catch { print(error) }
来源：http://hz.zhengqikj.top/gtwiyjaliu.html

[T28] Swift：枚举
来源：http://hz.redwolf501.top/gtvfzabdpb.html

enum Color { case red, green }
来源：http://hz.cqqwz.cn/gtksuqwavb.html

[T29] Swift：guard 提前返回
来源：http://hz.yj202588.top/gtipdrriye.html

guard let x = opt else { return }
来源：http://hz.gogol.net.cn/gtzgleclru.html

[T30] Swift：协议
来源：http://hz.aibaodan.cn/gtxnuyhtee.html

protocol Shape { func area() -> Double }
来源：http://hz.meibo888.top/gtmqceitqq.html

[T31] Lua：Hello World
来源：http://hz.havefunace.top/gtjpjtxssg.html

print("Hello")
来源：http://hz.9152youxi.cn/gtonnfyuhg.html

[T32] Lua：局部变量
来源：http://hz.52xcode.cn/gtqkfuxsze.html

local a = 1
来源：http://hz.jinghuilouyu.cn/gtpmcbhrkp.html

[T33] Lua：表（数组）
来源：http://hz.pycfn.com/gtidbbmall.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.c1oappe.top/gtjaoeurvp.html

[T34] Lua：遍历表
来源：http://hz.pycfn.com/gtsihtwjey.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yvedp.cn/gtopzyaufh.html

[T35] Lua：字典表
来源：http://hz.zhixingplan.top/gtllqixstb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtnoyelyfd.html

[T36] Lua：函数
来源：http://hz.mhx1999.top/gtwgwocatj.html

function add(a, b) return a + b end
来源：http://hz.gogol.net.cn/gtvxcqqzob.html

[T37] Lua：字符串拼接
来源：http://hz.yonumen.top/gtqdutdbtn.html

"a" .. "b"
来源：http://hz.jianghu66.top/gtcyfhartn.html

[T38] Lua：条件
来源：http://hz.jlsjyb.cn/gtfumqrtjh.html

if x > 0 then print("正") end
来源：http://hz.jianghu66.top/gtrwpzmdns.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtwnrnoran.html

string.find(s, "%d+")
来源：http://hz.yangfankeji.com/gtdbtpiazt.html

[T40] Lua：元表
来源：http://hz.aibaodan.cn/gtuhmhayii.html

setmetatable({}, { __index = base })
来源：http://hz.wangshuangyany.cn/gtneltglkq.html

[T41] Perl：Hello World
来源：http://hz.haohaochexian.top/gtoljyvdkg.html

print "Hello\n";
来源：http://hz.jlsjyb.cn/gtdoepplpw.html

[T42] Perl：变量类型
来源：http://hz.sufxvd.cn/gtrstnbulo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gtvikzujbu.html

[T43] Perl：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtzcxfghqx.html

"值: $a"
来源：http://hz.sysykeji.top/gteqmpextv.html

[T44] Perl：条件
来源：http://hz.aizwys.cn/gtpmxhhkvj.html

if ($a > 0) { print "正"; }
来源：http://hz.yongpay.top/gtgtbzusco.html

[T45] Perl：数组遍历
来源：http://hz.zhongyouzk.top/gtwpcgbzrg.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258.top/gtqzbcryeu.html

[T46] Perl：哈希操作
来源：http://hz.hongshengwenyu.top/gtakdwwuol.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cucudq.cn/gtonminqhj.html

[T47] Perl：正则捕获
来源：http://hz.yuanzhike.top/gtzyagzyuv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhaomingkeji.xyz/gtjhuirqol.html

[T48] Perl：正则替换
来源：http://hz.andypj.xyz/gtggwrpyme.html

$s =~ s/old/new/g;
来源：http://hz.havefunace.top/gtbhqhlbja.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtxprjaclz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yuxming.cn/gtgoxjeotk.html

[T50] Perl：逐行读文件
来源：http://hz.c1oappe.top/gtanqscuhu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jianghu66.top/gtoujylfgh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ybcxt.top/gtrfjozpos.html

[T51] Scala：Hello World
来源：http://hz.zhengqikj.top/gtofeczfga.html

println("Hello")
来源：http://hz.cucudq.cn/gtzhksukmt.html

[T52] Scala：变量
来源：http://hz.zhoulong.xyz/gtwarxeosu.html

val a = 1;  var b = 2
来源：http://hz.redwolf501.top/gttlyzqidd.html

[T53] Scala：字符串插值
来源：http://hz.zdqjudy.top/gtrnyihpvb.html

s"值: $b"
来源：http://hz.jlsjyb.cn/gtewmkpjtg.html

[T54] Scala：集合映射
来源：http://hz.jinqigufen.top/gtlkciwczs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shzxlz.cn/gtxvocgctt.html

[T55] Scala：集合过滤
来源：http://hz.pengpengdd.cyou/gthpdloisi.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zycfv.cn/gtzcvdlihk.html

[T56] Scala：样例类
来源：http://hz.fzhhl.top/gtcikuccjd.html

case class User(name: String, age: Int)
来源：http://hz.shuidangran.top/gtxdwzztnf.html

[T57] Scala：模式匹配
来源：http://hz.zhiwuduotai.top/gtqakpaqej.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hywenlv.cn/gtktzeftix.html

[T58] Scala：函数定义
来源：http://hz.yangfankeji.com/gteczjjvbp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.smart0.xyz/gtfolnhibt.html

[T59] Scala：循环
来源：http://hz.316326.xyz/gtnohwhbjt.html

for (i <- 1 to 10) println(i)
来源：http://hz.sufxvd.cn/gtfybivgip.html

[T60] Scala：折叠
来源：http://hz.chenlongwang.top/gtszfvcgcw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nanxinkj.top/gtocoipdbk.html

================================================================================
来源：http://hz.zdqjudy.top/gtjdibfjtn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gtzfmsgrzd.html

================================================================================
来源：http://hz.fzhhl.top/gttkllbufv.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtikjzwazu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guowangkeji.top/gtzxkwwgzo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gteqbpnqtr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhiwuduotai.top/gtbeabeevs.html

[U03] Py：加载 .env 配置
来源：http://hz.gotoacloud.top/gtsechdzyd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhoulong.xyz/gtdorvszdh.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangkeji.top/gtfuandebk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shangyingyoupin.top/gtyxmdpgdj.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gtpsoxzveh.html

list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtllhhpleb.html

[U06] Py：合并两个字典
来源：http://hz.hywenlv.cn/gtlnzuuvpm.html

{**a, **b}
来源：http://hz.wangdashe.top/gtcoxnjkjg.html


<!-- 参考信息 -->