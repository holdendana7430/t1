代发 wailian999

df -h;  du -sh *
来源：http://hz.hongshengwenyu.top/gtogjmvyko.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gttxejmmta.html

du -ah . | sort -rh | head -10
来源：http://hz.shzxlz.cn/gtvftpwakg.html

[R63] 内存与进程
来源：http://hz.yj202588.top/gtwbyzcffs.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gtxsobuwtn.html

[R64] 结束进程
来源：http://hz.c1oappe.top/gtgaluhkwr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gtawzfzufn.html

[R65] 查看端口占用
来源：http://hz.ywan-chungtsiang.top/gtwwbjbdmf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hammf.cn/gtmkklhavo.html

[R66] 定时任务
来源：http://hz.kuanghao11.cn/gtadjqjjli.html

crontab -e;  crontab -l
来源：http://hz.0kj1m.cn/gtvckrlzil.html

[R67] 生成随机十六进制串
来源：http://hz.dianchejie.cn/gtbnfqslve.html

openssl rand -hex 16
来源：http://hz.shangyingyoupin.top/gttanclrak.html

[R68] 计算文件校验值
来源：http://hz.shangyingyoupin.top/gtczkygqhn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ybcxt.top/gtutozidrj.html

[R69] 生成随机密码
来源：http://hz.yueranfly.top/gtjbcvsmqz.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtcsksbmoq.html

[R70] 时间戳与互转
来源：http://hz.mhx1999.top/gtismphxpc.html

date +%s;  date -d @1700000000
来源：http://hz.kuanghao11.cn/gtjhvfgpgx.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtwwsihxgj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtmhxfmecj.html

[R72] 等待端口就绪
来源：http://hz.ydzc1.top/gtblrakqbm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtokixzbhq.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gtqbodqihm.html

split -l 1000 big.log part_
来源：http://hz.hfpthk.cn/gttvvtejti.html

[R74] 批量重命名
来源：http://hz.gogol.net.cn/gtfqfcynnm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gtzrutvizv.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtoazkapew.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gttppqmebi.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtunjwjdmb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtnilanfoa.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtvvzbcylu.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtucbmespm.html

[R78] 交互式菜单
来源：http://hz.jqgufenzy.top/gtmiotqoum.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtmeigufjt.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtotyjdbyg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtdwsmdhps.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gtnpgxkswu.html

time ./run.sh
来源：http://hz.yj20258888.top/gtykwafuca.html

================================================================================
来源：http://hz.0kj1m.cn/gtsswpfqxb.html

S. C / C++ 专题
来源：http://hz.wangdashe.top/gttfehlbcs.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthdzjyvat.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtcvbulfks.html

#include <stdio.h>
来源：http://hz.yanxiufei.cn/gtcywwicnt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gttwuvznnj.html

[S02] C：变量与格式化输出
来源：http://hz.zhoulong.xyz/gtlebfchoq.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuetiantiany.cn/gtspoipdot.html

[S03] C：读入整数
来源：http://hz.nanxinkj.top/gtlpgwhjua.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gtyhcisqbw.html

[S04] C：字符串复制
来源：http://hz.dianchejie.cn/gthhyjgwiy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shuidangran.top/gtgchqduhr.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtczmpaaxv.html

strlen(s)
来源：http://hz.ydzc1.top/gtycehfoiy.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gtuhqswngn.html

strcmp(a, b) == 0
来源：http://hz.iojbl.cn/gtwfrvprqk.html

[S07] C：数组遍历求和
来源：http://hz.yanxiufei.cn/gtdsgdsvmf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtbjnukdvg.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtldqqyhbi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hysaishi.cn/gtdvntcpib.html

[S09] C：结构体定义与初始化
来源：http://hz.shzxlz.cn/gtqyceevze.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtvaagkzfu.html

[S10] C：指针与解引用
来源：http://hz.ybcxt.top/gtskjyygle.html

int *p = &a;  *p = 5;
来源：http://hz.dashuyun.cn/gthejcbnpn.html

[S11] C：逐行读文件
来源：http://hz.zhijiandao.cn/gtobxctwll.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gtfjypkriu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtjwubxyii.html

fclose(f);
来源：http://hz.guowangkeji.top/gtofqvzlbe.html

