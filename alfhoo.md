代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.xuetiantiany.cn/gtexbtkpqo.html

[R64] 结束进程
来源：http://hz.jiagoushi.top/gtmplapecx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.52xcode.cn/gtoajivfhb.html

[R65] 查看端口占用
来源：http://hz.jqgfzy.top/gtdztndrpy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yangfankeji.com/gtkqbveuwh.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtqratokqj.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gtxmjbmlkh.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gtqkfyaajb.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtpxiqcgus.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gtrbmgrlin.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenlongwang.top/gthdianzae.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gteoffehti.html

head -c 16 /dev/urandom | base64
来源：http://hz.shuidangran.top/gttkyrbbxe.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtoxpusyrv.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtmdjmnuev.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gtmijauaza.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gterfnmnuf.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtdvmrmyxp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ehwqpu.com/gtdxypzvev.html

[R73] 分割大日志
来源：http://hz.nanxinkj.top/gtjcrxtdyu.html

split -l 1000 big.log part_
来源：http://hz.andypj.xyz/gtsvwsmoov.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtgxheztyp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.52xcode.cn/gthbwkxntt.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtzinjwtqx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtzemdgdbd.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gtbgxyctvd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtasxfdubu.html

[R77] 读取用户输入
来源：http://hz.xuanzx.com/gtpuyjsylt.html

read -rp "请输入: " ans
来源：http://hz.zhiwuduotai.top/gtnnxzvmvt.html

[R78] 交互式菜单
来源：http://hz.hnxiangtu.top/gtlvnjvmcb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtxpwadhbc.html

[R79] 解析命令行选项
来源：http://hz.guowangkeji.top/gtdhxmpmqw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xylfe.cn/gtgysyyikw.html

[R80] 查看脚本执行耗时
来源：http://hz.hysaishi.cn/gtmxkyohpl.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtgmzhemvr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnlbeprjr.html

S. C / C++ 专题
来源：http://hz.hongshengwenyu.top/gtfwftdqdy.html

================================================================================
来源：http://hz.hfpthk.cn/gtdystuljm.html

[S01] C：Hello World
来源：http://hz.mhx1999.top/gtkumgwskl.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtpacfcljk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nwbrower.top/gtmxwolhxm.html

[S02] C：变量与格式化输出
来源：http://hz.gaohongyu789.top/gtkncaansh.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gtbjeaoeza.html

[S03] C：读入整数
来源：http://hz.kuanghao11.cn/gtmdmcmgna.html

int x; scanf("%d", &x);
来源：http://hz.hywenlv.cn/gtxpnuwymn.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtequkvcrb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hfpthk.cn/gtpllnctcg.html

[S05] C：字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtmofycmfe.html

strlen(s)
来源：http://hz.jqgfzy.top/gtulduojnx.html

[S06] C：字符串比较
来源：http://hz.redwolf501.top/gtximovopz.html

strcmp(a, b) == 0
来源：http://hz.jinyuanbaomall.cn/gtvkwpknhd.html

[S07] C：数组遍历求和
来源：http://hz.jqgufenzy.top/gtoxtsqwpf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhengqikj.top/gtrjwnsejt.html

[S08] C：动态内存分配与释放
来源：http://hz.dashuyun.cn/gtcavpscft.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gtflcywdtc.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtozhpcqwo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jlsjyb.cn/gtfuyqcgrg.html

[S10] C：指针与解引用
来源：http://hz.tian-w.cn/gtckhspnru.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtzztykvxg.html

[S11] C：逐行读文件
来源：http://hz.zhixingplan.top/gtisxezili.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.vqdsnc.cn/gtulflidlg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.smart0.xyz/gtacaqsyhj.html

fclose(f);
来源：http://hz.shanyushiyangkeji.top/gtylxjtgdl.html

[S12] C：写文件
来源：http://hz.jianghu66.top/gtnmmwryyg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gtwmunqywk.html

[S13] C：宏定义
来源：http://hz.birdmap.top/gtetcwdyel.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhongyouzk.top/gtyekpovkf.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtraayyjws.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pengpengdd.cyou/gtwfbjitad.html

