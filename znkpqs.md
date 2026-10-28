代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtsrndfwzp.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhixingplan.top/gtwnbajqbc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuetiantiany.cn/gtwacemskk.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gtksxdihxa.html

df -h;  du -sh *
来源：http://hz.nanxuanxn.top/gtoljirdud.html

[R62] 找最占空间的文件
来源：http://hz.shangyingyoupin.top/gtoiweozhg.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtwhysyrpx.html

[R63] 内存与进程
来源：http://hz.jlsjyb.cn/gtucowyffj.html

free -h;  ps aux | grep nginx
来源：http://hz.fzhhl.top/gtwfykqazw.html

[R64] 结束进程
来源：http://hz.bjfxy.top/gttaxrsjav.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtocnnvhwc.html

[R65] 查看端口占用
来源：http://hz.hongshengwenyu.top/gtuvfzgiuq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangtech.top/gtwobfhhpx.html

[R66] 定时任务
来源：http://hz.zhijiandao.cn/gthmrswout.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtqaknoslv.html

[R67] 生成随机十六进制串
来源：http://hz.ywan-chungtsiang.top/gtdhopeenq.html

openssl rand -hex 16
来源：http://hz.tianlin.xyz/gtixebiikk.html

[R68] 计算文件校验值
来源：http://hz.yanxiufei.cn/gtwzyhevce.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.iojbl.cn/gtubrkiukg.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gtoszyamou.html

head -c 16 /dev/urandom | base64
来源：http://hz.cheryme.top/gtopbzqcxs.html

[R70] 时间戳与互转
来源：http://hz.daxiang520.top/gthptlfywz.html

date +%s;  date -d @1700000000
来源：http://hz.mhx1999.top/gtviaxobxs.html

[R71] 日期格式化
来源：http://hz.bjfxy.top/gtwpvjelgr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gtmrgxzhvh.html

[R72] 等待端口就绪
来源：http://hz.fengsongda.top/gtqerykhhg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgfzy.top/gtdarxjtjf.html

[R73] 分割大日志
来源：http://hz.yuxming.cn/gtcscplsef.html

split -l 1000 big.log part_
来源：http://hz.zycfv.cn/gtglagjyry.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gthtwtwwgp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shangyingyoupin.top/gtqvcehiuu.html

[R75] 导出环境变量
来源：http://hz.cucudq.cn/gtngoxnvsd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gthsfwfclu.html

[R76] 使用临时文件
来源：http://hz.andypj.xyz/gtipxjfpus.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtpoxqzcmg.html

[R77] 读取用户输入
来源：http://hz.ydjk.org.cn/gtynbaflcx.html

read -rp "请输入: " ans
来源：http://hz.jiagoushi.top/gtkhxyifry.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtusercyrj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuanzx.com/gtnaibzprn.html

[R79] 解析命令行选项
来源：http://hz.yanxiufei.cn/gtbladuyja.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.c1oappe.top/gtcvdkhdtn.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgfzy.top/gtcslnswdz.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtdphyqmwt.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgapcipfz.html

S. C / C++ 专题
来源：http://hz.jinqigfzy.top/gttkmxvodg.html

================================================================================
来源：http://hz.yangfankeji.com/gtefefjgjm.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtnzufypcb.html

#include <stdio.h>
来源：http://hz.chenlongwang.top/gtbyxnyifk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.haohaochexian.top/gtaxuuagth.html

[S02] C：变量与格式化输出
来源：http://hz.ydjk.org.cn/gtiydnjmxn.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gtudiuarsb.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtwmdzemxb.html

int x; scanf("%d", &x);
来源：http://hz.hammf.cn/gtumfborsw.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gtbdnltkpd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.c1oappe.top/gtgfanoern.html

[S05] C：字符串长度
来源：http://hz.ywan-chungtsiang.top/gtpldtynnh.html

strlen(s)
来源：http://hz.nanxinkj.top/gtunmjpgrn.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gtrzsphffx.html

