代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtmddgdocg.html

[R64] 结束进程
来源：http://hz.hnxiangtu.top/gtxywthbsj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtsxwlfykf.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gtpfmjfcia.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtouhklplz.html

[R66] 定时任务
来源：http://hz.jyoumei.cn/gtijtllmia.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtrtkyhopx.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gtakwmzylc.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtobnoemra.html

[R68] 计算文件校验值
来源：http://hz.haohaochexian.top/gtrlfkegoy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtldjnaxkc.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtljxugjgy.html

head -c 16 /dev/urandom | base64
来源：http://hz.cqqwz.cn/gtumocjhnn.html

[R70] 时间戳与互转
来源：http://hz.guowangkeji.top/gtvbfxnobo.html

date +%s;  date -d @1700000000
来源：http://hz.xingfuxueyuan.xyz/gtwcksspkz.html

[R71] 日期格式化
来源：http://hz.wangshuangyany.cn/gtonqlvmbr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxinkj.top/gtpnhnonmh.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtgtdjrqwq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangdashe.top/gtmgjvgwvs.html

[R73] 分割大日志
来源：http://hz.gogol.net.cn/gtvttjakps.html

split -l 1000 big.log part_
来源：http://hz.chenlongwang.top/gtyygwvxkf.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtanwgsomc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gtaefyzgnn.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtnrrshwid.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtvjkohaqn.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtcurnglle.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtdvuzkwbs.html

[R77] 读取用户输入
来源：http://hz.yongpay.top/gtvnpqsiyj.html

read -rp "请输入: " ans
来源：http://hz.xingfuxueyuan.xyz/gtvnqaoecm.html

[R78] 交互式菜单
来源：http://hz.zhijiandao.cn/gtwkoigzxi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gtndqmktge.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtvjrmjpnq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.svipenyu.cn/gtpnsairqj.html

[R80] 查看脚本执行耗时
来源：http://hz.jlsjyb.cn/gtegmtxzqf.html

time ./run.sh
来源：http://hz.tianlin.xyz/gtthizykhb.html

================================================================================
来源：http://hz.gzhubu.top/gtifzgwooi.html

S. C / C++ 专题
来源：http://hz.meibo888.top/gtjewuybwm.html

================================================================================
来源：http://hz.0kj1m.cn/gtfqnpugzu.html

[S01] C：Hello World
来源：http://hz.hammf.cn/gtzhhhdqrj.html

#include <stdio.h>
来源：http://hz.jinqigfzy.top/gtmjucytco.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shuidangran.top/gteeebuyya.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigfzy.top/gtgxbfsgso.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gtwugiflit.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtwhrctffi.html

int x; scanf("%d", &x);
来源：http://hz.gotoacloud.top/gtitpdwsap.html

[S04] C：字符串复制
来源：http://hz.haohaochexian.top/gtqjqgrgso.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtboojqpvr.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gtplkaxdyo.html

strlen(s)
来源：http://hz.zhijiandao.cn/gtyltkdvjg.html

[S06] C：字符串比较
来源：http://hz.chenlongwang.top/gtjsydyqds.html

strcmp(a, b) == 0
来源：http://hz.quarkkingdee.top/gtycllmntt.html

[S07] C：数组遍历求和
来源：http://hz.zhijiandao.cn/gtrlxwpixy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.redwolf501.top/gtdbasrtak.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtibhptztb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daria6918.cn/gttfotrxpt.html

[S09] C：结构体定义与初始化
来源：http://hz.wangshuangyany.cn/gticksedpd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangshuangyany.cn/gtagnqhbur.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtrydiulym.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtbkhymjpj.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtckugdrsr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtsmhgpofe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuanzhike.top/gttjwvtxzx.html

fclose(f);
来源：http://hz.redwolf501.top/gtciwhmorg.html

[S12] C：写文件
来源：http://hz.cashguo.top/gtdnvwocca.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtbzayspbh.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gtcdpgqjkz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cashguo.top/gthqzlbxvv.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtxxswaaji.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hfpthk.cn/gtdszvlmgz.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtkztqvuom.html

