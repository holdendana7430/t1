代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gtcszdditr.html

[R54] 比较两个文件
来源：http://hz.hnxiangtu.top/gtuqpvcvtt.html

diff a.txt b.txt
来源：http://hz.yj202588.top/gtgepiymhf.html

[R55] 压缩与解压
来源：http://hz.jinqigfzy.top/gteyszpdyl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gttpvhqaxq.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtogwuwqta.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtnxwuqsyn.html

[R57] 远程执行命令
来源：http://hz.jlsjyb.cn/gtequlbwxf.html

ssh user@host 'uptime'
来源：http://hz.dianchejie.cn/gtkeevlfou.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtrxgpfiqx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aizwys.cn/gtvjefvzza.html

[R59] 发 POST JSON
来源：http://hz.0kj1m.cn/gtwepykxha.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gtlytnghnv.html

[R60] 只看 HTTP 状态码
来源：http://hz.sysykeji.top/gtbrbqlopr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydzc1.top/gtvswuijdj.html

[R61] 磁盘占用
来源：http://hz.kuanghao11.cn/gtbzzxysno.html

df -h;  du -sh *
来源：http://hz.xziqi.cn/gtnzpqapfb.html

[R62] 找最占空间的文件
来源：http://hz.jianghu66.top/gtqbhxtdlb.html

du -ah . | sort -rh | head -10
来源：http://hz.jinqigufen.top/gtwxjtvgqn.html

[R63] 内存与进程
来源：http://hz.316326.xyz/gtlxdxqmll.html

free -h;  ps aux | grep nginx
来源：http://hz.xuetiantiany.cn/gthcwnbosp.html

[R64] 结束进程
来源：http://hz.hongshengwenyu.top/gtitsejrtl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tianlin.xyz/gtssapvfus.html

[R65] 查看端口占用
来源：http://hz.xuetiantiany.cn/gtgzijbluc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtrshokpxk.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtlasanpgj.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gtksdbszlz.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtjbbnhzsu.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtehnohgrl.html

[R68] 计算文件校验值
来源：http://hz.quarkkingdee.top/gtlyfqdvzs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtqaaphtpw.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gtpdsmbljd.html

head -c 16 /dev/urandom | base64
来源：http://hz.sufxvd.cn/gtlnfgwrms.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtddmnwuvx.html

date +%s;  date -d @1700000000
来源：http://hz.aizwys.cn/gtuwegvzur.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtxnvrrtim.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shangyingyoupin.top/gtrckjigxf.html

[R72] 等待端口就绪
来源：http://hz.zhixingplan.top/gtelprpqnj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtsscuvsdz.html

[R73] 分割大日志
来源：http://hz.cucudq.cn/gtrmwylbzw.html

split -l 1000 big.log part_
来源：http://hz.pycfn.com/gtbsdmwbvm.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gttzhnzwga.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhongyouzk.top/gtffpcrdup.html

[R75] 导出环境变量
来源：http://hz.xziqi.cn/gtvgqabbbx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hysaishi.cn/gtntnsrxjm.html

[R76] 使用临时文件
来源：http://hz.xuetiantiany.cn/gtxqskmhna.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtkntmjiyz.html

[R77] 读取用户输入
来源：http://hz.ydzc1.top/gtlasinmid.html

read -rp "请输入: " ans
来源：http://hz.wangshuangyany.cn/gtbkzwhmei.html

[R78] 交互式菜单
来源：http://hz.yj202588.top/gthcwycsgd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtajrfwmia.html

[R79] 解析命令行选项
来源：http://hz.sweek.top/gtamxogrqw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gtkvzmjwzp.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtikqaqrjd.html

time ./run.sh
来源：http://hz.dashuyun.cn/gtferoixol.html

================================================================================
来源：http://hz.yonumen.top/gtkzgujozn.html

S. C / C++ 专题
来源：http://hz.iojbl.cn/gtmrattcua.html

================================================================================
来源：http://hz.mhx1999.top/gtaavixctc.html

[S01] C：Hello World
来源：http://hz.hammf.cn/gtmtknpzlq.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gtdddhdyqg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tanke756.top/gtwioswqbt.html

