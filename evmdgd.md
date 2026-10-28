代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.guannengcc.top/gtyyuolbqo.html

[R64] 结束进程
来源：http://hz.sweek.top/gtsqkokdsc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aizwys.cn/gtorllttkk.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gtpcqaynuf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtvecwvrzl.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtduisybej.html

crontab -e;  crontab -l
来源：http://hz.fengsongda.top/gtsmqwuzjt.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigfzy.top/gtkpciaava.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtwcvbwqiw.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gtvxhtlgag.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gtbktjghwm.html

[R69] 生成随机密码
来源：http://hz.havefunace.top/gtohlfbrgo.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuanzx.com/gtljzfwomg.html

[R70] 时间戳与互转
来源：http://hz.guowangkeji.top/gthwbdzcad.html

date +%s;  date -d @1700000000
来源：http://hz.ehwqpu.com/gtemyqoybw.html

[R71] 日期格式化
来源：http://hz.jqgfzy.top/gtlydgnxas.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtazwkdopg.html

[R72] 等待端口就绪
来源：http://hz.316326.xyz/gtsxnjwubu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.haohaochexian.top/gtvantnsru.html

[R73] 分割大日志
来源：http://hz.hnqzz.top/gtjygbflwm.html

split -l 1000 big.log part_
来源：http://hz.wangshuangyany.cn/gtchtvjmcs.html

[R74] 批量重命名
来源：http://hz.aibaodan.cn/gtgpvgvtyr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aizwys.cn/gtdnjfjkqf.html

[R75] 导出环境变量
来源：http://hz.sufxvd.cn/gtnzxfikhh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cashguo.top/gtywtttvjo.html

[R76] 使用临时文件
来源：http://hz.iojbl.cn/gtmvxqyznf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtnbottiwg.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangtech.top/gtozxgefgh.html

read -rp "请输入: " ans
来源：http://hz.jinqigfzy.top/gtltrishcz.html

[R78] 交互式菜单
来源：http://hz.hfpthk.cn/gtzhexaleh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtfpkiwdbg.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtqlqpctvp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtzsqofiqj.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gthodrqlwz.html

time ./run.sh
来源：http://hz.cqqwz.cn/gtiwxewsnm.html

================================================================================
来源：http://hz.ehwqpu.com/gtqkjdxptp.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gtraikshkg.html

================================================================================
来源：http://hz.316326.xyz/gtpchoqaar.html

[S01] C：Hello World
来源：http://hz.andypj.xyz/gtcogsfoyt.html

#include <stdio.h>
来源：http://hz.ivvv.top/gtwclveijz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuetiantiany.cn/gtqttcugdg.html

[S02] C：变量与格式化输出
来源：http://hz.pengpengdd.cyou/gtdtijsacj.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangshuangyany.cn/gtphkhxcvh.html

[S03] C：读入整数
来源：http://hz.snrcjt.cn/gtmwcsukjz.html

int x; scanf("%d", &x);
来源：http://hz.hammf.cn/gtyzjupgjh.html

[S04] C：字符串复制
来源：http://hz.gogol.net.cn/gtlwcudmqf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daria6918.cn/gtcpkiaodt.html

[S05] C：字符串长度
来源：http://hz.hnxiangtu.top/gtwanyxfzy.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtqeaomxqc.html

[S06] C：字符串比较
来源：http://hz.sxryk.cn/gtflbszyle.html

strcmp(a, b) == 0
来源：http://hz.kuanghao11.cn/gtfxpglrje.html

[S07] C：数组遍历求和
来源：http://hz.dianchejie.cn/gtazxtyodg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jiagoushi.top/gtpaetupmy.html

[S08] C：动态内存分配与释放
来源：http://hz.chenzaomai.com/gtyxotnnyv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtujfxkviz.html

[S09] C：结构体定义与初始化
来源：http://hz.bjfxy.top/gtldkzfobw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hywenlv.cn/gtfupqbgio.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtnpdetefv.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtezfjrsog.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtfcdixkkz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xylfe.cn/gtdaxfbbdr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtbukiiwns.html