strcmp(a, b) == 0
来源：http://hz.316326.xyz/gtjohxznok.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtjywtbule.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yanxiufei.cn/gtbmsvfqhx.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigfzy.top/gtjgolhnek.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.meibo888.top/gtozpbffxq.html

[S09] C：结构体定义与初始化
来源：http://hz.9152youxi.cn/gtibxhbyfy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xinyue.icu/gtxywyjndw.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gtoeqvmruu.html

int *p = &a;  *p = 5;
来源：http://hz.zdqjudy.top/gtrufizdgo.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtufdlkdna.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gttvmypkkm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangdashe.top/gtenobprbw.html

fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtikugiduf.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtqhgcerqb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xylfe.cn/gtugqsjbet.html

[S13] C：宏定义
来源：http://hz.jlsjyb.cn/gtqzinmtza.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daria6918.cn/gtxoqqpncg.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtpxpmrufx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtzygieokn.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtjtpobidd.html

(double) a / b
来源：http://hz.yj20258.top/gtxvkfebzc.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtfzjtfski.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gtvdiaeccn.html

[S17] C：安全拼接字符串
来源：http://hz.hammf.cn/gtimadoqde.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtqtkylfmu.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtpmpytslc.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtiryqazgd.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gtbizhytiw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guannengcc.top/gteuptdsnt.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtngvgolva.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtvjnllzzn.html

[S21] C：字符类别判断
来源：http://hz.yangfankeji.com/gtrzbpzyzk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigufen.top/gtlbothqtn.html

[S22] C：字符串转数字
来源：http://hz.yongpay.top/gtqetgtbfg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenlongwang.top/gtykvqmyan.html

[S23] C：随机数
来源：http://hz.yj20258888.top/gtnioqhyzh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtjjzovrua.html

[S24] C：获取本地时间
来源：http://hz.yj20258.top/gtafxdtpgt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtxwfuwjut.html

[S25] C：内存拷贝
来源：http://hz.yvedp.cn/gtaufsgoda.html

memcpy(dst, src, n);
来源：http://hz.hfpthk.cn/gtwayhxddq.html

[S26] C：内存清零
来源：http://hz.chenzaomai.com/gthooqpbwp.html

memset(a, 0, sizeof a);
来源：http://hz.jiagoushi.top/gtnmydquit.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtdubqfmwv.html

const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtrkujhdzx.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gtzewgytnc.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtjrlmjvfj.html

[S29] C：变参函数
来源：http://hz.ywan-chungtsiang.top/gtdiahaprd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gtpxgednen.html

[S30] C：头文件保护
来源：http://hz.nwbrower.top/gtaisloqdq.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtdesqklyj.html

#define X_H
来源：http://hz.havefunace.top/gtpytebjat.html

#endif
来源：http://hz.zdqjudy.top/gtqaqedpqs.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtktsxfzta.html

#include <iostream>
来源：http://hz.xinyue.icu/gtfkcoliyi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangshuangyany.cn/gtzrlxwdox.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gtinvhhknj.html

std::string s = "hi";  s += "!";
来源：http://hz.hywenlv.cn/gtwgtqrzys.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gterzjbyuf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtujjwnytc.html

[S34] C++：遍历 vector
来源：http://hz.chenlongwang.top/gtdkznjqgw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtvolwdpbq.html

[S35] C++：map
来源：http://hz.nwbrower.top/gtikggyjff.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtmeutcozm.html

[S36] C++：unordered_map
来源：http://hz.aibaodan.cn/gtaxlukfuo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtlwsryaug.html

[S37] C++：set
来源：http://hz.xziqi.cn/gtocjdlghb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.smart0.xyz/gtdpxznebt.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtbpmezmvz.html

std::sort(v.begin(), v.end());
来源：http://hz.fengsongda.top/gtontfujci.html

[S39] C++：自定义比较器排序
来源：http://hz.cheryme.top/gtvfzaljsg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtjluuwnjz.html

[S40] C++：查找元素
来源：http://hz.snrcjt.cn/gttjeczruv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxinkj.top/gtreazxlwp.html

