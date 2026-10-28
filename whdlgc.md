代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtotdibdgc.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtcziuiqub.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sysykeji.top/gtfquqyncn.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gtfciycgae.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yueranfly.top/gtpolmymqb.html

[R66] 定时任务
来源：http://hz.hnqzz.top/gtdbhkngpq.html

crontab -e;  crontab -l
来源：http://hz.sxryk.cn/gtfgnkjoqf.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtxytwnksb.html

openssl rand -hex 16
来源：http://hz.0kj1m.cn/gtgtrqlsam.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtxqpitupn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hfpthk.cn/gttcqmvzoa.html

[R69] 生成随机密码
来源：http://hz.sweek.top/gtdtjffqix.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtcenhedzv.html

[R70] 时间戳与互转
来源：http://hz.yj20258888.top/gtejfudmwe.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gtcictkkmz.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtokgtpdfa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guannengcc.top/gtwdecmreg.html

[R72] 等待端口就绪
来源：http://hz.daxiang520.top/gtzpytunnp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cashguo.top/gteuqyhvdx.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtuuxbdoia.html

split -l 1000 big.log part_
来源：http://hz.sufxvd.cn/gthrnlrlpd.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtsscxpnhn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtusnyxtmo.html

[R75] 导出环境变量
来源：http://hz.jinqigfzy.top/gtimirknwl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gogol.net.cn/gtoeuiwjbg.html

[R76] 使用临时文件
来源：http://hz.yj202588.top/gtijsmlqog.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gtovghgmic.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtucaaaxjr.html

read -rp "请输入: " ans
来源：http://hz.sweek.top/gtboyjtbim.html

[R78] 交互式菜单
来源：http://hz.shzxlz.cn/gtybeacttr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gthzjlswip.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtbyuteufi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hysaishi.cn/gtpxdwhofm.html

[R80] 查看脚本执行耗时
来源：http://hz.ydzc1.top/gtbzlitnla.html

time ./run.sh
来源：http://hz.hysaishi.cn/gtcmpldkuf.html

================================================================================
来源：http://hz.havefunace.top/gthzdqmbno.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtygwzyxnh.html

================================================================================
来源：http://hz.cheryme.top/gttckirqko.html

[S01] C：Hello World
来源：http://hz.xylfe.cn/gtjwobcxla.html

#include <stdio.h>
来源：http://hz.tian-w.cn/gtnamkqwtp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuanzx.com/gthiwmqonn.html

[S02] C：变量与格式化输出
来源：http://hz.tianlin.xyz/gtafpxwzyv.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxuanxn.top/gthipwqcoi.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtkhrxvvnv.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtqionjdap.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtfwbesjzk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.redwolf501.top/gtnnjnfnio.html

[S05] C：字符串长度
来源：http://hz.ehwqpu.com/gtpbccdmor.html

strlen(s)
来源：http://hz.zhongyouzk.top/gtytuddbwt.html

[S06] C：字符串比较
来源：http://hz.yj20258.top/gtbhmhytjg.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtiuwvmlqq.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtwupdmxco.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yonumen.top/gtcwwzemnu.html

[S08] C：动态内存分配与释放
来源：http://hz.cdnleiting.top/gtpyzpgixb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtjhoadyye.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtbnaivltk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gaohongyu789.top/gtgkglrdfv.html

[S10] C：指针与解引用
来源：http://hz.jyoumei.cn/gtowxhnrqw.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258.top/gtzanqfgyn.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtdlceeqcm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtdskggztu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yanxiufei.cn/gtcpgsursh.html

fclose(f);
来源：http://hz.jqgufenzy.top/gtgwuvubkx.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtgjdkrybx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gtcapotujw.html

[S13] C：宏定义
来源：http://hz.cashguo.top/gtuhppaxvo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.redwolf501.top/gtcrqtgjev.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtyngikgdh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtaaupagvq.html

[S15] C：类型转换
来源：http://hz.aibaodan.cn/gtmcxtljtg.html

