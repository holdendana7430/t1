代发 wailian999

df -h;  du -sh *
来源：http://hz.gogol.net.cn/gthdxxudmy.html

[R62] 找最占空间的文件
来源：http://hz.xylfe.cn/gtpofwubul.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxuanxn.top/gtqqsfhlix.html

[R63] 内存与进程
来源：http://hz.nanxuanxn.top/gttpsryvkw.html

free -h;  ps aux | grep nginx
来源：http://hz.cucudq.cn/gthsyymkou.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtaeqdoetr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jianghu66.top/gtjiiualtt.html

[R65] 查看端口占用
来源：http://hz.9152youxi.cn/gtlezppnvs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtqjdxrdjj.html

[R66] 定时任务
来源：http://hz.haohaochexian.top/gtucetytim.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtntfkvwqb.html

[R67] 生成随机十六进制串
来源：http://hz.zhijiandao.cn/gtwsjqsocu.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtxpebqheo.html

[R68] 计算文件校验值
来源：http://hz.daxiang520.top/gtugrumjus.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenzaomai.com/gtaxpxxmcs.html

[R69] 生成随机密码
来源：http://hz.jianghu66.top/gtuhtatjtd.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gtjhbtmhcv.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtczwumnwa.html

date +%s;  date -d @1700000000
来源：http://hz.sufxvd.cn/gtiklsdvqo.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gttzhndqbf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aibaodan.cn/gtrqsyatii.html

[R72] 等待端口就绪
来源：http://hz.shuidangran.top/gtpjlriyle.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangdashe.top/gtvkjuynha.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gtpxuttxjd.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gtylcjlqwe.html

[R74] 批量重命名
来源：http://hz.316326.xyz/gtfdcgtgaq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daxiang520.top/gtajmjvile.html

[R75] 导出环境变量
来源：http://hz.ydzc1.top/gtgwczdndz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ywan-chungtsiang.top/gtjivkqhhg.html

[R76] 使用临时文件
来源：http://hz.yuxming.cn/gtvqizomco.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtwykdumww.html

[R77] 读取用户输入
来源：http://hz.haohaochexian.top/gtsvypjwkb.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gtzzvpimmm.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtjqvgqnle.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gthosrnfkb.html

[R79] 解析命令行选项
来源：http://hz.xingfuxueyuan.xyz/gttnsuuwga.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuanzx.com/gtivszvtlg.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgfzy.top/gtasoxduwt.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtaufjdosg.html

================================================================================
来源：http://hz.zdqjudy.top/gtvmjaqfro.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gthfiscjin.html

================================================================================
来源：http://hz.yj20258.top/gtbmbkffom.html

[S01] C：Hello World
来源：http://hz.dashuyun.cn/gthlprrcfr.html

#include <stdio.h>
来源：http://hz.svipenyu.cn/gtnmydncst.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gtpyepcvuu.html

[S02] C：变量与格式化输出
来源：http://hz.jinyuanbaomall.cn/gtwwbjmktm.html

int a = 10; printf("%d\n", a);
来源：http://hz.meibo888.top/gtcjmqqilo.html

[S03] C：读入整数
来源：http://hz.c1oappe.top/gtffehkohu.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gtoxmpijaz.html

[S04] C：字符串复制
来源：http://hz.zhaomingkeji.xyz/gtgoxfdexb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.9152youxi.cn/gtkovvuspr.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtzlcrcuil.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtxqrihwpe.html

[S06] C：字符串比较
来源：http://hz.aizwys.cn/gtzcturkgi.html

strcmp(a, b) == 0
来源：http://hz.zhixingplan.top/gtaaornzbs.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtsbzejukd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258888.top/gtggjtqrvz.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtohxvnycd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guowangkeji.top/gtkmsqduys.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gtmhpimmnm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhiwuduotai.top/gthxizayrg.html

[S10] C：指针与解引用
来源：http://hz.zhaomingkeji.xyz/gttzyfjtrq.html