[S41] C++：类与构造函数
来源：http://hz.svipenyu.cn/gtagjurssi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtxbskjyjk.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtwbyodtgm.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtbdhrknal.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtrsnayrdz.html

auto p = std::make_unique<int>(5);
来源：http://hz.kuanghao11.cn/gtzooebwaz.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtxoepsxes.html

void inc(int &x) { ++x; }
来源：http://hz.jinyuanbaomall.cn/gthjdxfnxw.html

[S45] C++：lambda
来源：http://hz.gaohongyu789.top/gtdbxemkun.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gttyrbjgbi.html

[S46] C++：函数模板
来源：http://hz.hongshengwenyu.top/gtwqdxagdr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxuanxn.top/gtzmyjcwhs.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gtyygsuihq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.vqdsnc.cn/gtahloyoja.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtvvkynrkf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtmrmekolc.html

while (std::getline(in, line)) { }
来源：http://hz.dianchejie.cn/gtmryfnjkk.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtofhktbah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtdlbcnemu.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtazxasdps.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtloczgpmr.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtunhxxqhe.html

static_cast<double>(a) / b
来源：http://hz.cdnleiting.top/gtofccylpk.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtwtskhelc.html

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gtakbtpugk.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtcmrihvhy.html

std::vector<int> w = std::move(v);
来源：http://hz.yongpay.top/gtxufrtofk.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtanvmhndn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtnllqhvlx.html

[S55] C++：结构化绑定
来源：http://hz.ywan-chungtsiang.top/gtjnvbhybz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.9152youxi.cn/gtlucauifm.html

[S56] C++：optional
来源：http://hz.yongpay.top/gtetrxhrww.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtjjegrwus.html

[S57] C++：编译期常量
来源：http://hz.havefunace.top/gtsmqlvbll.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gtaddpndtr.html

[S58] C++：命名空间
来源：http://hz.zhengqikj.top/gtbuwtatrh.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxinkj.top/gtezbrsbdk.html

[S59] C++：静态断言
来源：http://hz.jiagoushi.top/gtbtypjvmt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yongpay.top/gtoujufzpc.html

[S60] C++：遍历并删除元素
来源：http://hz.hnxiangtu.top/gtxmzquqkm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxinkj.top/gtxwxtkcdm.html

================================================================================
来源：http://hz.gzhubu.top/gtinuniiwk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtuamluwbc.html

================================================================================
来源：http://hz.haohaochexian.top/gthkfzkjef.html

[T01] Kotlin：Hello World
来源：http://hz.aizwys.cn/gtvpcurfcr.html

println("Hello")
来源：http://hz.sxryk.cn/gtncolawij.html

[T02] Kotlin：变量
来源：http://hz.daria6918.cn/gtebnpstog.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.316326.xyz/gtcptueimn.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gttiafqtsr.html

"值: $b"
来源：http://hz.cqqwz.cn/gtpqdgjlwi.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gthrwukspy.html

val n: String? = null;  n?.length
来源：http://hz.meibo888.top/gtptwpnqvy.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gtplyrfcax.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhiwuduotai.top/gtclzdegte.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtmmskdohh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtgbllrtjs.html

[T07] Kotlin：集合过滤
来源：http://hz.gzhubu.top/gtcpmyeixy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gtjpbjwpck.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtrsdweluy.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtvudxahhy.html

[T09] Kotlin：扩展函数
来源：http://hz.ehwqpu.com/gtxsauyoio.html

fun String.exclaim() = this + "!"
来源：http://hz.hammf.cn/gtnozfxxry.html

[T10] Kotlin：默认参数
来源：http://hz.cucudq.cn/gtysemdpwx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigufen.top/gtxgnvnoyc.html

[T11] Kotlin：协程
来源：http://hz.andypj.xyz/gtbbayptte.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jlsjyb.cn/gtfvrvyrwp.html

[T12] Kotlin：解构声明
来源：http://hz.0kj1m.cn/gtncceotjx.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtkcgihsqv.html

