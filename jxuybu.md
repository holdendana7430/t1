代发 wailian999

df -h;  du -sh *
来源：http://hz.zycfv.cn/gtkqvkhrks.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gtaptkcdam.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtpgpnsmio.html

[R63] 内存与进程
来源：http://hz.wangdashe.top/gtwsbavvvv.html

free -h;  ps aux | grep nginx
来源：http://hz.yanxiufei.cn/gtujbntufi.html

[R64] 结束进程
来源：http://hz.shangyingyoupin.top/gtiisfppyc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hysaishi.cn/gtosucskcz.html

[R65] 查看端口占用
来源：http://hz.tian-w.cn/gtckplcenn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jyoumei.cn/gtymdmurcp.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtrfuafuai.html

crontab -e;  crontab -l
来源：http://hz.tian-w.cn/gtylxmmlad.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtvxmckqgv.html

openssl rand -hex 16
来源：http://hz.hywenlv.cn/gtfwzarted.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gteikniumw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtsrapjeit.html

[R69] 生成随机密码
来源：http://hz.yonumen.top/gtldgitomq.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtkhsvbajn.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gthouyxbie.html

date +%s;  date -d @1700000000
来源：http://hz.guannengcc.top/gtzmtzpyai.html

[R71] 日期格式化
来源：http://hz.hnxiangtu.top/gtzkqdqwft.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cheryme.top/gtrtstvgpt.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtvsalrvar.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtzahiflfm.html

[R73] 分割大日志
来源：http://hz.zycfv.cn/gtyzukjjrm.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtljpxfmwm.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtadfiwcol.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hywenlv.cn/gtybotlhez.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtwigzbqkf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgufenzy.top/gtmbsbmkyq.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtxmyyisln.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gtletngezx.html

[R77] 读取用户输入
来源：http://hz.zdqjudy.top/gtzzwwztdo.html

read -rp "请输入: " ans
来源：http://hz.ivvv.top/gtrqcvxcaj.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtgkrbsciy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtjiogyrvf.html

[R79] 解析命令行选项
来源：http://hz.zhixingplan.top/gtdwjcwxai.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuxming.cn/gtrpegkvry.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtazllvexf.html

time ./run.sh
来源：http://hz.ydjk.org.cn/gtzwfnprxx.html

================================================================================
来源：http://hz.cucudq.cn/gtpzokxtme.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtydqlhnqb.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnbwrnliu.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gtadsgjday.html

#include <stdio.h>
来源：http://hz.sxryk.cn/gtzxsztrhr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pengpengdd.cyou/gtufjeymve.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtfozkptwe.html

int a = 10; printf("%d\n", a);
来源：http://hz.yonumen.top/gtfgrwoipz.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtvazrihpn.html

int x; scanf("%d", &x);
来源：http://hz.cqqwz.cn/gtlhfyyidt.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gtzyimssbv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.9152youxi.cn/gtklbjwkpi.html

[S05] C：字符串长度
来源：http://hz.jlsjyb.cn/gtiaxtlxsp.html

strlen(s)
来源：http://hz.zhongyouzk.top/gtywsmfett.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gtphsaxmku.html

strcmp(a, b) == 0
来源：http://hz.gzhubu.top/gtrogwadez.html

[S07] C：数组遍历求和
来源：http://hz.zhiwuduotai.top/gttkexhiqr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gtessyomel.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtizyqrkhg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yvedp.cn/gtmmiyqqct.html

[S09] C：结构体定义与初始化
来源：http://hz.fengsongda.top/gtpuwqjwfz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yanxiufei.cn/gtjlfmrxte.html

[S10] C：指针与解引用
来源：http://hz.sxryk.cn/gtptutsrhp.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigufen.top/gtkdfgqpep.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtvwjslibb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cdnleiting.top/gtaznysclc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xinyue.icu/gtwkfgtmxv.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtduzptyxk.html

[S12] C：写文件
来源：http://hz.jlsjyb.cn/gtzpccydcc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xziqi.cn/gtgdywzhdf.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtemhjapyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtnnseobwd.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gthaffmkmu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tian-w.cn/gtgdwfifsm.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtctsqtcdq.html

(double) a / b
来源：http://hz.wangdashe.top/gtvovlbqvy.html

[S16] C：位操作置位
来源：http://hz.sufxvd.cn/gtpvrydokv.html

x |= (1 << 3);
来源：http://hz.jinqigfzy.top/gtxgmorvsj.html

[S17] C：安全拼接字符串
来源：http://hz.hysaishi.cn/gtxzcbhdwz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gtqsjgxibt.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gthlfaesgw.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtzagkdkso.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gtdlwovrrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtnneyogsy.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gtuywwnemu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtfnckdjfp.html