[S15] C：类型转换
来源：http://hz.xuetiantiany.cn/gtrmhtrpxo.html

(double) a / b
来源：http://hz.iojbl.cn/gtjochahgs.html

[S16] C：位操作置位
来源：http://hz.fzhhl.top/gtujibewue.html

x |= (1 << 3);
来源：http://hz.jqgufenzy.top/gtcvviwven.html

[S17] C：安全拼接字符串
来源：http://hz.zdqjudy.top/gtorvqazqz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.quarkkingdee.top/gtdsxvpshx.html

[S18] C：命令行参数
来源：http://hz.vqdsnc.cn/gtgcbjzxvh.html

int main(int argc, char **argv)
来源：http://hz.yj202588.top/gtvbwlgczh.html

[S19] C：快速排序
来源：http://hz.yuanzhike.top/gtjetjquwu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtxgfifwau.html

[S20] C：二分查找
来源：http://hz.wangshuangyany.cn/gttrlaelvl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtedhesith.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtdmthbexe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ybcxt.top/gtgqqgtagc.html

[S22] C：字符串转数字
来源：http://hz.cucudq.cn/gtylzovhhu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangshuangyany.cn/gtoqfzdlvd.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtvutbtagy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cashguo.top/gtgnrwjytr.html

[S24] C：获取本地时间
来源：http://hz.ywan-chungtsiang.top/gtdrxvkfkn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gttdcmstjt.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gtoymxyfmd.html

memcpy(dst, src, n);
来源：http://hz.shzxlz.cn/gtxrsqlknm.html

[S26] C：内存清零
来源：http://hz.zhengqikj.top/gtjurtefsk.html

memset(a, 0, sizeof a);
来源：http://hz.quarkkingdee.top/gtlptzlmwn.html

[S27] C：定义常量
来源：http://hz.jinghuilouyu.cn/gtvxitcwpy.html

const double PI = 3.14159;
来源：http://hz.tian-w.cn/gtgxgeguap.html

[S28] C：静态变量
来源：http://hz.pengpengdd.cyou/gtqfmkeimf.html

static int counter = 0;
来源：http://hz.sysykeji.top/gtjauoasvl.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtptbulizg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gogol.net.cn/gtxwlvbzzg.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtzovqhlum.html

#ifndef X_H
来源：http://hz.yj202588.top/gtnzakggtw.html

#define X_H
来源：http://hz.hysaishi.cn/gttxlvpfel.html

#endif
来源：http://hz.yanxiufei.cn/gthooaghoy.html

[S31] C++：Hello World
来源：http://hz.ybcxt.top/gtqfmhzibq.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtwnkxqzza.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ywan-chungtsiang.top/gtibfzvhua.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtmvjwzeix.html

std::string s = "hi";  s += "!";
来源：http://hz.tanke756.top/gtlwglxkmc.html

[S33] C++：vector 增删
来源：http://hz.shzxlz.cn/gttrojumeh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtajqlvwak.html

[S34] C++：遍历 vector
来源：http://hz.meibo888.top/gtrrmftard.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gtzfuyyfkc.html

[S35] C++：map
来源：http://hz.hammf.cn/gtjceqvizj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtmlnvlxfb.html

[S36] C++：unordered_map
来源：http://hz.xuetiantiany.cn/gtyxnggmla.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtvsxampzc.html

[S37] C++：set
来源：http://hz.chenzaomai.com/gtftuwddfr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtwtzhhjit.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtstighgip.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtfhtnphix.html

[S39] C++：自定义比较器排序
来源：http://hz.yuxming.cn/gtqozdenmf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aizwys.cn/gtvqcsbfns.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtxvfffgxu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ppjwa.cn/gtdxpzblqm.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtmzkbchcd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnqzz.top/gtftqkonin.html

[S42] C++：继承与虚函数
来源：http://hz.hnqzz.top/gtzeuemnho.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtojphrpji.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtmzzypdxj.html

auto p = std::make_unique<int>(5);
来源：http://hz.hammf.cn/gtpftaccuk.html

