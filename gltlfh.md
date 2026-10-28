代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.dashuyun.cn/gtrbcqrscd.html

[R64] 结束进程
来源：http://hz.jqgufenzy.top/gtyhpcjfhe.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhoulong.xyz/gtkuyhkylp.html

[R65] 查看端口占用
来源：http://hz.zdqjudy.top/gtkgauqiyy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtshfhqyld.html

[R66] 定时任务
来源：http://hz.nanxuanxn.top/gtpplmtbmf.html

crontab -e;  crontab -l
来源：http://hz.wangshuangyany.cn/gtoaqprjfs.html

[R67] 生成随机十六进制串
来源：http://hz.ppjwa.cn/gtoiixeoll.html

openssl rand -hex 16
来源：http://hz.wangshuangyany.cn/gtysllmyfa.html

[R68] 计算文件校验值
来源：http://hz.yj202588.top/gtcalgdzud.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.quarkkingdee.top/gtliocjjpe.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gtzaagfbui.html

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gttqdnsskp.html

[R70] 时间戳与互转
来源：http://hz.ivvv.top/gtfjtpgnja.html

date +%s;  date -d @1700000000
来源：http://hz.pengpengdd.cyou/gtgfclsgoa.html

[R71] 日期格式化
来源：http://hz.jiagoushi.top/gtjmtrgvrv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangdashe.top/gtrofsacun.html

[R72] 等待端口就绪
来源：http://hz.9152youxi.cn/gtzvuxsklh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtlyjxxxad.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gtrabhesir.html

split -l 1000 big.log part_
来源：http://hz.nanxuanxn.top/gteafdyhmm.html

[R74] 批量重命名
来源：http://hz.wangdashe.top/gtbxdnuepd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cucudq.cn/gtwgmhmmck.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtcewtgcde.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sxryk.cn/gthpjwluyq.html

[R76] 使用临时文件
来源：http://hz.xuanzx.com/gtuxhsftup.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtknnfmbno.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtpbtrwzuf.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtnffkgfgk.html

[R78] 交互式菜单
来源：http://hz.yj202588.top/gtdungsiqm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gthtojxkob.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gtljfqvaoi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnqzz.top/gtmipjqsnm.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgufenzy.top/gtgzyiyxex.html

time ./run.sh
来源：http://hz.redwolf501.top/gtkxhonore.html

================================================================================
来源：http://hz.mhx1999.top/gtwxcfkvla.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gthnldpqfc.html

================================================================================
来源：http://hz.52xcode.cn/gtbdapymfp.html

[S01] C：Hello World
来源：http://hz.gogol.net.cn/gtnabhguuk.html

#include <stdio.h>
来源：http://hz.xinyue.icu/gtlywvjcsh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gtkokxtyvl.html

[S02] C：变量与格式化输出
来源：http://hz.9152youxi.cn/gtyzivebtr.html

int a = 10; printf("%d\n", a);
来源：http://hz.sweek.top/gtwqebnfhm.html

[S03] C：读入整数
来源：http://hz.bjfxy.top/gtzczkucrd.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gtfeklsdbe.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtbzdupgmt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hysaishi.cn/gtmfhkmtug.html

[S05] C：字符串长度
来源：http://hz.nanxinkj.top/gtmvyndffl.html

strlen(s)
来源：http://hz.bjfxy.top/gtxelwsjjj.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtniwmmtqf.html

strcmp(a, b) == 0
来源：http://hz.hongshengwenyu.top/gtsihcwivh.html

[S07] C：数组遍历求和
来源：http://hz.feifeiyinyue.top/gtonwtoaxw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hongshengwenyu.top/gtiprgacwl.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtoyjxqmdo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtbdntsycc.html

[S09] C：结构体定义与初始化
来源：http://hz.andypj.xyz/gtygofghvg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhoulong.xyz/gtpruanlhd.html

[S10] C：指针与解引用
来源：http://hz.aizwys.cn/gtehbtqols.html

int *p = &a;  *p = 5;
来源：http://hz.pengpengdd.cyou/gtchyshogh.html

[S11] C：逐行读文件
来源：http://hz.shangyingyoupin.top/gtvfrexakf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aibaodan.cn/gtgzswyzpl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtsgppawfm.html