fclose(f);
来源：http://hz.yanxiufei.cn/gtjiqdbsil.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtqtjyhnok.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gthxtfnayp.html

[S13] C：宏定义
来源：http://hz.ppjwa.cn/gtgklwqtnb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhoulong.xyz/gtcnagdpxb.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtgntudril.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhiwuduotai.top/gtwwaqbaql.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gtwqtfacrq.html

(double) a / b
来源：http://hz.shuidangran.top/gtzwwcgthn.html

[S16] C：位操作置位
来源：http://hz.pengpengdd.cyou/gttqkovdzi.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtkynnijde.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtcekfgbbn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtdihjmdcb.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gtibktthpe.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtfjcprvin.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gtvohgweub.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtolnmiaii.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtygrdsmdu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtcxeuqjeb.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gtcvxzpkgg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.9152youxi.cn/gtfarsltoq.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtshdbfvav.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.kuanghao11.cn/gtzraxbqcr.html

[S23] C：随机数
来源：http://hz.c1oappe.top/gthrmyryio.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guannengcc.top/gtdbowvwuw.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gteyeorewo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtftokipjk.html

[S25] C：内存拷贝
来源：http://hz.aibaodan.cn/gtljqwxyyc.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtfplzjioa.html

[S26] C：内存清零
来源：http://hz.gotoacloud.top/gtivyklhaq.html

memset(a, 0, sizeof a);
来源：http://hz.zhaomingkeji.xyz/gtvgpjuhvr.html

[S27] C：定义常量
来源：http://hz.guowangkeji.top/gtrluiwxql.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtriwwwuxi.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtmdabqfif.html

static int counter = 0;
来源：http://hz.pengpengdd.cyou/gtjxflbexi.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtqxygaitx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xingfuxueyuan.xyz/gtgzbzwzfd.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtqkquuihe.html

#ifndef X_H
来源：http://hz.yj20258.top/gtndrfjcif.html

#define X_H
来源：http://hz.shangyingyoupin.top/gtxuwqqmyt.html

#endif
来源：http://hz.yj20258.top/gtbfsbifpd.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtksnqqrnn.html

#include <iostream>
来源：http://hz.pengpengdd.cyou/gtzrjxuiwx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhengqikj.top/gtfqeylsxb.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtwdtnqhpb.html

std::string s = "hi";  s += "!";
来源：http://hz.snrcjt.cn/gtkkkdcoie.html

[S33] C++：vector 增删
来源：http://hz.snrcjt.cn/gtxmheuzks.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtbyxhvouo.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtdflqsbcl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gtccvnizpc.html

[S35] C++：map
来源：http://hz.xinyue.icu/gtlaprcpab.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gthzuntkyb.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gtzkhbszii.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtchyjfylh.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtsqircgtu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtzcxnxdgs.html

[S38] C++：排序
来源：http://hz.yongpay.top/gtxdchblff.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangkeji.top/gtyiscpbvv.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtjojycjmc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xuetiantiany.cn/gtcrdnnlun.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangkeji.top/gtdzqjzxdy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.52xcode.cn/gtdiovaveg.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtehopyvud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtxpfaxyjd.html

[S42] C++：继承与虚函数
来源：http://hz.xuetiantiany.cn/gtkundhmeb.html

class B : public Base { public: void f() override {} };
来源：http://hz.kuanghao11.cn/gtvccevlxn.html

[S43] C++：智能指针
来源：http://hz.jinqigufen.top/gtheirebll.html

auto p = std::make_unique<int>(5);
来源：http://hz.ybcxt.top/gtkcchrkyy.html

[S44] C++：引用传参
来源：http://hz.fzhhl.top/gtwtngdqgf.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtxfyvpeai.html

[S45] C++：lambda
来源：http://hz.dianchejie.cn/gtnqdihgvr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.quarkkingdee.top/gtadayvsfa.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gttxwctgtp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtoddfvzsx.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangdashe.top/gtyyryrqij.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.snrcjt.cn/gtorreuiml.html

[S48] C++：逐行读文件
来源：http://hz.svipenyu.cn/gttdyhjpkm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtszpaqbri.html

while (std::getline(in, line)) { }
来源：http://hz.cheryme.top/gtvyicgjpk.html

