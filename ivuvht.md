代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtpieacqjd.html

[R60] 只看 HTTP 状态码
来源：http://hz.cqqwz.cn/gtlsfgvmrv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sweek.top/gtrcbaepix.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtmdtxohpc.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtyldnntjn.html

[R62] 找最占空间的文件
来源：http://hz.ybcxt.top/gtumlmxgdl.html

du -ah . | sort -rh | head -10
来源：http://hz.sysykeji.top/gtsguopspz.html

[R63] 内存与进程
来源：http://hz.yj20258888.top/gtfddfilyw.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gthbmmjtlp.html

[R64] 结束进程
来源：http://hz.jinqigfzy.top/gtsdwuohpi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gtgnudelbh.html

[R65] 查看端口占用
来源：http://hz.jlsjyb.cn/gtzxlbjgnl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zycfv.cn/gtmwrrawjf.html

[R66] 定时任务
来源：http://hz.havefunace.top/gtjsxgoplc.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gtadxsejzd.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gthcovfidc.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtctpqefuo.html

[R68] 计算文件校验值
来源：http://hz.dashuyun.cn/gtvjbjmcci.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtrvqldqer.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gttwyzyrhd.html

head -c 16 /dev/urandom | base64
来源：http://hz.cheryme.top/gttajlctgw.html

[R70] 时间戳与互转
来源：http://hz.ppjwa.cn/gtvnijyckf.html

date +%s;  date -d @1700000000
来源：http://hz.vqdsnc.cn/gtasdcqwxw.html

[R71] 日期格式化
来源：http://hz.yonumen.top/gttuflcihs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258888.top/gtjiaazqze.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtdfavnurq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cdnleiting.top/gtgyylunnu.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gthveskzad.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gteqpvcyka.html

[R74] 批量重命名
来源：http://hz.smart0.xyz/gtvikrewid.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuanzx.com/gtalzxzomd.html

[R75] 导出环境变量
来源：http://hz.yj20258.top/gtgxetvakv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangkeji.top/gtyuqescwg.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtognpjtui.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtxqtsdbqh.html

[R77] 读取用户输入
来源：http://hz.chenlongwang.top/gthxnpqgkp.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtjfctbcpm.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gttdsqozvy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yonumen.top/gtyllynucl.html

[R79] 解析命令行选项
来源：http://hz.9152youxi.cn/gtoqrbgjxf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.9152youxi.cn/gtjmgxzjpo.html

[R80] 查看脚本执行耗时
来源：http://hz.zhixingplan.top/gtczowkdop.html

time ./run.sh
来源：http://hz.gzhubu.top/gtwpvefeux.html

================================================================================
来源：http://hz.ivvv.top/gtjvgehfmn.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtxtjvctdh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtimgebrsk.html

[S01] C：Hello World
来源：http://hz.ppjwa.cn/gtijfgejra.html

#include <stdio.h>
来源：http://hz.hammf.cn/gtjtpvcwje.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pengpengdd.cyou/gtvubfsafl.html

[S02] C：变量与格式化输出
来源：http://hz.andypj.xyz/gtmcpxkvcp.html

int a = 10; printf("%d\n", a);
来源：http://hz.yanxiufei.cn/gtgervntkt.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gteuywdwij.html

int x; scanf("%d", &x);
来源：http://hz.tian-w.cn/gtqiqzcydc.html

[S04] C：字符串复制
来源：http://hz.nanxuanxn.top/gtxtqbqxou.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgufenzy.top/gtrcfkdlyn.html

[S05] C：字符串长度
来源：http://hz.gaohongyu789.top/gthbwqxwpd.html

strlen(s)
来源：http://hz.shanyushiyangkeji.top/gtwqbepfjz.html

[S06] C：字符串比较
来源：http://hz.316326.xyz/gthgoxphix.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtdsrngiwf.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtmztdzcqj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258888.top/gthtdxmnpp.html

[S08] C：动态内存分配与释放
来源：http://hz.316326.xyz/gtyeovrfmh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guowangkeji.top/gtsbjwdhtm.html