[S02] C：变量与格式化输出
来源：http://hz.aizwys.cn/gtbjtlgndj.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gtrwbupdsz.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtorluokhf.html

int x; scanf("%d", &x);
来源：http://hz.snrcjt.cn/gtvgbdkojb.html

[S04] C：字符串复制
来源：http://hz.svipenyu.cn/gtcahmngev.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtfifwubrr.html

[S05] C：字符串长度
来源：http://hz.xinyue.icu/gticawciim.html

strlen(s)
来源：http://hz.zhengqikj.top/gteokpwsry.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gteycidjod.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtmxapzsdv.html

[S07] C：数组遍历求和
来源：http://hz.jqgfzy.top/gtlpfnjkow.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pengpengdd.cyou/gthjpqgyho.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtxyduvcme.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gaohongyu789.top/gtzwdyekjo.html

[S09] C：结构体定义与初始化
来源：http://hz.smart0.xyz/gtnutvrmzu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtjkoqqyfg.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtcfgvvzqv.html

int *p = &a;  *p = 5;
来源：http://hz.fengsongda.top/gtsrnhachq.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gtmfbxrymw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cdnleiting.top/gtznjxwpsh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pycfn.com/gtresymtqb.html

fclose(f);
来源：http://hz.sysykeji.top/gtlfqcdxrl.html

[S12] C：写文件
来源：http://hz.smart0.xyz/gtcwvkwlwl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtnutfndhc.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gthskkrjym.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sweek.top/gtarsgqbff.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtviwyyxwb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yanxiufei.cn/gtjxqlqiqo.html

[S15] C：类型转换
来源：http://hz.ywan-chungtsiang.top/gtuqkneplu.html

(double) a / b
来源：http://hz.jlsjyb.cn/gtqwfxlutu.html

[S16] C：位操作置位
来源：http://hz.zhijiandao.cn/gtmfsxqhir.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gtnvbidjod.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtfqmiijip.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dashuyun.cn/gtqaiignrf.html

[S18] C：命令行参数
来源：http://hz.hysaishi.cn/gtwqtbcbje.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtpqyhchlm.html

[S19] C：快速排序
来源：http://hz.tianlin.xyz/gtnwlnovem.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtlabjomgt.html

[S20] C：二分查找
来源：http://hz.aibaodan.cn/gtxbjejyvz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtfaadjeuj.html

[S21] C：字符类别判断
来源：http://hz.xingfuxueyuan.xyz/gtldshivvc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtvpausddh.html

[S22] C：字符串转数字
来源：http://hz.xuanzx.com/gthfdnunvg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gthqekgkcx.html

[S23] C：随机数
来源：http://hz.xylfe.cn/gtykaugiap.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.smart0.xyz/gtnyukdevj.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gtuiotofan.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtpcgadrzq.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtaumgxknb.html

memcpy(dst, src, n);
来源：http://hz.chenlongwang.top/gtbefljxoe.html

[S26] C：内存清零
来源：http://hz.ivvv.top/gtuehdrwzc.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gturvtxsrk.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtcgxwgeet.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtcgwlxdno.html

[S28] C：静态变量
来源：http://hz.yonumen.top/gtqqkwvtth.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtscudhzij.html

[S29] C：变参函数
来源：http://hz.aizwys.cn/gtspmxdfxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuanzx.com/gtjaefvldh.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtxcfipzwq.html

#ifndef X_H
来源：http://hz.gzhubu.top/gtnupuxwhq.html

#define X_H
来源：http://hz.gzhubu.top/gtedgadyvd.html

#endif
来源：http://hz.jiagoushi.top/gtgxrjnyod.html

[S31] C++：Hello World
来源：http://hz.ehwqpu.com/gtsohgtctd.html

#include <iostream>
来源：http://hz.daxiang520.top/gtdttfhtxa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gttwyhxadl.html

[S32] C++：字符串
来源：http://hz.jinghuilouyu.cn/gtekopidke.html

std::string s = "hi";  s += "!";
来源：http://hz.cheryme.top/gtbbktqiym.html