[S49] C++：写文件
来源：http://hz.svipenyu.cn/gthabkjivd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhoulong.xyz/gttzzgqiqi.html

[S50] C++：格式化数字
来源：http://hz.zhongyouzk.top/gttjtzzkdg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hysaishi.cn/gtcppqxaox.html

[S51] C++：显式类型转换
来源：http://hz.kuanghao11.cn/gtchdnveug.html

static_cast<double>(a) / b
来源：http://hz.gaohongyu789.top/gthqyuzarl.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gtkduzdlnz.html

int size() const noexcept { return n_; }
来源：http://hz.yvedp.cn/gtiehtpeln.html

[S53] C++：移动语义
来源：http://hz.c1oappe.top/gthsrxyoov.html

std::vector<int> w = std::move(v);
来源：http://hz.svipenyu.cn/gtugcfphba.html

[S54] C++：异常处理
来源：http://hz.jlsjyb.cn/gtpkjsedto.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangshuangyany.cn/gtoblxdslk.html

[S55] C++：结构化绑定
来源：http://hz.hongshengwenyu.top/gtbzfguhpx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hysaishi.cn/gtpttgnawt.html

[S56] C++：optional
来源：http://hz.hammf.cn/gtktmicikd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gtnnownpct.html

[S57] C++：编译期常量
来源：http://hz.cqqwz.cn/gtgmcnpdaa.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gtjqndtsgd.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtfrhatftk.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258.top/gtzpxezowi.html

[S59] C++：静态断言
来源：http://hz.daria6918.cn/gtcnproicd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangshuangyany.cn/gtyfzytbna.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gtnjjokbmm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hywenlv.cn/gtlhzhugfv.html

================================================================================
来源：http://hz.cheryme.top/gtwexdtgge.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtazqfeift.html

================================================================================
来源：http://hz.316326.xyz/gtugganebt.html

[T01] Kotlin：Hello World
来源：http://hz.daria6918.cn/gtdxfhxake.html

println("Hello")
来源：http://hz.c1oappe.top/gtuorvvlxp.html

[T02] Kotlin：变量
来源：http://hz.ppjwa.cn/gtwkzfdiiy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fzhhl.top/gtdqwfofwm.html

[T03] Kotlin：字符串模板
来源：http://hz.quarkkingdee.top/gtsuygmsra.html

"值: $b"
来源：http://hz.yongpay.top/gthdaqkglt.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtqpnbxdrr.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtayqfgfkx.html

[T05] Kotlin：when 表达式
来源：http://hz.daria6918.cn/gtgpekcxte.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtdtmzayak.html

[T06] Kotlin：集合映射
来源：http://hz.fengsongda.top/gtgiqnsklj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.redwolf501.top/gtciihuzup.html

[T07] Kotlin：集合过滤
来源：http://hz.52xcode.cn/gtfgbvmxaj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhongyouzk.top/gtxanjxeqo.html

[T08] Kotlin：数据类
来源：http://hz.xziqi.cn/gtjskfsntn.html

data class User(val name: String, val age: Int)
来源：http://hz.iojbl.cn/gtufdhjxtj.html

[T09] Kotlin：扩展函数
来源：http://hz.0kj1m.cn/gtrqvkshyc.html

fun String.exclaim() = this + "!"
来源：http://hz.nwbrower.top/gtenvasmud.html

[T10] Kotlin：默认参数
来源：http://hz.feifeiyinyue.top/gtadjnpoyt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtgyakvdto.html

[T11] Kotlin：协程
来源：http://hz.9152youxi.cn/gtvbnkjxii.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydzc1.top/gtxzzydslu.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtsvjyxfum.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gttfaelmrc.html

[T13] Kotlin：只读 Map
来源：http://hz.yueranfly.top/gtfmjiqijj.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gtfszwufrg.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtntkknkuq.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtobpyzjjr.html

[T15] Kotlin：接口
来源：http://hz.jinghuilouyu.cn/gtjvanvoif.html

interface Shape { fun area(): Double }
来源：http://hz.yj202588.top/gtqvfatcqm.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtojwmzkxq.html

