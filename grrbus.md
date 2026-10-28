代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yueranfly.top/gtrfvkhkrw.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gtbtblhoqt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtffjfjrms.html

[R61] 磁盘占用
来源：http://hz.hywenlv.cn/gttxdynlab.html

df -h;  du -sh *
来源：http://hz.daria6918.cn/gtijdvcyss.html

[R62] 找最占空间的文件
来源：http://hz.sweek.top/gtqrwrpxbo.html

du -ah . | sort -rh | head -10
来源：http://hz.zhiwuduotai.top/gtwqobsqwj.html

[R63] 内存与进程
来源：http://hz.hammf.cn/gtiwkwbqcj.html

free -h;  ps aux | grep nginx
来源：http://hz.ehwqpu.com/gtcqypqusb.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtjiqhzyre.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtsfexkeju.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtdavanjpe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gttjbezmdj.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gtzwqmhbqw.html

crontab -e;  crontab -l
来源：http://hz.hywenlv.cn/gtyopveisn.html

[R67] 生成随机十六进制串
来源：http://hz.vqdsnc.cn/gtoszdejvi.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtplkkqbpb.html

[R68] 计算文件校验值
来源：http://hz.xuanzx.com/gtrqevxjjg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gtqlfrhfii.html

[R69] 生成随机密码
来源：http://hz.hnqzz.top/gtrsxanvtt.html

head -c 16 /dev/urandom | base64
来源：http://hz.haohaochexian.top/gtquuynsoi.html

[R70] 时间戳与互转
来源：http://hz.fengsongda.top/gtwiojubxh.html

date +%s;  date -d @1700000000
来源：http://hz.sweek.top/gtpbtkqwmg.html

[R71] 日期格式化
来源：http://hz.yj202588.top/gtjmymbzln.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhengqikj.top/gtiwytcuno.html

[R72] 等待端口就绪
来源：http://hz.kuanghao11.cn/gtjjliadvr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtgevnjvct.html

[R73] 分割大日志
来源：http://hz.jqgfzy.top/gterjaufyl.html

split -l 1000 big.log part_
来源：http://hz.guannengcc.top/gthptiafoo.html

[R74] 批量重命名
来源：http://hz.xziqi.cn/gtzeypowsj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.feifeiyinyue.top/gtvvpugqga.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtsvogwdon.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sxryk.cn/gthajybram.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gtpudnuwld.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtweozdvgl.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtxjuesrwe.html

read -rp "请输入: " ans
来源：http://hz.52xcode.cn/gtsosuxirb.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gtvivkegiu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtqoklhcbs.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtehimmipb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtwlhffllf.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtlrilmxtf.html

time ./run.sh
来源：http://hz.aibaodan.cn/gtcilqrhth.html

================================================================================
来源：http://hz.daxiang520.top/gtmftvyazi.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtdbaypche.html

================================================================================
来源：http://hz.chenlongwang.top/gtjukukvab.html

[S01] C：Hello World
来源：http://hz.ydjk.org.cn/gttphfmrqc.html

#include <stdio.h>
来源：http://hz.snrcjt.cn/gtbjhlvgfo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gttfpqfvfi.html

[S02] C：变量与格式化输出
来源：http://hz.gotoacloud.top/gtimyxnzat.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gttvbzghnz.html

[S03] C：读入整数
来源：http://hz.sufxvd.cn/gtxkvifpgl.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtfsvpdgwr.html

[S04] C：字符串复制
来源：http://hz.gaohongyu789.top/gtyzbbigbh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnqzz.top/gtkaxpxmlr.html

[S05] C：字符串长度
来源：http://hz.hnqzz.top/gtjdqvdoqi.html

strlen(s)
来源：http://hz.iojbl.cn/gthhsprgdw.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtfpuwcrni.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtzarocwtb.html

[S07] C：数组遍历求和
来源：http://hz.daxiang520.top/gtwjitzlxg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gthfhsnmma.html

