代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.aibaodan.cn/gtpoqzmnhc.html

[R64] 结束进程
来源：http://hz.zhijiandao.cn/gtdqhsalcg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hysaishi.cn/gtuzkuaahe.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtgbpoohqn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtpdmbqrqk.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtfdigqzkg.html

crontab -e;  crontab -l
来源：http://hz.jinghuilouyu.cn/gtykurrfjq.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtjvsvwrfm.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gttsvkbrug.html

[R68] 计算文件校验值
来源：http://hz.jyoumei.cn/gtlvyavsct.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxuanxn.top/gtpmmzcdge.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gthikxjjvl.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtmaycryqu.html

[R70] 时间戳与互转
来源：http://hz.jqgfzy.top/gtamlgihej.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangkeji.top/gtqlzjaoxo.html

[R71] 日期格式化
来源：http://hz.zycfv.cn/gtewprvruz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtlbqpbafl.html

[R72] 等待端口就绪
来源：http://hz.wangshuangyany.cn/gtvixyqwni.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gotoacloud.top/gtahtsxjrg.html

[R73] 分割大日志
来源：http://hz.ydzc1.top/gtytdoolbs.html

split -l 1000 big.log part_
来源：http://hz.svipenyu.cn/gtdjljgnni.html

[R74] 批量重命名
来源：http://hz.bjfxy.top/gtqhinnvzj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hfpthk.cn/gtukiisjtg.html

[R75] 导出环境变量
来源：http://hz.chenlongwang.top/gtstjidbsk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtkoyofitw.html

[R76] 使用临时文件
来源：http://hz.jinghuilouyu.cn/gtuodggsto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtfyzjxcda.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gtcktddaie.html

read -rp "请输入: " ans
来源：http://hz.ybcxt.top/gtrbeheeyk.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtcjrentlt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtjpfonrwn.html

[R79] 解析命令行选项
来源：http://hz.ybcxt.top/gtdavjlxda.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxinkj.top/gtcafymqfj.html

[R80] 查看脚本执行耗时
来源：http://hz.hnqzz.top/gtwabqkzbo.html

time ./run.sh
来源：http://hz.havefunace.top/gtxypvvwat.html

================================================================================
来源：http://hz.fzhhl.top/gttwxakohv.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gthvxkmeqr.html

================================================================================
来源：http://hz.hysaishi.cn/gtiggbamgn.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gtbyqnnwaj.html

#include <stdio.h>
来源：http://hz.zhongyouzk.top/gtslfvbysk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gtwuqkrpva.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtzwvotuop.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuxming.cn/gttvdroprh.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtinakmaqv.html

int x; scanf("%d", &x);
来源：http://hz.xylfe.cn/gtckdfxtip.html

[S04] C：字符串复制
来源：http://hz.xuetiantiany.cn/gtsogonrbf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.quarkkingdee.top/gtustwvorh.html

[S05] C：字符串长度
来源：http://hz.zhiwuduotai.top/gtlaghoyhf.html

strlen(s)
来源：http://hz.nwbrower.top/gtgphppjjb.html

[S06] C：字符串比较
来源：http://hz.shzxlz.cn/gtoyamitkt.html

strcmp(a, b) == 0
来源：http://hz.iojbl.cn/gtgdqrzpbz.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtjejibait.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuxming.cn/gtedpyhimj.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtixfsdxpw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangkeji.top/gteeaaubms.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtqdadhmly.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.kuanghao11.cn/gtdwrifbun.html

[S10] C：指针与解引用
来源：http://hz.yj20258888.top/gtstndfnge.html

int *p = &a;  *p = 5;
来源：http://hz.chenjidiqi.icu/gtvqogvzrc.html

[S11] C：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtkyzighuq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jianghu66.top/gthphjaokl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangkeji.top/gtwzokwyet.html

fclose(f);
来源：http://hz.shzxlz.cn/gtomwukptf.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gtngwccyzd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gthqfznyvw.html

[S13] C：宏定义
来源：http://hz.cheryme.top/gtqimxprps.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ehwqpu.com/gtxvmxfvwx.html