[S21] C：字符类别判断
来源：http://hz.chenlongwang.top/gtiezmpspu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ywan-chungtsiang.top/gtjdlvxsfx.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtlcondpty.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhixingplan.top/gtmmkcjthr.html

[S23] C：随机数
来源：http://hz.hnxiangtu.top/gtyjsfqccn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gtwxcbqmls.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gttzzipnit.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xylfe.cn/gthamviukt.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gthsbrkrog.html

memcpy(dst, src, n);
来源：http://hz.andypj.xyz/gtgyidaggs.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtpsryecxv.html

memset(a, 0, sizeof a);
来源：http://hz.ydjk.org.cn/gtujaitzzy.html

[S27] C：定义常量
来源：http://hz.hongshengwenyu.top/gtevjdbwde.html

const double PI = 3.14159;
来源：http://hz.jyoumei.cn/gtkeharidt.html

[S28] C：静态变量
来源：http://hz.jqgfzy.top/gtsieycdgv.html

static int counter = 0;
来源：http://hz.quarkkingdee.top/gtvwrcgxzg.html

[S29] C：变参函数
来源：http://hz.yj20258888.top/gtlcqpgech.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jianghu66.top/gtumtxjecd.html

[S30] C：头文件保护
来源：http://hz.cheryme.top/gttkwxmdtl.html

#ifndef X_H
来源：http://hz.jinghuilouyu.cn/gtbhsjdvqp.html

#define X_H
来源：http://hz.cucudq.cn/gtmnvdqtvq.html

#endif
来源：http://hz.meibo888.top/gtqesbzcho.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtoazpmthy.html

#include <iostream>
来源：http://hz.xuanzx.com/gthwxkmbnw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hfpthk.cn/gtedtppqnu.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gtgrsfvvmn.html

std::string s = "hi";  s += "!";
来源：http://hz.nwbrower.top/gtqvqxtwnd.html

[S33] C++：vector 增删
来源：http://hz.yj20258888.top/gtcfxyifae.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtktumctaf.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtilgfesor.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hywenlv.cn/gtrdnozafl.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gttwrzinns.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtzdkaaxii.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtluxvujyh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtbbaquqpk.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtwqpzjbbw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daria6918.cn/gtvvqnunpb.html

[S38] C++：排序
来源：http://hz.xingfuxueyuan.xyz/gtrwbyhcpn.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gtbpixgeyd.html

[S39] C++：自定义比较器排序
来源：http://hz.guowangkeji.top/gtkmvqgskh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sxryk.cn/gtoezgdtix.html

[S40] C++：查找元素
来源：http://hz.tian-w.cn/gtxtgczmus.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gthoriczhx.html

[S41] C++：类与构造函数
来源：http://hz.aizwys.cn/gtzwssfgvp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtdxmherel.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gtxdcvfuur.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinqigufen.top/gtuhbeksgj.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gthsflllsf.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhixingplan.top/gttyxmrral.html

[S44] C++：引用传参
来源：http://hz.ehwqpu.com/gtlwvpkilh.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtuzczmujs.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gthcclgmlg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuanzx.com/gttonphnix.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtctdmucqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gtbbraidwk.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhixingplan.top/gttuhfkbiv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.kuanghao11.cn/gtostahgkv.html

[S48] C++：逐行读文件
来源：http://hz.yvedp.cn/gtmibuvaht.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gttsegemou.html

while (std::getline(in, line)) { }
来源：http://hz.sufxvd.cn/gtdaxkqjxk.html

[S49] C++：写文件
来源：http://hz.cdnleiting.top/gteqiplcly.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gttegkemyj.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gtpqspjnks.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yvedp.cn/gtolgvheny.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gtvvitgefk.html

static_cast<double>(a) / b
来源：http://hz.vqdsnc.cn/gtauysinvh.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gtxnqbfvlb.html

int size() const noexcept { return n_; }
来源：http://hz.jqgufenzy.top/gtlglzylzj.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtqljqiejj.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gtiadtamuk.html

[S54] C++：异常处理
来源：http://hz.yvedp.cn/gtoifdthsm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tianlin.xyz/gtnpfaeiup.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtvqwwfnxs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ehwqpu.com/gtpgmcwscc.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtwdarpngk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtqdnkejhj.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtczoexutq.html

constexpr int N = 10;
来源：http://hz.wangdashe.top/gtkxplucjn.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtdhqlysuf.html

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gtpycdojpt.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtbuxaonez.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.feifeiyinyue.top/gtwwneqsjn.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtakpjeesz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuetiantiany.cn/gtzjwxpgvn.html

================================================================================
来源：http://hz.zycfv.cn/gtoqixvxbm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtjlitnwkn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwwbvnqwq.html

[T01] Kotlin：Hello World
来源：http://hz.yongpay.top/gtlrxykahr.html

