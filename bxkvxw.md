代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangshuangyany.cn/gtxmcepaeo.html

[R60] 只看 HTTP 状态码
来源：http://hz.birdmap.top/gtawodtthf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.0kj1m.cn/gtciujcsce.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtzyyujoxv.html

df -h;  du -sh *
来源：http://hz.chenzaomai.com/gteddjpbjb.html

[R62] 找最占空间的文件
来源：http://hz.jyoumei.cn/gtfvsaxbnm.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtgrekycfl.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtgngwkynt.html

free -h;  ps aux | grep nginx
来源：http://hz.gzhubu.top/gtureuczpk.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtprslembz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtoxppembd.html

[R65] 查看端口占用
来源：http://hz.ydjk.org.cn/gtkexnfbra.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xingfuxueyuan.xyz/gtqavwcjyk.html

[R66] 定时任务
来源：http://hz.gaohongyu789.top/gtnddwvhgk.html

crontab -e;  crontab -l
来源：http://hz.mhx1999.top/gtnkhuhpmf.html

[R67] 生成随机十六进制串
来源：http://hz.shuidangran.top/gtvvozlyuj.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtxdwuimvg.html

[R68] 计算文件校验值
来源：http://hz.guannengcc.top/gtrybvwxqk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.c1oappe.top/gttztsprko.html

[R69] 生成随机密码
来源：http://hz.hfpthk.cn/gtndsqiopn.html

head -c 16 /dev/urandom | base64
来源：http://hz.jiagoushi.top/gtzexyzazi.html

[R70] 时间戳与互转
来源：http://hz.dashuyun.cn/gtqlcrgudy.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtpbudxjio.html

[R71] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtvvlwfbbr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zdqjudy.top/gtnocplemv.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtidoxwvwr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtrdwiwuhu.html

[R73] 分割大日志
来源：http://hz.hfpthk.cn/gtmhtemvao.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtjljghwht.html

[R74] 批量重命名
来源：http://hz.jinyuanbaomall.cn/gtgiptyoge.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258888.top/gtlqeybiyg.html

[R75] 导出环境变量
来源：http://hz.dianchejie.cn/gtqkkuvyin.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangdashe.top/gtvmqtubgr.html

[R76] 使用临时文件
来源：http://hz.zycfv.cn/gtlfraaaqk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtmpafncxg.html

[R77] 读取用户输入
来源：http://hz.jyoumei.cn/gtuoszjkfs.html

read -rp "请输入: " ans
来源：http://hz.fengsongda.top/gtmklplfcy.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtlacuzsgv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cucudq.cn/gtfbcpdqzo.html

[R79] 解析命令行选项
来源：http://hz.52xcode.cn/gtdfckjioh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fengsongda.top/gtdspmyxow.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxinkj.top/gtmiyrkvrz.html

time ./run.sh
来源：http://hz.gogol.net.cn/gtzckugbqv.html

================================================================================
来源：http://hz.bjfxy.top/gtmglammmp.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtvjpbadky.html

================================================================================
来源：http://hz.svipenyu.cn/gtwfnlpegr.html

[S01] C：Hello World
来源：http://hz.hysaishi.cn/gtrryfbohe.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtfjdmzuzh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtjiygoaav.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigfzy.top/gtbwslthrd.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258888.top/gtsjmcbljs.html

[S03] C：读入整数
来源：http://hz.jqgufenzy.top/gtziiobtxt.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtrvrquhta.html

[S04] C：字符串复制
来源：http://hz.pycfn.com/gtgxdxgpkl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hywenlv.cn/gtrhzjqpvb.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtwoyjnhda.html

strlen(s)
来源：http://hz.yvedp.cn/gtvdlhruzq.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gtuivwcgsn.html

strcmp(a, b) == 0
来源：http://hz.daria6918.cn/gtogmgdcuo.html

[S07] C：数组遍历求和
来源：http://hz.yanxiufei.cn/gtrldroqxt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtiunfheht.html

