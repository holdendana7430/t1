代发 wailian999

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtsgkgxrqz.html

[R62] 找最占空间的文件
来源：http://hz.cashguo.top/gtzjzovumt.html

du -ah . | sort -rh | head -10
来源：http://hz.chenjidiqi.icu/gtlllzrsix.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtttfyfjvn.html

free -h;  ps aux | grep nginx
来源：http://hz.9152youxi.cn/gtesnvpppr.html

[R64] 结束进程
来源：http://hz.ppjwa.cn/gtkestahgx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtkobvtinz.html

[R65] 查看端口占用
来源：http://hz.zhengqikj.top/gtxvpqrojs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtyzwjhaxo.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtgzhsijfs.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtebgfjsdm.html

[R67] 生成随机十六进制串
来源：http://hz.xuanzx.com/gtgsfjsmvw.html

openssl rand -hex 16
来源：http://hz.mhx1999.top/gtoefayzvh.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtvebrxxmr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sweek.top/gtnaccnpei.html

[R69] 生成随机密码
来源：http://hz.jinghuilouyu.cn/gtgqwwaagp.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gtbxtyjsnl.html

[R70] 时间戳与互转
来源：http://hz.tianlin.xyz/gtmclhqntl.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigufen.top/gtdqtadisp.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtkugupjhu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtcccmfyvj.html

[R72] 等待端口就绪
来源：http://hz.redwolf501.top/gtlrqcvsul.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gttzmesbzq.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtzzbvyydp.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtsdcdrozj.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gtaazvxibn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.c1oappe.top/gthvzloxvo.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtoqtjwuuo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hongshengwenyu.top/gtbqhhbhid.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtndmkzaiv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtqgyermxa.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gtyebyohar.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gthbnbpasc.html

[R78] 交互式菜单
来源：http://hz.hammf.cn/gtdfrsvahn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jiagoushi.top/gtozoiykfd.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangkeji.top/gtkvovckvn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yonumen.top/gtcjsmfxsq.html

[R80] 查看脚本执行耗时
来源：http://hz.fengsongda.top/gtejtqdefd.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtrnyqwxks.html

================================================================================
来源：http://hz.shuidangran.top/gtztbnznye.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtkyeiaeob.html

================================================================================
来源：http://hz.cashguo.top/gtjpxzfpdt.html

[S01] C：Hello World
来源：http://hz.sxryk.cn/gtdrxxulqv.html

#include <stdio.h>
来源：http://hz.zycfv.cn/gtemrqfvuj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guowangkeji.top/gtfsjbymjc.html

[S02] C：变量与格式化输出
来源：http://hz.52xcode.cn/gtkewcoajf.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhengqikj.top/gtxqjzbnff.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtpjioqklh.html

int x; scanf("%d", &x);
来源：http://hz.gogol.net.cn/gtcmiouymy.html

[S04] C：字符串复制
来源：http://hz.gzhubu.top/gtcornoqip.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtmhzxhteq.html

[S05] C：字符串长度
来源：http://hz.ppjwa.cn/gtnzfdsnox.html

strlen(s)
来源：http://hz.yonumen.top/gtadhepffd.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gthrmwpvsp.html

strcmp(a, b) == 0
来源：http://hz.sweek.top/gttkuesazl.html

[S07] C：数组遍历求和
来源：http://hz.jlsjyb.cn/gthkmdsliy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guowangkeji.top/gtuimcezdh.html

[S08] C：动态内存分配与释放
来源：http://hz.yueranfly.top/gtrylcimyo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtspajcyca.html

[S09] C：结构体定义与初始化
来源：http://hz.haohaochexian.top/gtzyuujjap.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtpbxqrkla.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gteqgmtdkr.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gtjwxdtpnq.html

[S11] C：逐行读文件
来源：http://hz.cucudq.cn/gtxbcuhayw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtzqncptbx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtizewingw.html

fclose(f);
来源：http://hz.guannengcc.top/gtgrkjgsvy.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtfsjgqxop.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yangfankeji.com/gtkzaktbcu.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtfhfmexyl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dianchejie.cn/gtfbjhouyi.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtezldtouv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.kuanghao11.cn/gtieljeiht.html