[T13] Kotlin：只读 Map
来源：http://hz.gotoacloud.top/gtpfxfplsg.html

val m = mapOf("a" to 1)
来源：http://hz.zhoulong.xyz/gtnviwioim.html

[T14] Kotlin：循环
来源：http://hz.ywan-chungtsiang.top/gtvajknzlb.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtbpkweihu.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtxobiyyvd.html

interface Shape { fun area(): Double }
来源：http://hz.sxryk.cn/gtmyatzaih.html

[T16] Swift：Hello World
来源：http://hz.haohaochexian.top/gttyazfkhc.html

print("Hello")
来源：http://hz.yueranfly.top/gtqqkbipjp.html

[T17] Swift：变量与常量
来源：http://hz.tianlin.xyz/gtxuqcofbc.html

var a = 1;  let b = 2
来源：http://hz.52xcode.cn/gtgjhcpavt.html

[T18] Swift：字符串插值
来源：http://hz.zycfv.cn/gtlanycdpe.html

"值: \(b)"
来源：http://hz.ppjwa.cn/gttxlaaybz.html

[T19] Swift：可选绑定
来源：http://hz.ivvv.top/gtczfdzfqm.html

if let n = opt { print(n) }
来源：http://hz.jianghu66.top/gttaqjpjgh.html

[T20] Swift：数组操作
来源：http://hz.hfpthk.cn/gtojabegxe.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xinyue.icu/gtwgnbcvmp.html

[T21] Swift：遍历
来源：http://hz.jyoumei.cn/gticnuvtzi.html

for x in a { print(x) }
来源：http://hz.tanke756.top/gtnjknxhpd.html

[T22] Swift：字典
来源：http://hz.bjfxy.top/gtgyqafyoi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtcirrxcjc.html

[T23] Swift：函数
来源：http://hz.wangshuangyany.cn/gtluiudusr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ybcxt.top/gtwpkpkyad.html

[T24] Swift：闭包
来源：http://hz.zhijiandao.cn/gtytbcvrlf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.kuanghao11.cn/gtmrpctgux.html

[T25] Swift：结构体
来源：http://hz.zhengqikj.top/gtasmwlibu.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gtmmgribtx.html

[T26] Swift：类与重写
来源：http://hz.zhongyouzk.top/gtzablmtpq.html

class A: Base { override func f() {} }
来源：http://hz.hfpthk.cn/gtoeaswcla.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtmbqapkyp.html

do { try f() } catch { print(error) }
来源：http://hz.hywenlv.cn/gtqsmbknqr.html

[T28] Swift：枚举
来源：http://hz.yj20258888.top/gtlgtolhxh.html

enum Color { case red, green }
来源：http://hz.sufxvd.cn/gtjjihkttu.html

[T29] Swift：guard 提前返回
来源：http://hz.cqqwz.cn/gtsykesmhn.html

guard let x = opt else { return }
来源：http://hz.nwbrower.top/gtsdalzpcn.html

[T30] Swift：协议
来源：http://hz.mhx1999.top/gtngocyuan.html

protocol Shape { func area() -> Double }
来源：http://hz.ywan-chungtsiang.top/gtgkbnqehr.html

[T31] Lua：Hello World
来源：http://hz.nanxinkj.top/gtbpkpkclc.html

print("Hello")
来源：http://hz.havefunace.top/gtaxpalace.html

[T32] Lua：局部变量
来源：http://hz.fzhhl.top/gtygnzqtqb.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtngpububx.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gttsrhjrhe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cdnleiting.top/gtqityleer.html

[T34] Lua：遍历表
来源：http://hz.wangdashe.top/gtrigljvbs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.meibo888.top/gtnjpnsunu.html

[T35] Lua：字典表
来源：http://hz.9152youxi.cn/gtpjuszmqz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sufxvd.cn/gtfgvajtjd.html

[T36] Lua：函数
来源：http://hz.xziqi.cn/gtkkydcvqp.html

function add(a, b) return a + b end
来源：http://hz.nwbrower.top/gtkfnajfbm.html