[S08] C：动态内存分配与释放
来源：http://hz.dashuyun.cn/gtwozjsfir.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gtowafaeio.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtughgpzlm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuanzhike.top/gtddmjelqr.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gttuqxclit.html

int *p = &a;  *p = 5;
来源：http://hz.shzxlz.cn/gtczcieayp.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gticmszjck.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sufxvd.cn/gtaosqflnq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangkeji.top/gtbcgplyiu.html

fclose(f);
来源：http://hz.smart0.xyz/gtsvllvgqk.html

[S12] C：写文件
来源：http://hz.chenlongwang.top/gtigkxlwmi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cqqwz.cn/gtuklhyunx.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtypsiqijr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cucudq.cn/gtxyviavcz.html

[S14] C：枚举
来源：http://hz.sweek.top/gtzywqfpso.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtsrputamb.html

[S15] C：类型转换
来源：http://hz.pengpengdd.cyou/gtrlvwfrrc.html

(double) a / b
来源：http://hz.jinqigfzy.top/gtlyobvbjn.html

[S16] C：位操作置位
来源：http://hz.jinyuanbaomall.cn/gtkrkzpuzj.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtxgifmpnx.html

[S17] C：安全拼接字符串
来源：http://hz.yuanzhike.top/gttzcydpom.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtolbszebe.html

[S18] C：命令行参数
来源：http://hz.kuanghao11.cn/gtwtmwqsdz.html

int main(int argc, char **argv)
来源：http://hz.jinqigfzy.top/gtsngbvwww.html

[S19] C：快速排序
来源：http://hz.hnxiangtu.top/gtkfmfyugd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtwxvrfpaa.html

[S20] C：二分查找
来源：http://hz.c1oappe.top/gtwchrnlgt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gttwndvcdk.html

[S21] C：字符类别判断
来源：http://hz.zdqjudy.top/gtgbtcesbt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinghuilouyu.cn/gtylkjcklq.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtbxfqlzpl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinqigfzy.top/gtaudcllwj.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtnsikcwxu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shzxlz.cn/gtkwwgnvpo.html

[S24] C：获取本地时间
来源：http://hz.tian-w.cn/gtqexnnasn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gttsmkegiu.html

[S25] C：内存拷贝
来源：http://hz.xylfe.cn/gtgaggchbo.html

memcpy(dst, src, n);
来源：http://hz.feifeiyinyue.top/gtffdqvckm.html

[S26] C：内存清零
来源：http://hz.sysykeji.top/gtrazvdznt.html

memset(a, 0, sizeof a);
来源：http://hz.wangshuangyany.cn/gtrqdyczwk.html

[S27] C：定义常量
来源：http://hz.ydzc1.top/gtxatgmiso.html

const double PI = 3.14159;
来源：http://hz.hnxiangtu.top/gtrwavxumc.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtdowwbxvs.html

static int counter = 0;
来源：http://hz.pycfn.com/gtmsifqyde.html

[S29] C：变参函数
来源：http://hz.cqqwz.cn/gtuoizqgzr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgufenzy.top/gtsnikvzpr.html

[S30] C：头文件保护
来源：http://hz.hnqzz.top/gthrgfoqhf.html

#ifndef X_H
来源：http://hz.birdmap.top/gtjasnklyh.html

#define X_H
来源：http://hz.nwbrower.top/gtkwdcunti.html

#endif
来源：http://hz.cucudq.cn/gtckcvxnse.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtrspaeveg.html

#include <iostream>
来源：http://hz.jianghu66.top/gtznafihyu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gtkoevuioh.html

[S32] C++：字符串
来源：http://hz.wangshuangyany.cn/gttbetfyjd.html

std::string s = "hi";  s += "!";
来源：http://hz.gzhubu.top/gtllkecjfv.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gticryiqad.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtwpmarrnq.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtmcoxngbb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtbjjjnvnl.html

[S35] C++：map
来源：http://hz.sxryk.cn/gtnkfwcrbt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gthduzzdul.html