fclose(f);
来源：http://hz.fzhhl.top/gtmczimtmo.html

[S12] C：写文件
来源：http://hz.yj20258888.top/gtmyypsxqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gtymhsurvn.html

[S13] C：宏定义
来源：http://hz.hfpthk.cn/gtvknaamtl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.redwolf501.top/gtvjmpzzrd.html

[S14] C：枚举
来源：http://hz.snrcjt.cn/gteaqnzurm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtbnbyonpw.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gtctewhlbj.html

(double) a / b
来源：http://hz.sweek.top/gtdjjwcvky.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtkutwngix.html

x |= (1 << 3);
来源：http://hz.jyoumei.cn/gtyijushfy.html

[S17] C：安全拼接字符串
来源：http://hz.jqgufenzy.top/gtgiuvuupc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhengqikj.top/gthcpbajhz.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gtxowuekbp.html

int main(int argc, char **argv)
来源：http://hz.yanxiufei.cn/gtgodvlnct.html

[S19] C：快速排序
来源：http://hz.zycfv.cn/gthmffsnod.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtvollnxsn.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtqlgnallw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtvvjgiiyv.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtrxiufyvb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtovylrtty.html

[S22] C：字符串转数字
来源：http://hz.guannengcc.top/gtoahhqhfs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gttfrccmsm.html

[S23] C：随机数
来源：http://hz.ydjk.org.cn/gtvgtmlwxr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.haohaochexian.top/gtirlqcank.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtzvhdafxg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtsjfapnkl.html

[S25] C：内存拷贝
来源：http://hz.pengpengdd.cyou/gtitserxik.html

memcpy(dst, src, n);
来源：http://hz.fengsongda.top/gtszathdja.html

[S26] C：内存清零
来源：http://hz.chenzaomai.com/gttcbwaleg.html

memset(a, 0, sizeof a);
来源：http://hz.smart0.xyz/gtikxjugip.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gttrfrqrmi.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtblhvdfue.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtzvrymzuu.html

static int counter = 0;
来源：http://hz.daria6918.cn/gtceuiurzu.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gtethwfgoj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.bjfxy.top/gtxnmgeixw.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gtgrxeciog.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtaaddwyih.html

#define X_H
来源：http://hz.ppjwa.cn/gttmxlqsow.html

#endif
来源：http://hz.gaohongyu789.top/gtgucwthzh.html

[S31] C++：Hello World
来源：http://hz.dashuyun.cn/gtdookidbq.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtuuxgbsou.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gtngmfwzde.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtpmgcxgyi.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtctnkydeq.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtejbcujvm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtwbkzootb.html

[S34] C++：遍历 vector
来源：http://hz.aizwys.cn/gtcbmfcenj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.birdmap.top/gtarfjqgtf.html

[S35] C++：map
来源：http://hz.sxryk.cn/gtaspiibid.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtdtzdlmuk.html

[S36] C++：unordered_map
来源：http://hz.cashguo.top/gtpmfdkiue.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtgnohjxjp.html

[S37] C++：set
来源：http://hz.jyoumei.cn/gtavdqiuxx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gtoualkpzf.html

[S38] C++：排序
来源：http://hz.zdqjudy.top/gthbnchtpj.html

std::sort(v.begin(), v.end());
来源：http://hz.feifeiyinyue.top/gtwuqbztip.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtbrgkyadj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigufen.top/gtievkohqs.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gtbrcplbuq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gtugkzfndy.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gthgxncjbn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtmtkkysdf.html

[S42] C++：继承与虚函数
来源：http://hz.ppjwa.cn/gthjuvuqul.html

class B : public Base { public: void f() override {} };
来源：http://hz.9152youxi.cn/gtvqpqwodx.html

[S43] C++：智能指针
来源：http://hz.cucudq.cn/gtlmdqchsq.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydjk.org.cn/gtorglkvzl.html

[S44] C++：引用传参
来源：http://hz.zhaomingkeji.xyz/gtzwwjeymn.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gtpxfqacrm.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtclhrizrs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtrboejezm.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtnkulnlyt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.0kj1m.cn/gtburkcwvn.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuanzhike.top/gthzoryvix.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sxryk.cn/gtqgqaprue.html

