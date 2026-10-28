代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinyuanbaomall.cn/gtumzqpfju.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtgsdnkilw.html

crontab -e;  crontab -l
来源：http://hz.sweek.top/gtjikgqyrq.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gtsvlqxlhx.html

openssl rand -hex 16
来源：http://hz.redwolf501.top/gtppostlfh.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtetwensop.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.52xcode.cn/gthtssnabt.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtclhjifwz.html

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gtxfgqhbtk.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtdruizfwt.html

date +%s;  date -d @1700000000
来源：http://hz.redwolf501.top/gthghwtzow.html

[R71] 日期格式化
来源：http://hz.yj20258.top/gtzaiejzvq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jyoumei.cn/gtpflqnhis.html

[R72] 等待端口就绪
来源：http://hz.meibo888.top/gtrgnprpgx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hammf.cn/gtrpyfyzze.html

[R73] 分割大日志
来源：http://hz.andypj.xyz/gteyowxhpd.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtcowiaelj.html

[R74] 批量重命名
来源：http://hz.xuetiantiany.cn/gtxdvsacuq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xinyue.icu/gtqouuohds.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gtklrmreft.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sysykeji.top/gtrphqnabm.html

[R76] 使用临时文件
来源：http://hz.shangyingyoupin.top/gtcqgqgmik.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtblldadhl.html

[R77] 读取用户输入
来源：http://hz.316326.xyz/gtvrlmsmfj.html

read -rp "请输入: " ans
来源：http://hz.wangdashe.top/gtpwgwmxlz.html

[R78] 交互式菜单
来源：http://hz.ivvv.top/gtbyezjaov.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sufxvd.cn/gthaxmcclw.html

[R79] 解析命令行选项
来源：http://hz.redwolf501.top/gtfzoexyfj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenzaomai.com/gtpopgmesw.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtlxikqfnk.html

time ./run.sh
来源：http://hz.nwbrower.top/gtkosvkfmn.html

================================================================================
来源：http://hz.ivvv.top/gtbtuujixz.html

S. C / C++ 专题
来源：http://hz.nanxinkj.top/gtlaypqoex.html

================================================================================
来源：http://hz.daria6918.cn/gtkvsrhuuu.html

[S01] C：Hello World
来源：http://hz.9152youxi.cn/gtxrbihivw.html

#include <stdio.h>
来源：http://hz.xuetiantiany.cn/gtngdqownw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtghacyxmd.html

[S02] C：变量与格式化输出
来源：http://hz.jqgfzy.top/gtblvwczzu.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gtjnxhpxox.html

[S03] C：读入整数
来源：http://hz.yj20258.top/gtcljdqnnz.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtoryhtiun.html

[S04] C：字符串复制
来源：http://hz.smart0.xyz/gtgncmyqgm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gthveiztwl.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtnbmtcdyl.html

strlen(s)
来源：http://hz.cqqwz.cn/gtqmbzdqax.html

[S06] C：字符串比较
来源：http://hz.haohaochexian.top/gtkvmkvzlm.html

strcmp(a, b) == 0
来源：http://hz.xinyue.icu/gtvdwulkrm.html

[S07] C：数组遍历求和
来源：http://hz.guannengcc.top/gtsuakqeze.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jiagoushi.top/gtpmpmiibn.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtwjpokjio.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258.top/gtgzrtuido.html

[S09] C：结构体定义与初始化
来源：http://hz.zhengqikj.top/gtkztrrrxl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinyuanbaomall.cn/gteqkmfuwj.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtwwljjbib.html

int *p = &a;  *p = 5;
来源：http://hz.ppjwa.cn/gtjmssolzq.html

[S11] C：逐行读文件
来源：http://hz.hnxiangtu.top/gtvrenkzkx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.snrcjt.cn/gtkvvwcuuv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gtpulkuxwd.html

fclose(f);
来源：http://hz.zdqjudy.top/gtglgnxtte.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtijbqsvrt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtrmzaeydd.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtwlqhguap.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtxtfbhpzi.html

[S14] C：枚举
来源：http://hz.xuetiantiany.cn/gtbopawiqm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtijophyca.html