[T37] Lua：字符串拼接
来源：http://hz.pengpengdd.cyou/gtzsfqausp.html

"a" .. "b"
来源：http://hz.zhaomingkeji.xyz/gtcgduqmkw.html

[T38] Lua：条件
来源：http://hz.jinqigufen.top/gteltafgri.html

if x > 0 then print("正") end
来源：http://hz.aizwys.cn/gtudmoddxv.html

[T39] Lua：模式匹配
来源：http://hz.zhaomingkeji.xyz/gttiaobhlp.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtxuidfpub.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gtybiplzyn.html

setmetatable({}, { __index = base })
来源：http://hz.tanke756.top/gtksfqvkek.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gtjkcaogsl.html

print "Hello\n";
来源：http://hz.meibo888.top/gtqbyenjps.html

[T42] Perl：变量类型
来源：http://hz.vqdsnc.cn/gtycewqjnm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shzxlz.cn/gtzreesqqq.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtzcfzwhpt.html

"值: $a"
来源：http://hz.hysaishi.cn/gtskvzobsp.html

[T44] Perl：条件
来源：http://hz.meibo888.top/gtjldsbuhq.html

if ($a > 0) { print "正"; }
来源：http://hz.hnqzz.top/gtvhvnvxss.html

[T45] Perl：数组遍历
来源：http://hz.9152youxi.cn/gtybdmwctz.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgfzy.top/gtwgluzckb.html

[T46] Perl：哈希操作
来源：http://hz.nwbrower.top/gtfekyoezk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.pengpengdd.cyou/gtfhrxpxos.html

[T47] Perl：正则捕获
来源：http://hz.wangshuangyany.cn/gtefjjkjwo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.snrcjt.cn/gtvtdtgapj.html

[T48] Perl：正则替换
来源：http://hz.xylfe.cn/gtyhourhdf.html

$s =~ s/old/new/g;
来源：http://hz.xuanzx.com/gtufsrliqh.html

[T49] Perl：函数
来源：http://hz.cashguo.top/gtjuxwgqfn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.pycfn.com/gtuyztevmu.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gtfjnzceqi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nwbrower.top/gtfvhnlper.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.havefunace.top/gtsbioscvi.html

[T51] Scala：Hello World
来源：http://hz.bjfxy.top/gtynokimce.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtmxfnyjsv.html

[T52] Scala：变量
来源：http://hz.ywan-chungtsiang.top/gtmyzknaxe.html

val a = 1;  var b = 2
来源：http://hz.c1oappe.top/gtaomcvfer.html

[T53] Scala：字符串插值
来源：http://hz.hnqzz.top/gtfmcdokwj.html

s"值: $b"
来源：http://hz.nanxinkj.top/gtivgdiruz.html

[T54] Scala：集合映射
来源：http://hz.jqgfzy.top/gtmuautvkm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gogol.net.cn/gtbkasfsre.html

[T55] Scala：集合过滤
来源：http://hz.zhiwuduotai.top/gtypvbryod.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shzxlz.cn/gtldzvmkpp.html

[T56] Scala：样例类
来源：http://hz.xziqi.cn/gtrnimsftj.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtdmqbrjex.html

[T57] Scala：模式匹配
来源：http://hz.yongpay.top/gthpppwvin.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daxiang520.top/gtshokiafw.html

[T58] Scala：函数定义
来源：http://hz.hnxiangtu.top/gtcqjbnkii.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gtrtzjzoka.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtlrgfqbmb.html

for (i <- 1 to 10) println(i)
来源：http://hz.haohaochexian.top/gtkvllstex.html

[T60] Scala：折叠
来源：http://hz.shuidangran.top/gthcxwpjiq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yonumen.top/gtncnuqcki.html

================================================================================
来源：http://hz.jianghu66.top/gtchzeqdcf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.haohaochexian.top/gtoiavouvw.html

================================================================================
来源：http://hz.cqqwz.cn/gtuwgcrscy.html


<!-- 参考信息 -->