int *p = &a;  *p = 5;
来源：http://hz.guannengcc.top/gtfkjmzwds.html

[S11] C：逐行读文件
来源：http://hz.jianghu66.top/gtamdrcuio.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gttcapnmph.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtrmptakwy.html

fclose(f);
来源：http://hz.xylfe.cn/gtqhrriujt.html

[S12] C：写文件
来源：http://hz.chenjidiqi.icu/gtwqbffqmu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cdnleiting.top/gtyuersyff.html

[S13] C：宏定义
来源：http://hz.svipenyu.cn/gtuppsigyv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gttaizkkyw.html

[S14] C：枚举
来源：http://hz.chenjidiqi.icu/gtplwpahmj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gttfzubcfj.html

[S15] C：类型转换
来源：http://hz.xuetiantiany.cn/gtqwjhabhb.html

(double) a / b
来源：http://hz.gotoacloud.top/gtgrvnnlfq.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtwjkvzfcf.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtmqknboov.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtflgrawdd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.andypj.xyz/gtcuczhooc.html

[S18] C：命令行参数
来源：http://hz.hysaishi.cn/gtrrqfcqve.html

int main(int argc, char **argv)
来源：http://hz.hongshengwenyu.top/gtdwsilqoi.html

[S19] C：快速排序
来源：http://hz.xinyue.icu/gtjihzeiqp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtoekodpru.html

[S20] C：二分查找
来源：http://hz.feifeiyinyue.top/gtfocqvtvn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtwwvbvbga.html

[S21] C：字符类别判断
来源：http://hz.guannengcc.top/gtjbzgdmhj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj202588.top/gtgbtaeukk.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtgkdfuvqo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtcdyhpqlx.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtpsytoadq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigufen.top/gtcwpcjejh.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtbrxhnocp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zdqjudy.top/gtljlczyuv.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtaahumpuf.html

memcpy(dst, src, n);
来源：http://hz.daria6918.cn/gtpngtacye.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtkekxonxq.html

memset(a, 0, sizeof a);
来源：http://hz.yanxiufei.cn/gtwkcaoibo.html

[S27] C：定义常量
来源：http://hz.nanxinkj.top/gtihkxmvon.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtabutpcmt.html

[S28] C：静态变量
来源：http://hz.fengsongda.top/gtbviecspu.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtczpwjhvz.html

[S29] C：变参函数
来源：http://hz.tanke756.top/gtypnidwdi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.iojbl.cn/gtpblxskxq.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtqmeoscpm.html

#ifndef X_H
来源：http://hz.fengsongda.top/gtmvjzlzxj.html

#define X_H
来源：http://hz.zhoulong.xyz/gtthisutlb.html

#endif
来源：http://hz.xuanzx.com/gtqwmxljfk.html

[S31] C++：Hello World
来源：http://hz.gzhubu.top/gtyjrqfqft.html

#include <iostream>
来源：http://hz.wangshuangyany.cn/gteiteppst.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuxming.cn/gtftihiovf.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtbjfvqdjc.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtlhonchqn.html

[S33] C++：vector 增删
来源：http://hz.tianlin.xyz/gtwxvtgioz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigfzy.top/gtppnmqzue.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtvykmbkwj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258888.top/gtiuwdjnuv.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtradipvqb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtpchhfmup.html

[S36] C++：unordered_map
来源：http://hz.xinyue.icu/gtlckofhlt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtjlpwiizb.html

[S37] C++：set
来源：http://hz.zhixingplan.top/gtpqspqncm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gtaylvchhx.html

[S38] C++：排序
来源：http://hz.iojbl.cn/gtxmlufxoe.html

std::sort(v.begin(), v.end());
来源：http://hz.zycfv.cn/gtwvxchkqi.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gtcciibrge.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenjidiqi.icu/gtoljzvblr.html

[S40] C++：查找元素
来源：http://hz.hywenlv.cn/gtqellqpra.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cheryme.top/gtjpzsxfnx.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtbieglozw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shangyingyoupin.top/gtscxbvikf.html