(double) a / b
来源：http://hz.mhx1999.top/gtgbcnpgfn.html

[S16] C：位操作置位
来源：http://hz.zdqjudy.top/gtqelvelzy.html

x |= (1 << 3);
来源：http://hz.jqgufenzy.top/gtfkiwybum.html

[S17] C：安全拼接字符串
来源：http://hz.shzxlz.cn/gtwzcbeosn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shuidangran.top/gteigshyop.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangtech.top/gtbplspfgb.html

int main(int argc, char **argv)
来源：http://hz.haohaochexian.top/gtadometdn.html

[S19] C：快速排序
来源：http://hz.daxiang520.top/gtymrhrxia.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtmuvuiadd.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gtuobtpavi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtbglspviz.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtditpjcra.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtdbtsmtye.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtxxpcidad.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinqigufen.top/gtbtassdrg.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtkgbsxvfj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xingfuxueyuan.xyz/gtmzuaiyyh.html

[S24] C：获取本地时间
来源：http://hz.kuanghao11.cn/gtfozekurn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgfzy.top/gtimfukfkl.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtibrsohgi.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtiuandcim.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gthmixlhyn.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gtaxsxgizc.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtpgmjevpb.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtcsjgiffm.html

[S28] C：静态变量
来源：http://hz.sysykeji.top/gtvmibmurt.html

static int counter = 0;
来源：http://hz.ppjwa.cn/gtinlpnnwb.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gtqiphyfmi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yongpay.top/gttfqgrudq.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangkeji.top/gtbvisvoov.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtwpqmikwt.html

#define X_H
来源：http://hz.xinyue.icu/gtyokwhous.html

#endif
来源：http://hz.guowangkeji.top/gtzwszusun.html

[S31] C++：Hello World
来源：http://hz.jinghuilouyu.cn/gtyczzynlb.html

#include <iostream>
来源：http://hz.aibaodan.cn/gtziqyqxci.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtbngefnna.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gtggfvehnd.html

std::string s = "hi";  s += "!";
来源：http://hz.fengsongda.top/gtydfffppg.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtjufunvid.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj202588.top/gtnnpklnea.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtredlotcw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnxiangtu.top/gttyzysttj.html

[S35] C++：map
来源：http://hz.guowangkeji.top/gtgjkuphct.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gthmkrulnp.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtyvjposdf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtxtnrrpfl.html

[S37] C++：set
来源：http://hz.chenlongwang.top/gtaphhcodl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.mhx1999.top/gtgqcxgrxq.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gtfqhhpcsj.html

std::sort(v.begin(), v.end());
来源：http://hz.hammf.cn/gtskgtcbyg.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtpefjhoqi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenzaomai.com/gtmdfymmlb.html

[S40] C++：查找元素
来源：http://hz.jyoumei.cn/gtanlutglv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtnoglokip.html

[S41] C++：类与构造函数
来源：http://hz.guannengcc.top/gtfkfrvqhz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.mhx1999.top/gtyvguhoog.html

[S42] C++：继承与虚函数
来源：http://hz.snrcjt.cn/gtcsirkiwd.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gthfatgacf.html

[S43] C++：智能指针
来源：http://hz.iojbl.cn/gtavunlpqs.html

auto p = std::make_unique<int>(5);
来源：http://hz.nwbrower.top/gthlqhpprd.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtqlygjbmz.html

void inc(int &x) { ++x; }
来源：http://hz.xuetiantiany.cn/gtojwglqlh.html

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gtmuhyxsat.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtsnsgonwy.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtcbvmdfqj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gtgxqdspzh.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtcfglcxzd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinyuanbaomall.cn/gtbvmdmgac.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtqkrhmppz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gtkjfmwbfl.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gttssbshxg.html

[S49] C++：写文件
来源：http://hz.smart0.xyz/gtbrouusjt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tianlin.xyz/gtdbsconfm.html