[S48] C++：逐行读文件
来源：http://hz.smart0.xyz/gtzodzqbwc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xziqi.cn/gtoqzmjjqx.html

while (std::getline(in, line)) { }
来源：http://hz.fzhhl.top/gtjmvfwuit.html

[S49] C++：写文件
来源：http://hz.wangshuangyany.cn/gteahqvrgb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtbfebemgu.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtnsjqhzml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shuidangran.top/gtlbvaondd.html

[S51] C++：显式类型转换
来源：http://hz.havefunace.top/gtsnqtmkxk.html

static_cast<double>(a) / b
来源：http://hz.meibo888.top/gtvpctigmn.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gtiybgryxz.html

int size() const noexcept { return n_; }
来源：http://hz.guannengcc.top/gturpseizg.html

[S53] C++：移动语义
来源：http://hz.yj20258888.top/gtlrdymfjx.html

std::vector<int> w = std::move(v);
来源：http://hz.shangyingyoupin.top/gtzauitnfr.html

[S54] C++：异常处理
来源：http://hz.birdmap.top/gthabfzxfx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtjsxfyofh.html

[S55] C++：结构化绑定
来源：http://hz.daria6918.cn/gtaahauoht.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sufxvd.cn/gtmnhnnikb.html

[S56] C++：optional
来源：http://hz.nwbrower.top/gtwmkqgylw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.meibo888.top/gtjubofwpv.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtuynuoqsg.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtbjhjrjcw.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtiidamfit.html

namespace ns { int f() { return 1; } }
来源：http://hz.ivvv.top/gttcnnlavv.html

[S59] C++：静态断言
来源：http://hz.zhixingplan.top/gtzhjvhmuh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ehwqpu.com/gtfgahsdmg.html

[S60] C++：遍历并删除元素
来源：http://hz.tian-w.cn/gtgdjhurnm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cqqwz.cn/gtknbjvkjv.html

================================================================================
来源：http://hz.wangdashe.top/gttbuxkqev.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtlrgfzgdh.html

================================================================================
来源：http://hz.chenlongwang.top/gttskrjhoy.html

[T01] Kotlin：Hello World
来源：http://hz.feifeiyinyue.top/gtbfuusugy.html

println("Hello")
来源：http://hz.aizwys.cn/gtgfzarmdn.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gtqwmzjgju.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gtqtplkxvq.html

[T03] Kotlin：字符串模板
来源：http://hz.yvedp.cn/gtazeppmjx.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtcgrhvszy.html

[T04] Kotlin：空安全
来源：http://hz.yonumen.top/gtqpwzqwin.html

val n: String? = null;  n?.length
来源：http://hz.yangfankeji.com/gtdyvppiaj.html

[T05] Kotlin：when 表达式
来源：http://hz.jianghu66.top/gtbmtozdhn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gtfkpahahn.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gtpyrqsgue.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangtech.top/gtcxwwlsho.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258888.top/gttuielhku.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fengsongda.top/gtkhwxbgoa.html

[T08] Kotlin：数据类
来源：http://hz.smart0.xyz/gtonhqjtcv.html

data class User(val name: String, val age: Int)
来源：http://hz.cqqwz.cn/gtljbsjjwx.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxinkj.top/gtiinydjms.html

fun String.exclaim() = this + "!"
来源：http://hz.hysaishi.cn/gtdzhgzqae.html

[T10] Kotlin：默认参数
来源：http://hz.shangyingyoupin.top/gtmbbbphof.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gttzpzlnhg.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtyvpibafl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hammf.cn/gtqyoqwghl.html

[T12] Kotlin：解构声明
来源：http://hz.tianlin.xyz/gtjntuxreo.html

val (a, b) = Pair(1, 2)
来源：http://hz.zdqjudy.top/gtsbdzadkm.html

[T13] Kotlin：只读 Map
来源：http://hz.redwolf501.top/gtoyyhzyza.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gtjvoesnsx.html

[T14] Kotlin：循环
来源：http://hz.dianchejie.cn/gtyvaqyaen.html