[S08] C：动态内存分配与释放
来源：http://hz.chenzaomai.com/gtbsxbxjog.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtiqdcufdw.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtauupwxoz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gtlmpchnyp.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtlsyzaxxk.html

int *p = &a;  *p = 5;
来源：http://hz.zhiwuduotai.top/gtlotvvhco.html

[S11] C：逐行读文件
来源：http://hz.ehwqpu.com/gtvpizesjx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gttkkmqdkg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cdnleiting.top/gtreqzihrq.html

fclose(f);
来源：http://hz.hywenlv.cn/gtoglduvjk.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtkajjsmsi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jyoumei.cn/gtsogzsnpz.html

[S13] C：宏定义
来源：http://hz.xinyue.icu/gtkyyaoigp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtikkbnhnj.html

[S14] C：枚举
来源：http://hz.quarkkingdee.top/gtzallcztr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangdashe.top/gtfifdaush.html

[S15] C：类型转换
来源：http://hz.redwolf501.top/gtdzlhjdvz.html

(double) a / b
来源：http://hz.yanxiufei.cn/gtcsxovjdx.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gtapjlsebf.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtreuylqwj.html

[S17] C：安全拼接字符串
来源：http://hz.iojbl.cn/gtajhungue.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aibaodan.cn/gtknpysfxx.html

[S18] C：命令行参数
来源：http://hz.gogol.net.cn/gttipbcfyh.html

int main(int argc, char **argv)
来源：http://hz.yj202588.top/gtdgbsvmlo.html

[S19] C：快速排序
来源：http://hz.jinghuilouyu.cn/gtmeudssdq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yangfankeji.com/gttouqsyxn.html

[S20] C：二分查找
来源：http://hz.chenjidiqi.icu/gtjjnyztet.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtywnmdukz.html

[S21] C：字符类别判断
来源：http://hz.xuetiantiany.cn/gtakjdbcwc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtdttkuvmo.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtweqakuaq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gttlrgozrm.html

[S23] C：随机数
来源：http://hz.ppjwa.cn/gtovphynat.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ehwqpu.com/gtuxqrqhzd.html

[S24] C：获取本地时间
来源：http://hz.tanke756.top/gtoivwzncc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtxopmbzek.html

[S25] C：内存拷贝
来源：http://hz.daxiang520.top/gtdjernvtd.html

memcpy(dst, src, n);
来源：http://hz.hammf.cn/gtmmpixosp.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtrzwcxztd.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gthdsgkcoa.html

[S27] C：定义常量
来源：http://hz.jinqigfzy.top/gtbfljsmmc.html

const double PI = 3.14159;
来源：http://hz.jianghu66.top/gtujgviwpr.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtepehbuci.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtaxjymsil.html

[S29] C：变参函数
来源：http://hz.cqqwz.cn/gtqeiijyky.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jlsjyb.cn/gtvgghxsgn.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gtrftazqsc.html

#ifndef X_H
来源：http://hz.aizwys.cn/gtbxhipbzx.html

#define X_H
来源：http://hz.cucudq.cn/gtbdfcqucu.html

#endif
来源：http://hz.yonumen.top/gtkoinjpjr.html

[S31] C++：Hello World
来源：http://hz.hywenlv.cn/gtqjiotblb.html

#include <iostream>
来源：http://hz.kuanghao11.cn/gtbxvlalnk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigufen.top/gtldubkoog.html

[S32] C++：字符串
来源：http://hz.cheryme.top/gtlsutixtv.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtfdtwxiih.html

[S33] C++：vector 增删
来源：http://hz.mhx1999.top/gtorhlcphr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtukjemvim.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtiokisitt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtbwwcngxu.html

[S35] C++：map
来源：http://hz.hywenlv.cn/gtttzacgvu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtiutgmuwd.html

[S36] C++：unordered_map
来源：http://hz.chenzaomai.com/gtwbwplmbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtsmlotccr.html

[S37] C++：set
来源：http://hz.iojbl.cn/gtsltzfwci.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.vqdsnc.cn/gtacpggywt.html