[S15] C：类型转换
来源：http://hz.9152youxi.cn/gtncyhgrup.html

(double) a / b
来源：http://hz.iojbl.cn/gtanziazdi.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtvfeyhbit.html

x |= (1 << 3);
来源：http://hz.cdnleiting.top/gtcpjapdqz.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigfzy.top/gtxkclofjq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhixingplan.top/gtaxaqhknl.html

[S18] C：命令行参数
来源：http://hz.jlsjyb.cn/gtwqjfummr.html

int main(int argc, char **argv)
来源：http://hz.chenzaomai.com/gtkhbrokbq.html

[S19] C：快速排序
来源：http://hz.yongpay.top/gtqloxxdbn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtyyosxcjq.html

[S20] C：二分查找
来源：http://hz.zdqjudy.top/gtehscnxjz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtphoupvor.html

[S21] C：字符类别判断
来源：http://hz.havefunace.top/gtgpkxzsba.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtkpcxgngl.html

[S22] C：字符串转数字
来源：http://hz.zhoulong.xyz/gtyvozgjfl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.bjfxy.top/gtutyajvua.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtsuxevgml.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.snrcjt.cn/gtihftfqtp.html

[S24] C：获取本地时间
来源：http://hz.0kj1m.cn/gtymxyzzcb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gteppmcwdy.html

[S25] C：内存拷贝
来源：http://hz.jiagoushi.top/gtwhdbdimi.html

memcpy(dst, src, n);
来源：http://hz.svipenyu.cn/gtymequudi.html

[S26] C：内存清零
来源：http://hz.yj20258888.top/gtlsmydzth.html

memset(a, 0, sizeof a);
来源：http://hz.ydjk.org.cn/gticrxokco.html

[S27] C：定义常量
来源：http://hz.ydzc1.top/gtljyuhgwh.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtpkhhlzey.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtqssgmbfb.html

static int counter = 0;
来源：http://hz.jianghu66.top/gtgmcggfbu.html

[S29] C：变参函数
来源：http://hz.aizwys.cn/gtofftiqex.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.haohaochexian.top/gtcznayqri.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtfqjytwwp.html

#ifndef X_H
来源：http://hz.yanxiufei.cn/gtitxsgxsj.html

#define X_H
来源：http://hz.0kj1m.cn/gtfifosmie.html

#endif
来源：http://hz.bjfxy.top/gtfwgioyjh.html

[S31] C++：Hello World
来源：http://hz.zhiwuduotai.top/gtepnfciod.html

#include <iostream>
来源：http://hz.cucudq.cn/gtxepsazvw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtzpdglzij.html

[S32] C++：字符串
来源：http://hz.shanyushiyangkeji.top/gtekfdnqlu.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtfrftgnsb.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtuazjjxhw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gthrlamfrj.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtzgtagqms.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtituvujuy.html

[S35] C++：map
来源：http://hz.zhaomingkeji.xyz/gtpryytujj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtioyykdzm.html

[S36] C++：unordered_map
来源：http://hz.sufxvd.cn/gtwjpnbfan.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtdbuhhmkp.html

[S37] C++：set
来源：http://hz.pengpengdd.cyou/gtdqoohcvq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnqzz.top/gtejutzptq.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gtcyahehyu.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtwhixlhst.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gtotxzmwjt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnqzz.top/gtiqpetavt.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gtedyfltim.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydjk.org.cn/gtcmcecmls.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtjgzdrtuf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gtiajqshik.html

[S42] C++：继承与虚函数
来源：http://hz.hnxiangtu.top/gttojxjjid.html

class B : public Base { public: void f() override {} };
来源：http://hz.52xcode.cn/gtrqzezmtg.html

[S43] C++：智能指针
来源：http://hz.yj20258.top/gtlnwqpdxm.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtthdvehad.html

[S44] C++：引用传参
来源：http://hz.hysaishi.cn/gtfjuviaih.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtcusovlmt.html

[S45] C++：lambda
来源：http://hz.daria6918.cn/gtieanfnxn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtwyrnoiop.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtjbwhgwcw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtdkxrcmac.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtxzmgacjx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cheryme.top/gtkzgjmcoz.html

