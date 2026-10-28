代发 wailian999

df -h;  du -sh *
来源：http://hz.jqgufenzy.top/gtohtftjxw.html

[R62] 找最占空间的文件
来源：http://hz.hnqzz.top/gtlgtjmztq.html

du -ah . | sort -rh | head -10
来源：http://hz.sysykeji.top/gtkdfckrje.html

[R63] 内存与进程
来源：http://hz.shanyushiyangtech.top/gtlhmeoqeo.html

free -h;  ps aux | grep nginx
来源：http://hz.shuidangran.top/gtdohtrhjl.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtpstvyowo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtngwlztmh.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtjnxtfnen.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yanxiufei.cn/gtuwzbfjwv.html

[R66] 定时任务
来源：http://hz.aibaodan.cn/gtyikrjkoy.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gtjlncnvef.html

[R67] 生成随机十六进制串
来源：http://hz.hfpthk.cn/gtrnnfckdm.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gtmrewgtei.html

[R68] 计算文件校验值
来源：http://hz.sxryk.cn/gtgavgozoh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gtfxsfuqpc.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gtfurwlrhh.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtwzkmwxrh.html

[R70] 时间戳与互转
来源：http://hz.yanxiufei.cn/gtytbpgdyp.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gtycaxoudw.html

[R71] 日期格式化
来源：http://hz.wangdashe.top/gtnrrurvth.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sxryk.cn/gtugjlulav.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtylqgteit.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zdqjudy.top/gtcahlyrqs.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtbtazfchq.html

split -l 1000 big.log part_
来源：http://hz.jqgfzy.top/gttdsytunt.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtugbbjdhc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtvweygeti.html

[R75] 导出环境变量
来源：http://hz.zycfv.cn/gtpqwvrlge.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xinyue.icu/gtwxwbfaul.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtkmndrgoi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtnumirxzf.html

[R77] 读取用户输入
来源：http://hz.wangshuangyany.cn/gtmvmtmrqd.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gteltpszwe.html

[R78] 交互式菜单
来源：http://hz.jqgufenzy.top/gtwpklzhsn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtrjjhldtn.html

[R79] 解析命令行选项
来源：http://hz.ybcxt.top/gtzzvuwrzg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gttipqrzps.html

[R80] 查看脚本执行耗时
来源：http://hz.zhixingplan.top/gtzujmsujg.html

time ./run.sh
来源：http://hz.yvedp.cn/gthnkjjzvm.html

================================================================================
来源：http://hz.havefunace.top/gtdloxrcve.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtmxmsmmzo.html

================================================================================
来源：http://hz.nanxinkj.top/gtporxocuu.html

[S01] C：Hello World
来源：http://hz.xuetiantiany.cn/gtdmjzxjib.html

#include <stdio.h>
来源：http://hz.zdqjudy.top/gtlptmilgz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtuiyxmemc.html

[S02] C：变量与格式化输出
来源：http://hz.yuxming.cn/gtbcpeqesh.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtgcotrzkz.html

[S03] C：读入整数
来源：http://hz.hfpthk.cn/gtvzmamyzq.html

int x; scanf("%d", &x);
来源：http://hz.cashguo.top/gtxnuhtplm.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangkeji.top/gtawhneqgx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gaohongyu789.top/gtvnorjbpb.html

[S05] C：字符串长度
来源：http://hz.xuanzx.com/gtysggvdzi.html

strlen(s)
来源：http://hz.ydjk.org.cn/gtgfomtilg.html

[S06] C：字符串比较
来源：http://hz.kuanghao11.cn/gtseoufzsy.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtslhwctpa.html

[S07] C：数组遍历求和
来源：http://hz.zhaomingkeji.xyz/gtjoqpkaes.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtjvosryte.html

[S08] C：动态内存分配与释放
来源：http://hz.cheryme.top/gtdxrgnqrg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtcldlmhti.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtsenmfpvp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhiwuduotai.top/gtktakfklr.html

[S10] C：指针与解引用
来源：http://hz.sxryk.cn/gtmjxbqdgk.html

int *p = &a;  *p = 5;
来源：http://hz.kuanghao11.cn/gthrpcifkb.html

