代发 wailian999

df -h;  du -sh *
来源：http://hz.jqgufenzy.top/gtmeuxazlp.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtfwmctxdk.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtzgecvkdt.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtbqrifvrr.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtoesarfpu.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gtvqnywpxq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fzhhl.top/gtfdwhqcnm.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtuokefxmf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtvymkrhvf.html

[R66] 定时任务
来源：http://hz.xingfuxueyuan.xyz/gtemfcaxsy.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtrmsupriy.html

[R67] 生成随机十六进制串
来源：http://hz.yongpay.top/gteufyuosd.html

openssl rand -hex 16
来源：http://hz.xingfuxueyuan.xyz/gtbsoswtdf.html

[R68] 计算文件校验值
来源：http://hz.cashguo.top/gtyrvnurbr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sweek.top/gtfsujyuhl.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gtztszygzr.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtklexmpzi.html

[R70] 时间戳与互转
来源：http://hz.zhoulong.xyz/gtqtbmqzdw.html

date +%s;  date -d @1700000000
来源：http://hz.yj202588.top/gtoptnqcjj.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtnhebcvhb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xinyue.icu/gtcvfwjjjb.html

[R72] 等待端口就绪
来源：http://hz.zhoulong.xyz/gtkbofltgq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtfbrygmyq.html

[R73] 分割大日志
来源：http://hz.xingfuxueyuan.xyz/gtmzhlqvqy.html

split -l 1000 big.log part_
来源：http://hz.dashuyun.cn/gtckysuolv.html

[R74] 批量重命名
来源：http://hz.hysaishi.cn/gtsfuzlkyq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sweek.top/gtnlmqzspp.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtcbpvqnxh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sysykeji.top/gtaizsuuym.html

[R76] 使用临时文件
来源：http://hz.daria6918.cn/gteulbihpk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtouwcpbgj.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtjmxrwmoy.html

read -rp "请输入: " ans
来源：http://hz.316326.xyz/gtgvdixubk.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtlusvbsfm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guowangkeji.top/gtupdwvdru.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtqbmkqeat.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.wangshuangyany.cn/gtjmgkwusy.html

[R80] 查看脚本执行耗时
来源：http://hz.jyoumei.cn/gtdlwlvtst.html

time ./run.sh
来源：http://hz.havefunace.top/gtzbrotscc.html

================================================================================
来源：http://hz.zycfv.cn/gtiluzbljj.html

S. C / C++ 专题
来源：http://hz.dashuyun.cn/gtxqwkhahl.html

================================================================================
来源：http://hz.wangdashe.top/gtxgenpgdf.html

[S01] C：Hello World
来源：http://hz.sxryk.cn/gtdgrudrsx.html

#include <stdio.h>
来源：http://hz.chenzaomai.com/gtplfdbbse.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgufenzy.top/gtmpphahzj.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtbbfeuzkw.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gtrwjphmmp.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtluxxgmgc.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gtamaudqpe.html

[S04] C：字符串复制
来源：http://hz.xziqi.cn/gtbfcfdpjt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.iojbl.cn/gtjmresbla.html

[S05] C：字符串长度
来源：http://hz.chenlongwang.top/gtbhbpoesd.html

strlen(s)
来源：http://hz.0kj1m.cn/gtmclakxlt.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtgtqbnmjm.html

strcmp(a, b) == 0
来源：http://hz.chenjidiqi.icu/gtdrzywccr.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtlnbpipee.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jianghu66.top/gtsbgfbnjt.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gtuejdaupr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yanxiufei.cn/gtftixtuac.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gtnsrxjzgz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenlongwang.top/gtpydrthuq.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtvyxsifoi.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gtwxkypzca.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtxrtfudci.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtcksmjlow.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.birdmap.top/gtitmtpxcr.html

fclose(f);
来源：http://hz.pycfn.com/gtbayqxpye.html

[S12] C：写文件
来源：http://hz.xuanzx.com/gtynrhmvxe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.quarkkingdee.top/gtybzuwwsy.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtkoombeys.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj202588.top/gtonizfqbq.html