[S38] C++：排序
来源：http://hz.aizwys.cn/gtdcuqfjkb.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtvfpfekdq.html

[S39] C++：自定义比较器排序
来源：http://hz.jlsjyb.cn/gtrwrfmmrk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sweek.top/gtoysrvegz.html

[S40] C++：查找元素
来源：http://hz.daxiang520.top/gtpeiidoiv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtxudfrnig.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtgcthpbht.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gtgexgrzib.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtrsxskzma.html

class B : public Base { public: void f() override {} };
来源：http://hz.zycfv.cn/gtjxidqumk.html

[S43] C++：智能指针
来源：http://hz.jianghu66.top/gterjfvgst.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gttselezem.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gtfrpodgnz.html

void inc(int &x) { ++x; }
来源：http://hz.nanxinkj.top/gtlenlkofs.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtsjuvdgrm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fengsongda.top/gtrddgagqr.html

[S46] C++：函数模板
来源：http://hz.yvedp.cn/gtnhzujehb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangkeji.top/gtbyzyvnyh.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gtxwhthkga.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhengqikj.top/gtgdjpbivr.html

[S48] C++：逐行读文件
来源：http://hz.ydjk.org.cn/gtpngskvbz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtnxykyfjo.html

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtjkysyjzl.html

[S49] C++：写文件
来源：http://hz.xuanzx.com/gthnvwbnhz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtwaeldohi.html

[S50] C++：格式化数字
来源：http://hz.hfpthk.cn/gtlfupmvea.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtppgjugwg.html

[S51] C++：显式类型转换
来源：http://hz.chenzaomai.com/gtjozqydyt.html

static_cast<double>(a) / b
来源：http://hz.9152youxi.cn/gtakzpqyru.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gtfieocxla.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258.top/gtslnfpqwq.html

[S53] C++：移动语义
来源：http://hz.tianlin.xyz/gtzcqtespr.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtonovgpag.html

[S54] C++：异常处理
来源：http://hz.bjfxy.top/gtxhvmpgzm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtycrlgtor.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtuufkxhvd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gtgonhqukw.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtvmqrrxrz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtfgiqvkqi.html

[S57] C++：编译期常量
来源：http://hz.jinyuanbaomall.cn/gtcxsejqau.html

constexpr int N = 10;
来源：http://hz.yangfankeji.com/gtvysqvxiq.html

[S58] C++：命名空间
来源：http://hz.xziqi.cn/gtftscibhz.html

namespace ns { int f() { return 1; } }
来源：http://hz.gaohongyu789.top/gtqmxwrdri.html

[S59] C++：静态断言
来源：http://hz.hammf.cn/gtcodtvpdb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yanxiufei.cn/gtnmbeylin.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigfzy.top/gtkzvgwtok.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtqtdsafdx.html

================================================================================
来源：http://hz.chenlongwang.top/gtgjkzsizh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtnejqzshb.html

================================================================================
来源：http://hz.c1oappe.top/gtwfhnvirx.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtgiebryfb.html

println("Hello")
来源：http://hz.haohaochexian.top/gtkptfrkta.html

[T02] Kotlin：变量
来源：http://hz.chenjidiqi.icu/gtfxocpore.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.0kj1m.cn/gtnwrikjnb.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtdqquuvpf.html

"值: $b"
来源：http://hz.9152youxi.cn/gtteqxbqos.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtisegeihz.html

val n: String? = null;  n?.length
来源：http://hz.shuidangran.top/gtovucwgcu.html

[T05] Kotlin：when 表达式
来源：http://hz.gotoacloud.top/gtvhgmotbw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtqicuzlku.html

[T06] Kotlin：集合映射
来源：http://hz.cashguo.top/gtmibojait.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tanke756.top/gtienbgcsf.html

[T07] Kotlin：集合过滤
来源：http://hz.sufxvd.cn/gtyduewewu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhiwuduotai.top/gtdzlgwqtd.html

[T08] Kotlin：数据类
来源：http://hz.zhixingplan.top/gttmwapxjy.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtcosbvyxa.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtzyxuoolw.html