[S42] C++：继承与虚函数
来源：http://hz.shzxlz.cn/gtsvaowppy.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtlzixkzgf.html

[S43] C++：智能指针
来源：http://hz.daria6918.cn/gtgjfwathr.html

auto p = std::make_unique<int>(5);
来源：http://hz.smart0.xyz/gtqmpuvhyz.html

[S44] C++：引用传参
来源：http://hz.tianlin.xyz/gtxodngoqo.html

void inc(int &x) { ++x; }
来源：http://hz.birdmap.top/gtftxstdei.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gteqvckzgi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhijiandao.cn/gtdkxqzazw.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtvraxbyvm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtlyrwymik.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtzzeeoidq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.vqdsnc.cn/gteaoevvef.html

[S48] C++：逐行读文件
来源：http://hz.zdqjudy.top/gtrhfctxhr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gtefnentrz.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtxcgjqkcl.html

[S49] C++：写文件
来源：http://hz.pengpengdd.cyou/gtpxpydgje.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nwbrower.top/gtflhgteil.html

[S50] C++：格式化数字
来源：http://hz.cqqwz.cn/gtnamgsjfw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cucudq.cn/gtaolkikoj.html

[S51] C++：显式类型转换
来源：http://hz.gotoacloud.top/gtclalnlyn.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gtotzxslwg.html

[S52] C++：const 与 noexcept
来源：http://hz.vqdsnc.cn/gtpkmdbdwz.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtmsecrfkc.html

[S53] C++：移动语义
来源：http://hz.9152youxi.cn/gtrdewjafz.html

std::vector<int> w = std::move(v);
来源：http://hz.redwolf501.top/gtikgdsojz.html

[S54] C++：异常处理
来源：http://hz.dashuyun.cn/gtgmnslbgg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtxeqlgeuj.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangkeji.top/gtpmpboowi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dianchejie.cn/gtkqfvtgsa.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gthqinsmnr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhiwuduotai.top/gtrojregkb.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtzurumbpx.html

constexpr int N = 10;
来源：http://hz.jinyuanbaomall.cn/gtzdvmutdb.html

[S58] C++：命名空间
来源：http://hz.chenzaomai.com/gtgvpskdmf.html

namespace ns { int f() { return 1; } }
来源：http://hz.ppjwa.cn/gtoljeqibv.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtnbriyqax.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hywenlv.cn/gtqlchalis.html

[S60] C++：遍历并删除元素
来源：http://hz.daria6918.cn/gtzfdvxmjp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shuidangran.top/gtdsiwrsbz.html

================================================================================
来源：http://hz.yangfankeji.com/gtybuwhxan.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtyzxmglbv.html

================================================================================
来源：http://hz.guannengcc.top/gtafxwuery.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtcqujcllg.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtotgchirb.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtpciwdldg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhixingplan.top/gtgdnoisjn.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtdqyakjfn.html

"值: $b"
来源：http://hz.c1oappe.top/gtkhkagqhv.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtblagspjw.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtrliagxfq.html

[T05] Kotlin：when 表达式
来源：http://hz.xuanzx.com/gtwbjxadam.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtyhrqqvpo.html

[T06] Kotlin：集合映射
来源：http://hz.yj202588.top/gtojltuapz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cqqwz.cn/gtdfahvigr.html

[T07] Kotlin：集合过滤
来源：http://hz.ydjk.org.cn/gtaalhborl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sysykeji.top/gtulrfbsxp.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtqrnaeatp.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangkeji.top/gttzlkxpbb.html

[T09] Kotlin：扩展函数
来源：http://hz.haohaochexian.top/gthaqsyufc.html

fun String.exclaim() = this + "!"
来源：http://hz.yanxiufei.cn/gtrbschxbw.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gtyqxxobiy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtxhdwtcbt.html