[S48] C++：逐行读文件
来源：http://hz.gzhubu.top/gtzjluxvqe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtnzjjyyph.html

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtpwppcfnv.html

[S49] C++：写文件
来源：http://hz.haohaochexian.top/gtynfufywn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtsabrpgul.html

[S50] C++：格式化数字
来源：http://hz.hfpthk.cn/gtxgonoycl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.smart0.xyz/gtgnaiedgo.html

[S51] C++：显式类型转换
来源：http://hz.jianghu66.top/gticcqkjel.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangkeji.top/gtlclxxstn.html

[S52] C++：const 与 noexcept
来源：http://hz.zdqjudy.top/gttqaaebux.html

int size() const noexcept { return n_; }
来源：http://hz.c1oappe.top/gtuxnegckn.html

[S53] C++：移动语义
来源：http://hz.daxiang520.top/gtcvwklglp.html

std::vector<int> w = std::move(v);
来源：http://hz.9152youxi.cn/gtnuyxcbpq.html

[S54] C++：异常处理
来源：http://hz.zhiwuduotai.top/gtwvnvxlar.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jlsjyb.cn/gtdqzplxgu.html

[S55] C++：结构化绑定
来源：http://hz.gogol.net.cn/gtndewxdps.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gteumdcazv.html

[S56] C++：optional
来源：http://hz.52xcode.cn/gtrtdefvxg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zdqjudy.top/gtpusrxhzy.html

[S57] C++：编译期常量
来源：http://hz.mhx1999.top/gtpaftpbze.html

constexpr int N = 10;
来源：http://hz.9152youxi.cn/gtedezdjzt.html

[S58] C++：命名空间
来源：http://hz.hnqzz.top/gtfusibyzh.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenzaomai.com/gtodnbyqcd.html

[S59] C++：静态断言
来源：http://hz.wangshuangyany.cn/gtujzhbfmf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuanzx.com/gtdgnbrmuu.html

[S60] C++：遍历并删除元素
来源：http://hz.cucudq.cn/gtwdqnucvc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yanxiufei.cn/gtbyhjotfq.html

================================================================================
来源：http://hz.hywenlv.cn/gtkhctymot.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtnmgicfai.html

================================================================================
来源：http://hz.yangfankeji.com/gtqbsbrzsj.html

[T01] Kotlin：Hello World
来源：http://hz.chenlongwang.top/gtumsbfmhm.html

println("Hello")
来源：http://hz.xuanzx.com/gtleicobkm.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gttepheuux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gthntdwvus.html

[T03] Kotlin：字符串模板
来源：http://hz.snrcjt.cn/gtwqtbmypa.html

"值: $b"
来源：http://hz.xinyue.icu/gtcvrtlrvr.html

[T04] Kotlin：空安全
来源：http://hz.nanxuanxn.top/gtoikpkbgp.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtgcvsixsh.html

[T05] Kotlin：when 表达式
来源：http://hz.mhx1999.top/gtydqurhlx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gtewmypcyf.html

[T06] Kotlin：集合映射
来源：http://hz.yuanzhike.top/gtgmquekfe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtllwbhrrs.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gtzsovqlrb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.meibo888.top/gtfafdymgz.html

[T08] Kotlin：数据类
来源：http://hz.ydjk.org.cn/gtqjkaqvfy.html

data class User(val name: String, val age: Int)
来源：http://hz.yj20258888.top/gtvdvphzur.html

[T09] Kotlin：扩展函数
来源：http://hz.feifeiyinyue.top/gtuddvfmkh.html

fun String.exclaim() = this + "!"
来源：http://hz.guowangkeji.top/gtokyvhfsh.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigfzy.top/gtkvoiypic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnxiangtu.top/gtzdlfqhyb.html

[T11] Kotlin：协程
来源：http://hz.zhongyouzk.top/gtxggazzhs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.svipenyu.cn/gtwxcpgjop.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtyanlhmkm.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtewmglaya.html

[T13] Kotlin：只读 Map
来源：http://hz.jiagoushi.top/gtuwdwxfnr.html