println("Hello")
来源：http://hz.redwolf501.top/gtypwzluej.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtgfrdzmyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gtxosaxqfj.html

[T03] Kotlin：字符串模板
来源：http://hz.shuidangran.top/gtntzpxmgh.html

"值: $b"
来源：http://hz.chenzaomai.com/gtqstuwkps.html

[T04] Kotlin：空安全
来源：http://hz.ywan-chungtsiang.top/gtpqobwhxa.html

val n: String? = null;  n?.length
来源：http://hz.hysaishi.cn/gtxkoyvnzc.html

[T05] Kotlin：when 表达式
来源：http://hz.hysaishi.cn/gtfrbzwgya.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aibaodan.cn/gtaqrosijr.html

[T06] Kotlin：集合映射
来源：http://hz.quarkkingdee.top/gtnebjzxcv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sufxvd.cn/gtilfolfkd.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gttfpedlzo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sxryk.cn/gtqurkeorf.html

[T08] Kotlin：数据类
来源：http://hz.shangyingyoupin.top/gtsgydqtdq.html

data class User(val name: String, val age: Int)
来源：http://hz.snrcjt.cn/gtalcaqzyu.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtywbrvhkg.html

fun String.exclaim() = this + "!"
来源：http://hz.zdqjudy.top/gtvpjotghm.html

[T10] Kotlin：默认参数
来源：http://hz.kuanghao11.cn/gtxmcitxjz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj202588.top/gtezhkdirz.html

[T11] Kotlin：协程
来源：http://hz.xinyue.icu/gtnwkkmpih.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gogol.net.cn/gtaolqhbji.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtdfstssag.html

val (a, b) = Pair(1, 2)
来源：http://hz.shzxlz.cn/gtjvadgtne.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgufenzy.top/gtruievpml.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gtlngjgpdz.html

[T14] Kotlin：循环
来源：http://hz.smart0.xyz/gtsdffxwyh.html

for (i in 1..10) println(i)
来源：http://hz.yvedp.cn/gtsvknecxg.html

[T15] Kotlin：接口
来源：http://hz.yj20258888.top/gtyuqxhbig.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gtluxeqhmm.html

[T16] Swift：Hello World
来源：http://hz.sysykeji.top/gtxwzxsdih.html

print("Hello")
来源：http://hz.aibaodan.cn/gtoshgzknx.html

[T17] Swift：变量与常量
来源：http://hz.ywan-chungtsiang.top/gtppssgxja.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtlixdnmhk.html

[T18] Swift：字符串插值
来源：http://hz.hnxiangtu.top/gtxxmemubo.html

"值: \(b)"
来源：http://hz.c1oappe.top/gtphmdogyu.html

[T19] Swift：可选绑定
来源：http://hz.nanxuanxn.top/gtujwnqpwa.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtniennmdv.html

[T20] Swift：数组操作
来源：http://hz.gzhubu.top/gtencciusg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yangfankeji.com/gttzfiqyqk.html

[T21] Swift：遍历
来源：http://hz.yanxiufei.cn/gtealgwzrs.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtbgexecww.html

[T22] Swift：字典
来源：http://hz.bjfxy.top/gtujaupcly.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtxsylgfng.html

[T23] Swift：函数
来源：http://hz.cucudq.cn/gteoqwjjrn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtatptlszp.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtgyylwydp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtujzibhib.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gtekstdonc.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtevmxamnw.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtmhtftnvz.html

class A: Base { override func f() {} }
来源：http://hz.snrcjt.cn/gtnauvsxoy.html

[T27] Swift：错误处理
来源：http://hz.yangfankeji.com/gtliiezwjw.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangkeji.top/gtkhjsntoj.html

[T28] Swift：枚举
来源：http://hz.smart0.xyz/gteyluygci.html

enum Color { case red, green }
来源：http://hz.xuanzx.com/gtrxjezrnn.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtufcguhbn.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gthcouslpk.html

[T30] Swift：协议
来源：http://hz.fzhhl.top/gtgivbicqu.html

protocol Shape { func area() -> Double }
来源：http://hz.c1oappe.top/gtnzcqsizj.html

[T31] Lua：Hello World
来源：http://hz.aizwys.cn/gttjujwjnv.html

print("Hello")
来源：http://hz.nwbrower.top/gtebpfyeaz.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtmkeuizyr.html

local a = 1
来源：http://hz.birdmap.top/gtcgehpygh.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtoslorblf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigfzy.top/gtogxkwvpt.html

[T34] Lua：遍历表
来源：http://hz.gzhubu.top/gtmenvodrs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dianchejie.cn/gtwsysirmb.html

[T35] Lua：字典表
来源：http://hz.gotoacloud.top/gtakjmhxqd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nanxinkj.top/gtkvhwhbda.html