[S09] C：结构体定义与初始化
来源：http://hz.shangyingyoupin.top/gtefzosckn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtscffkiux.html

[S10] C：指针与解引用
来源：http://hz.havefunace.top/gtfuaqiayv.html

int *p = &a;  *p = 5;
来源：http://hz.shangyingyoupin.top/gtnxczqktf.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtvfsbtqmg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ppjwa.cn/gtoljqodte.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sufxvd.cn/gttcufktpp.html

fclose(f);
来源：http://hz.meibo888.top/gtkzntxyeo.html

[S12] C：写文件
来源：http://hz.hongshengwenyu.top/gtczqvdhki.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtmrcqagop.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtyvglspsx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.9152youxi.cn/gthulockhp.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtqowxhops.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shuidangran.top/gtsoglwvkk.html

[S15] C：类型转换
来源：http://hz.ydzc1.top/gtellzgplb.html

(double) a / b
来源：http://hz.316326.xyz/gtbplzupnm.html

[S16] C：位操作置位
来源：http://hz.sxryk.cn/gthbzfqmjr.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtpiaqhbdi.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangtech.top/gtdomybgmw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtbgosrcrl.html

[S18] C：命令行参数
来源：http://hz.wangdashe.top/gtbswarkyn.html

int main(int argc, char **argv)
来源：http://hz.aibaodan.cn/gtdxxqajbv.html

[S19] C：快速排序
来源：http://hz.c1oappe.top/gtxmropstq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtebzcbdmk.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtgxwwoauw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtgwnxjebd.html

[S21] C：字符类别判断
来源：http://hz.jqgfzy.top/gtwfdgjwgp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cheryme.top/gtiycefcsr.html

[S22] C：字符串转数字
来源：http://hz.gaohongyu789.top/gtmmtipctr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhoulong.xyz/gtcpqlvfts.html

[S23] C：随机数
来源：http://hz.gzhubu.top/gtnrdnkjts.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuxming.cn/gtrcawmkwf.html

[S24] C：获取本地时间
来源：http://hz.chenjidiqi.icu/gtglfzcxhx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtputdctqz.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gtgvutbyim.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangkeji.top/gtguxxlchj.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtttkrdowh.html

memset(a, 0, sizeof a);
来源：http://hz.zhijiandao.cn/gtbwhpndhr.html

[S27] C：定义常量
来源：http://hz.ydjk.org.cn/gtqxlydhxg.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtupqxpafv.html

[S28] C：静态变量
来源：http://hz.yanxiufei.cn/gtjlizjudk.html

static int counter = 0;
来源：http://hz.pycfn.com/gtyfjodngf.html

[S29] C：变参函数
来源：http://hz.nanxuanxn.top/gtjapuvybv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtpcwwpluf.html

[S30] C：头文件保护
来源：http://hz.vqdsnc.cn/gtcnwivaqr.html

#ifndef X_H
来源：http://hz.fengsongda.top/gtimgtbtsv.html

#define X_H
来源：http://hz.shanyushiyangkeji.top/gtnovykkyr.html

#endif
来源：http://hz.aibaodan.cn/gtmqcwakce.html

[S31] C++：Hello World
来源：http://hz.yj20258888.top/gtrgsackoq.html

#include <iostream>
来源：http://hz.yueranfly.top/gtqjlgvpjk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhijiandao.cn/gtcavpmryj.html

[S32] C++：字符串
来源：http://hz.zhengqikj.top/gtkoazzerk.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtwhpszkhl.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangkeji.top/gtnyzgbfxl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtsixkgfuy.html

[S34] C++：遍历 vector
来源：http://hz.tian-w.cn/gtaxtyxmbn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtmpayzkhj.html

[S35] C++：map
来源：http://hz.jinqigfzy.top/gtwqkgqgqj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtusysvxrc.html

[S36] C++：unordered_map
来源：http://hz.316326.xyz/gtpfdwmovz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtqcomwwsu.html