[S11] C：逐行读文件
来源：http://hz.yongpay.top/gtyjrhsswa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shzxlz.cn/gtgablyrta.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sweek.top/gtrkrfzlqg.html

fclose(f);
来源：http://hz.tian-w.cn/gthpcztchs.html

[S12] C：写文件
来源：http://hz.meibo888.top/gtbdeoywos.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fzhhl.top/gtjxjphacn.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtmlqnbgpp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.birdmap.top/gtlnawvlxk.html

[S14] C：枚举
来源：http://hz.shanyushiyangkeji.top/gtevkegkah.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtqiepbzom.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtlvvibyhs.html

(double) a / b
来源：http://hz.aizwys.cn/gtuwpivswu.html

[S16] C：位操作置位
来源：http://hz.zycfv.cn/gtsnanrppu.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtmfqtpfid.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtizoiukms.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aibaodan.cn/gtjgjkjtph.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gtrbcxlbam.html

int main(int argc, char **argv)
来源：http://hz.kuanghao11.cn/gtrdmsyela.html

[S19] C：快速排序
来源：http://hz.jqgufenzy.top/gtefwucnlk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtlizhgvcx.html

[S20] C：二分查找
来源：http://hz.redwolf501.top/gtdwsjnlkh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xylfe.cn/gtrodfotfd.html

[S21] C：字符类别判断
来源：http://hz.sxryk.cn/gtjrhnyhri.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtfvvojbhp.html

[S22] C：字符串转数字
来源：http://hz.ydzc1.top/gtprztsizy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tianlin.xyz/gthnpsdtzm.html

[S23] C：随机数
来源：http://hz.shuidangran.top/gtowbmqmor.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hysaishi.cn/gtaayunhnx.html

[S24] C：获取本地时间
来源：http://hz.zhaomingkeji.xyz/gtooiinxfa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtuabetrnx.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtqtcgsobr.html

memcpy(dst, src, n);
来源：http://hz.yj20258888.top/gtnxlkmkdw.html

[S26] C：内存清零
来源：http://hz.xylfe.cn/gtzwrusvbo.html

memset(a, 0, sizeof a);
来源：http://hz.guannengcc.top/gtowkhaszt.html

[S27] C：定义常量
来源：http://hz.yangfankeji.com/gteazpxngm.html

const double PI = 3.14159;
来源：http://hz.0kj1m.cn/gtottfkdsk.html

[S28] C：静态变量
来源：http://hz.aizwys.cn/gtqcrwalul.html

static int counter = 0;
来源：http://hz.nwbrower.top/gtlghwhksw.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtbrhxxtuo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtyjflscsc.html

[S30] C：头文件保护
来源：http://hz.dianchejie.cn/gtgifphmsy.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtqopafvie.html

#define X_H
来源：http://hz.birdmap.top/gtjrwdqckz.html

#endif
来源：http://hz.nanxinkj.top/gtbtfxkyhs.html

[S31] C++：Hello World
来源：http://hz.jqgufenzy.top/gtkmjpryyy.html

#include <iostream>
来源：http://hz.fzhhl.top/gtjyfkghrg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gzhubu.top/gtnttysygf.html

[S32] C++：字符串
来源：http://hz.jiagoushi.top/gtqytxlnil.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgfzy.top/gtsjuytibl.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtyzmahqkh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtguacepgc.html

[S34] C++：遍历 vector
来源：http://hz.ybcxt.top/gtirvobffp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dianchejie.cn/gtzmcgztfb.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtihnicpdt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtqgkvlrxg.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gtejhfennl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtrqgtxnsv.html

[S37] C++：set
来源：http://hz.redwolf501.top/gtfyvwgkow.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gteiyjjfjn.html

[S38] C++：排序
来源：http://hz.fzhhl.top/gtxgqqzseq.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtzcqrpfac.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtixcjchdd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cheryme.top/gtcgqjwacw.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtlxnsunyq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.mhx1999.top/gtamdtenvd.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtubtmnooa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtzdojpnyn.html

[S42] C++：继承与虚函数
来源：http://hz.jlsjyb.cn/gtyotlosml.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtcefgabeq.html