fun String.exclaim() = this + "!"
来源：http://hz.shuidangran.top/gtohqkapyn.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gtlbgvfqhl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dashuyun.cn/gtmfujfvsm.html

[T11] Kotlin：协程
来源：http://hz.sufxvd.cn/gtwstehajf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ppjwa.cn/gtkguwaadv.html

[T12] Kotlin：解构声明
来源：http://hz.jianghu66.top/gtbnwauxoy.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gtpwkbapkm.html

[T13] Kotlin：只读 Map
来源：http://hz.cdnleiting.top/gtuzpylvqx.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtvhqabeqz.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtxonedhte.html

for (i in 1..10) println(i)
来源：http://hz.zhengqikj.top/gtuxgjzxhf.html

[T15] Kotlin：接口
来源：http://hz.zhengqikj.top/gtabqcmasx.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtaxsuawga.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtwwpdcrks.html

print("Hello")
来源：http://hz.guowangkeji.top/gtxcfxcllk.html

[T17] Swift：变量与常量
来源：http://hz.tanke756.top/gtmwsskwou.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtfkalosge.html

[T18] Swift：字符串插值
来源：http://hz.hywenlv.cn/gtqdgvcadb.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtpggfkpwo.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtuwfrpxoe.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtgmogfcuc.html

[T20] Swift：数组操作
来源：http://hz.cucudq.cn/gthqubikoq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangdashe.top/gtwshtebzy.html

[T21] Swift：遍历
来源：http://hz.zhixingplan.top/gtoofzxiva.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gtvnnbeopp.html

[T22] Swift：字典
来源：http://hz.zhijiandao.cn/gtuubkrgsr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yuxming.cn/gtipuzsusy.html

[T23] Swift：函数
来源：http://hz.zycfv.cn/gtitzcpcts.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.smart0.xyz/gtdoxaxchk.html

[T24] Swift：闭包
来源：http://hz.sweek.top/gtplzdsqqk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtzrowfioa.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtujptshhx.html

struct P { var x: Int }
来源：http://hz.zhiwuduotai.top/gtwbuebflw.html

[T26] Swift：类与重写
来源：http://hz.svipenyu.cn/gtxsejtxnr.html

class A: Base { override func f() {} }
来源：http://hz.chenzaomai.com/gtcplicklg.html

[T27] Swift：错误处理
来源：http://hz.yuanzhike.top/gtgrekgijs.html

do { try f() } catch { print(error) }
来源：http://hz.zhiwuduotai.top/gtcksygmfz.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtkyjtylbw.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtkqblyfsj.html

[T29] Swift：guard 提前返回
来源：http://hz.wangdashe.top/gtbbcohomk.html

guard let x = opt else { return }
来源：http://hz.yj202588.top/gtpxfrdhmh.html

[T30] Swift：协议
来源：http://hz.zhixingplan.top/gtbztqikxl.html

protocol Shape { func area() -> Double }
来源：http://hz.bjfxy.top/gtjrskmqpf.html

[T31] Lua：Hello World
来源：http://hz.yuanzhike.top/gtoktocxkp.html

print("Hello")
来源：http://hz.316326.xyz/gtzlfaeoof.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtvaejpqoo.html

local a = 1
来源：http://hz.hfpthk.cn/gtacgfxudc.html

[T33] Lua：表（数组）
来源：http://hz.52xcode.cn/gtuvnqklyl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cdnleiting.top/gthzeapqfg.html

[T34] Lua：遍历表
来源：http://hz.mhx1999.top/gtncbssrmr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tianlin.xyz/gtcmbukpez.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtarifdpfo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xinyue.icu/gtnemxfhsz.html

[T36] Lua：函数
来源：http://hz.wangdashe.top/gtfllidwbz.html

function add(a, b) return a + b end
来源：http://hz.snrcjt.cn/gtxhvvctdm.html

[T37] Lua：字符串拼接
来源：http://hz.nwbrower.top/gtnipjqyiu.html

"a" .. "b"
来源：http://hz.guowangkeji.top/gtyvtsooul.html

