代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gtuqdrzcev.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtyiyrtjoz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtcfkqovsi.html

[R65] 查看端口占用
来源：http://hz.wangshuangyany.cn/gtdvgzthtj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gthltjlzcr.html

[R66] 定时任务
来源：http://hz.jianghu66.top/gtlwlhqqqq.html

crontab -e;  crontab -l
来源：http://hz.yongpay.top/gtkfigalfe.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtejcjmezb.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtdxrohcox.html

[R68] 计算文件校验值
来源：http://hz.zdqjudy.top/gttqqjpeej.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gtfkosusxy.html

[R69] 生成随机密码
来源：http://hz.svipenyu.cn/gtiagpfdjk.html

head -c 16 /dev/urandom | base64
来源：http://hz.pengpengdd.cyou/gtriehtbyx.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtywwjanbh.html

date +%s;  date -d @1700000000
来源：http://hz.gaohongyu789.top/gtytdkzcqm.html

[R71] 日期格式化
来源：http://hz.sxryk.cn/gtipqkmdzl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.vqdsnc.cn/gthbbbqyoi.html

[R72] 等待端口就绪
来源：http://hz.hywenlv.cn/gtmleqyshc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tanke756.top/gtvpgovfwg.html

[R73] 分割大日志
来源：http://hz.shangyingyoupin.top/gtmygfzbwj.html

split -l 1000 big.log part_
来源：http://hz.haohaochexian.top/gtbxfrxezn.html

[R74] 批量重命名
来源：http://hz.ywan-chungtsiang.top/gtxxdexrbr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtzynyoxgh.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtapeyxalr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtvbcphnht.html

[R76] 使用临时文件
来源：http://hz.gotoacloud.top/gtcgelgdij.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtgbybitgq.html

[R77] 读取用户输入
来源：http://hz.tianlin.xyz/gtmqtxwhfy.html

read -rp "请输入: " ans
来源：http://hz.52xcode.cn/gthiaxcsrj.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gthmhfodpy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.9152youxi.cn/gtmqosmnja.html

[R79] 解析命令行选项
来源：http://hz.cdnleiting.top/gteodahspe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj20258888.top/gtunjxccne.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtrhxlofrx.html

time ./run.sh
来源：http://hz.bjfxy.top/gtpsteczog.html

================================================================================
来源：http://hz.yuanzhike.top/gtdpkqcajl.html

S. C / C++ 专题
来源：http://hz.redwolf501.top/gtnzystbau.html

================================================================================
来源：http://hz.jyoumei.cn/gtsjykzuwe.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtswsbixna.html

#include <stdio.h>
来源：http://hz.wangshuangyany.cn/gtaqnibigf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtiewopzoz.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gthxzvssjw.html

int a = 10; printf("%d\n", a);
来源：http://hz.gaohongyu789.top/gtdyctfwxp.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gttghegfue.html

int x; scanf("%d", &x);
来源：http://hz.ivvv.top/gtwyklmaui.html

[S04] C：字符串复制
来源：http://hz.sysykeji.top/gtsmnaqlor.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yanxiufei.cn/gtuvwolisb.html

[S05] C：字符串长度
来源：http://hz.pengpengdd.cyou/gtvirjkpnt.html

strlen(s)
来源：http://hz.tianlin.xyz/gtynmbeubx.html

[S06] C：字符串比较
来源：http://hz.zhoulong.xyz/gtxugqmdjl.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gtjdfoqpnx.html

[S07] C：数组遍历求和
来源：http://hz.yuxming.cn/gtvjktfgti.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtvfbvmfnh.html

[S08] C：动态内存分配与释放
来源：http://hz.gaohongyu789.top/gtptehjhfh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xinyue.icu/gtnvtizapw.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtootecngu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtfqozgcvn.html

[S10] C：指针与解引用
来源：http://hz.yuanzhike.top/gtzasbxndm.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtjobhwhuu.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtnhaxsyig.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gotoacloud.top/gtfruxfsod.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yongpay.top/gttviasibd.html