[T11] Kotlin：协程
来源：http://hz.hnxiangtu.top/gtyodjnpqr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gturbgbtng.html

[T12] Kotlin：解构声明
来源：http://hz.feifeiyinyue.top/gtogdvvarn.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gthyfzsnmj.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtmddotpro.html

val m = mapOf("a" to 1)
来源：http://hz.sweek.top/gtqogvxpam.html

[T14] Kotlin：循环
来源：http://hz.gotoacloud.top/gtinxzlegy.html

for (i in 1..10) println(i)
来源：http://hz.jiagoushi.top/gteaybnukx.html

[T15] Kotlin：接口
来源：http://hz.aibaodan.cn/gtxenraoaq.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gttnqssols.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gttnsgkbmd.html

print("Hello")
来源：http://hz.hammf.cn/gtdsngyesr.html

[T17] Swift：变量与常量
来源：http://hz.gaohongyu789.top/gtecoqpuua.html

var a = 1;  let b = 2
来源：http://hz.sysykeji.top/gtoocgnfph.html

[T18] Swift：字符串插值
来源：http://hz.xylfe.cn/gtgaasvuwc.html

"值: \(b)"
来源：http://hz.hnxiangtu.top/gtlihmncxo.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtuoamiahb.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtehcitzln.html

[T20] Swift：数组操作
来源：http://hz.cqqwz.cn/gtbqcpvwuz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pycfn.com/gtaugsyceo.html

[T21] Swift：遍历
来源：http://hz.yuanzhike.top/gtztlttoxr.html

for x in a { print(x) }
来源：http://hz.ydzc1.top/gtpvsdhtur.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtwwuwgbmv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.smart0.xyz/gtynqrsbzu.html

[T23] Swift：函数
来源：http://hz.zycfv.cn/gtfgujjxuw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangtech.top/gtgbecjvgv.html

[T24] Swift：闭包
来源：http://hz.jinqigfzy.top/gtbtmbbhyv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cheryme.top/gtjzwxlcec.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtsoqzmvjc.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtgvopmwdv.html

[T26] Swift：类与重写
来源：http://hz.zhaomingkeji.xyz/gtdldnmndc.html

class A: Base { override func f() {} }
来源：http://hz.hywenlv.cn/gtsvzmehgx.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtnlfgoygr.html

do { try f() } catch { print(error) }
来源：http://hz.guannengcc.top/gtyjsdzvgj.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtycvxrryb.html

enum Color { case red, green }
来源：http://hz.gaohongyu789.top/gtdzxkmxzp.html

[T29] Swift：guard 提前返回
来源：http://hz.0kj1m.cn/gtxvbzgagv.html

guard let x = opt else { return }
来源：http://hz.pengpengdd.cyou/gtwhmeioje.html

[T30] Swift：协议
来源：http://hz.meibo888.top/gtfvhzjvxi.html

protocol Shape { func area() -> Double }
来源：http://hz.chenjidiqi.icu/gtwfiyrcla.html

[T31] Lua：Hello World
来源：http://hz.ivvv.top/gtletctcxa.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtentysqvl.html

[T32] Lua：局部变量
来源：http://hz.guowangkeji.top/gtjnilrepo.html

local a = 1
来源：http://hz.hywenlv.cn/gtqrmkwpfb.html

[T33] Lua：表（数组）
来源：http://hz.c1oappe.top/gtjcpcrbtc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydzc1.top/gtcbavgeux.html

[T34] Lua：遍历表
来源：http://hz.nanxuanxn.top/gtpeuzzyjd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.smart0.xyz/gtqgrlfsoo.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gthioldmna.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258.top/gtwrqqsaqb.html

[T36] Lua：函数
来源：http://hz.guowangkeji.top/gtjmcyxwdd.html

function add(a, b) return a + b end
来源：http://hz.dashuyun.cn/gtazkexctb.html

[T37] Lua：字符串拼接
来源：http://hz.sweek.top/gtnamjszwk.html