(double) a / b
来源：http://hz.ivvv.top/gtfryumwbw.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtnomlcpac.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gthfbzkbqr.html

[S17] C：安全拼接字符串
来源：http://hz.nanxinkj.top/gtwqedpzjm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gtexwdnphp.html

[S18] C：命令行参数
来源：http://hz.sysykeji.top/gtjshiehzg.html

int main(int argc, char **argv)
来源：http://hz.jiagoushi.top/gtlvphewzm.html

[S19] C：快速排序
来源：http://hz.gzhubu.top/gtbnklitqf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtsyicxcft.html

[S20] C：二分查找
来源：http://hz.dianchejie.cn/gteojvlytt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtssepjzrt.html

[S21] C：字符类别判断
来源：http://hz.bjfxy.top/gthrniwejv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aizwys.cn/gtcokwclte.html

[S22] C：字符串转数字
来源：http://hz.gzhubu.top/gtfqwcdoji.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yvedp.cn/gtputvpqvp.html

[S23] C：随机数
来源：http://hz.yj20258888.top/gtbleauvpw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yueranfly.top/gthtnymhlg.html

[S24] C：获取本地时间
来源：http://hz.cheryme.top/gtlnnagutp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gtykqedaeh.html

[S25] C：内存拷贝
来源：http://hz.316326.xyz/gtgtlxnqex.html

memcpy(dst, src, n);
来源：http://hz.sysykeji.top/gtjuftzsuq.html

[S26] C：内存清零
来源：http://hz.ppjwa.cn/gtfgneezew.html

memset(a, 0, sizeof a);
来源：http://hz.jinyuanbaomall.cn/gtibifdfls.html

[S27] C：定义常量
来源：http://hz.gogol.net.cn/gtumyorzfa.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtktzctzho.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtxsdzetnp.html

static int counter = 0;
来源：http://hz.xinyue.icu/gtdctacpts.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtoyewrlnx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jiagoushi.top/gtleabiybs.html

[S30] C：头文件保护
来源：http://hz.meibo888.top/gtvmmrdstj.html

#ifndef X_H
来源：http://hz.zhoulong.xyz/gtvktxiezs.html

#define X_H
来源：http://hz.cheryme.top/gtvocwfmzt.html

#endif
来源：http://hz.yanxiufei.cn/gtgvhxsddu.html

[S31] C++：Hello World
来源：http://hz.cucudq.cn/gtkoiarxxe.html

#include <iostream>
来源：http://hz.chenjidiqi.icu/gtgdfxbitf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fengsongda.top/gtgergzsal.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtzjmerxws.html

std::string s = "hi";  s += "!";
来源：http://hz.shangyingyoupin.top/gtnivejkvc.html

[S33] C++：vector 增删
来源：http://hz.xingfuxueyuan.xyz/gtsywswpxt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigfzy.top/gtxzeomfly.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtazvgkslr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ppjwa.cn/gtcwqrwztl.html

[S35] C++：map
来源：http://hz.yj202588.top/gtibpzfehp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtxuqrwnmj.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gtpzunoajx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtadyprzex.html

[S37] C++：set
来源：http://hz.ppjwa.cn/gtzfhtzxce.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xziqi.cn/gtfuemyavu.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtaxxksonu.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangtech.top/gtmonahamv.html

[S39] C++：自定义比较器排序
来源：http://hz.hywenlv.cn/gtbkcntglm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cdnleiting.top/gtxggxarqk.html

[S40] C++：查找元素
来源：http://hz.fengsongda.top/gtelaqstry.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gtvyxrzntk.html

[S41] C++：类与构造函数
来源：http://hz.guannengcc.top/gtkrqorfdd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hfpthk.cn/gtqxysazxo.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gtcykkroeu.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhijiandao.cn/gtyeztvzjv.html

[S43] C++：智能指针
来源：http://hz.zycfv.cn/gtbslcretk.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gthelmbngm.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtenejxrcy.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gtpnjzmqof.html

[S45] C++：lambda
来源：http://hz.zhoulong.xyz/gturcvgfwb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.0kj1m.cn/gtotfkxrso.html