[S12] C：写文件
来源：http://hz.hammf.cn/gtdvjsebcp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dashuyun.cn/gtkimjapec.html

[S13] C：宏定义
来源：http://hz.xziqi.cn/gtcslcbeuy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gthccoiqlf.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtgvgopaph.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtjnmkivhy.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gtxdyvwdbe.html

(double) a / b
来源：http://hz.aizwys.cn/gtxpnpsbxj.html

[S16] C：位操作置位
来源：http://hz.jinyuanbaomall.cn/gtgefqnord.html

x |= (1 << 3);
来源：http://hz.ywan-chungtsiang.top/gttjobvaeb.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gtdcuyczes.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtxiikldju.html

[S18] C：命令行参数
来源：http://hz.quarkkingdee.top/gtzupyhqcr.html

int main(int argc, char **argv)
来源：http://hz.jinqigufen.top/gtnixknebq.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gticdtoozl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtyhzxkoea.html

[S20] C：二分查找
来源：http://hz.jinqigfzy.top/gtzurllvsf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtkhvpsznr.html

[S21] C：字符类别判断
来源：http://hz.sufxvd.cn/gttnwldxdr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xylfe.cn/gtpbpaaxwh.html

[S22] C：字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtqswmyghl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.iojbl.cn/gtfzcwgzab.html

[S23] C：随机数
来源：http://hz.tanke756.top/gtdfqruuuk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtmeodgiid.html

[S24] C：获取本地时间
来源：http://hz.havefunace.top/gtstckecdv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.haohaochexian.top/gtwlwtvvki.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtswvaqrcd.html

memcpy(dst, src, n);
来源：http://hz.wangdashe.top/gtdmsxagcv.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtezbnxpci.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gtmsdtorcc.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtnrwpshby.html

const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtxjeirgjh.html

[S28] C：静态变量
来源：http://hz.jinghuilouyu.cn/gtdbamjvtr.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtgjhpkrlu.html

[S29] C：变参函数
来源：http://hz.jinyuanbaomall.cn/gtjsboktzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.iojbl.cn/gtjxpzewvy.html

[S30] C：头文件保护
来源：http://hz.havefunace.top/gtljmuewec.html

#ifndef X_H
来源：http://hz.ehwqpu.com/gtaiyuxhag.html

#define X_H
来源：http://hz.snrcjt.cn/gtwaifgyov.html

#endif
来源：http://hz.tanke756.top/gtyigoocoq.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtlzzwbbkl.html

#include <iostream>
来源：http://hz.zhaomingkeji.xyz/gthdkrzhil.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuanzx.com/gtaduuvugp.html

[S32] C++：字符串
来源：http://hz.ydjk.org.cn/gtwsmhxbds.html

std::string s = "hi";  s += "!";
来源：http://hz.snrcjt.cn/gtdxmutabh.html

[S33] C++：vector 增删
来源：http://hz.cucudq.cn/gtthbfhpie.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtxkqzkmwm.html

[S34] C++：遍历 vector
来源：http://hz.aizwys.cn/gtnhsnccud.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hammf.cn/gtetonijxu.html

[S35] C++：map
来源：http://hz.yuxming.cn/gtfukaohnz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtdmszahuc.html

[S36] C++：unordered_map
来源：http://hz.cdnleiting.top/gtaaylyscd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtkpemwqlt.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtsnrpvyjy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.birdmap.top/gtuninbsbn.html

[S38] C++：排序
来源：http://hz.pycfn.com/gtheijafmv.html

std::sort(v.begin(), v.end());
来源：http://hz.andypj.xyz/gtrzccsefp.html

[S39] C++：自定义比较器排序
来源：http://hz.tian-w.cn/gtrkwsawfl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tanke756.top/gtaongfxof.html

[S40] C++：查找元素
来源：http://hz.jlsjyb.cn/gtcnrfrhcb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtkriuorjd.html

[S41] C++：类与构造函数
来源：http://hz.gzhubu.top/gtgsdocmhq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxuanxn.top/gtyzrqvisd.html

[S42] C++：继承与虚函数
来源：http://hz.gogol.net.cn/gtocfzxovr.html

class B : public Base { public: void f() override {} };
来源：http://hz.nwbrower.top/gthhlqalgx.html