[S14] C：枚举
来源：http://hz.ywan-chungtsiang.top/gthggusogu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtllggszcu.html

[S15] C：类型转换
来源：http://hz.316326.xyz/gtpjqwqljo.html

(double) a / b
来源：http://hz.cashguo.top/gtwimbofhk.html

[S16] C：位操作置位
来源：http://hz.yangfankeji.com/gtbgflfmga.html

x |= (1 << 3);
来源：http://hz.ybcxt.top/gtqrmiipus.html

[S17] C：安全拼接字符串
来源：http://hz.chenjidiqi.icu/gtrbvonkuo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gthpmgglmw.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtwsehcuvy.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtbaqfmlux.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtliiwquyu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtelpmeklv.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtjbpcjqvf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daxiang520.top/gtmlhqeudr.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gthfyhaayz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.birdmap.top/gtbrvqcowa.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtzjybksoo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangtech.top/gthoygpqfm.html

[S23] C：随机数
来源：http://hz.ivvv.top/gttnwrfpvw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hywenlv.cn/gtfbltgqks.html

[S24] C：获取本地时间
来源：http://hz.sufxvd.cn/gtoktlpaga.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tianlin.xyz/gtlwkelmiz.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gtugjngujj.html

memcpy(dst, src, n);
来源：http://hz.quarkkingdee.top/gtxxmnkfno.html

[S26] C：内存清零
来源：http://hz.wangdashe.top/gtdyhtmufy.html

memset(a, 0, sizeof a);
来源：http://hz.dianchejie.cn/gtazpglqmm.html

[S27] C：定义常量
来源：http://hz.zhongyouzk.top/gtiexmedik.html

const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtqvdxvggv.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gtsgnifauw.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtmjpntvdx.html

[S29] C：变参函数
来源：http://hz.ydjk.org.cn/gtsvbwxiqw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtjmffmyiq.html

[S30] C：头文件保护
来源：http://hz.tian-w.cn/gtxufuawkf.html

#ifndef X_H
来源：http://hz.chenlongwang.top/gtxbijsxsy.html

#define X_H
来源：http://hz.cheryme.top/gtkbdrwsld.html

#endif
来源：http://hz.nwbrower.top/gtjlnyvrtw.html

[S31] C++：Hello World
来源：http://hz.zdqjudy.top/gtatyucyvw.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtvhcgllha.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.svipenyu.cn/gthtunvekh.html

[S32] C++：字符串
来源：http://hz.aizwys.cn/gtuhkoqtlh.html

std::string s = "hi";  s += "!";
来源：http://hz.xuetiantiany.cn/gtqoapplfz.html

[S33] C++：vector 增删
来源：http://hz.nanxinkj.top/gtmyimaxlu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhengqikj.top/gtrdgbclhn.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtebbmljum.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtpvxsixip.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtglvlztlm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtunmjjsvt.html

[S36] C++：unordered_map
来源：http://hz.feifeiyinyue.top/gttcfezlbn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtlayjnyef.html

[S37] C++：set
来源：http://hz.dashuyun.cn/gtyetkidfk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.316326.xyz/gtymcptkle.html

[S38] C++：排序
来源：http://hz.aibaodan.cn/gtpxpptxic.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gtpfarobxk.html

[S39] C++：自定义比较器排序
来源：http://hz.kuanghao11.cn/gtvtlqnddk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtpjlafeid.html

[S40] C++：查找元素
来源：http://hz.chenlongwang.top/gtlbvrongs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.bjfxy.top/gtwynjwekd.html

[S41] C++：类与构造函数
来源：http://hz.jyoumei.cn/gtkkeolady.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtovfgligu.html

[S42] C++：继承与虚函数
来源：http://hz.c1oappe.top/gtfovcprih.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gttlurouae.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gthmwcyakw.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgufenzy.top/gtvinkvwlg.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtwxfkjhyj.html