[S46] C++：函数模板
来源：http://hz.zycfv.cn/gtfodvenmq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dashuyun.cn/gtzlmaumgs.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gtoxrgtjrn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.316326.xyz/gtkwlxxucw.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtifsvmtta.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtmenspqpd.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtotcadzmv.html

[S49] C++：写文件
来源：http://hz.wangshuangyany.cn/gtntcjljvd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtjrootqlb.html

[S50] C++：格式化数字
来源：http://hz.tanke756.top/gtiuoyqchg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gogol.net.cn/gtwulhmzux.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gtwclsdbgs.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtksiuoclj.html

[S52] C++：const 与 noexcept
来源：http://hz.birdmap.top/gttrnnbjqu.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtrhizvpav.html

[S53] C++：移动语义
来源：http://hz.yuxming.cn/gtxrwpfckn.html

std::vector<int> w = std::move(v);
来源：http://hz.hongshengwenyu.top/gtfadsjmmz.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtfghzfmjx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtueemlims.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gtrvlzyrua.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hammf.cn/gtqfayljsx.html

[S56] C++：optional
来源：http://hz.hammf.cn/gtbzugious.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shangyingyoupin.top/gtoqonksrd.html

[S57] C++：编译期常量
来源：http://hz.sweek.top/gtgoqbciai.html

constexpr int N = 10;
来源：http://hz.ivvv.top/gtazcvlosv.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtbweawgsm.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtxgtzmnme.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gthltgdwpt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtugpbpqaw.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtgwlurxlh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.9152youxi.cn/gtwsuygswh.html

================================================================================
来源：http://hz.chenlongwang.top/gteyskijfm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtvaenmvfi.html

================================================================================
来源：http://hz.pycfn.com/gtggkltbkd.html

[T01] Kotlin：Hello World
来源：http://hz.316326.xyz/gtmlpujtaq.html

println("Hello")
来源：http://hz.c1oappe.top/gtrnojxuin.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtezorkscx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtonndjszf.html

[T03] Kotlin：字符串模板
来源：http://hz.ehwqpu.com/gtotdnykrb.html

"值: $b"
来源：http://hz.gaohongyu789.top/gtvbokiadj.html

[T04] Kotlin：空安全
来源：http://hz.fengsongda.top/gtktynsmiw.html

val n: String? = null;  n?.length
来源：http://hz.xziqi.cn/gtddgqiqju.html

[T05] Kotlin：when 表达式
来源：http://hz.wangdashe.top/gtweltmumt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtzvoofaju.html

[T06] Kotlin：集合映射
来源：http://hz.yueranfly.top/gtizpzzhph.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yueranfly.top/gtaxgsnkdf.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtujmgyiix.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shzxlz.cn/gtfzhbhzmr.html

[T08] Kotlin：数据类
来源：http://hz.hammf.cn/gthzbysube.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtaxegvnma.html

[T09] Kotlin：扩展函数
来源：http://hz.fzhhl.top/gtntjmwbdu.html

fun String.exclaim() = this + "!"
来源：http://hz.zycfv.cn/gtgugtxybn.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gtkfqpcggw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gzhubu.top/gtloeirggl.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtdzxkscok.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hywenlv.cn/gteepjqvfs.html

[T12] Kotlin：解构声明
来源：http://hz.guowangkeji.top/gtrjphizgp.html

val (a, b) = Pair(1, 2)
来源：http://hz.snrcjt.cn/gtbfjxvaey.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtwlqmfode.html

val m = mapOf("a" to 1)
来源：http://hz.smart0.xyz/gttdzugxfr.html

[T14] Kotlin：循环
来源：http://hz.kuanghao11.cn/gtnsjonqsq.html

for (i in 1..10) println(i)
来源：http://hz.iojbl.cn/gtyxhrzywz.html

[T15] Kotlin：接口
来源：http://hz.shangyingyoupin.top/gtsxqnozst.html

interface Shape { fun area(): Double }
来源：http://hz.smart0.xyz/gtlocbsgvx.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtpanqsvcw.html