[S37] C++：set
来源：http://hz.xuanzx.com/gtehlnhcek.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gttzvktsix.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtkqlbkkdv.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtalzjiuvp.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtwlrvbtcu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtxrdvmgch.html

[S40] C++：查找元素
来源：http://hz.gogol.net.cn/gtnmtruzze.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cucudq.cn/gtghqirelq.html

[S41] C++：类与构造函数
来源：http://hz.svipenyu.cn/gtdcalzupe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gtofoglrnn.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtfaeawcfg.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtqkyuquiq.html

[S43] C++：智能指针
来源：http://hz.tianlin.xyz/gttxhvwnud.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhijiandao.cn/gtfucznmec.html

[S44] C++：引用传参
来源：http://hz.tianlin.xyz/gtbrrqkdzd.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtqsdiibxf.html

[S45] C++：lambda
来源：http://hz.pengpengdd.cyou/gtovixvxgy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgufenzy.top/gtfejehzis.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtfomnvhzy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gtzubemdql.html

[S47] C++：结构化绑定遍历
来源：http://hz.vqdsnc.cn/gtmsdoearb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hfpthk.cn/gtrcsqpisv.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtjhfluvaq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fengsongda.top/gtwoujhfcr.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gtkyqlamdv.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtcirfavgo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jyoumei.cn/gthirqabat.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtrlczlcue.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ppjwa.cn/gtecgctjbj.html

[S51] C++：显式类型转换
来源：http://hz.svipenyu.cn/gtgntqxiro.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtksfubqjg.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtjqxzlkee.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangtech.top/gtzdiohige.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtulwtpppa.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtewxuifyx.html

[S54] C++：异常处理
来源：http://hz.ydjk.org.cn/gtccpshknh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhixingplan.top/gtmtuqtkmn.html

[S55] C++：结构化绑定
来源：http://hz.ehwqpu.com/gtnqjkqkrm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yonumen.top/gtvggtfwxe.html

[S56] C++：optional
来源：http://hz.wangshuangyany.cn/gtxjghhrwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zdqjudy.top/gtzjqtsdnb.html

[S57] C++：编译期常量
来源：http://hz.meibo888.top/gtknaspwoi.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtdvydlira.html

[S58] C++：命名空间
来源：http://hz.guannengcc.top/gtdexqpyes.html

namespace ns { int f() { return 1; } }
来源：http://hz.gaohongyu789.top/gtxfojtopj.html

[S59] C++：静态断言
来源：http://hz.nanxinkj.top/gtxqwpzknh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hywenlv.cn/gttwdvzvqa.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gtrpiocrxv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gtnwixaiej.html

================================================================================
来源：http://hz.shuidangran.top/gtgokqlehc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtfksduzsf.html

================================================================================
来源：http://hz.daxiang520.top/gtqkxhaeci.html

[T01] Kotlin：Hello World
来源：http://hz.hywenlv.cn/gtvmfcnctf.html

println("Hello")
来源：http://hz.tianlin.xyz/gtcgwykmtk.html

[T02] Kotlin：变量
来源：http://hz.sufxvd.cn/gtzylssmpy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.birdmap.top/gtnavezxmr.html

[T03] Kotlin：字符串模板
来源：http://hz.guannengcc.top/gteopyuykl.html

"值: $b"
来源：http://hz.hongshengwenyu.top/gtqxjgyjsi.html

[T04] Kotlin：空安全
来源：http://hz.yangfankeji.com/gtyglciwap.html

val n: String? = null;  n?.length
来源：http://hz.aibaodan.cn/gtiwwbbxul.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtlhkrsrfm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daxiang520.top/gtcewmckwj.html

[T06] Kotlin：集合映射
来源：http://hz.jinyuanbaomall.cn/gtluhpvnww.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gtjubajgfv.html

[T07] Kotlin：集合过滤
来源：http://hz.guowangkeji.top/gtvhzyxvkj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtsuggrheu.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtwotpfdbc.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtapiwgrti.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtwuhybozc.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gtzepnbuiv.html