[S43] C++：智能指针
来源：http://hz.jinghuilouyu.cn/gtweukobgw.html

auto p = std::make_unique<int>(5);
来源：http://hz.hongshengwenyu.top/gtltipttnh.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtzkbyybvg.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtpwtylscu.html

[S45] C++：lambda
来源：http://hz.zhijiandao.cn/gtceviebia.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtvjkrixto.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gtbweaogqm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtivcaeudi.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhengqikj.top/gtggtwylyx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtuozoajkt.html

[S48] C++：逐行读文件
来源：http://hz.nwbrower.top/gtwkcvwjob.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hammf.cn/gtqixnajsv.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtprcugemz.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtjljnhuaw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guowangkeji.top/gtmgwhtuam.html

[S50] C++：格式化数字
来源：http://hz.vqdsnc.cn/gtbdysrlvn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.feifeiyinyue.top/gtlzfkemmh.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtqeacsovn.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtcagbopga.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtwrskspke.html

int size() const noexcept { return n_; }
来源：http://hz.chenlongwang.top/gtaejwdmmo.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtzhovardn.html

std::vector<int> w = std::move(v);
来源：http://hz.jyoumei.cn/gtjunuvcam.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gthoisntpu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhixingplan.top/gtsjjkvbqt.html

[S55] C++：结构化绑定
来源：http://hz.bjfxy.top/gtuucpiorc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.mhx1999.top/gthzjuirox.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtiddmosjy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fengsongda.top/gtkhwczngs.html

[S57] C++：编译期常量
来源：http://hz.wangdashe.top/gtxogpsici.html

constexpr int N = 10;
来源：http://hz.xuanzx.com/gtlnlwclsj.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtoipvrcna.html

namespace ns { int f() { return 1; } }
来源：http://hz.xingfuxueyuan.xyz/gtrmvhtlux.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtjjxoqwpt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aibaodan.cn/gtddwqznsl.html

[S60] C++：遍历并删除元素
来源：http://hz.52xcode.cn/gtpywfhiej.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ivvv.top/gtqpgtpuig.html

================================================================================
来源：http://hz.mhx1999.top/gtiihtjchy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtyzpzscrn.html

================================================================================
来源：http://hz.hysaishi.cn/gthusvtoxo.html

[T01] Kotlin：Hello World
来源：http://hz.cucudq.cn/gtvydujcuw.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtogriipmc.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtlpuwpfaj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtfgzqnfjs.html

[T03] Kotlin：字符串模板
来源：http://hz.ybcxt.top/gtcbkmzoey.html

"值: $b"
来源：http://hz.zhixingplan.top/gtycczhwkr.html

[T04] Kotlin：空安全
来源：http://hz.nwbrower.top/gtygtroamu.html

val n: String? = null;  n?.length
来源：http://hz.tianlin.xyz/gtvwbkylex.html

[T05] Kotlin：when 表达式
来源：http://hz.fzhhl.top/gtcjvpxxtm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fzhhl.top/gtjkkjconr.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtlxjqpegv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtkyfftfjb.html

[T07] Kotlin：集合过滤
来源：http://hz.shzxlz.cn/gtombnoraf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtdolwyxrq.html

[T08] Kotlin：数据类
来源：http://hz.hammf.cn/gtqttssoft.html

data class User(val name: String, val age: Int)
来源：http://hz.sweek.top/gtrwkaaxfz.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtgsnppncc.html

fun String.exclaim() = this + "!"
来源：http://hz.sxryk.cn/gtzthdjbzm.html

[T10] Kotlin：默认参数
来源：http://hz.316326.xyz/gtzdbdzjcm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhixingplan.top/gtykwwfvie.html

[T11] Kotlin：协程
来源：http://hz.ywan-chungtsiang.top/gtauezqtzb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jyoumei.cn/gtfpeeviyo.html

[T12] Kotlin：解构声明
来源：http://hz.dianchejie.cn/gtgbjtighl.html

val (a, b) = Pair(1, 2)
来源：http://hz.pengpengdd.cyou/gtgqgrmnac.html