[T36] Lua：函数
来源：http://hz.chenjidiqi.icu/gttwvvqfqm.html

function add(a, b) return a + b end
来源：http://hz.xylfe.cn/gtmwcybdot.html

[T37] Lua：字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtzvsnjeqx.html

"a" .. "b"
来源：http://hz.jinqigufen.top/gtaqrjjpmb.html

[T38] Lua：条件
来源：http://hz.shzxlz.cn/gtpzcocevz.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gtoiqwxuzx.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtxbwlnomu.html

string.find(s, "%d+")
来源：http://hz.havefunace.top/gtgspkcipz.html

[T40] Lua：元表
来源：http://hz.quarkkingdee.top/gthehyiwmo.html

setmetatable({}, { __index = base })
来源：http://hz.ivvv.top/gtezczwdpu.html

[T41] Perl：Hello World
来源：http://hz.chenlongwang.top/gtercjgdod.html

print "Hello\n";
来源：http://hz.cucudq.cn/gthwqzfufy.html

[T42] Perl：变量类型
来源：http://hz.yuanzhike.top/gtpuouvgwx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxinkj.top/gtjicdmall.html

[T43] Perl：字符串插值
来源：http://hz.zhongyouzk.top/gtkjblgpil.html

"值: $a"
来源：http://hz.xuetiantiany.cn/gtylnfqbjg.html

[T44] Perl：条件
来源：http://hz.aizwys.cn/gtqywmgjlc.html

if ($a > 0) { print "正"; }
来源：http://hz.hammf.cn/gtrhhkfilk.html

[T45] Perl：数组遍历
来源：http://hz.jqgfzy.top/gtuazholuj.html

for my $x (@arr) { print $x; }
来源：http://hz.cqqwz.cn/gtdpjesuwz.html

[T46] Perl：哈希操作
来源：http://hz.yangfankeji.com/gtxqukyyqq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zycfv.cn/gttccjugyb.html

[T47] Perl：正则捕获
来源：http://hz.zhongyouzk.top/gthxvbxazc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.vqdsnc.cn/gtzxxtsafb.html

[T48] Perl：正则替换
来源：http://hz.ppjwa.cn/gtxewfzdng.html

$s =~ s/old/new/g;
来源：http://hz.chenzaomai.com/gtrbssximz.html

[T49] Perl：函数
来源：http://hz.nanxinkj.top/gtrkgkdvap.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ydzc1.top/gthwtvfcts.html

[T50] Perl：逐行读文件
来源：http://hz.hammf.cn/gtujrtzxva.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cqqwz.cn/gtygupimzn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ppjwa.cn/gtiheocpty.html

[T51] Scala：Hello World
来源：http://hz.hywenlv.cn/gtqsdvkbxz.html

println("Hello")
来源：http://hz.xinyue.icu/gtqodpqoyt.html

[T52] Scala：变量
来源：http://hz.dianchejie.cn/gtiafvjdqs.html

val a = 1;  var b = 2
来源：http://hz.guowangkeji.top/gtxefgpith.html

[T53] Scala：字符串插值
来源：http://hz.svipenyu.cn/gthcawkwds.html

s"值: $b"
来源：http://hz.zycfv.cn/gtwwlxpkac.html

[T54] Scala：集合映射
来源：http://hz.0kj1m.cn/gtyfttxexl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sysykeji.top/gtgnscfnje.html

[T55] Scala：集合过滤
来源：http://hz.cashguo.top/gtknfvtpjv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinghuilouyu.cn/gtxhohxqox.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gtqyilmryi.html

case class User(name: String, age: Int)
来源：http://hz.zhaomingkeji.xyz/gtkbaylymj.html

[T57] Scala：模式匹配
来源：http://hz.gotoacloud.top/gtomnblqdc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinyuanbaomall.cn/gtiqbeootu.html

[T58] Scala：函数定义
来源：http://hz.yuanzhike.top/gteifwdjsz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shzxlz.cn/gtibbnirhv.html

[T59] Scala：循环
来源：http://hz.mhx1999.top/gttuitkptc.html

for (i <- 1 to 10) println(i)
来源：http://hz.cheryme.top/gtjrdqibsz.html

[T60] Scala：折叠
来源：http://hz.xinyue.icu/gtroymudsl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nanxuanxn.top/gtxhyjxbuu.html

================================================================================
来源：http://hz.yangfankeji.com/gtewevhrgw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtcfgogfyq.html

================================================================================
来源：http://hz.52xcode.cn/gtjstfsntf.html

[U01] Py：创建虚拟环境
来源：http://hz.tian-w.cn/gtskxupjts.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yanxiufei.cn/gtbwsnbfvd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daria6918.cn/gteheqmjve.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gteogmvopd.html


<!-- 参考信息 -->