[T10] Kotlin：默认参数
来源：http://hz.birdmap.top/gtocdobqvy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gogol.net.cn/gtalhqbusk.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtaqtotaoj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigufen.top/gtkhvfctul.html

[T12] Kotlin：解构声明
来源：http://hz.bjfxy.top/gtrevudevx.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuanzhike.top/gtbfogebdj.html

[T13] Kotlin：只读 Map
来源：http://hz.xinyue.icu/gtxfakyjoo.html

val m = mapOf("a" to 1)
来源：http://hz.fengsongda.top/gthdurozcc.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gthcomarqk.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtokcgsfdt.html

[T15] Kotlin：接口
来源：http://hz.svipenyu.cn/gttkuxryot.html

interface Shape { fun area(): Double }
来源：http://hz.hysaishi.cn/gtpuxdhonv.html

[T16] Swift：Hello World
来源：http://hz.jinqigufen.top/gtpnawjlte.html

print("Hello")
来源：http://hz.mhx1999.top/gtjfgexfzn.html

[T17] Swift：变量与常量
来源：http://hz.yueranfly.top/gttpfseiqe.html

var a = 1;  let b = 2
来源：http://hz.hnqzz.top/gtngstuyll.html

[T18] Swift：字符串插值
来源：http://hz.nanxinkj.top/gtyvfddbzc.html

"值: \(b)"
来源：http://hz.feifeiyinyue.top/gtqimbsepf.html

[T19] Swift：可选绑定
来源：http://hz.ydzc1.top/gtllzkqgrr.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtpoxrjhsm.html

[T20] Swift：数组操作
来源：http://hz.snrcjt.cn/gtpyjvwilo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtkhfpfpvt.html

[T21] Swift：遍历
来源：http://hz.ydjk.org.cn/gtzwxpijfs.html

for x in a { print(x) }
来源：http://hz.shzxlz.cn/gtppidnynp.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtgdubqgtk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenjidiqi.icu/gtkihoqgzo.html

[T23] Swift：函数
来源：http://hz.c1oappe.top/gtonmsmrfk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenzaomai.com/gtnyugpwmd.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangkeji.top/gtewxrvylp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.52xcode.cn/gtusuzargu.html

[T25] Swift：结构体
来源：http://hz.quarkkingdee.top/gtauulqbxe.html

struct P { var x: Int }
来源：http://hz.jinyuanbaomall.cn/gtpgzltwqr.html

[T26] Swift：类与重写
来源：http://hz.gotoacloud.top/gtqantsddr.html

class A: Base { override func f() {} }
来源：http://hz.zhaomingkeji.xyz/gtafeflaoj.html

[T27] Swift：错误处理
来源：http://hz.ybcxt.top/gtdvovazuu.html

do { try f() } catch { print(error) }
来源：http://hz.jinghuilouyu.cn/gtemakwtpq.html

[T28] Swift：枚举
来源：http://hz.svipenyu.cn/gtibpbhurh.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtnhkawonu.html

[T29] Swift：guard 提前返回
来源：http://hz.jinyuanbaomall.cn/gtpabekiyk.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtnfcbfgtk.html

[T30] Swift：协议
来源：http://hz.xziqi.cn/gtbxgosyoe.html

protocol Shape { func area() -> Double }
来源：http://hz.jyoumei.cn/gtmwpheenk.html

[T31] Lua：Hello World
来源：http://hz.zhengqikj.top/gtavfrcyuh.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtkzazduxk.html

[T32] Lua：局部变量
来源：http://hz.jyoumei.cn/gtmbqgesbe.html

local a = 1
来源：http://hz.daxiang520.top/gtxdoivcsr.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtskizible.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtnytvswww.html

[T34] Lua：遍历表
来源：http://hz.hfpthk.cn/gtovuarvzp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yvedp.cn/gtfjoglkvz.html