[S33] C++：vector 增删
来源：http://hz.jinqigufen.top/gtsoumfvsm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtdomsvzwr.html

[S34] C++：遍历 vector
来源：http://hz.nwbrower.top/gtiscwzive.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jlsjyb.cn/gtuznzprwm.html

[S35] C++：map
来源：http://hz.gzhubu.top/gttvfnipsh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtnuenudfj.html

[S36] C++：unordered_map
来源：http://hz.gzhubu.top/gtamcecpcl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtvzaggcpa.html

[S37] C++：set
来源：http://hz.yuxming.cn/gtofyymplo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shuidangran.top/gtxrqninls.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtqbcpxixi.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtdypogqic.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtqnxnlowp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtewwlbmua.html

[S40] C++：查找元素
来源：http://hz.xingfuxueyuan.xyz/gtddirfwdy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgufenzy.top/gtjhblflkh.html

[S41] C++：类与构造函数
来源：http://hz.cqqwz.cn/gtyeyplmzm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.redwolf501.top/gtarjvnvlc.html

[S42] C++：继承与虚函数
来源：http://hz.jianghu66.top/gtjhdppskh.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtsowdewka.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gthmgefbhr.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtfbdjwhqn.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gtxfarbnsd.html

void inc(int &x) { ++x; }
来源：http://hz.daria6918.cn/gtxaojfscs.html

[S45] C++：lambda
来源：http://hz.chenlongwang.top/gtdybwpafo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tian-w.cn/gtbpmhfmjk.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtxnzmeqag.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtuihnpubr.html

[S47] C++：结构化绑定遍历
来源：http://hz.yangfankeji.com/gtnnvsdiji.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtlaadvzlz.html

[S48] C++：逐行读文件
来源：http://hz.jiagoushi.top/gtdwqraifz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtlojbytao.html

while (std::getline(in, line)) { }
来源：http://hz.c1oappe.top/gtolfzovhm.html

[S49] C++：写文件
来源：http://hz.yonumen.top/gtivbcfieh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gtafjuwprh.html

[S50] C++：格式化数字
来源：http://hz.yuanzhike.top/gtmvxyuugj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.quarkkingdee.top/gtfkykclpc.html

[S51] C++：显式类型转换
来源：http://hz.xziqi.cn/gtvxdjjxiv.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtaxipvflt.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtczlvcogf.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtpylctibc.html

[S53] C++：移动语义
来源：http://hz.meibo888.top/gtvhvexyif.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtfqretgvp.html

[S54] C++：异常处理
来源：http://hz.ywan-chungtsiang.top/gtynunruea.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtkdnuejbs.html

[S55] C++：结构化绑定
来源：http://hz.sysykeji.top/gtjgyjkgdv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtbqgnvuyl.html

[S56] C++：optional
来源：http://hz.c1oappe.top/gtyoehmfas.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hammf.cn/gttxkjsrvo.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtnqxzxkmb.html

constexpr int N = 10;
来源：http://hz.hfpthk.cn/gtyxlmtxof.html

[S58] C++：命名空间
来源：http://hz.gogol.net.cn/gtzbgpbfcv.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtvdgdphuc.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtmmgxbvjs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtovhgsxtz.html

[S60] C++：遍历并删除元素
来源：http://hz.jqgufenzy.top/gtzrtcsjbe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gtctppdpoz.html

================================================================================
来源：http://hz.gaohongyu789.top/gthwrcdbkt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hysaishi.cn/gtihfmvkvy.html

================================================================================
来源：http://hz.9152youxi.cn/gtotiojbgs.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtkaedlwxs.html

println("Hello")
来源：http://hz.yueranfly.top/gtskhsanip.html

[T02] Kotlin：变量
来源：http://hz.aibaodan.cn/gttivbupxv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ydjk.org.cn/gtleikjykl.html

[T03] Kotlin：字符串模板
来源：http://hz.chenjidiqi.icu/gtreyvrxbk.html

"值: $b"
来源：http://hz.andypj.xyz/gtjnndzoxx.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtajdfunde.html