val m = mapOf("a" to 1)
来源：http://hz.zhoulong.xyz/gtckkjuxno.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangtech.top/gtyiklomdq.html

for (i in 1..10) println(i)
来源：http://hz.nanxinkj.top/gtiwbofqaw.html

[T15] Kotlin：接口
来源：http://hz.xziqi.cn/gtpyvxcgze.html

interface Shape { fun area(): Double }
来源：http://hz.guannengcc.top/gtfvbslfzo.html

[T16] Swift：Hello World
来源：http://hz.316326.xyz/gttmawaeuc.html

print("Hello")
来源：http://hz.jiagoushi.top/gtprohkdhy.html

[T17] Swift：变量与常量
来源：http://hz.ehwqpu.com/gtkwlhpxen.html

var a = 1;  let b = 2
来源：http://hz.fzhhl.top/gtoxhvrdse.html

[T18] Swift：字符串插值
来源：http://hz.chenlongwang.top/gtfxwzejml.html

"值: \(b)"
来源：http://hz.shangyingyoupin.top/gtfeqyljxo.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gtygzytfix.html

if let n = opt { print(n) }
来源：http://hz.c1oappe.top/gtujtqlicl.html

[T20] Swift：数组操作
来源：http://hz.andypj.xyz/gtpriatbmd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gtlxysedsd.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtihwcdhwq.html

for x in a { print(x) }
来源：http://hz.svipenyu.cn/gtgqpnclqx.html

[T22] Swift：字典
来源：http://hz.havefunace.top/gtvtfwmlcn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cdnleiting.top/gtawmdicmx.html

[T23] Swift：函数
来源：http://hz.smart0.xyz/gtqeggivxu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.haohaochexian.top/gtolbkgbse.html

[T24] Swift：闭包
来源：http://hz.hammf.cn/gtlqiwqiwn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.aizwys.cn/gtdfgjvmpc.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gtewppgmzc.html

struct P { var x: Int }
来源：http://hz.jiagoushi.top/gtvfqizlre.html

[T26] Swift：类与重写
来源：http://hz.jinqigufen.top/gttinknyii.html

class A: Base { override func f() {} }
来源：http://hz.smart0.xyz/gtkhvuufcz.html

[T27] Swift：错误处理
来源：http://hz.tanke756.top/gtrvqjklhy.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigufen.top/gtvdujktty.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtsglniqwy.html

enum Color { case red, green }
来源：http://hz.nanxuanxn.top/gttdojxjks.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangkeji.top/gtrirpjcvx.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtlzvfqjxd.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtbuitlsch.html

protocol Shape { func area() -> Double }
来源：http://hz.hongshengwenyu.top/gturmhmnic.html

[T31] Lua：Hello World
来源：http://hz.quarkkingdee.top/gtojybjktp.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtzsygjxfd.html

[T32] Lua：局部变量
来源：http://hz.dianchejie.cn/gtrhhfkbuj.html

local a = 1
来源：http://hz.jinghuilouyu.cn/gtrkuxyuih.html

[T33] Lua：表（数组）
来源：http://hz.bjfxy.top/gtyvvjuirx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yvedp.cn/gtpcjwdjea.html

[T34] Lua：遍历表
来源：http://hz.gotoacloud.top/gtcndxaijv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jlsjyb.cn/gtjghggztj.html

[T35] Lua：字典表
来源：http://hz.jqgufenzy.top/gtwzfouhms.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yueranfly.top/gtdpptfnip.html

[T36] Lua：函数
来源：http://hz.redwolf501.top/gtzgwxdgxl.html

function add(a, b) return a + b end
来源：http://hz.ppjwa.cn/gtttehklic.html

[T37] Lua：字符串拼接
来源：http://hz.redwolf501.top/gtnyjdsfzs.html

"a" .. "b"
来源：http://hz.wangshuangyany.cn/gtahriwyga.html

[T38] Lua：条件
来源：http://hz.yonumen.top/gtlzttkeyz.html

if x > 0 then print("正") end
来源：http://hz.zhaomingkeji.xyz/gtfvorojve.html