[S44] C++：引用传参
来源：http://hz.yj20258888.top/gtneaeiqzq.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtdeocrzwj.html

[S45] C++：lambda
来源：http://hz.zhiwuduotai.top/gttipnxges.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gthfbwpxxd.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtiqtnjuks.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigufen.top/gtzribwwfq.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtfnnpxzcr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yongpay.top/gtqwvtyasg.html

[S48] C++：逐行读文件
来源：http://hz.zdqjudy.top/gtkrdmenjz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guowangkeji.top/gtfdckhsaz.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gtrshbbpta.html

[S49] C++：写文件
来源：http://hz.cashguo.top/gtgjmmsoij.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgfzy.top/gtojcsucuw.html

[S50] C++：格式化数字
来源：http://hz.cdnleiting.top/gtjepolplx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.haohaochexian.top/gtgcbuncad.html

[S51] C++：显式类型转换
来源：http://hz.pengpengdd.cyou/gtytxdjhwd.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtmcirmjch.html

[S52] C++：const 与 noexcept
来源：http://hz.chenjidiqi.icu/gtjxeaqmxi.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtusjreqbw.html

[S53] C++：移动语义
来源：http://hz.bjfxy.top/gtugvvtvmi.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtuiwtawnc.html

[S54] C++：异常处理
来源：http://hz.feifeiyinyue.top/gttrpctrlx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hysaishi.cn/gtnihchyuq.html

[S55] C++：结构化绑定
来源：http://hz.pycfn.com/gtyjaeicix.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtqoyzcdup.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtuuyfthyv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnqzz.top/gtbewikyth.html

[S57] C++：编译期常量
来源：http://hz.ehwqpu.com/gtvwqqkppd.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtemjfcrvs.html

[S58] C++：命名空间
来源：http://hz.316326.xyz/gtrrznkczh.html

namespace ns { int f() { return 1; } }
来源：http://hz.nwbrower.top/gtghbkrkcd.html

[S59] C++：静态断言
来源：http://hz.jinghuilouyu.cn/gtyajzrriq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.feifeiyinyue.top/gtgimimcqk.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtbpugewql.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtxuirqmdb.html

================================================================================
来源：http://hz.iojbl.cn/gtbdzkxmua.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nwbrower.top/gtynzcwtni.html

================================================================================
来源：http://hz.52xcode.cn/gtwlbyypyb.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtsmqwjniw.html

println("Hello")
来源：http://hz.aibaodan.cn/gtmzigcmbj.html

[T02] Kotlin：变量
来源：http://hz.pengpengdd.cyou/gtfnsrsjrw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangshuangyany.cn/gttrreaknp.html

[T03] Kotlin：字符串模板
来源：http://hz.chenlongwang.top/gtjjbnprhc.html

"值: $b"
来源：http://hz.yangfankeji.com/gtjfuakydn.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gtfqehvvbt.html

val n: String? = null;  n?.length
来源：http://hz.sweek.top/gtvjjepvdb.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtgmlekrcw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnqzz.top/gtxtgcatif.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtzkgocmru.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.redwolf501.top/gtndlzlyyo.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtmraqgpgv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gthpkhbouj.html

[T08] Kotlin：数据类
来源：http://hz.xingfuxueyuan.xyz/gtslokdbfm.html

data class User(val name: String, val age: Int)
来源：http://hz.guannengcc.top/gtlqqrnycy.html

[T09] Kotlin：扩展函数
来源：http://hz.ydjk.org.cn/gtlnpzghed.html

fun String.exclaim() = this + "!"
来源：http://hz.hysaishi.cn/gtasnxkzmz.html

[T10] Kotlin：默认参数
来源：http://hz.0kj1m.cn/gtwawnzlnk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gttnxhydgl.html

[T11] Kotlin：协程
来源：http://hz.yanxiufei.cn/gteuvxpwgt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gtefhernur.html

[T12] Kotlin：解构声明
来源：http://hz.xingfuxueyuan.xyz/gttiwqbeel.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gteljwxvfy.html