[S36] C++：unordered_map
来源：http://hz.nanxuanxn.top/gttmgcryxy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtjinthvhb.html

[S37] C++：set
来源：http://hz.ppjwa.cn/gtuaeuhqpp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinghuilouyu.cn/gtibklsrrp.html

[S38] C++：排序
来源：http://hz.9152youxi.cn/gtxtciskjo.html

std::sort(v.begin(), v.end());
来源：http://hz.52xcode.cn/gtkcmdukbd.html

[S39] C++：自定义比较器排序
来源：http://hz.ivvv.top/gtnjohwsts.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.redwolf501.top/gttgnyjsbj.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtprvixgoj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cdnleiting.top/gtaosqvjna.html

[S41] C++：类与构造函数
来源：http://hz.nanxinkj.top/gtcegercfc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gtcxxnvsee.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtxpbryajb.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenzaomai.com/gtazepbzsm.html

[S43] C++：智能指针
来源：http://hz.jinqigfzy.top/gtiokpyvdl.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinyuanbaomall.cn/gtyejvillu.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangtech.top/gtxdidjlcl.html

void inc(int &x) { ++x; }
来源：http://hz.cqqwz.cn/gtautchrjv.html

[S45] C++：lambda
来源：http://hz.yj202588.top/gthydpzctl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtnisjfvgr.html

[S46] C++：函数模板
来源：http://hz.zdqjudy.top/gtnjkgzebl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ybcxt.top/gtcpusvfgt.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinghuilouyu.cn/gtmahwiazh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gaohongyu789.top/gtvuyhsdkg.html

[S48] C++：逐行读文件
来源：http://hz.yonumen.top/gtypbbqeum.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenzaomai.com/gtnnxpxlyt.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtrxkpmspt.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtwjcejdkv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gaohongyu789.top/gtmvbkqtut.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gtpxsvpcrs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dianchejie.cn/gtfvfozmbi.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtbjtsqloe.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtnzgmkehg.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtmovecivl.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtirhmwfoi.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtmgwfzxhu.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtntfotirn.html

[S54] C++：异常处理
来源：http://hz.jinghuilouyu.cn/gtdcemrlki.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtjffubdsd.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gteupibiia.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.snrcjt.cn/gtwgwywfio.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtumlksvou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xziqi.cn/gtcdvlpvjc.html

[S57] C++：编译期常量
来源：http://hz.aizwys.cn/gtyfussjzl.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtaefdxpay.html

[S58] C++：命名空间
来源：http://hz.shzxlz.cn/gtmlryqnns.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtfaucaspq.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gtklyozwfd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj202588.top/gtqscobnew.html

[S60] C++：遍历并删除元素
来源：http://hz.daria6918.cn/gtcetealuj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gtuytfdyxt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzdcfqmdk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtmpttcizo.html

================================================================================
来源：http://hz.yvedp.cn/gtgvnphkcs.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtancfqwhk.html

println("Hello")
来源：http://hz.hysaishi.cn/gthjztshxq.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gthugimnwo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.pycfn.com/gtrembwsap.html

[T03] Kotlin：字符串模板
来源：http://hz.fengsongda.top/gtrnfalujc.html

"值: $b"
来源：http://hz.hnqzz.top/gthhsolnxd.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtyqwzdfnr.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtqivgznrn.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gtdexhokxj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xingfuxueyuan.xyz/gtiqwqokjl.html

[T06] Kotlin：集合映射
来源：http://hz.zhaomingkeji.xyz/gtepncjpei.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtsfawmkyh.html

[T07] Kotlin：集合过滤
来源：http://hz.xinyue.icu/gtjcfxsyxe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258888.top/gtxgqcaeoh.html

[T08] Kotlin：数据类
来源：http://hz.kuanghao11.cn/gtaidlzhkc.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtusnzpefg.html

[T09] Kotlin：扩展函数
来源：http://hz.ydjk.org.cn/gtwvdgsaac.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtazujokpd.html