[S14] C：枚举
来源：http://hz.yvedp.cn/gtidvuakhs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtdvmypkcl.html

[S15] C：类型转换
来源：http://hz.yj202588.top/gtstkvhdjm.html

(double) a / b
来源：http://hz.316326.xyz/gtwwiljyjs.html

[S16] C：位操作置位
来源：http://hz.hnqzz.top/gtnyzbjqiw.html

x |= (1 << 3);
来源：http://hz.vqdsnc.cn/gtlgkrrrms.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtojakglwh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtjpquytyf.html

[S18] C：命令行参数
来源：http://hz.yangfankeji.com/gttfrjhutc.html

int main(int argc, char **argv)
来源：http://hz.gzhubu.top/gtkyedaums.html

[S19] C：快速排序
来源：http://hz.jlsjyb.cn/gtpdmruufy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtaxwkcbmr.html

[S20] C：二分查找
来源：http://hz.ydzc1.top/gtipnxfdns.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtmlaarmlm.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtkmhcyvfs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ywan-chungtsiang.top/gtsakgtllt.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtfpehiqnu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yueranfly.top/gtfxzfxvnt.html

[S23] C：随机数
来源：http://hz.ybcxt.top/gttlcvwjhi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nwbrower.top/gtuhxhcotu.html

[S24] C：获取本地时间
来源：http://hz.nwbrower.top/gtcapmzhiy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guannengcc.top/gtecasypqg.html

[S25] C：内存拷贝
来源：http://hz.9152youxi.cn/gtobkcplms.html

memcpy(dst, src, n);
来源：http://hz.meibo888.top/gthmjglbaj.html

[S26] C：内存清零
来源：http://hz.jiagoushi.top/gtkyngjljq.html

memset(a, 0, sizeof a);
来源：http://hz.jyoumei.cn/gtjxpfxcon.html

[S27] C：定义常量
来源：http://hz.vqdsnc.cn/gtyjaiccqo.html

const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gthznferot.html

[S28] C：静态变量
来源：http://hz.hongshengwenyu.top/gtkyxpaoci.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtvvbtdhku.html

[S29] C：变参函数
来源：http://hz.hammf.cn/gtkkfczrdf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtoitausxc.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangtech.top/gtrhsfjmwc.html

#ifndef X_H
来源：http://hz.jlsjyb.cn/gtfxzbdqaq.html

#define X_H
来源：http://hz.andypj.xyz/gtgwafjneh.html

#endif
来源：http://hz.9152youxi.cn/gtchasqblm.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtrvhipejx.html

#include <iostream>
来源：http://hz.hnqzz.top/gthfsnzeas.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhoulong.xyz/gtikcwkoqm.html

[S32] C++：字符串
来源：http://hz.yvedp.cn/gtbpvlelje.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtvyufsubr.html

[S33] C++：vector 增删
来源：http://hz.kuanghao11.cn/gtjtwowppn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.kuanghao11.cn/gtsujonhgu.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtrblpwhty.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sysykeji.top/gtuxbgoihb.html

[S35] C++：map
来源：http://hz.jinghuilouyu.cn/gtbcknbyhq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtvabnxfjy.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtzkqmefev.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtmxikcnra.html

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtppeilwcc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhiwuduotai.top/gtexepgdvm.html

[S38] C++：排序
来源：http://hz.jlsjyb.cn/gthirzctht.html

std::sort(v.begin(), v.end());
来源：http://hz.kuanghao11.cn/gtwjkruzmy.html

[S39] C++：自定义比较器排序
来源：http://hz.aizwys.cn/gtxfmiogwn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhoulong.xyz/gtjcprcrnb.html

[S40] C++：查找元素
来源：http://hz.xingfuxueyuan.xyz/gtfeadtkcj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sufxvd.cn/gtmufdrrho.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtohzhtoyz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yongpay.top/gtclhufzre.html

[S42] C++：继承与虚函数
来源：http://hz.xuetiantiany.cn/gtinhnqlxj.html

class B : public Base { public: void f() override {} };
来源：http://hz.ybcxt.top/gtwcqajaeu.html

[S43] C++：智能指针
来源：http://hz.yuanzhike.top/gtqjeqhkio.html