[S50] C++：格式化数字
来源：http://hz.jiagoushi.top/gtrkhzhwto.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258.top/gteviklmbc.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtwqouoqib.html

static_cast<double>(a) / b
来源：http://hz.yj20258.top/gtzvuwdyfs.html

[S52] C++：const 与 noexcept
来源：http://hz.chenjidiqi.icu/gtatvliauu.html

int size() const noexcept { return n_; }
来源：http://hz.pycfn.com/gttlskhwog.html

[S53] C++：移动语义
来源：http://hz.sufxvd.cn/gtehademwr.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtxcygrdnt.html

[S54] C++：异常处理
来源：http://hz.ywan-chungtsiang.top/gtmzqbcwkc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtalykzeua.html

[S55] C++：结构化绑定
来源：http://hz.52xcode.cn/gtfwrihfsr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtlbzywzxw.html

[S56] C++：optional
来源：http://hz.jlsjyb.cn/gtscanhygh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtyescahrx.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtgyjsybwx.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtapaeypxr.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtvxbgukfx.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtorvkldsy.html

[S59] C++：静态断言
来源：http://hz.yongpay.top/gtpgvlyunb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.bjfxy.top/gtpjoqlopk.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtsehovaba.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtlpfiujae.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxnitcmgw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtrzptrseh.html

================================================================================
来源：http://hz.havefunace.top/gtvibpngiw.html

[T01] Kotlin：Hello World
来源：http://hz.aizwys.cn/gtqssrnymm.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtzmtkfrrm.html

[T02] Kotlin：变量
来源：http://hz.ydzc1.top/gtriybwisq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ehwqpu.com/gtgwbmqjic.html

[T03] Kotlin：字符串模板
来源：http://hz.yueranfly.top/gtmhhdelwn.html

"值: $b"
来源：http://hz.aibaodan.cn/gtirrjvugh.html

[T04] Kotlin：空安全
来源：http://hz.smart0.xyz/gtkwqygnkh.html

val n: String? = null;  n?.length
来源：http://hz.havefunace.top/gtyrimtmrp.html

[T05] Kotlin：when 表达式
来源：http://hz.zhiwuduotai.top/gturajyhjy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.vqdsnc.cn/gteypfximz.html

[T06] Kotlin：集合映射
来源：http://hz.kuanghao11.cn/gtphxeufno.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hfpthk.cn/gtzdfisjvc.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigfzy.top/gtrbvgyxha.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtjsoakrbt.html

[T08] Kotlin：数据类
来源：http://hz.zdqjudy.top/gtcmcqwpzi.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtorwzrplo.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxuanxn.top/gteqnadqbr.html

fun String.exclaim() = this + "!"
来源：http://hz.vqdsnc.cn/gthlxrpduf.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gtvujnlhps.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtrqmtndeg.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtihxcreao.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtvpysalgm.html

[T12] Kotlin：解构声明
来源：http://hz.0kj1m.cn/gtmxnsbdaa.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtkxreuyqs.html

[T13] Kotlin：只读 Map
来源：http://hz.wangshuangyany.cn/gthntgwsau.html

val m = mapOf("a" to 1)
来源：http://hz.sweek.top/gtqxxqgslr.html

[T14] Kotlin：循环
来源：http://hz.smart0.xyz/gtuuyemeaf.html

for (i in 1..10) println(i)
来源：http://hz.daxiang520.top/gtywjgfqba.html

[T15] Kotlin：接口
来源：http://hz.hnxiangtu.top/gtqpdekahi.html

interface Shape { fun area(): Double }
来源：http://hz.hywenlv.cn/gtaymfwrvd.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gtugqxnzfv.html

print("Hello")
来源：http://hz.zhengqikj.top/gtyfkahyxx.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gttwtlcvfg.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtlfskqmpg.html

[T18] Swift：字符串插值
来源：http://hz.jlsjyb.cn/gtzsaefvwo.html