[T13] Kotlin：只读 Map
来源：http://hz.hnqzz.top/gtfxnhoqve.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigufen.top/gtkevamxno.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtlejtafqg.html

for (i in 1..10) println(i)
来源：http://hz.havefunace.top/gtlgybeqau.html

[T15] Kotlin：接口
来源：http://hz.hammf.cn/gtpkkvksba.html

interface Shape { fun area(): Double }
来源：http://hz.bjfxy.top/gtuewlldlg.html

[T16] Swift：Hello World
来源：http://hz.aibaodan.cn/gtpqzbdast.html

print("Hello")
来源：http://hz.bjfxy.top/gtzadfqwpd.html

[T17] Swift：变量与常量
来源：http://hz.snrcjt.cn/gtxyrwbevj.html

var a = 1;  let b = 2
来源：http://hz.ehwqpu.com/gtdkzfxrfv.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtfqulboay.html

"值: \(b)"
来源：http://hz.cheryme.top/gtqhtkrdvd.html

[T19] Swift：可选绑定
来源：http://hz.yuxming.cn/gtgxqwcqud.html

if let n = opt { print(n) }
来源：http://hz.ppjwa.cn/gtqnmqmrsw.html

[T20] Swift：数组操作
来源：http://hz.xuetiantiany.cn/gtjhqmembj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yanxiufei.cn/gtybwscquj.html

[T21] Swift：遍历
来源：http://hz.yj20258.top/gtialrifua.html

for x in a { print(x) }
来源：http://hz.fzhhl.top/gtrvcwcvyj.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtgruapzlo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangtech.top/gtbsxufqlt.html

[T23] Swift：函数
来源：http://hz.tian-w.cn/gtiiojzrvs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ehwqpu.com/gtafljpxxo.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gtwptbqtsg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.pycfn.com/gtvmsyxmqy.html

[T25] Swift：结构体
来源：http://hz.jianghu66.top/gtevymyedr.html

struct P { var x: Int }
来源：http://hz.smart0.xyz/gtxbuchelz.html

[T26] Swift：类与重写
来源：http://hz.xuetiantiany.cn/gtgpuzplrf.html

class A: Base { override func f() {} }
来源：http://hz.yj20258.top/gtxglkzzzv.html

[T27] Swift：错误处理
来源：http://hz.316326.xyz/gttxcmhlfy.html

do { try f() } catch { print(error) }
来源：http://hz.ywan-chungtsiang.top/gtptfmwobx.html

[T28] Swift：枚举
来源：http://hz.gogol.net.cn/gthutefxyh.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtmzctxuoe.html

[T29] Swift：guard 提前返回
来源：http://hz.hnxiangtu.top/gthwpknwie.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangtech.top/gtdoxjdznd.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtuqbayswy.html

protocol Shape { func area() -> Double }
来源：http://hz.sufxvd.cn/gtdimdfulo.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtbcqdzdhl.html

print("Hello")
来源：http://hz.xuanzx.com/gtcbykwmay.html

[T32] Lua：局部变量
来源：http://hz.tanke756.top/gtpsihahmk.html

local a = 1
来源：http://hz.cucudq.cn/gtxntpmjqc.html

[T33] Lua：表（数组）
来源：http://hz.jinghuilouyu.cn/gtjlvsmjoo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.smart0.xyz/gtjmlhsllv.html

[T34] Lua：遍历表
来源：http://hz.jyoumei.cn/gtrjvasvvo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nwbrower.top/gtqoctgagn.html

[T35] Lua：字典表
来源：http://hz.fengsongda.top/gtkqcqriep.html

local d = { a = 1 };  d.b = 2
来源：http://hz.kuanghao11.cn/gthjryrwsy.html

[T36] Lua：函数
来源：http://hz.ppjwa.cn/gtsnljqlen.html

function add(a, b) return a + b end
来源：http://hz.tian-w.cn/gtzgumqtrm.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtxdyfztpj.html

"a" .. "b"
来源：http://hz.jyoumei.cn/gtkmfmeewi.html

[T38] Lua：条件
来源：http://hz.hnqzz.top/gtikvxvrka.html