[S43] C++：智能指针
来源：http://hz.jiagoushi.top/gtdvmqispg.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gttslbsbbd.html

[S44] C++：引用传参
来源：http://hz.gaohongyu789.top/gtvvkhvqqg.html

void inc(int &x) { ++x; }
来源：http://hz.yonumen.top/gtiptrawym.html

[S45] C++：lambda
来源：http://hz.chenjidiqi.icu/gtkggojeiy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.52xcode.cn/gtcvczrjon.html

[S46] C++：函数模板
来源：http://hz.guannengcc.top/gtfeztuyya.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtrzyxtexk.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangtech.top/gtdtkpzout.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cheryme.top/gtcgznmajg.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtentryrbv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenzaomai.com/gtrqabhsub.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtksqtnikx.html

[S49] C++：写文件
来源：http://hz.9152youxi.cn/gtgnkjshox.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tanke756.top/gtfehroyse.html

[S50] C++：格式化数字
来源：http://hz.jiagoushi.top/gtwrcmvjpp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gtrfhitmsm.html

[S51] C++：显式类型转换
来源：http://hz.zhoulong.xyz/gtrheojqqq.html

static_cast<double>(a) / b
来源：http://hz.hongshengwenyu.top/gterjlaecw.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gtgvczgguf.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtdajalgvl.html

[S53] C++：移动语义
来源：http://hz.wangdashe.top/gtarhtwquj.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtdbblgalw.html

[S54] C++：异常处理
来源：http://hz.fzhhl.top/gtakqufbbt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtpeqliplh.html

[S55] C++：结构化绑定
来源：http://hz.jianghu66.top/gttyfylqqq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xylfe.cn/gtaeponnrb.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtjuyuvcbd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtrtwtlscb.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gttgycptqh.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gtkhvvxccb.html

[S58] C++：命名空间
来源：http://hz.smart0.xyz/gtztfxvcjh.html

namespace ns { int f() { return 1; } }
来源：http://hz.pengpengdd.cyou/gtyagicdtb.html

[S59] C++：静态断言
来源：http://hz.ppjwa.cn/gtjdzjmski.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shuidangran.top/gtevswofcu.html

[S60] C++：遍历并删除元素
来源：http://hz.tanke756.top/gtuhqyxlem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.birdmap.top/gtkihhzsyh.html

================================================================================
来源：http://hz.snrcjt.cn/gtdmvdilwz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gtulnluprg.html

================================================================================
来源：http://hz.sxryk.cn/gtvnyuyknm.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtupoyeseu.html

println("Hello")
来源：http://hz.zhixingplan.top/gtetherbvx.html

[T02] Kotlin：变量
来源：http://hz.wangdashe.top/gtsjyqwffp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtblhuahbz.html

[T03] Kotlin：字符串模板
来源：http://hz.zhengqikj.top/gttjbewgap.html

"值: $b"
来源：http://hz.chenzaomai.com/gtwddwjjah.html

[T04] Kotlin：空安全
来源：http://hz.dashuyun.cn/gtkxiimfqk.html

val n: String? = null;  n?.length
来源：http://hz.gotoacloud.top/gtlqjfrlmk.html

[T05] Kotlin：when 表达式
来源：http://hz.daria6918.cn/gtjwbogxsl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gtvjabhkrf.html

[T06] Kotlin：集合映射
来源：http://hz.cashguo.top/gtbdvoljnn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hfpthk.cn/gtyyupihcp.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gtlgakstpe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenzaomai.com/gttmqiwrkb.html

[T08] Kotlin：数据类
来源：http://hz.xuanzx.com/gtrengdluw.html

data class User(val name: String, val age: Int)
来源：http://hz.ybcxt.top/gtjsbgqpce.html

[T09] Kotlin：扩展函数
来源：http://hz.hysaishi.cn/gtefeoahso.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtkieqexql.html

[T10] Kotlin：默认参数
来源：http://hz.zycfv.cn/gtyabmbbxb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtocnauiuu.html

[T11] Kotlin：协程
来源：http://hz.vqdsnc.cn/gtdcqnrrwv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtsvouuurn.html

[T12] Kotlin：解构声明
来源：http://hz.ydzc1.top/gtkcbsmonh.html

val (a, b) = Pair(1, 2)
来源：http://hz.hfpthk.cn/gtpszrcsud.html