print("Hello")
来源：http://hz.yongpay.top/gtgehkmooq.html

[T17] Swift：变量与常量
来源：http://hz.c1oappe.top/gtwlnwwquk.html

var a = 1;  let b = 2
来源：http://hz.hongshengwenyu.top/gtspsonwba.html

[T18] Swift：字符串插值
来源：http://hz.shzxlz.cn/gtrzfsntez.html

"值: \(b)"
来源：http://hz.sweek.top/gtgcimmghb.html

[T19] Swift：可选绑定
来源：http://hz.yuanzhike.top/gtcrkrjkkh.html

if let n = opt { print(n) }
来源：http://hz.gotoacloud.top/gtwrlsjczv.html

[T20] Swift：数组操作
来源：http://hz.hongshengwenyu.top/gtoswdrsgq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj202588.top/gtfhrflymg.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtxbnqdzne.html

for x in a { print(x) }
来源：http://hz.guannengcc.top/gtotiunxeg.html

[T22] Swift：字典
来源：http://hz.0kj1m.cn/gtlygeduwn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtbpxpuasp.html

[T23] Swift：函数
来源：http://hz.shangyingyoupin.top/gtuhskxseo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jlsjyb.cn/gthmjigwnc.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gtamchknor.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tianlin.xyz/gtgvctgkas.html

[T25] Swift：结构体
来源：http://hz.jinqigufen.top/gtwydrfqdv.html

struct P { var x: Int }
来源：http://hz.haohaochexian.top/gtcgvooglz.html

[T26] Swift：类与重写
来源：http://hz.aibaodan.cn/gtntpfvret.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtmshkbsfo.html

[T27] Swift：错误处理
来源：http://hz.ivvv.top/gtdfzkzhuy.html

do { try f() } catch { print(error) }
来源：http://hz.hongshengwenyu.top/gtabdgvali.html

[T28] Swift：枚举
来源：http://hz.jianghu66.top/gtuhcdbrjb.html

enum Color { case red, green }
来源：http://hz.cheryme.top/gtexrmhzlb.html

[T29] Swift：guard 提前返回
来源：http://hz.zhijiandao.cn/gtlwoagxhj.html

guard let x = opt else { return }
来源：http://hz.iojbl.cn/gthbpvfkgh.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gtofaaftdu.html

protocol Shape { func area() -> Double }
来源：http://hz.jianghu66.top/gtgdnshitf.html

[T31] Lua：Hello World
来源：http://hz.yongpay.top/gtsnbnsqsv.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtgxrbsijb.html

[T32] Lua：局部变量
来源：http://hz.quarkkingdee.top/gtddzyvmqe.html

local a = 1
来源：http://hz.yj20258.top/gtwtsvcwnj.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtnmzdvfvi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gzhubu.top/gtljaudlvp.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtbcdskzrx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shzxlz.cn/gtywylclpm.html

[T35] Lua：字典表
来源：http://hz.shzxlz.cn/gtmzkpebvt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtygfkezmr.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtamcfifzo.html

function add(a, b) return a + b end
来源：http://hz.nanxinkj.top/gtqpprkoum.html

[T37] Lua：字符串拼接
来源：http://hz.jqgufenzy.top/gttzrhhepf.html

"a" .. "b"
来源：http://hz.yj202588.top/gtrrmnhwlf.html

[T38] Lua：条件
来源：http://hz.nanxuanxn.top/gtvcocdwju.html

if x > 0 then print("正") end
来源：http://hz.quarkkingdee.top/gtvzlnwkqx.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gtemvgacbr.html

string.find(s, "%d+")
来源：http://hz.yanxiufei.cn/gtrnjtarbd.html

[T40] Lua：元表
来源：http://hz.snrcjt.cn/gtetzeujth.html

setmetatable({}, { __index = base })
来源：http://hz.smart0.xyz/gtmzxrwebq.html

[T41] Perl：Hello World
来源：http://hz.ivvv.top/gtokcdytwk.html