void inc(int &x) { ++x; }
来源：http://hz.aizwys.cn/gtllvirsmu.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gtbtlofyel.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gthcrveoki.html

[S46] C++：函数模板
来源：http://hz.tian-w.cn/gtcovnzsxg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtoaiaksqq.html

[S47] C++：结构化绑定遍历
来源：http://hz.redwolf501.top/gtyqioeost.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ehwqpu.com/gtrvvcfijy.html

[S48] C++：逐行读文件
来源：http://hz.nwbrower.top/gthwzhlavl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtxeesrbgk.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtycahwxbe.html

[S49] C++：写文件
来源：http://hz.jinqigufen.top/gtiomsiixv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yonumen.top/gtfzczytyv.html

[S50] C++：格式化数字
来源：http://hz.dianchejie.cn/gtgmapmhod.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.9152youxi.cn/gteesmypgs.html

[S51] C++：显式类型转换
来源：http://hz.dianchejie.cn/gtijxfvmkg.html

static_cast<double>(a) / b
来源：http://hz.hnqzz.top/gtycakmilj.html

[S52] C++：const 与 noexcept
来源：http://hz.shuidangran.top/gtkhhsitst.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtezchzzwk.html

[S53] C++：移动语义
来源：http://hz.jianghu66.top/gtuyvagkcu.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtsqqsvaek.html

[S54] C++：异常处理
来源：http://hz.yonumen.top/gtoeakvluc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenjidiqi.icu/gtkjaditnx.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtnwtzrojh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtqcfphlpp.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtteuehszu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtnbzyjbjl.html

[S57] C++：编译期常量
来源：http://hz.chenjidiqi.icu/gtjkcunxsz.html

constexpr int N = 10;
来源：http://hz.wangshuangyany.cn/gtzyoexbra.html

[S58] C++：命名空间
来源：http://hz.cashguo.top/gtgnrqxksq.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtizkirjob.html

[S59] C++：静态断言
来源：http://hz.cqqwz.cn/gtgjirsplc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxuanxn.top/gtdhgzjcxa.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtbgonvtdj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtqghrbxux.html

================================================================================
来源：http://hz.fengsongda.top/gthmtgrobr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aizwys.cn/gtkfzsyjpi.html

================================================================================
来源：http://hz.yonumen.top/gtybyohijn.html

[T01] Kotlin：Hello World
来源：http://hz.cqqwz.cn/gtjogwqspe.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtqejyzdyh.html

[T02] Kotlin：变量
来源：http://hz.jyoumei.cn/gtrzzvqoyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gzhubu.top/gtquhzseuf.html

[T03] Kotlin：字符串模板
来源：http://hz.sxryk.cn/gtgodxceux.html

"值: $b"
来源：http://hz.pycfn.com/gtujumccni.html

[T04] Kotlin：空安全
来源：http://hz.chenzaomai.com/gtwgoxntta.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtbxpmfikg.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gtzspyezwl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtuxumgxdt.html

[T06] Kotlin：集合映射
来源：http://hz.guowangkeji.top/gtpaophfik.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tanke756.top/gtoikheenh.html

[T07] Kotlin：集合过滤
来源：http://hz.daria6918.cn/gtngmpjxqc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtijthzovy.html

[T08] Kotlin：数据类
来源：http://hz.ywan-chungtsiang.top/gttwbqdket.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gtbxtbbylp.html

[T09] Kotlin：扩展函数
来源：http://hz.nwbrower.top/gtxcsksrmw.html

fun String.exclaim() = this + "!"
来源：http://hz.shuidangran.top/gtmqzummdt.html

[T10] Kotlin：默认参数
来源：http://hz.mhx1999.top/gthvhtuwyp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.birdmap.top/gtgjxdvcuw.html

[T11] Kotlin：协程
来源：http://hz.c1oappe.top/gttvkhvnuj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gtmddqcnhc.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigfzy.top/gtpesegimz.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtfcaylsmi.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtcgsmiqsy.html