for (i in 1..10) println(i)
来源：http://hz.svipenyu.cn/gtexllgbdz.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtlovbhbkh.html

interface Shape { fun area(): Double }
来源：http://hz.yuxming.cn/gteibriziu.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtxrnsirvw.html

print("Hello")
来源：http://hz.svipenyu.cn/gtdvsyskiq.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangtech.top/gttznldpni.html

var a = 1;  let b = 2
来源：http://hz.chenlongwang.top/gtiwleofmu.html

[T18] Swift：字符串插值
来源：http://hz.shzxlz.cn/gtxvzkvyys.html

"值: \(b)"
来源：http://hz.aibaodan.cn/gtqbthjjft.html

[T19] Swift：可选绑定
来源：http://hz.mhx1999.top/gtmuusfnmp.html

if let n = opt { print(n) }
来源：http://hz.dashuyun.cn/gtkmlimobp.html

[T20] Swift：数组操作
来源：http://hz.fzhhl.top/gtlcqvxpwk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.52xcode.cn/gtsqrlnstq.html

[T21] Swift：遍历
来源：http://hz.zhiwuduotai.top/gttqtusjen.html

for x in a { print(x) }
来源：http://hz.cucudq.cn/gtdbayfipd.html

[T22] Swift：字典
来源：http://hz.pycfn.com/gthdbpvxhe.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gtxhwukudv.html

[T23] Swift：函数
来源：http://hz.chenjidiqi.icu/gtojtpqvld.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gotoacloud.top/gtdonjzatc.html

[T24] Swift：闭包
来源：http://hz.mhx1999.top/gtzmixmlii.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtwfgyqgjm.html

[T25] Swift：结构体
来源：http://hz.xylfe.cn/gtsykqhinn.html

struct P { var x: Int }
来源：http://hz.shangyingyoupin.top/gtkdvcnifx.html

[T26] Swift：类与重写
来源：http://hz.ydjk.org.cn/gtwovfrsnw.html

class A: Base { override func f() {} }
来源：http://hz.aibaodan.cn/gtumcelngn.html

[T27] Swift：错误处理
来源：http://hz.nanxuanxn.top/gtclfpueko.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtqxfbmvsx.html

[T28] Swift：枚举
来源：http://hz.snrcjt.cn/gthzrclyec.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtjehmqoqt.html

[T29] Swift：guard 提前返回
来源：http://hz.cashguo.top/gtplkdxtdw.html

guard let x = opt else { return }
来源：http://hz.ywan-chungtsiang.top/gtbeozzoyk.html

[T30] Swift：协议
来源：http://hz.zhoulong.xyz/gtwydocldu.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gthfprxhxw.html

[T31] Lua：Hello World
来源：http://hz.jinyuanbaomall.cn/gtjbdychcb.html

print("Hello")
来源：http://hz.hfpthk.cn/gtsnayonzx.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtpxtnijnm.html

local a = 1
来源：http://hz.ehwqpu.com/gttqkcffad.html

[T33] Lua：表（数组）
来源：http://hz.xylfe.cn/gtrtldztht.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.bjfxy.top/gtecxxegaz.html

[T34] Lua：遍历表
来源：http://hz.feifeiyinyue.top/gtirgeljem.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.haohaochexian.top/gtepzgofuw.html

[T35] Lua：字典表
来源：http://hz.zhaomingkeji.xyz/gtqitjlrpm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtitluxdtq.html

[T36] Lua：函数
来源：http://hz.svipenyu.cn/gtzpeijprq.html

function add(a, b) return a + b end
来源：http://hz.xuanzx.com/gtpohlsljt.html

[T37] Lua：字符串拼接
来源：http://hz.52xcode.cn/gtnbjrkbbv.html

"a" .. "b"
来源：http://hz.daria6918.cn/gthaugvzrd.html

[T38] Lua：条件
来源：http://hz.shanyushiyangtech.top/gtnqrufmbp.html

if x > 0 then print("正") end
来源：http://hz.yj20258.top/gtcnpqopjc.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtipgteidt.html

string.find(s, "%d+")
来源：http://hz.yonumen.top/gtrwxwrrhw.html