auto p = std::make_unique<int>(5);
来源：http://hz.tian-w.cn/gtvxbhrnjd.html

[S44] C++：引用传参
来源：http://hz.ydjk.org.cn/gtqwsuvhdy.html

void inc(int &x) { ++x; }
来源：http://hz.cucudq.cn/gtvyghzgjb.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtrwmtbepe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xingfuxueyuan.xyz/gtflrqtfqy.html

[S46] C++：函数模板
来源：http://hz.aizwys.cn/gtryyiwpmc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guowangkeji.top/gtzuigerka.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhaomingkeji.xyz/gtnaddmqyu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtwhspqhoz.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gthyvycfba.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtpwhfrqri.html

while (std::getline(in, line)) { }
来源：http://hz.dianchejie.cn/gtsgvxcorv.html

[S49] C++：写文件
来源：http://hz.jyoumei.cn/gtklnbxomc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtotheulrl.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtgmloaend.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.52xcode.cn/gtrwnuonzi.html

[S51] C++：显式类型转换
来源：http://hz.9152youxi.cn/gtwdlkjbhv.html

static_cast<double>(a) / b
来源：http://hz.pycfn.com/gtgopgljcl.html

[S52] C++：const 与 noexcept
来源：http://hz.cdnleiting.top/gtzrxxndxh.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtxdkgmtsh.html

[S53] C++：移动语义
来源：http://hz.hammf.cn/gtouoziywn.html

std::vector<int> w = std::move(v);
来源：http://hz.aibaodan.cn/gtrqqqyljy.html

[S54] C++：异常处理
来源：http://hz.zhongyouzk.top/gtzguxlrnk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuanzx.com/gtgvnbgpav.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtwyfkijhg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daria6918.cn/gtqqlhanrr.html

[S56] C++：optional
来源：http://hz.shangyingyoupin.top/gtzazedsat.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hammf.cn/gtzzuelfhi.html

[S57] C++：编译期常量
来源：http://hz.316326.xyz/gtrqflmkpw.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gthmsyjtmf.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtqbpelhhr.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtgmmmbivd.html

[S59] C++：静态断言
来源：http://hz.yonumen.top/gtajjcjzyt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.havefunace.top/gtdaybstkp.html

[S60] C++：遍历并删除元素
来源：http://hz.chenlongwang.top/gtaatcvmkr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhongyouzk.top/gtquvpqvob.html

================================================================================
来源：http://hz.sufxvd.cn/gtrnloiqxv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtljgovwkm.html

================================================================================
来源：http://hz.chenzaomai.com/gtgcrckhdl.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtygwsbuaa.html

println("Hello")
来源：http://hz.hfpthk.cn/gtxlqiiaqt.html

[T02] Kotlin：变量
来源：http://hz.zycfv.cn/gtfncfndle.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guowangkeji.top/gtmxmnahda.html

[T03] Kotlin：字符串模板
来源：http://hz.daxiang520.top/gtmqwltrfc.html

"值: $b"
来源：http://hz.haohaochexian.top/gtbbavtcye.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangtech.top/gtmckkcljo.html

val n: String? = null;  n?.length
来源：http://hz.xziqi.cn/gtsqbizyxx.html

[T05] Kotlin：when 表达式
来源：http://hz.haohaochexian.top/gtwzrgwnfk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnqzz.top/gtvatnqcdu.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtilbotqjr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangtech.top/gtaocnqkeq.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtfppzaije.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.0kj1m.cn/gtxdtwsrgm.html

[T08] Kotlin：数据类
来源：http://hz.sweek.top/gtkoidqcxu.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtaakgjady.html

[T09] Kotlin：扩展函数
来源：http://hz.cheryme.top/gtoszxiudm.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtpsfmccdg.html

[T10] Kotlin：默认参数
来源：http://hz.hammf.cn/gtlcthhnaj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhixingplan.top/gtyrozzfzn.html

[T11] Kotlin：协程
来源：http://hz.pengpengdd.cyou/gtzpbiltul.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.iojbl.cn/gthktybddq.html