val m = mapOf("a" to 1)
来源：http://hz.ppjwa.cn/gttnqodvpi.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtszulxqup.html

for (i in 1..10) println(i)
来源：http://hz.sysykeji.top/gtpfjhmuzm.html

[T15] Kotlin：接口
来源：http://hz.yvedp.cn/gtwxjwxran.html

interface Shape { fun area(): Double }
来源：http://hz.wangdashe.top/gtgjnwcetz.html

[T16] Swift：Hello World
来源：http://hz.hnqzz.top/gtyvohidzw.html

print("Hello")
来源：http://hz.yuxming.cn/gtxczzksxf.html

[T17] Swift：变量与常量
来源：http://hz.zhixingplan.top/gtzctexhhr.html

var a = 1;  let b = 2
来源：http://hz.aizwys.cn/gtbpasxhxq.html

[T18] Swift：字符串插值
来源：http://hz.birdmap.top/gtfrotkypk.html

"值: \(b)"
来源：http://hz.ybcxt.top/gtyxpuullr.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtwdiklzjo.html

if let n = opt { print(n) }
来源：http://hz.cqqwz.cn/gtzwhcxsso.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtxutgstum.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shangyingyoupin.top/gtbqerrwjj.html

[T21] Swift：遍历
来源：http://hz.cashguo.top/gtskatqdcj.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtqldmbidy.html

[T22] Swift：字典
来源：http://hz.yongpay.top/gtbzjxvjbj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gtxbhryaht.html

[T23] Swift：函数
来源：http://hz.jlsjyb.cn/gtxeegbmoy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.aizwys.cn/gtvcnwqctl.html

[T24] Swift：闭包
来源：http://hz.zhaomingkeji.xyz/gtwncghqtp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtgwlopghj.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtkkqvwusm.html

struct P { var x: Int }
来源：http://hz.zhoulong.xyz/gtiozigryh.html

[T26] Swift：类与重写
来源：http://hz.xziqi.cn/gtanpagmvk.html

class A: Base { override func f() {} }
来源：http://hz.zhaomingkeji.xyz/gtrzwbqqgy.html

[T27] Swift：错误处理
来源：http://hz.hysaishi.cn/gtgpvtwlxg.html

do { try f() } catch { print(error) }
来源：http://hz.cqqwz.cn/gtcgdgxewi.html

[T28] Swift：枚举
来源：http://hz.feifeiyinyue.top/gtogxrduhh.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gtpwftycie.html

[T29] Swift：guard 提前返回
来源：http://hz.gotoacloud.top/gttvrziymj.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtetmbxexd.html

[T30] Swift：协议
来源：http://hz.hnqzz.top/gtjxcrzocy.html

protocol Shape { func area() -> Double }
来源：http://hz.yongpay.top/gtdxkisjdu.html

[T31] Lua：Hello World
来源：http://hz.cucudq.cn/gtjwayeyen.html

print("Hello")
来源：http://hz.ydjk.org.cn/gtocaqrarb.html

[T32] Lua：局部变量
来源：http://hz.jqgufenzy.top/gtfdpsccqo.html

local a = 1
来源：http://hz.sxryk.cn/gtwbiwoxkl.html

[T33] Lua：表（数组）
来源：http://hz.hysaishi.cn/gtsnqdphqb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhijiandao.cn/gthfjqmgin.html

[T34] Lua：遍历表
来源：http://hz.hfpthk.cn/gtznxruvyg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.quarkkingdee.top/gtpwkyvfpy.html

[T35] Lua：字典表
来源：http://hz.redwolf501.top/gtqnqjtact.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtwkvaucok.html

[T36] Lua：函数
来源：http://hz.ydzc1.top/gtqgedolyy.html

function add(a, b) return a + b end
来源：http://hz.ppjwa.cn/gtpebfhiaz.html

[T37] Lua：字符串拼接
来源：http://hz.yuxming.cn/gttjzlypto.html

"a" .. "b"
来源：http://hz.0kj1m.cn/gtauimygdu.html