[T40] Lua：元表
来源：http://hz.zhaomingkeji.xyz/gtxqhutfjf.html

setmetatable({}, { __index = base })
来源：http://hz.yj202588.top/gtnqpoxpgv.html

[T41] Perl：Hello World
来源：http://hz.guannengcc.top/gtbpryqsgo.html

print "Hello\n";
来源：http://hz.zhijiandao.cn/gtpjbnozqj.html

[T42] Perl：变量类型
来源：http://hz.xuanzx.com/gtuxebitwb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.bjfxy.top/gtraestshc.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangtech.top/gtklgssnao.html

"值: $a"
来源：http://hz.cheryme.top/gtnizxuixx.html

[T44] Perl：条件
来源：http://hz.meibo888.top/gtyrxwanai.html

if ($a > 0) { print "正"; }
来源：http://hz.mhx1999.top/gtgroftjjz.html

[T45] Perl：数组遍历
来源：http://hz.sysykeji.top/gttroceeia.html

for my $x (@arr) { print $x; }
来源：http://hz.haohaochexian.top/gtprkrmpko.html

[T46] Perl：哈希操作
来源：http://hz.bjfxy.top/gtyuanpmpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.birdmap.top/gtzaboxplc.html

[T47] Perl：正则捕获
来源：http://hz.ppjwa.cn/gtwsywlkuu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xylfe.cn/gtgwagpxeo.html

[T48] Perl：正则替换
来源：http://hz.xinyue.icu/gtixlgmpnf.html

$s =~ s/old/new/g;
来源：http://hz.jqgufenzy.top/gtmecirelp.html

[T49] Perl：函数
来源：http://hz.yuxming.cn/gtecrlzfwv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtcefxfsjs.html

[T50] Perl：逐行读文件
来源：http://hz.dianchejie.cn/gtgppevfkg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydzc1.top/gtkpfmxmka.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtlcjcsfqn.html

[T51] Scala：Hello World
来源：http://hz.xuetiantiany.cn/gtkwwvqspn.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtjttclvsv.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtpvcyyoxj.html

val a = 1;  var b = 2
来源：http://hz.xingfuxueyuan.xyz/gthpiwledz.html

[T53] Scala：字符串插值
来源：http://hz.xinyue.icu/gtyvsdtwxs.html

s"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtthenhqte.html

[T54] Scala：集合映射
来源：http://hz.fzhhl.top/gtejdlmbaq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangshuangyany.cn/gtjpvstntj.html

[T55] Scala：集合过滤
来源：http://hz.zhiwuduotai.top/gttcxttxhk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hywenlv.cn/gtlxrexcqx.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtwnywsonq.html

case class User(name: String, age: Int)
来源：http://hz.fzhhl.top/gtufsahjrd.html

[T57] Scala：模式匹配
来源：http://hz.wangshuangyany.cn/gtplkszccp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.mhx1999.top/gtezrjfusj.html

[T58] Scala：函数定义
来源：http://hz.cheryme.top/gteytfskzk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhijiandao.cn/gtxevgnhvv.html

[T59] Scala：循环
来源：http://hz.daxiang520.top/gtjdrqkwms.html

for (i <- 1 to 10) println(i)
来源：http://hz.wangdashe.top/gtgktitmhu.html

[T60] Scala：折叠
来源：http://hz.mhx1999.top/gtgdkpdykl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuanzx.com/gtnnyxcpwh.html

================================================================================
来源：http://hz.jinqigufen.top/gtgdtljtyg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtuvwhrsti.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdokvkclm.html

[U01] Py：创建虚拟环境
来源：http://hz.shzxlz.cn/gteumwqrib.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.havefunace.top/gtvjbgfvhi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtddyudwht.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nanxinkj.top/gtwnczfzlj.html

[U03] Py：加载 .env 配置
来源：http://hz.gaohongyu789.top/gtaeylbsbq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ywan-chungtsiang.top/gtbumoaxcm.html

[U04] Py：变量调试打印
来源：http://hz.jinghuilouyu.cn/gtbpoxteid.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nwbrower.top/gtrglsfyie.html


<!-- 参考信息 -->