[T12] Kotlin：解构声明
来源：http://hz.shuidangran.top/gtdqibrvih.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gtplgtnjjn.html

[T13] Kotlin：只读 Map
来源：http://hz.cashguo.top/gtrbyjreoh.html

val m = mapOf("a" to 1)
来源：http://hz.hfpthk.cn/gthuqzlznz.html

[T14] Kotlin：循环
来源：http://hz.xuetiantiany.cn/gtayhkcoti.html

for (i in 1..10) println(i)
来源：http://hz.jiagoushi.top/gtyspmkojr.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gtzlvcdkzr.html

interface Shape { fun area(): Double }
来源：http://hz.yj202588.top/gtjehvtxdb.html

[T16] Swift：Hello World
来源：http://hz.aibaodan.cn/gtotpotdlu.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtxdqbalxs.html

[T17] Swift：变量与常量
来源：http://hz.jqgfzy.top/gtwcomaytw.html

var a = 1;  let b = 2
来源：http://hz.hysaishi.cn/gtsiprllsq.html

[T18] Swift：字符串插值
来源：http://hz.gotoacloud.top/gtbllqqyiv.html

"值: \(b)"
来源：http://hz.yj20258.top/gtlnwwldth.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtduzvrswu.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangtech.top/gtzknsdiur.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtjugfzzcy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.meibo888.top/gtmhxyykik.html

[T21] Swift：遍历
来源：http://hz.hnxiangtu.top/gtsejnyxca.html

for x in a { print(x) }
来源：http://hz.shuidangran.top/gtjtqnurcm.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtrbtyqpcp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yongpay.top/gtodkvngnl.html

[T23] Swift：函数
来源：http://hz.jqgufenzy.top/gtqyyjbzmy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pengpengdd.cyou/gtppkzbpig.html

[T24] Swift：闭包
来源：http://hz.dianchejie.cn/gtwfadndxv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtxyfbotwm.html

[T25] Swift：结构体
来源：http://hz.chenzaomai.com/gtuknvumuh.html

struct P { var x: Int }
来源：http://hz.ppjwa.cn/gtlefzjxzw.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtvpwfkgeh.html

class A: Base { override func f() {} }
来源：http://hz.hammf.cn/gtrloujwke.html

[T27] Swift：错误处理
来源：http://hz.havefunace.top/gtdlovkpbm.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtxzcuqdui.html

[T28] Swift：枚举
来源：http://hz.haohaochexian.top/gtedkstyyu.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtwbijzgrb.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtrauyfbxj.html

guard let x = opt else { return }
来源：http://hz.hnqzz.top/gtbunnbsnm.html

[T30] Swift：协议
来源：http://hz.zhengqikj.top/gtooynmnip.html

protocol Shape { func area() -> Double }
来源：http://hz.zhongyouzk.top/gtcasqsitw.html

[T31] Lua：Hello World
来源：http://hz.hnxiangtu.top/gtcfhyduwe.html

print("Hello")
来源：http://hz.yuxming.cn/gtqovkabon.html

[T32] Lua：局部变量
来源：http://hz.ybcxt.top/gtbuavwmms.html

local a = 1
来源：http://hz.cdnleiting.top/gtsemgsbas.html

[T33] Lua：表（数组）
来源：http://hz.jlsjyb.cn/gttfhyrvfi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cqqwz.cn/gtjmvstnnr.html

[T34] Lua：遍历表
来源：http://hz.cucudq.cn/gtcwewebus.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gaohongyu789.top/gtnghjvjjp.html

[T35] Lua：字典表
来源：http://hz.snrcjt.cn/gtplyzfays.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gtbcvvlpug.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gteffdfkbk.html

function add(a, b) return a + b end
来源：http://hz.tian-w.cn/gtxcxorlup.html

[T37] Lua：字符串拼接
来源：http://hz.gzhubu.top/gtwwkldike.html

"a" .. "b"
来源：http://hz.dashuyun.cn/gtgzkefiun.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtqprrscen.html

if x > 0 then print("正") end
来源：http://hz.xingfuxueyuan.xyz/gttpfvqqod.html

[T39] Lua：模式匹配
来源：http://hz.ppjwa.cn/gtguejabtp.html