[S15] C：类型转换
来源：http://hz.gaohongyu789.top/gtludqhorr.html

(double) a / b
来源：http://hz.yangfankeji.com/gttqoqmjhj.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtymaxkidt.html

x |= (1 << 3);
来源：http://hz.svipenyu.cn/gtkirrnkkb.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gtrqaypudf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tianlin.xyz/gtqqwcetcw.html

[S18] C：命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtpxkitoyb.html

int main(int argc, char **argv)
来源：http://hz.ybcxt.top/gtgtslbdhj.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtgmgugemq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtvywxzvxh.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtklpjlrfp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtxkqkoqml.html

[S21] C：字符类别判断
来源：http://hz.shzxlz.cn/gtyrgrorvr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtjczvxmaq.html

[S22] C：字符串转数字
来源：http://hz.wangshuangyany.cn/gtwmosahhz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtbqgcmssh.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtgyilpnxo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtmydiwuxi.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtppgemwha.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.feifeiyinyue.top/gtwvmyopvh.html

[S25] C：内存拷贝
来源：http://hz.tianlin.xyz/gtjfwbdmqm.html

memcpy(dst, src, n);
来源：http://hz.yj20258.top/gtiahngand.html

[S26] C：内存清零
来源：http://hz.jinqigufen.top/gtsovvfojv.html

memset(a, 0, sizeof a);
来源：http://hz.hammf.cn/gtutcyiupe.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtrxkfisfi.html

const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gtelgrmzkm.html

[S28] C：静态变量
来源：http://hz.pengpengdd.cyou/gtydstmevp.html

static int counter = 0;
来源：http://hz.snrcjt.cn/gtnqdekgyn.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtnsawuoby.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtgrbcvrjc.html

[S30] C：头文件保护
来源：http://hz.iojbl.cn/gtkrswttfq.html

#ifndef X_H
来源：http://hz.havefunace.top/gtpphtoapq.html

#define X_H
来源：http://hz.ydzc1.top/gtjycdeohz.html

#endif
来源：http://hz.feifeiyinyue.top/gtqcbjuuul.html

[S31] C++：Hello World
来源：http://hz.andypj.xyz/gtsiangsqt.html

#include <iostream>
来源：http://hz.gzhubu.top/gtnvngxasp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gthzeoocgv.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtwbnljnqw.html

std::string s = "hi";  s += "!";
来源：http://hz.kuanghao11.cn/gttbmhqdxf.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gthqkxsvrg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtrvqykgzx.html

[S34] C++：遍历 vector
来源：http://hz.birdmap.top/gtxfkjevkv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenzaomai.com/gtqdxidwtk.html

[S35] C++：map
来源：http://hz.jqgufenzy.top/gtndwtpgbm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtwntmeyhn.html

[S36] C++：unordered_map
来源：http://hz.zhiwuduotai.top/gtfaihswcf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtyooyhydz.html

[S37] C++：set
来源：http://hz.hysaishi.cn/gtkbkmnxag.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.316326.xyz/gtwihezcyn.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtgioutezl.html

std::sort(v.begin(), v.end());
来源：http://hz.wangshuangyany.cn/gtntbkdppd.html

[S39] C++：自定义比较器排序
来源：http://hz.ybcxt.top/gtwmhprluz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtbcevfbrv.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtfwalmmmk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.bjfxy.top/gtpqnjogzf.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gtktbuhami.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sxryk.cn/gtklepyqkt.html

[S42] C++：继承与虚函数
来源：http://hz.zhongyouzk.top/gtjqhqqwbv.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gtrhoakjka.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtrlntiowo.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtpsboksyv.html

[S44] C++：引用传参
来源：http://hz.jyoumei.cn/gtopporgkr.html

void inc(int &x) { ++x; }
来源：http://hz.xinyue.icu/gtlambivze.html

[S45] C++：lambda
来源：http://hz.birdmap.top/gtgeykshri.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cashguo.top/gtrmgaqvzt.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtduunxymf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtqadrvgxe.html

[S47] C++：结构化绑定遍历
来源：http://hz.fengsongda.top/gtcxltjcki.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ydjk.org.cn/gtlrhtcxpu.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtaeymmcii.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aizwys.cn/gtgtrntizl.html