fclose(f);
来源：http://hz.52xcode.cn/gtuxextbru.html

[S12] C：写文件
来源：http://hz.chenjidiqi.icu/gtgjgccttq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gtigjvninm.html

[S13] C：宏定义
来源：http://hz.zhiwuduotai.top/gtznbnwqxm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aibaodan.cn/gtrysirrgo.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtvfydjosm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhaomingkeji.xyz/gtnjjrcqai.html

[S15] C：类型转换
来源：http://hz.fzhhl.top/gtvkhcdabc.html

(double) a / b
来源：http://hz.nanxuanxn.top/gtdevgzlrv.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtpqmhceqx.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtrhwljesk.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtdxbtbdwy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zdqjudy.top/gtqzynbdjg.html

[S18] C：命令行参数
来源：http://hz.chenjidiqi.icu/gtfhfabxcj.html

int main(int argc, char **argv)
来源：http://hz.meibo888.top/gtguatizsa.html

[S19] C：快速排序
来源：http://hz.yongpay.top/gtncblootv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gtjtimirqv.html

[S20] C：二分查找
来源：http://hz.jqgufenzy.top/gtfucauyuc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtpcbacreo.html

[S21] C：字符类别判断
来源：http://hz.316326.xyz/gttsgiyiif.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shangyingyoupin.top/gtafihuvmv.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gthxihxbur.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shuidangran.top/gtrhhzczvi.html

[S23] C：随机数
来源：http://hz.haohaochexian.top/gtswfwixek.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtrgyhfaeq.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtfjgeznyr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gtgwwihovm.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gtcqsrfiog.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtvoyjlaoj.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtcuxtvyhb.html

memset(a, 0, sizeof a);
来源：http://hz.gotoacloud.top/gtfopadkhq.html

[S27] C：定义常量
来源：http://hz.feifeiyinyue.top/gtttdykxbq.html

const double PI = 3.14159;
来源：http://hz.316326.xyz/gtdjmtvlbr.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtpramosgo.html

static int counter = 0;
来源：http://hz.52xcode.cn/gthvrkcbqb.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gtcdyspzdm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cashguo.top/gtulawqghu.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gtfbplyywj.html

#ifndef X_H
来源：http://hz.tian-w.cn/gtwpnyugiq.html

#define X_H
来源：http://hz.fzhhl.top/gtinnyufql.html

#endif
来源：http://hz.tianlin.xyz/gtoksecdhd.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtlfnfjgoe.html

#include <iostream>
来源：http://hz.ydzc1.top/gtcqmvjqtq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigufen.top/gtqcepdaym.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtmjfjktev.html

std::string s = "hi";  s += "!";
来源：http://hz.fengsongda.top/gtmhmpgpte.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtsukxnpdm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtbgcikfyv.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtqogbcdvf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenjidiqi.icu/gtcskkywsl.html

[S35] C++：map
来源：http://hz.ivvv.top/gtnvgovccq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aizwys.cn/gtgiojrqas.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtjaxlqieq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtmnejzlvc.html

[S37] C++：set
来源：http://hz.tanke756.top/gtuldrdcfw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gtziestbxb.html

[S38] C++：排序
来源：http://hz.meibo888.top/gtmpfrpcpz.html

std::sort(v.begin(), v.end());
来源：http://hz.yongpay.top/gtcbbvnlsk.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtopczshkc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtfzupewig.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gtvpkgvlii.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuxming.cn/gtuoqsjqwh.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtplrhstav.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sxryk.cn/gtelotpytl.html

[S42] C++：继承与虚函数
来源：http://hz.havefunace.top/gtykiuuvyd.html

class B : public Base { public: void f() override {} };
来源：http://hz.gogol.net.cn/gttmbctvqa.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtfcoeobyn.html

auto p = std::make_unique<int>(5);
来源：http://hz.svipenyu.cn/gtoatocciv.html

[S44] C++：引用传参
来源：http://hz.guowangkeji.top/gtzljmmolk.html