[T13] Kotlin：只读 Map
来源：http://hz.tanke756.top/gtotvnduxj.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtihzyziok.html

[T14] Kotlin：循环
来源：http://hz.nwbrower.top/gtykklhmod.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtyqoahtkc.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gtxoyxrurq.html

interface Shape { fun area(): Double }
来源：http://hz.xuetiantiany.cn/gtsbxumnti.html

[T16] Swift：Hello World
来源：http://hz.zhixingplan.top/gtkcjfzywt.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtofzjnvpx.html

[T17] Swift：变量与常量
来源：http://hz.xziqi.cn/gtyrrvdeeo.html

var a = 1;  let b = 2
来源：http://hz.0kj1m.cn/gtmahwikcr.html

[T18] Swift：字符串插值
来源：http://hz.aibaodan.cn/gtssvzivkm.html

"值: \(b)"
来源：http://hz.nanxinkj.top/gthmybxgld.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtizbmmbqi.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtbljjjurl.html

[T20] Swift：数组操作
来源：http://hz.smart0.xyz/gtnfyphyou.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shangyingyoupin.top/gtpbkyncay.html

[T21] Swift：遍历
来源：http://hz.nwbrower.top/gtxilvdklf.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtgfncfwmi.html

[T22] Swift：字典
来源：http://hz.fengsongda.top/gtykklnmju.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gtetioajnx.html

[T23] Swift：函数
来源：http://hz.ivvv.top/gttalpnwdr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtlrxxhgjy.html

[T24] Swift：闭包
来源：http://hz.chenlongwang.top/gtiqhwrmrf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangtech.top/gtqkdscsav.html

[T25] Swift：结构体
来源：http://hz.jyoumei.cn/gtikxrlztt.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtrolkvkrz.html

[T26] Swift：类与重写
来源：http://hz.yanxiufei.cn/gtgtomokbq.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtafirkfvz.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gttiowrhyg.html

do { try f() } catch { print(error) }
来源：http://hz.bjfxy.top/gtmxphtorz.html

[T28] Swift：枚举
来源：http://hz.tanke756.top/gtqufguofo.html

enum Color { case red, green }
来源：http://hz.c1oappe.top/gtabunnhyh.html

[T29] Swift：guard 提前返回
来源：http://hz.yongpay.top/gtrbrdvfmz.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gthkmaqwul.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtzjtzkitc.html

protocol Shape { func area() -> Double }
来源：http://hz.ybcxt.top/gtvlkivfgi.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtjwazudmc.html

print("Hello")
来源：http://hz.chenzaomai.com/gtpeljiora.html

[T32] Lua：局部变量
来源：http://hz.ydjk.org.cn/gtmrytexmk.html

local a = 1
来源：http://hz.shanyushiyangkeji.top/gtzewemxpv.html

[T33] Lua：表（数组）
来源：http://hz.jinqigfzy.top/gtnudfbysv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtqftfeutp.html

[T34] Lua：遍历表
来源：http://hz.sxryk.cn/gtbcxffufl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.iojbl.cn/gtcgyyxkhs.html

[T35] Lua：字典表
来源：http://hz.52xcode.cn/gtmlbzdmjv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gthkeuhoxf.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtoxgiyzmy.html

function add(a, b) return a + b end
来源：http://hz.nwbrower.top/gtomluqtwj.html

[T37] Lua：字符串拼接
来源：http://hz.dashuyun.cn/gtobwgznbl.html

"a" .. "b"
来源：http://hz.hnqzz.top/gtalvnoeyy.html

[T38] Lua：条件
来源：http://hz.xinyue.icu/gtqjwijcky.html

if x > 0 then print("正") end
来源：http://hz.feifeiyinyue.top/gttlqlzmit.html

[T39] Lua：模式匹配
来源：http://hz.jyoumei.cn/gtsebeemlc.html

string.find(s, "%d+")
来源：http://hz.aizwys.cn/gtqtxxbhzz.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gthuehiztb.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigfzy.top/gtlmdwzpqh.html