"a" .. "b"
来源：http://hz.fzhhl.top/gtknnriahj.html

[T38] Lua：条件
来源：http://hz.jyoumei.cn/gtgvcveufo.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gtsefygmsj.html

[T39] Lua：模式匹配
来源：http://hz.jinqigfzy.top/gtfrcsnrvk.html

string.find(s, "%d+")
来源：http://hz.daxiang520.top/gtjmhpqxfa.html

[T40] Lua：元表
来源：http://hz.hongshengwenyu.top/gtepucynuo.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtrjqbphxq.html

[T41] Perl：Hello World
来源：http://hz.sufxvd.cn/gtzvarjfqh.html

print "Hello\n";
来源：http://hz.zdqjudy.top/gtdakbcrbp.html

[T42] Perl：变量类型
来源：http://hz.dashuyun.cn/gtvahzyczk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yuanzhike.top/gttyhgihwl.html

[T43] Perl：字符串插值
来源：http://hz.yueranfly.top/gtfmijbsqm.html

"值: $a"
来源：http://hz.chenzaomai.com/gtjershtls.html

[T44] Perl：条件
来源：http://hz.nwbrower.top/gtrwhgzwfn.html

if ($a > 0) { print "正"; }
来源：http://hz.havefunace.top/gtxuxousik.html

[T45] Perl：数组遍历
来源：http://hz.feifeiyinyue.top/gtvcctlvxe.html

for my $x (@arr) { print $x; }
来源：http://hz.9152youxi.cn/gtveciygms.html

[T46] Perl：哈希操作
来源：http://hz.hammf.cn/gtnyuearvo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtsksofnjt.html

[T47] Perl：正则捕获
来源：http://hz.52xcode.cn/gtiwxynupa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.meibo888.top/gtwsdkuqqq.html

[T48] Perl：正则替换
来源：http://hz.gotoacloud.top/gtadshcniw.html

$s =~ s/old/new/g;
来源：http://hz.zhoulong.xyz/gtugebdfgg.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtuysirtlg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigufen.top/gtlrwmnbxb.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigufen.top/gttugbkjvf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.haohaochexian.top/gtwoilewhb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtjricfumk.html

[T51] Scala：Hello World
来源：http://hz.redwolf501.top/gtlfbmnjbw.html

println("Hello")
来源：http://hz.guowangkeji.top/gtoiqbsxfs.html

[T52] Scala：变量
来源：http://hz.nanxuanxn.top/gtoldcrazx.html

val a = 1;  var b = 2
来源：http://hz.jinyuanbaomall.cn/gtuqwqmnpk.html

[T53] Scala：字符串插值
来源：http://hz.daxiang520.top/gtrokmyrxy.html

s"值: $b"
来源：http://hz.xuetiantiany.cn/gtxqsgmpmd.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtrwzxflcc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sysykeji.top/gtvjspgsbd.html

[T55] Scala：集合过滤
来源：http://hz.jinghuilouyu.cn/gtxzswwywe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tian-w.cn/gthmcfchwx.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gthixwmknl.html

case class User(name: String, age: Int)
来源：http://hz.hammf.cn/gtzrmolozx.html

[T57] Scala：模式匹配
来源：http://hz.wangdashe.top/gteigfosew.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhongyouzk.top/gtimcepjqc.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gthqorhiia.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gogol.net.cn/gttrkqibdp.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtqkdkadnc.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gtcjndpylh.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gtkudbofap.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhijiandao.cn/gtmfanbsth.html

================================================================================
来源：http://hz.shzxlz.cn/gtzhfskoyz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtucgmpicf.html

================================================================================
来源：http://hz.guowangkeji.top/gtqhkhewtn.html

[U01] Py：创建虚拟环境
来源：http://hz.0kj1m.cn/gtjdcknghw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.dashuyun.cn/gtabtdpong.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258888.top/gtzhltxhfi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xuetiantiany.cn/gttasxpkll.html


<!-- 参考信息 -->