[T35] Lua：字典表
来源：http://hz.mhx1999.top/gtqhvnkhho.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gthzypksrs.html

[T36] Lua：函数
来源：http://hz.cdnleiting.top/gthiwltfjr.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gtdjeaapez.html

[T37] Lua：字符串拼接
来源：http://hz.jlsjyb.cn/gtbpgdjbix.html

"a" .. "b"
来源：http://hz.aibaodan.cn/gtuxmcfwmg.html

[T38] Lua：条件
来源：http://hz.shangyingyoupin.top/gtpbgavxbd.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtgdzzsfma.html

[T39] Lua：模式匹配
来源：http://hz.zhijiandao.cn/gthvwlzfxz.html

string.find(s, "%d+")
来源：http://hz.zhengqikj.top/gtvcaoferu.html

[T40] Lua：元表
来源：http://hz.ywan-chungtsiang.top/gtjzfxzbxd.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtlqjwltzf.html

[T41] Perl：Hello World
来源：http://hz.yonumen.top/gtvnwvdkog.html

print "Hello\n";
来源：http://hz.vqdsnc.cn/gtbrrjlkqr.html

[T42] Perl：变量类型
来源：http://hz.pycfn.com/gtxpivfhts.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.c1oappe.top/gtjglouqny.html

[T43] Perl：字符串插值
来源：http://hz.ppjwa.cn/gtggfycglr.html

"值: $a"
来源：http://hz.yanxiufei.cn/gtujmmqdep.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtqiehfqce.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangkeji.top/gtfcwqbtmm.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtjjqqajsz.html

for my $x (@arr) { print $x; }
来源：http://hz.snrcjt.cn/gtpizpbjch.html

[T46] Perl：哈希操作
来源：http://hz.feifeiyinyue.top/gtsgzndfms.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.andypj.xyz/gtsoffyndp.html

[T47] Perl：正则捕获
来源：http://hz.feifeiyinyue.top/gtoqhfpcui.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.fzhhl.top/gtbxxfytaf.html

[T48] Perl：正则替换
来源：http://hz.mhx1999.top/gtnnngnoyx.html

$s =~ s/old/new/g;
来源：http://hz.cucudq.cn/gtzgpnbgfn.html

[T49] Perl：函数
来源：http://hz.aizwys.cn/gtpdezsefx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj20258888.top/gtbmnknmbb.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtaqfbqopx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.havefunace.top/gtsfiahsng.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtjmlfzpyc.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtuovlrnun.html

println("Hello")
来源：http://hz.shuidangran.top/gtoagrlnen.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gtsfqbijgx.html

val a = 1;  var b = 2
来源：http://hz.smart0.xyz/gtycuymyfe.html

[T53] Scala：字符串插值
来源：http://hz.shzxlz.cn/gthduwlawf.html

s"值: $b"
来源：http://hz.gotoacloud.top/gtsawmackm.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gtopjrpzua.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yongpay.top/gtfpzqcith.html

[T55] Scala：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtzhrhhszc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xuanzx.com/gtanravkmy.html

[T56] Scala：样例类
来源：http://hz.gaohongyu789.top/gtqzvwyjot.html

case class User(name: String, age: Int)
来源：http://hz.ywan-chungtsiang.top/gtrtjxpctn.html

[T57] Scala：模式匹配
来源：http://hz.dianchejie.cn/gtvnfaomso.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.haohaochexian.top/gtgsperiml.html

[T58] Scala：函数定义
来源：http://hz.gaohongyu789.top/gtyiekxsqn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ybcxt.top/gtacbwnkug.html

[T59] Scala：循环
来源：http://hz.ydzc1.top/gtcbwrnnro.html

for (i <- 1 to 10) println(i)
来源：http://hz.xinyue.icu/gthcweyqwf.html

[T60] Scala：折叠
来源：http://hz.nanxuanxn.top/gtsacvhzlj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.0kj1m.cn/gtwvxajkzp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvnjdevtj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtzhcoudxc.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmvvoyuda.html


<!-- 参考信息 -->