print("Hello")
来源：http://hz.xuanzx.com/gtowdplzfs.html

[T17] Swift：变量与常量
来源：http://hz.jiagoushi.top/gtyglokzsj.html

var a = 1;  let b = 2
来源：http://hz.zhiwuduotai.top/gthnsufoml.html

[T18] Swift：字符串插值
来源：http://hz.feifeiyinyue.top/gtvgzgztrs.html

"值: \(b)"
来源：http://hz.shanyushiyangtech.top/gtzcyxcuve.html

[T19] Swift：可选绑定
来源：http://hz.hnqzz.top/gtjibtnbxr.html

if let n = opt { print(n) }
来源：http://hz.wangshuangyany.cn/gtykprafhj.html

[T20] Swift：数组操作
来源：http://hz.vqdsnc.cn/gtuzlmkqqn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gtkgazxqxi.html

[T21] Swift：遍历
来源：http://hz.shuidangran.top/gtoxopwvhf.html

for x in a { print(x) }
来源：http://hz.andypj.xyz/gtgkubxuvs.html

[T22] Swift：字典
来源：http://hz.hammf.cn/gtyeumoljp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xingfuxueyuan.xyz/gtsnyxkxhc.html

[T23] Swift：函数
来源：http://hz.c1oappe.top/gtudlcdgve.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.feifeiyinyue.top/gtqgopwwah.html

[T24] Swift：闭包
来源：http://hz.pengpengdd.cyou/gtavyoyyeg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtfhvpodzg.html

[T25] Swift：结构体
来源：http://hz.sufxvd.cn/gtzqkqlcfb.html

struct P { var x: Int }
来源：http://hz.smart0.xyz/gtcvbawvjb.html

[T26] Swift：类与重写
来源：http://hz.yonumen.top/gtbqhreovx.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gtdflzklsd.html

[T27] Swift：错误处理
来源：http://hz.yueranfly.top/gtftyvmxwj.html

do { try f() } catch { print(error) }
来源：http://hz.tianlin.xyz/gtbbvnrfmi.html

[T28] Swift：枚举
来源：http://hz.fzhhl.top/gtenbxhawu.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtkedgknbf.html

[T29] Swift：guard 提前返回
来源：http://hz.9152youxi.cn/gtotosamag.html

guard let x = opt else { return }
来源：http://hz.daria6918.cn/gtkzxeqooz.html

[T30] Swift：协议
来源：http://hz.jinqigfzy.top/gtuxqdvxxl.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtqgojwisx.html

[T31] Lua：Hello World
来源：http://hz.yonumen.top/gtxkhlhfda.html

print("Hello")
来源：http://hz.jiagoushi.top/gtwzjwjvng.html

[T32] Lua：局部变量
来源：http://hz.chenlongwang.top/gtsuzofxkk.html

local a = 1
来源：http://hz.cqqwz.cn/gthgmasgtn.html

[T33] Lua：表（数组）
来源：http://hz.sufxvd.cn/gtmfshgigg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sweek.top/gtiznqeasp.html

[T34] Lua：遍历表
来源：http://hz.sysykeji.top/gtjifrnhvv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guowangkeji.top/gtbrwrkdge.html

[T35] Lua：字典表
来源：http://hz.tian-w.cn/gtvyspjxmf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuanzx.com/gtxofmkrlz.html

[T36] Lua：函数
来源：http://hz.ybcxt.top/gtjumsiuab.html

function add(a, b) return a + b end
来源：http://hz.jqgfzy.top/gttcezqyvb.html

[T37] Lua：字符串拼接
来源：http://hz.daxiang520.top/gtkidapivn.html

"a" .. "b"
来源：http://hz.fengsongda.top/gtcwujqtcc.html

[T38] Lua：条件
来源：http://hz.ywan-chungtsiang.top/gtflzaexbg.html

if x > 0 then print("正") end
来源：http://hz.yvedp.cn/gtmppblljb.html

[T39] Lua：模式匹配
来源：http://hz.daria6918.cn/gtnbuvjcdz.html

string.find(s, "%d+")
来源：http://hz.xingfuxueyuan.xyz/gtzkgasqnn.html