print "Hello\n";
来源：http://hz.guannengcc.top/gtncmqjaqu.html

[T42] Perl：变量类型
来源：http://hz.zhaomingkeji.xyz/gtzpwgumhg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.c1oappe.top/gtxkgsndwo.html

[T43] Perl：字符串插值
来源：http://hz.sweek.top/gtssawvggm.html

"值: $a"
来源：http://hz.jinqigufen.top/gtqukhyqzj.html

[T44] Perl：条件
来源：http://hz.jlsjyb.cn/gttcxapqtn.html

if ($a > 0) { print "正"; }
来源：http://hz.chenjidiqi.icu/gtqvafkrkr.html

[T45] Perl：数组遍历
来源：http://hz.wangdashe.top/gtdflcdvip.html

for my $x (@arr) { print $x; }
来源：http://hz.nwbrower.top/gtlvfuqafb.html

[T46] Perl：哈希操作
来源：http://hz.birdmap.top/gtxkntxvkl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jianghu66.top/gtewghtkpi.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtnojcatsg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gzhubu.top/gtytqsxqkg.html

[T48] Perl：正则替换
来源：http://hz.zhoulong.xyz/gtnzwisclb.html

$s =~ s/old/new/g;
来源：http://hz.fzhhl.top/gteqgzfxgg.html

[T49] Perl：函数
来源：http://hz.zdqjudy.top/gtrzkufpet.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtbpajdhsx.html

[T50] Perl：逐行读文件
来源：http://hz.zhiwuduotai.top/gttcdtpmlf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ybcxt.top/gthnxvnimo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xingfuxueyuan.xyz/gtpkkufycd.html

[T51] Scala：Hello World
来源：http://hz.yvedp.cn/gtkewhptmv.html

println("Hello")
来源：http://hz.birdmap.top/gthxpdroxr.html

[T52] Scala：变量
来源：http://hz.kuanghao11.cn/gtslaerlhi.html

val a = 1;  var b = 2
来源：http://hz.jinyuanbaomall.cn/gtthknyfnn.html

[T53] Scala：字符串插值
来源：http://hz.mhx1999.top/gtcvavjwun.html

s"值: $b"
来源：http://hz.hnqzz.top/gtlvyhjjlo.html

[T54] Scala：集合映射
来源：http://hz.zhixingplan.top/gtjenaecrp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yvedp.cn/gtmucpgnks.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtimylswnc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fzhhl.top/gtpzqfwtce.html

[T56] Scala：样例类
来源：http://hz.fengsongda.top/gtjsedszgx.html

case class User(name: String, age: Int)
来源：http://hz.shangyingyoupin.top/gtwzehmdbk.html

[T57] Scala：模式匹配
来源：http://hz.hnqzz.top/gtakrxfhwn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yvedp.cn/gtweftqzhh.html

[T58] Scala：函数定义
来源：http://hz.yueranfly.top/gtrlsevgxa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.mhx1999.top/gtbgjygqlr.html

[T59] Scala：循环
来源：http://hz.hfpthk.cn/gtegrtpujw.html

for (i <- 1 to 10) println(i)
来源：http://hz.hysaishi.cn/gtzowfbzuj.html

[T60] Scala：折叠
来源：http://hz.zhoulong.xyz/gtuyuikljr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnxiangtu.top/gtbiuyfuxa.html

================================================================================
来源：http://hz.zhoulong.xyz/gtihxpdkos.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ybcxt.top/gtqbcnutni.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqvqrewze.html

[U01] Py：创建虚拟环境
来源：http://hz.shangyingyoupin.top/gtozogvioy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aizwys.cn/gtecbcajqw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhijiandao.cn/gtkoevphsd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cashguo.top/gtzberiifr.html

[U03] Py：加载 .env 配置
来源：http://hz.c1oappe.top/gtigkqposj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuanzhike.top/gtgksrmipa.html

[U04] Py：变量调试打印
来源：http://hz.316326.xyz/gtyqstzqkk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ivvv.top/gtgtoqtktn.html


<!-- 参考信息 -->