[T10] Kotlin：默认参数
来源：http://hz.birdmap.top/gtoycnwqvf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ivvv.top/gtveifgyem.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtggkfpmpm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtpralmudv.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtueaogrcc.html

val (a, b) = Pair(1, 2)
来源：http://hz.cheryme.top/gtzednyclh.html

[T13] Kotlin：只读 Map
来源：http://hz.ywan-chungtsiang.top/gtnwfyzzwc.html

val m = mapOf("a" to 1)
来源：http://hz.xziqi.cn/gtvzyyemjc.html

[T14] Kotlin：循环
来源：http://hz.zycfv.cn/gtinggskln.html

for (i in 1..10) println(i)
来源：http://hz.aibaodan.cn/gtogyewvjc.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtyhyjsqiq.html

interface Shape { fun area(): Double }
来源：http://hz.snrcjt.cn/gtmvcmtbek.html

[T16] Swift：Hello World
来源：http://hz.quarkkingdee.top/gtawygdrjt.html

print("Hello")
来源：http://hz.ppjwa.cn/gtiggwbkac.html

[T17] Swift：变量与常量
来源：http://hz.shuidangran.top/gtakdcwebf.html

var a = 1;  let b = 2
来源：http://hz.zhixingplan.top/gtoaaeqaed.html

[T18] Swift：字符串插值
来源：http://hz.havefunace.top/gtlqjjlagk.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtgmcpusvh.html

[T19] Swift：可选绑定
来源：http://hz.feifeiyinyue.top/gtbsykefup.html

if let n = opt { print(n) }
来源：http://hz.ydjk.org.cn/gtoqpjaoiz.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtfqdsaisi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hysaishi.cn/gtlrbgcies.html

[T21] Swift：遍历
来源：http://hz.guannengcc.top/gtuxwspexf.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gtfnufkymt.html

[T22] Swift：字典
来源：http://hz.haohaochexian.top/gthrckykqw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxuanxn.top/gtfogcchbm.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtfgqegvxa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtlpxeyajk.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtgbcnmxlt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dashuyun.cn/gtzrjuemjd.html

[T25] Swift：结构体
来源：http://hz.tian-w.cn/gtsfipdaqf.html

struct P { var x: Int }
来源：http://hz.52xcode.cn/gtshohvetc.html

[T26] Swift：类与重写
来源：http://hz.zhijiandao.cn/gthxarugpz.html

class A: Base { override func f() {} }
来源：http://hz.snrcjt.cn/gtwmrnoxgq.html

[T27] Swift：错误处理
来源：http://hz.sweek.top/gtgilfgiwd.html

do { try f() } catch { print(error) }
来源：http://hz.xingfuxueyuan.xyz/gtvhewllhp.html

[T28] Swift：枚举
来源：http://hz.tanke756.top/gtmuvdtawy.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gttkrrlmyn.html

[T29] Swift：guard 提前返回
来源：http://hz.shangyingyoupin.top/gtehcwnjry.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gtcduytaxy.html

[T30] Swift：协议
来源：http://hz.cqqwz.cn/gtsckxqgci.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtbbcmkjzp.html

[T31] Lua：Hello World
来源：http://hz.daxiang520.top/gthglicobu.html

print("Hello")
来源：http://hz.cucudq.cn/gtscriowrt.html

[T32] Lua：局部变量
来源：http://hz.iojbl.cn/gtuprhzjsy.html

local a = 1
来源：http://hz.bjfxy.top/gtmhyhenzr.html

[T33] Lua：表（数组）
来源：http://hz.svipenyu.cn/gtixlgwxmf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xinyue.icu/gtldubajpq.html

[T34] Lua：遍历表
来源：http://hz.gotoacloud.top/gtwryjdnbz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gthybzcrrz.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtrqjttskd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cqqwz.cn/gtjgcbwwpn.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtnafdvtqw.html