string.find(s, "%d+")
来源：http://hz.ywan-chungtsiang.top/gtrajbblxr.html

[T40] Lua：元表
来源：http://hz.cashguo.top/gtevladacp.html

setmetatable({}, { __index = base })
来源：http://hz.fengsongda.top/gtxpyzzybf.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangtech.top/gtnipyrrkn.html

print "Hello\n";
来源：http://hz.hnqzz.top/gtbeakiekh.html

[T42] Perl：变量类型
来源：http://hz.jqgufenzy.top/gtpjqyacjo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jyoumei.cn/gtqczvrfhm.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtamcnbfwc.html

"值: $a"
来源：http://hz.zhongyouzk.top/gtodmdsyuc.html

[T44] Perl：条件
来源：http://hz.chenzaomai.com/gtgjigpbup.html

if ($a > 0) { print "正"; }
来源：http://hz.zhoulong.xyz/gtsyplgvqb.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtdqhuifme.html

for my $x (@arr) { print $x; }
来源：http://hz.haohaochexian.top/gtcajoycvt.html

[T46] Perl：哈希操作
来源：http://hz.yangfankeji.com/gtqisnganu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.9152youxi.cn/gtxeepwmmr.html

[T47] Perl：正则捕获
来源：http://hz.wangdashe.top/gtituituov.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gtibmmyafy.html

[T48] Perl：正则替换
来源：http://hz.wangshuangyany.cn/gtmvxwmnqp.html

$s =~ s/old/new/g;
来源：http://hz.cdnleiting.top/gtsgiwfjbn.html

[T49] Perl：函数
来源：http://hz.ydjk.org.cn/gtxhrclvuw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtqkzotehk.html

[T50] Perl：逐行读文件
来源：http://hz.daxiang520.top/gtizufzbpk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tianlin.xyz/gtykjalkuv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.kuanghao11.cn/gtqilmewrx.html

[T51] Scala：Hello World
来源：http://hz.cdnleiting.top/gtzobmcpap.html

println("Hello")
来源：http://hz.cdnleiting.top/gtnftklzsg.html

[T52] Scala：变量
来源：http://hz.kuanghao11.cn/gtndljexma.html

val a = 1;  var b = 2
来源：http://hz.ydzc1.top/gtgnioulwz.html

[T53] Scala：字符串插值
来源：http://hz.jqgfzy.top/gtbmrpilxf.html

s"值: $b"
来源：http://hz.iojbl.cn/gticbctwwy.html

[T54] Scala：集合映射
来源：http://hz.jinyuanbaomall.cn/gtwyesesdx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuanzhike.top/gtvtmvhlhh.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtdtpmiilz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.guowangkeji.top/gthcmxniwb.html

[T56] Scala：样例类
来源：http://hz.sufxvd.cn/gtpltkbowc.html

case class User(name: String, age: Int)
来源：http://hz.hnxiangtu.top/gtrrrpdnlr.html

[T57] Scala：模式匹配
来源：http://hz.shanyushiyangtech.top/gthkhcftkl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ehwqpu.com/gtrjrlddrz.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtunddtlgi.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gtmuhgxzzi.html

[T59] Scala：循环
来源：http://hz.hammf.cn/gtpcxwhnke.html

for (i <- 1 to 10) println(i)
来源：http://hz.hywenlv.cn/gthupndtoq.html

[T60] Scala：折叠
来源：http://hz.zhaomingkeji.xyz/gtfndpexqt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydzc1.top/gtnezncsbe.html

================================================================================
来源：http://hz.tian-w.cn/gttiqhlhgl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gteqofefho.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjhbzqyra.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258888.top/gtbbnfewku.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ivvv.top/gtcrqxaywh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.birdmap.top/gtuavggdnj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinghuilouyu.cn/gtjycdicgi.html

[U03] Py：加载 .env 配置
来源：http://hz.dashuyun.cn/gtaxtnsqsk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.andypj.xyz/gtorkrrzjz.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtxssbbupa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sufxvd.cn/gtwpzoasjf.html


<!-- 参考信息 -->