void inc(int &x) { ++x; }
来源：http://hz.zhengqikj.top/gtkohlrnhk.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gtnxilhddf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.9152youxi.cn/gtwvfbtjja.html

[S46] C++：函数模板
来源：http://hz.chenlongwang.top/gtsqxarhtr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.snrcjt.cn/gtktmxcuum.html

[S47] C++：结构化绑定遍历
来源：http://hz.gzhubu.top/gtjerisgfa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.snrcjt.cn/gtarmvbesq.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtwrkpvxfh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daria6918.cn/gtrlrexkil.html

while (std::getline(in, line)) { }
来源：http://hz.quarkkingdee.top/gthqwnzrfg.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gtirpijluv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtohmnauha.html

[S50] C++：格式化数字
来源：http://hz.smart0.xyz/gtchylnwml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnxiangtu.top/gtrffmvcvk.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gtnbrjdbib.html

static_cast<double>(a) / b
来源：http://hz.nanxuanxn.top/gtjfkiivta.html

[S52] C++：const 与 noexcept
来源：http://hz.fengsongda.top/gtjzsouaat.html

int size() const noexcept { return n_; }
来源：http://hz.xuanzx.com/gtsayaluxf.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtlwwpmysd.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgufenzy.top/gtjkhthrsp.html

[S54] C++：异常处理
来源：http://hz.iojbl.cn/gtizpejlsy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtkwxwcvxz.html

[S55] C++：结构化绑定
来源：http://hz.cdnleiting.top/gtkjyokqug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gaohongyu789.top/gtyvgkfiue.html

[S56] C++：optional
来源：http://hz.cashguo.top/gtusnotkdf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtnyyocvrg.html

[S57] C++：编译期常量
来源：http://hz.c1oappe.top/gttnxoaoix.html

constexpr int N = 10;
来源：http://hz.jinghuilouyu.cn/gtyxsnkpnd.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtligztgxb.html

namespace ns { int f() { return 1; } }
来源：http://hz.havefunace.top/gtgmootvne.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gtvqqnrtun.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtgfddsisb.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtuhsrldox.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gthyxcyahl.html

================================================================================
来源：http://hz.meibo888.top/gtexoezgda.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jlsjyb.cn/gtgjnvkqtc.html

================================================================================
来源：http://hz.bjfxy.top/gtpbjoavoc.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtscfdjiuy.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtggyntwwg.html

[T02] Kotlin：变量
来源：http://hz.hnxiangtu.top/gtoyuacyjd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.redwolf501.top/gtwcsqytrk.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gteaajrofg.html

"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtxkvjrlxc.html

[T04] Kotlin：空安全
来源：http://hz.hywenlv.cn/gtogohmijp.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtldsmkbjz.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtncvrtfhb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aizwys.cn/gtpcafoeto.html

[T06] Kotlin：集合映射
来源：http://hz.havefunace.top/gtzccjdesa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guannengcc.top/gtouoiwnbn.html

[T07] Kotlin：集合过滤
来源：http://hz.yangfankeji.com/gtedvvumvu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhoulong.xyz/gtunwwrrsg.html

[T08] Kotlin：数据类
来源：http://hz.vqdsnc.cn/gtwvwaaggy.html

data class User(val name: String, val age: Int)
来源：http://hz.sweek.top/gtrvtcydhk.html

[T09] Kotlin：扩展函数
来源：http://hz.jinghuilouyu.cn/gtxiumsqag.html

fun String.exclaim() = this + "!"
来源：http://hz.andypj.xyz/gtwikzkfwd.html

[T10] Kotlin：默认参数
来源：http://hz.zhiwuduotai.top/gtoqfjamvi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgufenzy.top/gtefltwpdb.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtgwriakki.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangdashe.top/gtqihhqmdu.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtgntrpubt.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangtech.top/gtmgkecokd.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtattbydfi.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gtllbjecga.html

[T14] Kotlin：循环
来源：http://hz.hnqzz.top/gtgvuvcmkm.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtcwbemfdb.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gtvmhatkiz.html