[T38] Lua：条件
来源：http://hz.fengsongda.top/gtrdaknaqp.html

if x > 0 then print("正") end
来源：http://hz.fzhhl.top/gtjthpuvpe.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangkeji.top/gtgqoaozgi.html

string.find(s, "%d+")
来源：http://hz.xingfuxueyuan.xyz/gtcrdioinr.html

[T40] Lua：元表
来源：http://hz.yanxiufei.cn/gtybhdrmba.html

setmetatable({}, { __index = base })
来源：http://hz.yanxiufei.cn/gtpciylqsz.html

[T41] Perl：Hello World
来源：http://hz.zhiwuduotai.top/gtgattdqbc.html

print "Hello\n";
来源：http://hz.quarkkingdee.top/gtkaaaxshe.html

[T42] Perl：变量类型
来源：http://hz.snrcjt.cn/gtttnjuquh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yonumen.top/gtwunrvmes.html

[T43] Perl：字符串插值
来源：http://hz.hywenlv.cn/gtmcdtfval.html

"值: $a"
来源：http://hz.smart0.xyz/gtashmcjxw.html

[T44] Perl：条件
来源：http://hz.sxryk.cn/gtnmfrqrcb.html

if ($a > 0) { print "正"; }
来源：http://hz.ydjk.org.cn/gtjufzuave.html

[T45] Perl：数组遍历
来源：http://hz.zhoulong.xyz/gteeaozcbu.html

for my $x (@arr) { print $x; }
来源：http://hz.gogol.net.cn/gtxkwhkfyz.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gtzorosbqu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yangfankeji.com/gtozqnvsss.html

[T47] Perl：正则捕获
来源：http://hz.redwolf501.top/gtpytnyngq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jiagoushi.top/gtdvhytrkz.html

[T48] Perl：正则替换
来源：http://hz.jlsjyb.cn/gtgcyeiqxz.html

$s =~ s/old/new/g;
来源：http://hz.nanxuanxn.top/gtozonkmdm.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gtjbqpybxn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zdqjudy.top/gthjvgsgnr.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtozrrpgdt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dashuyun.cn/gttvovrxlg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnxiangtu.top/gtsxuiuyeh.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtrokvsrsv.html

println("Hello")
来源：http://hz.smart0.xyz/gtbdscgnyp.html

[T52] Scala：变量
来源：http://hz.kuanghao11.cn/gtqcrcqbix.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangtech.top/gtrhzdgzwc.html

[T53] Scala：字符串插值
来源：http://hz.chenjidiqi.icu/gtzhgqxzsb.html

s"值: $b"
来源：http://hz.meibo888.top/gttjpyvhfk.html

[T54] Scala：集合映射
来源：http://hz.ywan-chungtsiang.top/gtfyxaibfg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtbsxeowgv.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gtwczbogog.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtgowfwnva.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtpkjkldew.html

case class User(name: String, age: Int)
来源：http://hz.yuxming.cn/gtoxbdzqgg.html

[T57] Scala：模式匹配
来源：http://hz.kuanghao11.cn/gthimqlymn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yuxming.cn/gtbpgifhdu.html

[T58] Scala：函数定义
来源：http://hz.hysaishi.cn/gtajeedpmq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.nanxuanxn.top/gtijgdnswh.html

[T59] Scala：循环
来源：http://hz.tian-w.cn/gtlofxbnha.html

for (i <- 1 to 10) println(i)
来源：http://hz.gotoacloud.top/gtvtuuamik.html

[T60] Scala：折叠
来源：http://hz.gzhubu.top/gtaazuzhve.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtqyvzewzx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtyoyvttnd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtdkrlymeh.html

================================================================================
来源：http://hz.xziqi.cn/gtpbqytzfl.html

[U01] Py：创建虚拟环境
来源：http://hz.hfpthk.cn/gtgbjargii.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gteofnrexj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pengpengdd.cyou/gthrerclro.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnqzz.top/gtowgpedde.html


<!-- 参考信息 -->