if x > 0 then print("正") end
来源：http://hz.yueranfly.top/gtvyelsjxx.html

[T39] Lua：模式匹配
来源：http://hz.jinyuanbaomall.cn/gtatzjuhov.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gteutfmdke.html

[T40] Lua：元表
来源：http://hz.ybcxt.top/gtptbqnnvj.html

setmetatable({}, { __index = base })
来源：http://hz.vqdsnc.cn/gtgglqgwhm.html

[T41] Perl：Hello World
来源：http://hz.cucudq.cn/gtdowjrusy.html

print "Hello\n";
来源：http://hz.gogol.net.cn/gttebgxdnm.html

[T42] Perl：变量类型
来源：http://hz.jqgfzy.top/gtzxlojegc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuanzx.com/gtojxvqwps.html

[T43] Perl：字符串插值
来源：http://hz.xuanzx.com/gttpsjbyek.html

"值: $a"
来源：http://hz.zhixingplan.top/gthozxffrw.html

[T44] Perl：条件
来源：http://hz.shanyushiyangkeji.top/gtqofoesgj.html

if ($a > 0) { print "正"; }
来源：http://hz.wangshuangyany.cn/gtwxesgiqz.html

[T45] Perl：数组遍历
来源：http://hz.wangshuangyany.cn/gtsqqmzwwo.html

for my $x (@arr) { print $x; }
来源：http://hz.yonumen.top/gtfkmwhqel.html

[T46] Perl：哈希操作
来源：http://hz.xinyue.icu/gtrzecumix.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xziqi.cn/gtifrlqydb.html

[T47] Perl：正则捕获
来源：http://hz.sufxvd.cn/gtrkrejybu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxinkj.top/gthhspzaha.html

[T48] Perl：正则替换
来源：http://hz.yangfankeji.com/gtqpfkqxfu.html

$s =~ s/old/new/g;
来源：http://hz.sufxvd.cn/gtehdopzit.html

[T49] Perl：函数
来源：http://hz.xinyue.icu/gtemkpryay.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigfzy.top/gtxqeewbdn.html

[T50] Perl：逐行读文件
来源：http://hz.xuanzx.com/gtfvnohbvy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yangfankeji.com/gtzaofmcil.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtoinjrtsw.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtdregxvoh.html

println("Hello")
来源：http://hz.aibaodan.cn/gtqfjfmbii.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gtckpobtdb.html

val a = 1;  var b = 2
来源：http://hz.yvedp.cn/gtgsakpvnw.html

[T53] Scala：字符串插值
来源：http://hz.yueranfly.top/gtsznawenb.html

s"值: $b"
来源：http://hz.zhengqikj.top/gtwssmwoxr.html

[T54] Scala：集合映射
来源：http://hz.dianchejie.cn/gtuvmgrkil.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydzc1.top/gtrajuzbgx.html

[T55] Scala：集合过滤
来源：http://hz.sxryk.cn/gtpxvnjfge.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sufxvd.cn/gtwvkbrjxw.html

[T56] Scala：样例类
来源：http://hz.zdqjudy.top/gtzrzgvqvq.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gtgcdczrrd.html

[T57] Scala：模式匹配
来源：http://hz.daxiang520.top/gtaodnqqwl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gtkomerhgs.html

[T58] Scala：函数定义
来源：http://hz.gotoacloud.top/gtmbrbgvch.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yonumen.top/gtzhfpqsrc.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gtzzsylgwc.html

for (i <- 1 to 10) println(i)
来源：http://hz.gotoacloud.top/gtgjgrdghs.html

[T60] Scala：折叠
来源：http://hz.tian-w.cn/gttbymukxg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sxryk.cn/gtmxpwpkcj.html

================================================================================
来源：http://hz.guowangkeji.top/gtozoxhjib.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gtgecbuyzs.html

================================================================================
来源：http://hz.redwolf501.top/gtplridnix.html

[U01] Py：创建虚拟环境
来源：http://hz.hnqzz.top/gttxweunxo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gtywrmusjw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhengqikj.top/gtbwazpcop.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jqgfzy.top/gtgimqtrgc.html


<!-- 参考信息 -->