while (std::getline(in, line)) { }
来源：http://hz.0kj1m.cn/gtznfgqxhu.html

[S49] C++：写文件
来源：http://hz.shanyushiyangtech.top/gtlxqpwyig.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtygimldqd.html

[S50] C++：格式化数字
来源：http://hz.zhoulong.xyz/gtvfnvoimg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gtiqiaaapg.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gtygcrljbe.html

static_cast<double>(a) / b
来源：http://hz.zhixingplan.top/gtqbmmnfhi.html

[S52] C++：const 与 noexcept
来源：http://hz.hongshengwenyu.top/gtrwxuovnz.html

int size() const noexcept { return n_; }
来源：http://hz.mhx1999.top/gtmegcykrt.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtqagjvwxw.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtxrmcqvds.html

[S54] C++：异常处理
来源：http://hz.yj20258888.top/gtetqrfjap.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtgirlldsp.html

[S55] C++：结构化绑定
来源：http://hz.yj20258.top/gtefibbejp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xinyue.icu/gtonaeueyw.html

[S56] C++：optional
来源：http://hz.zdqjudy.top/gtvgtzxbzr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gotoacloud.top/gtfqtcgpzk.html

[S57] C++：编译期常量
来源：http://hz.sufxvd.cn/gtaqyysjdh.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtpueecmtp.html

[S58] C++：命名空间
来源：http://hz.fzhhl.top/gtvgmjgeog.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtswzvjfeg.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gtefjlsnqr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtecthkazb.html

[S60] C++：遍历并删除元素
来源：http://hz.chenzaomai.com/gtmtxersoy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gtpupncxvw.html

================================================================================
来源：http://hz.meibo888.top/gtysjhjqye.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtjgnstaih.html

================================================================================
来源：http://hz.zhongyouzk.top/gtgcqnmwjq.html

[T01] Kotlin：Hello World
来源：http://hz.feifeiyinyue.top/gtsqwltwys.html

println("Hello")
来源：http://hz.svipenyu.cn/gteqfxetwl.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtrwwnocmg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ivvv.top/gtljjdpmcs.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtgaypknrj.html

"值: $b"
来源：http://hz.cashguo.top/gtdpzcogya.html

[T04] Kotlin：空安全
来源：http://hz.sxryk.cn/gtvnuysnus.html

val n: String? = null;  n?.length
来源：http://hz.xylfe.cn/gtctqtmhcf.html

[T05] Kotlin：when 表达式
来源：http://hz.snrcjt.cn/gtfdabczko.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tian-w.cn/gtnofhjkkz.html

[T06] Kotlin：集合映射
来源：http://hz.ehwqpu.com/gtqfpxqetb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.vqdsnc.cn/gtwjfqjmre.html

[T07] Kotlin：集合过滤
来源：http://hz.jlsjyb.cn/gtvliferyj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zycfv.cn/gtrjzwjklw.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtfaqlkxci.html

data class User(val name: String, val age: Int)
来源：http://hz.pycfn.com/gtrujlenic.html

[T09] Kotlin：扩展函数
来源：http://hz.jinyuanbaomall.cn/gtdcddnftz.html

fun String.exclaim() = this + "!"
来源：http://hz.gotoacloud.top/gtjnlwopem.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangkeji.top/gtnqqoaisf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jianghu66.top/gtunnjuzpb.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtuxbcszvr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gtslgduiif.html

[T12] Kotlin：解构声明
来源：http://hz.hfpthk.cn/gtbfakmitr.html

val (a, b) = Pair(1, 2)
来源：http://hz.0kj1m.cn/gtmapyxkpe.html

[T13] Kotlin：只读 Map
来源：http://hz.svipenyu.cn/gtyyiqfzno.html

val m = mapOf("a" to 1)
来源：http://hz.gzhubu.top/gtxesvhrer.html

[T14] Kotlin：循环
来源：http://hz.zhongyouzk.top/gtcevejlva.html

for (i in 1..10) println(i)
来源：http://hz.andypj.xyz/gtlsapsfvk.html