"值: \(b)"
来源：http://hz.9152youxi.cn/gtsmhqhkfg.html

[T19] Swift：可选绑定
来源：http://hz.shangyingyoupin.top/gtyrrdeakl.html

if let n = opt { print(n) }
来源：http://hz.ydzc1.top/gtcczophpb.html

[T20] Swift：数组操作
来源：http://hz.zhoulong.xyz/gtadqcorsv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dashuyun.cn/gtfkisykmr.html

[T21] Swift：遍历
来源：http://hz.pengpengdd.cyou/gtolbtzkyo.html

for x in a { print(x) }
来源：http://hz.xinyue.icu/gtigugzfmt.html

[T22] Swift：字典
来源：http://hz.zhiwuduotai.top/gtdbthetzb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tian-w.cn/gtaqbaiudy.html

[T23] Swift：函数
来源：http://hz.ehwqpu.com/gtpfhxevxw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtvwlwubry.html

[T24] Swift：闭包
来源：http://hz.yj202588.top/gtizltdevd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtnxlbhcef.html

[T25] Swift：结构体
来源：http://hz.andypj.xyz/gtawhczxvg.html

struct P { var x: Int }
来源：http://hz.pycfn.com/gtgntionrp.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtjzhjzpdt.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtzsmnpevs.html

[T27] Swift：错误处理
来源：http://hz.xuanzx.com/gtxvnjypju.html

do { try f() } catch { print(error) }
来源：http://hz.haohaochexian.top/gtrdtzcgza.html

[T28] Swift：枚举
来源：http://hz.hywenlv.cn/gtatlfuifp.html

enum Color { case red, green }
来源：http://hz.chenlongwang.top/gtdfzjwtng.html

[T29] Swift：guard 提前返回
来源：http://hz.ybcxt.top/gtigsuwkoo.html

guard let x = opt else { return }
来源：http://hz.ppjwa.cn/gtqsiubdgl.html

[T30] Swift：协议
来源：http://hz.ydjk.org.cn/gtgjazqazo.html

protocol Shape { func area() -> Double }
来源：http://hz.shangyingyoupin.top/gtqqzlxirv.html

[T31] Lua：Hello World
来源：http://hz.bjfxy.top/gtepooocms.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtrwqlovwf.html

[T32] Lua：局部变量
来源：http://hz.yj20258888.top/gtemohrxhz.html

local a = 1
来源：http://hz.sufxvd.cn/gtgypudkmv.html

[T33] Lua：表（数组）
来源：http://hz.ydzc1.top/gtymuaswgk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ybcxt.top/gtybptlthe.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtcfswxhbp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgfzy.top/gtppmczoit.html

[T35] Lua：字典表
来源：http://hz.c1oappe.top/gtkswanhbw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258888.top/gtwfsvggha.html

[T36] Lua：函数
来源：http://hz.dianchejie.cn/gtreillowp.html

function add(a, b) return a + b end
来源：http://hz.jinyuanbaomall.cn/gtlviznqpm.html

[T37] Lua：字符串拼接
来源：http://hz.jqgufenzy.top/gtkuchmzcf.html

"a" .. "b"
来源：http://hz.c1oappe.top/gtlgoqloss.html

[T38] Lua：条件
来源：http://hz.zhoulong.xyz/gtfapncrzz.html

if x > 0 then print("正") end
来源：http://hz.jqgfzy.top/gtrwinpuwj.html

[T39] Lua：模式匹配
来源：http://hz.jinqigufen.top/gtkykkpfau.html

string.find(s, "%d+")
来源：http://hz.iojbl.cn/gtbsopirrr.html

[T40] Lua：元表
来源：http://hz.nwbrower.top/gtsbnadebt.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtpiutslee.html

[T41] Perl：Hello World
来源：http://hz.hywenlv.cn/gtspygtrie.html

print "Hello\n";
来源：http://hz.sweek.top/gtlbborkyc.html