[T13] Kotlin：只读 Map
来源：http://hz.chenjidiqi.icu/gtzobhzzka.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gthhhbkbwx.html

[T14] Kotlin：循环
来源：http://hz.ybcxt.top/gtskktkkmq.html

for (i in 1..10) println(i)
来源：http://hz.aizwys.cn/gtthucdcfg.html

[T15] Kotlin：接口
来源：http://hz.gogol.net.cn/gtmdikixjf.html

interface Shape { fun area(): Double }
来源：http://hz.dashuyun.cn/gtprhzmwfk.html

[T16] Swift：Hello World
来源：http://hz.zycfv.cn/gtnwfawuxc.html

print("Hello")
来源：http://hz.mhx1999.top/gtrgpvonow.html

[T17] Swift：变量与常量
来源：http://hz.yj202588.top/gtavyqnrds.html

var a = 1;  let b = 2
来源：http://hz.shzxlz.cn/gtlhuaasnv.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gtzrxhruhk.html

"值: \(b)"
来源：http://hz.jlsjyb.cn/gtcgymjlgy.html

[T19] Swift：可选绑定
来源：http://hz.nwbrower.top/gtcqgrypky.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtqduopqua.html

[T20] Swift：数组操作
来源：http://hz.havefunace.top/gtfekhuikd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sufxvd.cn/gtxnablxlj.html

[T21] Swift：遍历
来源：http://hz.shanyushiyangtech.top/gtrqhfivcn.html

for x in a { print(x) }
来源：http://hz.shangyingyoupin.top/gtqlqummvl.html

[T22] Swift：字典
来源：http://hz.ivvv.top/gtvurjhmor.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cdnleiting.top/gtozyntxbc.html

[T23] Swift：函数
来源：http://hz.birdmap.top/gthdgzxcta.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gogol.net.cn/gtsjqincwt.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtxqjqbdmo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtxuodlrww.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtdvcuqcdz.html

struct P { var x: Int }
来源：http://hz.chenzaomai.com/gtuonlfslb.html

[T26] Swift：类与重写
来源：http://hz.xuetiantiany.cn/gtfcpnmcms.html

class A: Base { override func f() {} }
来源：http://hz.gogol.net.cn/gtiewugtux.html

[T27] Swift：错误处理
来源：http://hz.andypj.xyz/gtxxpxbxkm.html

do { try f() } catch { print(error) }
来源：http://hz.jqgufenzy.top/gtvamzqkhu.html

[T28] Swift：枚举
来源：http://hz.jlsjyb.cn/gtdtwzlgjv.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtjijttign.html

[T29] Swift：guard 提前返回
来源：http://hz.xziqi.cn/gtpgxhqxzb.html

guard let x = opt else { return }
来源：http://hz.yj20258888.top/gtupbontxo.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtgornilxy.html

protocol Shape { func area() -> Double }
来源：http://hz.shzxlz.cn/gtsddmeswv.html

[T31] Lua：Hello World
来源：http://hz.shuidangran.top/gtgowccdga.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtsvvtlwen.html

[T32] Lua：局部变量
来源：http://hz.chenlongwang.top/gtxjankezi.html

local a = 1
来源：http://hz.shangyingyoupin.top/gthcvlmarc.html

[T33] Lua：表（数组）
来源：http://hz.zhoulong.xyz/gtyxktsbmn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jianghu66.top/gtklplvoua.html

[T34] Lua：遍历表
来源：http://hz.hongshengwenyu.top/gtpwmpphxm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gtldpgzqpz.html

[T35] Lua：字典表
来源：http://hz.zhoulong.xyz/gtrvtegtrq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hfpthk.cn/gtnwrlkqgg.html

[T36] Lua：函数
来源：http://hz.yanxiufei.cn/gtgfaiwbcs.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtyusnpfdt.html

[T37] Lua：字符串拼接
来源：http://hz.shangyingyoupin.top/gtptkomluf.html

"a" .. "b"
来源：http://hz.gzhubu.top/gthwxhklzt.html

[T38] Lua：条件
来源：http://hz.guannengcc.top/gtimqbznit.html

if x > 0 then print("正") end
来源：http://hz.yuanzhike.top/gtrqkjvauy.html