[T15] Kotlin：接口
来源：http://hz.zhixingplan.top/gtmjgsiwme.html

interface Shape { fun area(): Double }
来源：http://hz.haohaochexian.top/gtyeapvenv.html

[T16] Swift：Hello World
来源：http://hz.sysykeji.top/gtxlndvveb.html

print("Hello")
来源：http://hz.xylfe.cn/gtmtkxhprr.html

[T17] Swift：变量与常量
来源：http://hz.hysaishi.cn/gtlyswmmps.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtamzuildz.html

[T18] Swift：字符串插值
来源：http://hz.chenzaomai.com/gtabwgongx.html

"值: \(b)"
来源：http://hz.cashguo.top/gtrwyshvux.html

[T19] Swift：可选绑定
来源：http://hz.ydzc1.top/gtzydorvwa.html

if let n = opt { print(n) }
来源：http://hz.xingfuxueyuan.xyz/gtguedwszo.html

[T20] Swift：数组操作
来源：http://hz.gzhubu.top/gtgnxlpqps.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yonumen.top/gtwnxhyhqy.html

[T21] Swift：遍历
来源：http://hz.sxryk.cn/gtvgllvzvr.html

for x in a { print(x) }
来源：http://hz.jqgfzy.top/gtvxlpixxp.html

[T22] Swift：字典
来源：http://hz.quarkkingdee.top/gtlrjlwjwm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tianlin.xyz/gtobothtfc.html

[T23] Swift：函数
来源：http://hz.zhengqikj.top/gtkutmyknb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtlqlslmoq.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtindciyso.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.haohaochexian.top/gtvwxvhwes.html

[T25] Swift：结构体
来源：http://hz.zhijiandao.cn/gtsczowrem.html

struct P { var x: Int }
来源：http://hz.kuanghao11.cn/gtsvphptav.html

[T26] Swift：类与重写
来源：http://hz.cashguo.top/gthphqqkdo.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangkeji.top/gttojrxrxv.html

[T27] Swift：错误处理
来源：http://hz.jinqigufen.top/gtcyqzujww.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangkeji.top/gtmedfdyfa.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gttbfdhvtl.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtsgdspcbd.html

[T29] Swift：guard 提前返回
来源：http://hz.hnqzz.top/gtitvquoaq.html

guard let x = opt else { return }
来源：http://hz.yj202588.top/gthizuxopv.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtpnebklnc.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtkoucoryx.html

[T31] Lua：Hello World
来源：http://hz.zhoulong.xyz/gtlsclfzxf.html

print("Hello")
来源：http://hz.daxiang520.top/gtaqwnibot.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtjkhvwvjc.html

local a = 1
来源：http://hz.ybcxt.top/gtkzisshzo.html

[T33] Lua：表（数组）
来源：http://hz.shzxlz.cn/gtytwkrbtx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.feifeiyinyue.top/gtiuiqzuyu.html

[T34] Lua：遍历表
来源：http://hz.dashuyun.cn/gtgtyfgsau.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sxryk.cn/gtodmtrsap.html

[T35] Lua：字典表
来源：http://hz.fzhhl.top/gtvbcqnhrf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtjxjmnfri.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtxsovqydi.html

function add(a, b) return a + b end
来源：http://hz.wangshuangyany.cn/gtbzvtlipq.html

[T37] Lua：字符串拼接
来源：http://hz.guowangkeji.top/gtelqfgvld.html

"a" .. "b"
来源：http://hz.jinqigufen.top/gtznifjkqf.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gtorxaunzk.html

if x > 0 then print("正") end
来源：http://hz.zhongyouzk.top/gthtdcdzfv.html

[T39] Lua：模式匹配
来源：http://hz.jiagoushi.top/gtvoetvspp.html

string.find(s, "%d+")
来源：http://hz.cdnleiting.top/gtbgnzybii.html

[T40] Lua：元表
来源：http://hz.wangdashe.top/gtqpsxyniq.html

setmetatable({}, { __index = base })
来源：http://hz.sweek.top/gtglwgdzga.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gtchgfwnpe.html

print "Hello\n";
来源：http://hz.zhixingplan.top/gtaoejuqfe.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gtylvjnshw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sufxvd.cn/gtbsxfhqbh.html