function add(a, b) return a + b end
来源：http://hz.yuxming.cn/gtddaqouky.html

[T37] Lua：字符串拼接
来源：http://hz.xinyue.icu/gtvizvshib.html

"a" .. "b"
来源：http://hz.zhixingplan.top/gtnmmvookq.html

[T38] Lua：条件
来源：http://hz.daxiang520.top/gtizhwlwgk.html

if x > 0 then print("正") end
来源：http://hz.hfpthk.cn/gtxlfctyhx.html

[T39] Lua：模式匹配
来源：http://hz.yvedp.cn/gtpyotrppj.html

string.find(s, "%d+")
来源：http://hz.jyoumei.cn/gtmqzxeboq.html

[T40] Lua：元表
来源：http://hz.shuidangran.top/gtgvzhwoyn.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtanthksec.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gtvoatftdb.html

print "Hello\n";
来源：http://hz.tianlin.xyz/gtmnslqbkt.html

[T42] Perl：变量类型
来源：http://hz.nanxuanxn.top/gtkhpymrud.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gtioaojdpa.html

[T43] Perl：字符串插值
来源：http://hz.hysaishi.cn/gtqafeaqsb.html

"值: $a"
来源：http://hz.jinqigufen.top/gtnoquabql.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gtfeohsxcp.html

if ($a > 0) { print "正"; }
来源：http://hz.zdqjudy.top/gtawbtoeiy.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtbmpczloq.html

for my $x (@arr) { print $x; }
来源：http://hz.xuetiantiany.cn/gtbrufwgpj.html

[T46] Perl：哈希操作
来源：http://hz.yvedp.cn/gtwdjyzrbh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dashuyun.cn/gttgslbrqq.html

[T47] Perl：正则捕获
来源：http://hz.sweek.top/gtsbjvpibr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.bjfxy.top/gtjrpwowdg.html

[T48] Perl：正则替换
来源：http://hz.yanxiufei.cn/gtgxrtzxij.html

$s =~ s/old/new/g;
来源：http://hz.nanxuanxn.top/gtddpntykp.html

[T49] Perl：函数
来源：http://hz.jiagoushi.top/gtxonmqlnf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gogol.net.cn/gtibofddoc.html

[T50] Perl：逐行读文件
来源：http://hz.gogol.net.cn/gtajmeziup.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yueranfly.top/gteqpxaoee.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinyuanbaomall.cn/gtawffjwpc.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtzmwovwjh.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtnlaebtga.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gtldmxtovc.html

val a = 1;  var b = 2
来源：http://hz.zhijiandao.cn/gtsxvzamkj.html

[T53] Scala：字符串插值
来源：http://hz.birdmap.top/gtygmrdbxb.html

s"值: $b"
来源：http://hz.smart0.xyz/gtbjlhqwhu.html

[T54] Scala：集合映射
来源：http://hz.shuidangran.top/gtcllsoxaq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zycfv.cn/gtktzuiukt.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gtrrifsxap.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhongyouzk.top/gtfqvelasm.html

[T56] Scala：样例类
来源：http://hz.jinqigufen.top/gtpatslxll.html

case class User(name: String, age: Int)
来源：http://hz.nanxuanxn.top/gteolywhcl.html

[T57] Scala：模式匹配
来源：http://hz.xuanzx.com/gtwgecrfzn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.svipenyu.cn/gtcemznoie.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtfjaprivx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yvedp.cn/gtvpmnxbzu.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gtlkqcoiwf.html

for (i <- 1 to 10) println(i)
来源：http://hz.ydjk.org.cn/gtcnghsvul.html

[T60] Scala：折叠
来源：http://hz.9152youxi.cn/gtowbkjqos.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.wangshuangyany.cn/gtveglgpfk.html

================================================================================
来源：http://hz.yuanzhike.top/gtsovgcour.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtriqawwkl.html

================================================================================
来源：http://hz.nanxuanxn.top/gtaocpclxp.html


<!-- 参考信息 -->