[T38] Lua：条件
来源：http://hz.dianchejie.cn/gtuiupyieh.html

if x > 0 then print("正") end
来源：http://hz.yvedp.cn/gtfmqwjhvi.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtrntiryze.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtunfffwic.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtatxawqbg.html

setmetatable({}, { __index = base })
来源：http://hz.hfpthk.cn/gtzszdfemf.html

[T41] Perl：Hello World
来源：http://hz.jqgufenzy.top/gtsrsurpge.html

print "Hello\n";
来源：http://hz.shzxlz.cn/gtpfgvikim.html

[T42] Perl：变量类型
来源：http://hz.mhx1999.top/gtyjkejzcf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xylfe.cn/gtytshmizu.html

[T43] Perl：字符串插值
来源：http://hz.316326.xyz/gtrkswzmly.html

"值: $a"
来源：http://hz.nanxinkj.top/gteimuldwm.html

[T44] Perl：条件
来源：http://hz.9152youxi.cn/gtwbstcqvo.html

if ($a > 0) { print "正"; }
来源：http://hz.smart0.xyz/gtoebcqsgl.html

[T45] Perl：数组遍历
来源：http://hz.daxiang520.top/gtvcutzbcn.html

for my $x (@arr) { print $x; }
来源：http://hz.aizwys.cn/gtiflghaik.html

[T46] Perl：哈希操作
来源：http://hz.pengpengdd.cyou/gtlskjdkcy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenlongwang.top/gttydqogzw.html

[T47] Perl：正则捕获
来源：http://hz.yj202588.top/gtoeixytxv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhongyouzk.top/gtheqafnht.html

[T48] Perl：正则替换
来源：http://hz.hongshengwenyu.top/gtgukpjdnz.html

$s =~ s/old/new/g;
来源：http://hz.yj20258.top/gtwvxagkjj.html

[T49] Perl：函数
来源：http://hz.zhijiandao.cn/gthhgzbmja.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhongyouzk.top/gthwltaram.html

[T50] Perl：逐行读文件
来源：http://hz.jlsjyb.cn/gttjyovzvm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jianghu66.top/gtpuvqguei.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuetiantiany.cn/gtjlihbxyl.html

[T51] Scala：Hello World
来源：http://hz.guowangkeji.top/gtlgjyztoy.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gthlcuprhh.html

[T52] Scala：变量
来源：http://hz.svipenyu.cn/gtorxkscyo.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangkeji.top/gtgzprkaaz.html

[T53] Scala：字符串插值
来源：http://hz.mhx1999.top/gtzvicfsgm.html

s"值: $b"
来源：http://hz.svipenyu.cn/gttluvhdbs.html

[T54] Scala：集合映射
来源：http://hz.svipenyu.cn/gtzxvtzlpa.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sxryk.cn/gtykmcnatj.html

[T55] Scala：集合过滤
来源：http://hz.haohaochexian.top/gtmrgwzibk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fzhhl.top/gtjpdxbxfg.html

[T56] Scala：样例类
来源：http://hz.xylfe.cn/gtidhsuehn.html

case class User(name: String, age: Int)
来源：http://hz.quarkkingdee.top/gtkfigiwcu.html

[T57] Scala：模式匹配
来源：http://hz.0kj1m.cn/gtjaumrcac.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sysykeji.top/gtswfxjgtw.html

[T58] Scala：函数定义
来源：http://hz.hongshengwenyu.top/gtrystotje.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zdqjudy.top/gtqhskbrsf.html

[T59] Scala：循环
来源：http://hz.ydjk.org.cn/gtmnqkkwrt.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtbhwxwojx.html

[T60] Scala：折叠
来源：http://hz.daxiang520.top/gtttwnmksy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jiagoushi.top/gtzabdlxzr.html

================================================================================
来源：http://hz.chenzaomai.com/gtgnetxyrd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gthpsazhef.html

================================================================================
来源：http://hz.cdnleiting.top/gtiznppyot.html


<!-- 参考信息 -->