[T39] Lua：模式匹配
来源：http://hz.jinqigufen.top/gtltmrlwlg.html

string.find(s, "%d+")
来源：http://hz.fzhhl.top/gtjssfrjce.html

[T40] Lua：元表
来源：http://hz.zhongyouzk.top/gtjttwrdrj.html

setmetatable({}, { __index = base })
来源：http://hz.jqgfzy.top/gtdqyxeitq.html

[T41] Perl：Hello World
来源：http://hz.zycfv.cn/gtvslphbux.html

print "Hello\n";
来源：http://hz.sysykeji.top/gthcmxuzgc.html

[T42] Perl：变量类型
来源：http://hz.gaohongyu789.top/gtwtteqzzt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zdqjudy.top/gtkqaqiuqp.html

[T43] Perl：字符串插值
来源：http://hz.jyoumei.cn/gthptnkluh.html

"值: $a"
来源：http://hz.hysaishi.cn/gtccmaqlws.html

[T44] Perl：条件
来源：http://hz.zycfv.cn/gtxoedgabj.html

if ($a > 0) { print "正"; }
来源：http://hz.vqdsnc.cn/gtckaxhiic.html

[T45] Perl：数组遍历
来源：http://hz.feifeiyinyue.top/gtqsmhwofi.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtsulkkuln.html

[T46] Perl：哈希操作
来源：http://hz.zhiwuduotai.top/gthxgpvelg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhaomingkeji.xyz/gthdoushww.html

[T47] Perl：正则捕获
来源：http://hz.zhaomingkeji.xyz/gtwgixiuga.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.tianlin.xyz/gtichgsrax.html

[T48] Perl：正则替换
来源：http://hz.nwbrower.top/gtetowcnsu.html

$s =~ s/old/new/g;
来源：http://hz.yuanzhike.top/gtmuqldnud.html

[T49] Perl：函数
来源：http://hz.quarkkingdee.top/gtuanafxgc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yongpay.top/gtcsdscqvv.html

[T50] Perl：逐行读文件
来源：http://hz.52xcode.cn/gtejvmiidb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.0kj1m.cn/gtfloxvezu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jlsjyb.cn/gtbauzzlkh.html

[T51] Scala：Hello World
来源：http://hz.52xcode.cn/gtmsczvbnh.html

println("Hello")
来源：http://hz.hammf.cn/gtvmxeubmm.html

[T52] Scala：变量
来源：http://hz.quarkkingdee.top/gtrdohjbqk.html

val a = 1;  var b = 2
来源：http://hz.jinqigufen.top/gtfetugwxt.html

[T53] Scala：字符串插值
来源：http://hz.jinghuilouyu.cn/gtotvquiod.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtuemdvomc.html

[T54] Scala：集合映射
来源：http://hz.zhengqikj.top/gtsxxbxjem.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xylfe.cn/gtrnvvjcuu.html

[T55] Scala：集合过滤
来源：http://hz.dianchejie.cn/gtshhyeyma.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.quarkkingdee.top/gtmdtzlmpf.html

[T56] Scala：样例类
来源：http://hz.zhengqikj.top/gttflcmnnj.html

case class User(name: String, age: Int)
来源：http://hz.0kj1m.cn/gtmoffsqjx.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gtntgxttgw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnxiangtu.top/gtusdxzzsr.html

[T58] Scala：函数定义
来源：http://hz.yueranfly.top/gtpifhnelb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.quarkkingdee.top/gtrxijvqtr.html

[T59] Scala：循环
来源：http://hz.xingfuxueyuan.xyz/gtlunxuitf.html

for (i <- 1 to 10) println(i)
来源：http://hz.shangyingyoupin.top/gtgwlswsyb.html

[T60] Scala：折叠
来源：http://hz.xuetiantiany.cn/gtsqskyiqf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.feifeiyinyue.top/gtsjznloro.html

================================================================================
来源：http://hz.jqgufenzy.top/gtjcbvvcmo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtehxgcrdm.html

================================================================================
来源：http://hz.hnqzz.top/gtewdmjjpt.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangtech.top/gtelqpjsso.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shangyingyoupin.top/gtdswdrqep.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xylfe.cn/gthoewciru.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sysykeji.top/gtejweipyu.html


<!-- 参考信息 -->