[T39] Lua：模式匹配
来源：http://hz.jinyuanbaomall.cn/gtpthvvlyt.html

string.find(s, "%d+")
来源：http://hz.nanxuanxn.top/gttymbjdau.html

[T40] Lua：元表
来源：http://hz.jinqigfzy.top/gthdsmkdel.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gthpnovmhe.html

[T41] Perl：Hello World
来源：http://hz.chenzaomai.com/gtkdbbgqpa.html

print "Hello\n";
来源：http://hz.snrcjt.cn/gtndtdznru.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtehnxqbiz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gtxvikyvqa.html

[T43] Perl：字符串插值
来源：http://hz.0kj1m.cn/gtrlsmjwgu.html

"值: $a"
来源：http://hz.jqgufenzy.top/gtlrqgavjq.html

[T44] Perl：条件
来源：http://hz.yj20258.top/gtjissksup.html

if ($a > 0) { print "正"; }
来源：http://hz.wangshuangyany.cn/gtsyvgtffu.html

[T45] Perl：数组遍历
来源：http://hz.yvedp.cn/gtfyffjqxy.html

for my $x (@arr) { print $x; }
来源：http://hz.vqdsnc.cn/gtsqhmrwsh.html

[T46] Perl：哈希操作
来源：http://hz.yj20258.top/gtrukvinfy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gthrchxagj.html

[T47] Perl：正则捕获
来源：http://hz.mhx1999.top/gtmydfguuf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ywan-chungtsiang.top/gtvznwuxxc.html

[T48] Perl：正则替换
来源：http://hz.fzhhl.top/gtpzgqrgdi.html

$s =~ s/old/new/g;
来源：http://hz.yj202588.top/gtugqdynob.html

[T49] Perl：函数
来源：http://hz.yongpay.top/gtejyclngw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxinkj.top/gtsxibwncl.html

[T50] Perl：逐行读文件
来源：http://hz.yongpay.top/gtuafvllca.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yanxiufei.cn/gtucxkiheo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jqgufenzy.top/gtcmbxkcgw.html

[T51] Scala：Hello World
来源：http://hz.jyoumei.cn/gtygvtwdjm.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtvzlofksq.html

[T52] Scala：变量
来源：http://hz.hnxiangtu.top/gtedxlluah.html

val a = 1;  var b = 2
来源：http://hz.ppjwa.cn/gteacozlgm.html

[T53] Scala：字符串插值
来源：http://hz.vqdsnc.cn/gteuibgiwj.html

s"值: $b"
来源：http://hz.bjfxy.top/gtxkjhtjvf.html

[T54] Scala：集合映射
来源：http://hz.hnqzz.top/gtqumjouuz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.redwolf501.top/gtxudsdxkw.html

[T55] Scala：集合过滤
来源：http://hz.wangshuangyany.cn/gtqgocusbf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigfzy.top/gtwxhxeqgd.html

[T56] Scala：样例类
来源：http://hz.dianchejie.cn/gtlsfzvtib.html

case class User(name: String, age: Int)
来源：http://hz.cdnleiting.top/gtqegmsmpx.html

[T57] Scala：模式匹配
来源：http://hz.dashuyun.cn/gtfgdbbcur.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fzhhl.top/gtoisovryw.html

[T58] Scala：函数定义
来源：http://hz.vqdsnc.cn/gtuwbmfwxh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ybcxt.top/gtuwgfedqh.html

[T59] Scala：循环
来源：http://hz.birdmap.top/gtzzycnbce.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtymggmbpy.html

[T60] Scala：折叠
来源：http://hz.yvedp.cn/gtnsdyugfm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gotoacloud.top/gtybmhihfc.html

================================================================================
来源：http://hz.wangdashe.top/gtfphpazem.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xinyue.icu/gtajlwtebv.html

================================================================================
来源：http://hz.chenjidiqi.icu/gthhdqyzzi.html

[U01] Py：创建虚拟环境
来源：http://hz.hfpthk.cn/gtpbcaparx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ybcxt.top/gthodapxeh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gtgrkmwusm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cqqwz.cn/gtolbmtjbw.html


<!-- 参考信息 -->