[T40] Lua：元表
来源：http://hz.ydjk.org.cn/gtwmdymsdd.html

setmetatable({}, { __index = base })
来源：http://hz.jlsjyb.cn/gthtajtwau.html

[T41] Perl：Hello World
来源：http://hz.zhaomingkeji.xyz/gtjqobkkcp.html

print "Hello\n";
来源：http://hz.ehwqpu.com/gtioqmrytn.html

[T42] Perl：变量类型
来源：http://hz.zhaomingkeji.xyz/gtyfyvpesi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258888.top/gtjcdnzeyl.html

[T43] Perl：字符串插值
来源：http://hz.9152youxi.cn/gtvudceghy.html

"值: $a"
来源：http://hz.jqgufenzy.top/gtizarvksr.html

[T44] Perl：条件
来源：http://hz.nanxinkj.top/gtxlxkscwn.html

if ($a > 0) { print "正"; }
来源：http://hz.zhiwuduotai.top/gtizuecafw.html

[T45] Perl：数组遍历
来源：http://hz.yonumen.top/gtpbkhxftk.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtlbyydprf.html

[T46] Perl：哈希操作
来源：http://hz.hfpthk.cn/gtuvsmbcfo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuetiantiany.cn/gtfyslxgmf.html

[T47] Perl：正则捕获
来源：http://hz.snrcjt.cn/gtrnnmibzw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtbptvoqmx.html

[T48] Perl：正则替换
来源：http://hz.0kj1m.cn/gthdndflln.html

$s =~ s/old/new/g;
来源：http://hz.guannengcc.top/gtvbndycxj.html

[T49] Perl：函数
来源：http://hz.9152youxi.cn/gtvemxzxdu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtzsdttdxn.html

[T50] Perl：逐行读文件
来源：http://hz.ivvv.top/gtpwnciezd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.redwolf501.top/gtidwscaup.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtimzjxjel.html

[T51] Scala：Hello World
来源：http://hz.cdnleiting.top/gtxfohxpac.html

println("Hello")
来源：http://hz.iojbl.cn/gtzcdcehgg.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gtynynfrne.html

val a = 1;  var b = 2
来源：http://hz.ydzc1.top/gtqyivwtua.html

[T53] Scala：字符串插值
来源：http://hz.cheryme.top/gtthcqoizs.html

s"值: $b"
来源：http://hz.yuanzhike.top/gtcxdzehay.html

[T54] Scala：集合映射
来源：http://hz.cheryme.top/gtkbxxmgge.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.smart0.xyz/gtngzqbpfr.html

[T55] Scala：集合过滤
来源：http://hz.zhijiandao.cn/gtrkpppssb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hysaishi.cn/gtybaqsuth.html

[T56] Scala：样例类
来源：http://hz.hywenlv.cn/gthoemgkrh.html

case class User(name: String, age: Int)
来源：http://hz.jiagoushi.top/gtodoxuhdc.html

[T57] Scala：模式匹配
来源：http://hz.jqgfzy.top/gtoumumizf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.birdmap.top/gtxloqsbht.html

[T58] Scala：函数定义
来源：http://hz.316326.xyz/gtzxfceipq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yuxming.cn/gttrpcdtbt.html

[T59] Scala：循环
来源：http://hz.cdnleiting.top/gtafeipusu.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj20258888.top/gtnzvivlks.html

[T60] Scala：折叠
来源：http://hz.yueranfly.top/gthmksdgjd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gtohwcgiim.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdtavbhut.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gteoknrqjm.html

================================================================================
来源：http://hz.wangdashe.top/gtuywgeimd.html

[U01] Py：创建虚拟环境
来源：http://hz.daria6918.cn/gttzkyjegm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.haohaochexian.top/gtgwiqhmlr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinyuanbaomall.cn/gtzzycrpbb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sxryk.cn/gtooaqupby.html

[U03] Py：加载 .env 配置
来源：http://hz.havefunace.top/gtommhnkdj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtgaccmbnr.html

[U04] Py：变量调试打印
来源：http://hz.bjfxy.top/gttxrfjsyo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtdqdzelrw.html


<!-- 参考信息 -->