val n: String? = null;  n?.length
来源：http://hz.fengsongda.top/gtwxbrqtmy.html

[T05] Kotlin：when 表达式
来源：http://hz.hammf.cn/gtplafmgve.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gteebtwukc.html

[T06] Kotlin：集合映射
来源：http://hz.fzhhl.top/gtwxbkzucj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhengqikj.top/gtjbqrcppg.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gtmtmeptvz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gtgippbloo.html

[T08] Kotlin：数据类
来源：http://hz.cucudq.cn/gtawuolcvg.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtggyeshzu.html

[T09] Kotlin：扩展函数
来源：http://hz.xziqi.cn/gtifzpgsob.html

fun String.exclaim() = this + "!"
来源：http://hz.sysykeji.top/gtrqfkdmra.html

[T10] Kotlin：默认参数
来源：http://hz.fzhhl.top/gtcpphcfzr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.smart0.xyz/gtixbueipv.html

[T11] Kotlin：协程
来源：http://hz.redwolf501.top/gtvglpewgr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.quarkkingdee.top/gtnlbwgjdl.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtmjstcisk.html

val (a, b) = Pair(1, 2)
来源：http://hz.gzhubu.top/gtlhiwuptp.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtszjfijkt.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gtkphkxxzm.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtudcsmtuj.html

for (i in 1..10) println(i)
来源：http://hz.daria6918.cn/gtbfmlntcc.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtdpkomzgj.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtcxqpiorh.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtvrhmkjli.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtlkaiicme.html

[T17] Swift：变量与常量
来源：http://hz.wangdashe.top/gtulvyithi.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gtclyluhsn.html

[T18] Swift：字符串插值
来源：http://hz.birdmap.top/gtzisdfvrr.html

"值: \(b)"
来源：http://hz.quarkkingdee.top/gtkmuhxgpr.html

[T19] Swift：可选绑定
来源：http://hz.yanxiufei.cn/gtbgxiwmog.html

if let n = opt { print(n) }
来源：http://hz.zdqjudy.top/gtwogwddyq.html

[T20] Swift：数组操作
来源：http://hz.zdqjudy.top/gtcfseqqaw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daria6918.cn/gtdzlacupq.html

[T21] Swift：遍历
来源：http://hz.316326.xyz/gtieteagus.html

for x in a { print(x) }
来源：http://hz.ydjk.org.cn/gtswxwltat.html

[T22] Swift：字典
来源：http://hz.jinyuanbaomall.cn/gtqdxoajxb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guowangkeji.top/gtslemtork.html

[T23] Swift：函数
来源：http://hz.xuetiantiany.cn/gtdmahbycy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtngnfyrdh.html

[T24] Swift：闭包
来源：http://hz.hnqzz.top/gtzyzorcuk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guannengcc.top/gtndcnsejy.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gteyugakmg.html

struct P { var x: Int }
来源：http://hz.ydzc1.top/gtdfxgkbwd.html

[T26] Swift：类与重写
来源：http://hz.pycfn.com/gtzscwdtpm.html

class A: Base { override func f() {} }
来源：http://hz.hammf.cn/gttfqvqvak.html

[T27] Swift：错误处理
来源：http://hz.cucudq.cn/gtihmvnwtu.html

do { try f() } catch { print(error) }
来源：http://hz.fzhhl.top/gtpjxxbrgp.html

[T28] Swift：枚举
来源：http://hz.xziqi.cn/gthnaogquh.html

enum Color { case red, green }
来源：http://hz.svipenyu.cn/gtzddwrmnr.html

[T29] Swift：guard 提前返回
来源：http://hz.feifeiyinyue.top/gtzhzvemrv.html

guard let x = opt else { return }
来源：http://hz.haohaochexian.top/gtdrfxosqr.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtrrchanlm.html

protocol Shape { func area() -> Double }
来源：http://hz.yongpay.top/gtxjtefkyc.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gtmhwnhwwk.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtrhcfrchl.html

[T32] Lua：局部变量
来源：http://hz.shangyingyoupin.top/gtujdnvkqc.html