interface Shape { fun area(): Double }
来源：http://hz.svipenyu.cn/gtuzfqhmkm.html

[T16] Swift：Hello World
来源：http://hz.pengpengdd.cyou/gtfpvomnvk.html

print("Hello")
来源：http://hz.hywenlv.cn/gtatiaaiqo.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtwujbkuhd.html

var a = 1;  let b = 2
来源：http://hz.cucudq.cn/gthhpogjxd.html

[T18] Swift：字符串插值
来源：http://hz.cqqwz.cn/gtucdyxchi.html

"值: \(b)"
来源：http://hz.sxryk.cn/gthykyhpft.html

[T19] Swift：可选绑定
来源：http://hz.hfpthk.cn/gtxgoppkha.html

if let n = opt { print(n) }
来源：http://hz.vqdsnc.cn/gtzmohkieg.html

[T20] Swift：数组操作
来源：http://hz.vqdsnc.cn/gtaxmzfkrz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtqndnplwq.html

[T21] Swift：遍历
来源：http://hz.daxiang520.top/gtwgunfkap.html

for x in a { print(x) }
来源：http://hz.jqgufenzy.top/gtcdudhany.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtjijtxvnr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sweek.top/gtxphoaeil.html

[T23] Swift：函数
来源：http://hz.tianlin.xyz/gtxegfqtkd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtaujqpghy.html

[T24] Swift：闭包
来源：http://hz.cashguo.top/gtuuqjtocu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtdovcrncr.html

[T25] Swift：结构体
来源：http://hz.yj20258888.top/gtylqyqxfw.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtkldisowm.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtrbkplmuu.html

class A: Base { override func f() {} }
来源：http://hz.yangfankeji.com/gtlosjftvj.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtgnqkhymx.html

do { try f() } catch { print(error) }
来源：http://hz.aibaodan.cn/gtyooacjmn.html

[T28] Swift：枚举
来源：http://hz.fzhhl.top/gtdwgnzwdm.html

enum Color { case red, green }
来源：http://hz.sxryk.cn/gtmxlywgco.html

[T29] Swift：guard 提前返回
来源：http://hz.shzxlz.cn/gtjynqolov.html

guard let x = opt else { return }
来源：http://hz.fengsongda.top/gtgmfiwjxc.html

[T30] Swift：协议
来源：http://hz.sysykeji.top/gtkidievea.html

protocol Shape { func area() -> Double }
来源：http://hz.hammf.cn/gtigrvtyox.html

[T31] Lua：Hello World
来源：http://hz.gogol.net.cn/gtrbzkhghb.html

print("Hello")
来源：http://hz.hfpthk.cn/gtpwofamvj.html

[T32] Lua：局部变量
来源：http://hz.shzxlz.cn/gtueeaypnd.html

local a = 1
来源：http://hz.gaohongyu789.top/gtharxzzqn.html

[T33] Lua：表（数组）
来源：http://hz.zhixingplan.top/gtejsivcev.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhiwuduotai.top/gtxsizwynt.html

[T34] Lua：遍历表
来源：http://hz.xylfe.cn/gtfkxgxrgm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pengpengdd.cyou/gtcjusqjyu.html

[T35] Lua：字典表
来源：http://hz.shuidangran.top/gtczwpgpoc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.haohaochexian.top/gtuxlrnqwh.html

[T36] Lua：函数
来源：http://hz.ydzc1.top/gtilbgqxfe.html

function add(a, b) return a + b end
来源：http://hz.havefunace.top/gtvvtexlgv.html

[T37] Lua：字符串拼接
来源：http://hz.yj20258.top/gtyhnlynxa.html

"a" .. "b"
来源：http://hz.ivvv.top/gtynipzmfs.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gtucznltnz.html

if x > 0 then print("正") end
来源：http://hz.snrcjt.cn/gtcpflqmen.html

[T39] Lua：模式匹配
来源：http://hz.zhengqikj.top/gtabxasfll.html

string.find(s, "%d+")
来源：http://hz.yanxiufei.cn/gtegzqjgbp.html