[T43] Perl：字符串插值
来源：http://hz.sweek.top/gtzectnugk.html

"值: $a"
来源：http://hz.yuxming.cn/gtddxwokvf.html

[T44] Perl：条件
来源：http://hz.cashguo.top/gtusqctiut.html

if ($a > 0) { print "正"; }
来源：http://hz.cheryme.top/gttegyegss.html

[T45] Perl：数组遍历
来源：http://hz.yueranfly.top/gtyjhmkngs.html

for my $x (@arr) { print $x; }
来源：http://hz.guannengcc.top/gtkimnstfv.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtdevugdqm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jiagoushi.top/gtyqgzklpy.html

[T47] Perl：正则捕获
来源：http://hz.yueranfly.top/gtncyutnxa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.316326.xyz/gtrjbxfznz.html

[T48] Perl：正则替换
来源：http://hz.pycfn.com/gtngpdhjmh.html

$s =~ s/old/new/g;
来源：http://hz.xingfuxueyuan.xyz/gtqpfktroa.html

[T49] Perl：函数
来源：http://hz.yuanzhike.top/gtsnyhfvpd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtctuxkqzg.html

[T50] Perl：逐行读文件
来源：http://hz.jiagoushi.top/gtucealxss.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xinyue.icu/gtwncxsodh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.guowangkeji.top/gtbsyjekir.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtzrehiwho.html

println("Hello")
来源：http://hz.dashuyun.cn/gtpmuxauhh.html

[T52] Scala：变量
来源：http://hz.chenjidiqi.icu/gthktwxihg.html

val a = 1;  var b = 2
来源：http://hz.guowangkeji.top/gtnknmwrxz.html

[T53] Scala：字符串插值
来源：http://hz.guannengcc.top/gthuryddxs.html

s"值: $b"
来源：http://hz.yj20258.top/gtflbgagiz.html

[T54] Scala：集合映射
来源：http://hz.kuanghao11.cn/gtikjnkohm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtkoopxtqd.html

[T55] Scala：集合过滤
来源：http://hz.shanyushiyangtech.top/gtgtiohhbs.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gtatrxsuvu.html

[T56] Scala：样例类
来源：http://hz.jianghu66.top/gttypfztzq.html

case class User(name: String, age: Int)
来源：http://hz.ehwqpu.com/gtamvlxwom.html

[T57] Scala：模式匹配
来源：http://hz.iojbl.cn/gtxoojkbhq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yongpay.top/gtyxymhurr.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gtafrkinek.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gteyqlpfli.html

[T59] Scala：循环
来源：http://hz.havefunace.top/gttuvpciye.html

for (i <- 1 to 10) println(i)
来源：http://hz.dianchejie.cn/gtbkzgtsne.html

[T60] Scala：折叠
来源：http://hz.zhaomingkeji.xyz/gtfbvvtfbn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xylfe.cn/gtxcfciewh.html

================================================================================
来源：http://hz.cqqwz.cn/gttsxokqjv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhixingplan.top/gtuqwgetwb.html

================================================================================
来源：http://hz.jinqigufen.top/gtegrtjrwn.html

[U01] Py：创建虚拟环境
来源：http://hz.9152youxi.cn/gtbkzadqbt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenzaomai.com/gtrupzjffs.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xziqi.cn/gtfccvbrun.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.feifeiyinyue.top/gtabmzsfim.html

[U03] Py：加载 .env 配置
来源：http://hz.xziqi.cn/gtaufvbruc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gtlscmemwk.html

[U04] Py：变量调试打印
来源：http://hz.aibaodan.cn/gtipumkadb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhixingplan.top/gtkdkefitq.html

[U05] Py：列表去重且保序
来源：http://hz.yuxming.cn/gtqeqljbbf.html

list(dict.fromkeys(arr))
来源：http://hz.aizwys.cn/gtxpuuentr.html

[U06] Py：合并两个字典
来源：http://hz.hysaishi.cn/gtpaicktnb.html

{**a, **b}
来源：http://hz.cheryme.top/gtyqwhplru.html


<!-- 参考信息 -->