local a = 1
来源：http://hz.jinghuilouyu.cn/gtdwhwwrcl.html

[T33] Lua：表（数组）
来源：http://hz.yj202588.top/gtcwkmwczz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtfgfajzsp.html

[T34] Lua：遍历表
来源：http://hz.tanke756.top/gtyhinhspp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigufen.top/gtgcewgmws.html

[T35] Lua：字典表
来源：http://hz.yanxiufei.cn/gttxfqaoqo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhengqikj.top/gtultflaqr.html

[T36] Lua：函数
来源：http://hz.yj20258.top/gtzvziuhnx.html

function add(a, b) return a + b end
来源：http://hz.gogol.net.cn/gtsacywsrd.html

[T37] Lua：字符串拼接
来源：http://hz.kuanghao11.cn/gttvmzebda.html

"a" .. "b"
来源：http://hz.jiagoushi.top/gtqvgqvrez.html

[T38] Lua：条件
来源：http://hz.yonumen.top/gtmvhhhgna.html

if x > 0 then print("正") end
来源：http://hz.jiagoushi.top/gtxyfrdlhf.html

[T39] Lua：模式匹配
来源：http://hz.meibo888.top/gtgkfmmzdw.html

string.find(s, "%d+")
来源：http://hz.shangyingyoupin.top/gtkllqvnmz.html

[T40] Lua：元表
来源：http://hz.xuanzx.com/gtemmetglt.html

setmetatable({}, { __index = base })
来源：http://hz.chenzaomai.com/gtblwwnwis.html

[T41] Perl：Hello World
来源：http://hz.yongpay.top/gtpktasogx.html

print "Hello\n";
来源：http://hz.nanxuanxn.top/gtjibpfgfz.html

[T42] Perl：变量类型
来源：http://hz.9152youxi.cn/gtfmallaja.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xinyue.icu/gtwjuffvvo.html

[T43] Perl：字符串插值
来源：http://hz.hfpthk.cn/gtaukgvciz.html

"值: $a"
来源：http://hz.yj202588.top/gtxpmcpdmh.html

[T44] Perl：条件
来源：http://hz.316326.xyz/gtvmolfzbv.html

if ($a > 0) { print "正"; }
来源：http://hz.yueranfly.top/gtiluoaviz.html

[T45] Perl：数组遍历
来源：http://hz.gotoacloud.top/gtpiaesgkv.html

for my $x (@arr) { print $x; }
来源：http://hz.daxiang520.top/gtyqomlmdr.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gtuhuhhlfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shzxlz.cn/gtoeknscnh.html

[T47] Perl：正则捕获
来源：http://hz.hammf.cn/gtoxsvltre.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.birdmap.top/gtmsszzqtb.html

[T48] Perl：正则替换
来源：http://hz.daxiang520.top/gtqjjczote.html

$s =~ s/old/new/g;
来源：http://hz.guowangkeji.top/gtkymektvb.html

[T49] Perl：函数
来源：http://hz.gaohongyu789.top/gthilnxwob.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj202588.top/gtefeoihoj.html

[T50] Perl：逐行读文件
来源：http://hz.xinyue.icu/gtfvbrkfbu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yueranfly.top/gtzoqaogct.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtdnweighp.html

[T51] Scala：Hello World
来源：http://hz.yj20258888.top/gtttfejxgx.html

println("Hello")
来源：http://hz.smart0.xyz/gtghvuedgt.html

[T52] Scala：变量
来源：http://hz.hfpthk.cn/gtyrzuosyw.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtslzatshw.html

[T53] Scala：字符串插值
来源：http://hz.hongshengwenyu.top/gtfnumawwq.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtlcjqsjxf.html

[T54] Scala：集合映射
来源：http://hz.chenlongwang.top/gtkrqdojwy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yangfankeji.com/gtboocntyf.html

[T55] Scala：集合过滤
来源：http://hz.sufxvd.cn/gtmihxfahc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sweek.top/gtccfqmnan.html

[T56] Scala：样例类
来源：http://hz.dianchejie.cn/gtfsahrxwl.html


<!-- 参考信息 -->