[T42] Perl：变量类型
来源：http://hz.guowangkeji.top/gtnfydtmjl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.meibo888.top/gtcxwbmypl.html

[T43] Perl：字符串插值
来源：http://hz.fzhhl.top/gtiyoamqja.html

"值: $a"
来源：http://hz.smart0.xyz/gtdnwrottb.html

[T44] Perl：条件
来源：http://hz.chenzaomai.com/gtkxjhejjg.html

if ($a > 0) { print "正"; }
来源：http://hz.jyoumei.cn/gtwvmgnzly.html

[T45] Perl：数组遍历
来源：http://hz.chenzaomai.com/gtdxekwhtf.html

for my $x (@arr) { print $x; }
来源：http://hz.wangdashe.top/gtbogoqghz.html

[T46] Perl：哈希操作
来源：http://hz.zhiwuduotai.top/gtvuuendlu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258.top/gtmfvmopjl.html

[T47] Perl：正则捕获
来源：http://hz.cheryme.top/gtkbzmwywm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sufxvd.cn/gtrzanozsq.html

[T48] Perl：正则替换
来源：http://hz.ehwqpu.com/gtoujkyphn.html

$s =~ s/old/new/g;
来源：http://hz.cucudq.cn/gtabpbvcqj.html

[T49] Perl：函数
来源：http://hz.iojbl.cn/gtqnbrtzhu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tianlin.xyz/gtmqxfefan.html

[T50] Perl：逐行读文件
来源：http://hz.tianlin.xyz/gtypvlbznp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sufxvd.cn/gtzkhoonya.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtusmjgmbn.html

[T51] Scala：Hello World
来源：http://hz.mhx1999.top/gtevjerdbj.html

println("Hello")
来源：http://hz.ydzc1.top/gtphqjuxxi.html

[T52] Scala：变量
来源：http://hz.yj20258888.top/gtctitzzmg.html

val a = 1;  var b = 2
来源：http://hz.shzxlz.cn/gtvpmhhajm.html

[T53] Scala：字符串插值
来源：http://hz.xinyue.icu/gtveaztnat.html

s"值: $b"
来源：http://hz.snrcjt.cn/gtjuizontg.html

[T54] Scala：集合映射
来源：http://hz.tanke756.top/gtowppgdlw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ivvv.top/gtlzzlykfp.html

[T55] Scala：集合过滤
来源：http://hz.daria6918.cn/gtasybhjyj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.guowangkeji.top/gtgklhlexv.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtporzqelv.html

case class User(name: String, age: Int)
来源：http://hz.dashuyun.cn/gtagoapsgg.html

[T57] Scala：模式匹配
来源：http://hz.jinghuilouyu.cn/gtkaqkzhnv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daxiang520.top/gtibyikzgm.html

[T58] Scala：函数定义
来源：http://hz.ydjk.org.cn/gtvnblfywm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hnqzz.top/gthkjrklaj.html

[T59] Scala：循环
来源：http://hz.iojbl.cn/gtsidxndey.html

for (i <- 1 to 10) println(i)
来源：http://hz.zdqjudy.top/gtozgkwfig.html

[T60] Scala：折叠
来源：http://hz.zhixingplan.top/gtccelnqnm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtqfdpsyxo.html

================================================================================
来源：http://hz.hywenlv.cn/gthdqkmuuq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.snrcjt.cn/gtctencaql.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtydmfgjuw.html

[U01] Py：创建虚拟环境
来源：http://hz.pycfn.com/gtfgjwjtsg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xziqi.cn/gtieykjets.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhongyouzk.top/gtasuwuqrz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhongyouzk.top/gtayxhcybg.html

[U03] Py：加载 .env 配置
来源：http://hz.quarkkingdee.top/gtotfprdif.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xingfuxueyuan.xyz/gtjxzmzwfo.html

[U04] Py：变量调试打印
来源：http://hz.quarkkingdee.top/gtnkfnlblb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhongyouzk.top/gtqgxjhojx.html


<!-- 参考信息 -->