[T41] Perl：Hello World
来源：http://hz.c1oappe.top/gtkeplsunb.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtlomioauv.html

[T42] Perl：变量类型
来源：http://hz.gaohongyu789.top/gtwvgdfzek.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.snrcjt.cn/gtryvagpgm.html

[T43] Perl：字符串插值
来源：http://hz.gogol.net.cn/gtdayaltby.html

"值: $a"
来源：http://hz.haohaochexian.top/gtjaofgmle.html

[T44] Perl：条件
来源：http://hz.yvedp.cn/gtaqiqkusa.html

if ($a > 0) { print "正"; }
来源：http://hz.pycfn.com/gtlfontxpj.html

[T45] Perl：数组遍历
来源：http://hz.cdnleiting.top/gtnchhqevo.html

for my $x (@arr) { print $x; }
来源：http://hz.pengpengdd.cyou/gttldncyph.html

[T46] Perl：哈希操作
来源：http://hz.9152youxi.cn/gtnmigjcan.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.svipenyu.cn/gttyacdsjp.html

[T47] Perl：正则捕获
来源：http://hz.xuanzx.com/gtvfrdgwrx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gtvnhpkxft.html

[T48] Perl：正则替换
来源：http://hz.yvedp.cn/gtddskmxim.html

$s =~ s/old/new/g;
来源：http://hz.svipenyu.cn/gtsmfucrti.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtdfokjbci.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtdrhaehtt.html

[T50] Perl：逐行读文件
来源：http://hz.shangyingyoupin.top/gtqvujhoxv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgfzy.top/gtlfvaqtsn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jqgfzy.top/gtqppchdfi.html

[T51] Scala：Hello World
来源：http://hz.guowangkeji.top/gtgwesrrbb.html

println("Hello")
来源：http://hz.yueranfly.top/gtjzrhqzkz.html

[T52] Scala：变量
来源：http://hz.shanyushiyangkeji.top/gtcoprjkxh.html

val a = 1;  var b = 2
来源：http://hz.pycfn.com/gttjrnulkt.html

[T53] Scala：字符串插值
来源：http://hz.yueranfly.top/gtpiivhszf.html

s"值: $b"
来源：http://hz.jqgfzy.top/gtljredqup.html

[T54] Scala：集合映射
来源：http://hz.hongshengwenyu.top/gtqwtbcbtz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daxiang520.top/gtcitujqzc.html

[T55] Scala：集合过滤
来源：http://hz.daria6918.cn/gtahxdaoob.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenlongwang.top/gtlkgfldfq.html

[T56] Scala：样例类
来源：http://hz.nanxinkj.top/gtvyfqohkd.html

case class User(name: String, age: Int)
来源：http://hz.redwolf501.top/gtfzavfybp.html

[T57] Scala：模式匹配
来源：http://hz.aibaodan.cn/gtajndggha.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gtkcigwokc.html

[T58] Scala：函数定义
来源：http://hz.bjfxy.top/gteiczvsya.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.bjfxy.top/gtsffwrvxj.html

[T59] Scala：循环
来源：http://hz.hammf.cn/gtmllnwxcw.html

for (i <- 1 to 10) println(i)
来源：http://hz.shangyingyoupin.top/gtaqaxuifm.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gtluirevvr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuxming.cn/gtwyvnljqj.html

================================================================================
来源：http://hz.tianlin.xyz/gtgvnyojid.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtydfjzbwj.html

================================================================================
来源：http://hz.chenlongwang.top/gtfiuxsrgk.html

[U01] Py：创建虚拟环境
来源：http://hz.jianghu66.top/gtamvfngql.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.havefunace.top/gtdmjozons.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenzaomai.com/gtscbumgnz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fengsongda.top/gtfwtnkboc.html

[U03] Py：加载 .env 配置
来源：http://hz.zhaomingkeji.xyz/gtaadzxgse.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.vqdsnc.cn/gtabpcbmnt.html

[U04] Py：变量调试打印
来源：http://hz.tanke756.top/gttcxkuwbh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxuanxn.top/gtnbrcqjlj.html


<!-- 参考信息 -->