[T40] Lua：元表
来源：http://hz.cqqwz.cn/gtcbpjmxif.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtgkyhtlfb.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtngfiqmis.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gteydbglku.html

[T42] Perl：变量类型
来源：http://hz.jiagoushi.top/gtfasgdtgh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinghuilouyu.cn/gtjypvvygz.html

[T43] Perl：字符串插值
来源：http://hz.zycfv.cn/gtvdcutlab.html

"值: $a"
来源：http://hz.shanyushiyangtech.top/gtwnhuixbb.html

[T44] Perl：条件
来源：http://hz.jqgufenzy.top/gtrqstlsrm.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gttnzyvjnu.html

[T45] Perl：数组遍历
来源：http://hz.ywan-chungtsiang.top/gtoufguvmz.html

for my $x (@arr) { print $x; }
来源：http://hz.xylfe.cn/gtcvyqjhrj.html

[T46] Perl：哈希操作
来源：http://hz.guannengcc.top/gtsybnkeul.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenzaomai.com/gtvwkxkbla.html

[T47] Perl：正则捕获
来源：http://hz.daxiang520.top/gtqxldlann.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yueranfly.top/gtqjkoqace.html

[T48] Perl：正则替换
来源：http://hz.zhengqikj.top/gtzfhxycln.html

$s =~ s/old/new/g;
来源：http://hz.jinghuilouyu.cn/gterbdpbeg.html

[T49] Perl：函数
来源：http://hz.tianlin.xyz/gtleanapfc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jianghu66.top/gtmyfdvxwq.html

[T50] Perl：逐行读文件
来源：http://hz.hnxiangtu.top/gtcefmswvd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shuidangran.top/gtgcqupqvn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.svipenyu.cn/gtrdtgtbda.html

[T51] Scala：Hello World
来源：http://hz.ppjwa.cn/gtuikvektc.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtsiohlokw.html

[T52] Scala：变量
来源：http://hz.zhaomingkeji.xyz/gtacwodvyi.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtjmtkwvgc.html

[T53] Scala：字符串插值
来源：http://hz.jqgfzy.top/gtbcgiszvq.html

s"值: $b"
来源：http://hz.gotoacloud.top/gtqcgfadsx.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtqcwendaw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nwbrower.top/gtjzvntgmy.html

[T55] Scala：集合过滤
来源：http://hz.hysaishi.cn/gtikdgtvnb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sufxvd.cn/gtcrbidneh.html

[T56] Scala：样例类
来源：http://hz.sufxvd.cn/gtcyqfckds.html

case class User(name: String, age: Int)
来源：http://hz.birdmap.top/gtfpuzsrps.html

[T57] Scala：模式匹配
来源：http://hz.ywan-chungtsiang.top/gtqiivsjpb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinqigufen.top/gtzutghrji.html

[T58] Scala：函数定义
来源：http://hz.tianlin.xyz/gtafpqbvfk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.52xcode.cn/gtmqaiblgg.html

[T59] Scala：循环
来源：http://hz.nanxinkj.top/gtgcrlrvko.html

for (i <- 1 to 10) println(i)
来源：http://hz.tian-w.cn/gtrmuorwbn.html

[T60] Scala：折叠
来源：http://hz.smart0.xyz/gtkweotwec.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangkeji.top/gtiuexuqeg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgenmlnix.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sxryk.cn/gtxqbfhidv.html

================================================================================
来源：http://hz.iojbl.cn/gttekuneqf.html

[U01] Py：创建虚拟环境
来源：http://hz.ydzc1.top/gtpfdadlig.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgfzy.top/gtmyqtwzqb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.birdmap.top/gtwnotfojw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtkssrrixx.html

[U03] Py：加载 .env 配置
来源：http://hz.316326.xyz/gtbrjgnhjb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.iojbl.cn/gtwwcnagtw.html

[U04] Py：变量调试打印
来源：http://hz.xuanzx.com/gtkiagjrex.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gttggonxdl.html


<!-- 参考信息 -->