代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtmfekqmsh.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtzfovqkde.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigfzy.top/gtcqeffjtn.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtltxupgev.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtaofzeuix.html

[R66] 定时任务
来源：http://hz.sysykeji.top/gtqmyqhypn.html

crontab -e;  crontab -l
来源：http://hz.cashguo.top/gtojvmhzka.html

[R67] 生成随机十六进制串
来源：http://hz.0kj1m.cn/gtqbtjsmlu.html

openssl rand -hex 16
来源：http://hz.zhengqikj.top/gtojbbftlp.html

[R68] 计算文件校验值
来源：http://hz.yuanzhike.top/gtpxmfueer.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tian-w.cn/gtkkgaavvu.html

[R69] 生成随机密码
来源：http://hz.hnxiangtu.top/gtlljghspo.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtshjlpytm.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtsarsyazx.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gtlbajzpvi.html

[R71] 日期格式化
来源：http://hz.xylfe.cn/gtapxiwluc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtoqcfblrm.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtbewylxug.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtqurufxij.html

[R73] 分割大日志
来源：http://hz.chenjidiqi.icu/gtngvwcyra.html

split -l 1000 big.log part_
来源：http://hz.birdmap.top/gtmuchrzpt.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gtlyhbbpsn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258888.top/gtrwfhlqwb.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtnmjiaqbw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtspejtjxl.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtiuzojtyf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtdcdrphwi.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtixndqyid.html

read -rp "请输入: " ans
来源：http://hz.cashguo.top/gtmaatiqrh.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtmbspftxd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhongyouzk.top/gttizalnkw.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gtduzaqqqb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gtwgnjrslp.html

[R80] 查看脚本执行耗时
来源：http://hz.guowangkeji.top/gttmukaekw.html

time ./run.sh
来源：http://hz.mhx1999.top/gtueutwdre.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsoywhhom.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtxtmtpisj.html

================================================================================
来源：http://hz.cqqwz.cn/gtevbwzbdj.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtreazvifl.html

#include <stdio.h>
来源：http://hz.sysykeji.top/gtfucqqunc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtizqfjmwi.html

[S02] C：变量与格式化输出
来源：http://hz.52xcode.cn/gtswltxnxe.html

int a = 10; printf("%d\n", a);
来源：http://hz.xylfe.cn/gtrlpjnqyr.html

[S03] C：读入整数
来源：http://hz.zhengqikj.top/gtdcpudxyc.html

int x; scanf("%d", &x);
来源：http://hz.chenjidiqi.icu/gttwmecine.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtnljijdde.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pycfn.com/gtycqwuxdc.html

[S05] C：字符串长度
来源：http://hz.yuanzhike.top/gttbbdubbr.html

strlen(s)
来源：http://hz.yuanzhike.top/gthzmamgpk.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtcwojustv.html

strcmp(a, b) == 0
来源：http://hz.yj20258888.top/gtlakvbrzr.html

[S07] C：数组遍历求和
来源：http://hz.xziqi.cn/gtokaxioab.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhaomingkeji.xyz/gtqszafafm.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtbkinxall.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gotoacloud.top/gtrvqkxkrt.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtyarvkasm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.pycfn.com/gtmkokhvdh.html

[S10] C：指针与解引用
来源：http://hz.ydzc1.top/gtcmniyrdb.html

int *p = &a;  *p = 5;
来源：http://hz.kuanghao11.cn/gtxaiekkex.html

[S11] C：逐行读文件
来源：http://hz.gaohongyu789.top/gthoojkmdl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtonyuoadn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtlzzxvvan.html

fclose(f);
来源：http://hz.sxryk.cn/gtirfbhysg.html

[S12] C：写文件
来源：http://hz.dashuyun.cn/gtiawyzvbb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.snrcjt.cn/gtgncpwtkj.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtqxrbrmdc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtishgrlat.html

[S14] C：枚举
来源：http://hz.yueranfly.top/gtundttjpv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sxryk.cn/gtvczzlodu.html

[S15] C：类型转换
来源：http://hz.hywenlv.cn/gtvsexktgx.html

(double) a / b
来源：http://hz.fzhhl.top/gthdzkqxnz.html

[S16] C：位操作置位
来源：http://hz.aibaodan.cn/gtpzqgtwtx.html

x |= (1 << 3);
来源：http://hz.jyoumei.cn/gtbcpfhbpy.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtvjltdqcg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ivvv.top/gtmgmqbxag.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gtnyazbbnl.html

int main(int argc, char **argv)
来源：http://hz.52xcode.cn/gtcaotigxr.html

[S19] C：快速排序
来源：http://hz.jinqigfzy.top/gtslumawqo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtusswwigy.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtzmfewhwg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258888.top/gtaqosryjv.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtatvqeouu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtuhtfqtxs.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtlbwrtfcz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtltpajnnv.html

[S23] C：随机数
来源：http://hz.yj20258.top/gtzshuoxkf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.birdmap.top/gtrmucqmml.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangtech.top/gtdzqhcdzq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgfzy.top/gtjtmmpyze.html

[S25] C：内存拷贝
来源：http://hz.birdmap.top/gtwlvbssld.html

memcpy(dst, src, n);
来源：http://hz.zhongyouzk.top/gttyyzfbtu.html

[S26] C：内存清零
来源：http://hz.xziqi.cn/gtmbjtekug.html

memset(a, 0, sizeof a);
来源：http://hz.snrcjt.cn/gtyojosdbr.html

[S27] C：定义常量
来源：http://hz.jianghu66.top/gteohxiiqa.html

const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtmvfbutus.html

[S28] C：静态变量
来源：http://hz.xylfe.cn/gtlodigeaf.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtorrrnybu.html

[S29] C：变参函数
来源：http://hz.zhixingplan.top/gtmxuvxjlg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtrwpbjnur.html

[S30] C：头文件保护
来源：http://hz.sweek.top/gtekvruvwi.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtysrbgnok.html

#define X_H
来源：http://hz.daria6918.cn/gtcjdigjgz.html

#endif
来源：http://hz.ybcxt.top/gtghkpwszt.html

[S31] C++：Hello World
来源：http://hz.hywenlv.cn/gtupfrelug.html

#include <iostream>
来源：http://hz.guowangkeji.top/gtztbbjwgm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtwldyaqsy.html

[S32] C++：字符串
来源：http://hz.guowangkeji.top/gtmrlxvspi.html

std::string s = "hi";  s += "!";
来源：http://hz.tanke756.top/gtecxhuflo.html

[S33] C++：vector 增删
来源：http://hz.xziqi.cn/gtjgkrrxwv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daxiang520.top/gtxsieyuzh.html

[S34] C++：遍历 vector
来源：http://hz.jianghu66.top/gtlveqyowb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sxryk.cn/gtqpssxdyg.html

[S35] C++：map
来源：http://hz.mhx1999.top/gtalmesxiz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtcptlnrth.html

[S36] C++：unordered_map
来源：http://hz.nanxuanxn.top/gtlggcfibl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtrilkyeci.html

[S37] C++：set
来源：http://hz.chenzaomai.com/gtvelyhlyd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yvedp.cn/gtjgglckuz.html

[S38] C++：排序
来源：http://hz.dianchejie.cn/gtgczzastg.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtxkamwmlh.html

[S39] C++：自定义比较器排序
来源：http://hz.xingfuxueyuan.xyz/gtlwkruthr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.vqdsnc.cn/gtvunkkxnu.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtzwujeuuv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtjwglfcyp.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtpslfhgui.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxinkj.top/gtvydtugix.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gtgavbvgdn.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinyuanbaomall.cn/gtbyhbylhp.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtwwepqkaf.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtxbbawyfe.html

[S44] C++：引用传参
来源：http://hz.zhijiandao.cn/gtflsxorkk.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtzvsweclz.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtkgfmajen.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtwwxvgufa.html

[S46] C++：函数模板
来源：http://hz.hnqzz.top/gtmxznmxfs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhongyouzk.top/gtoudzkqfh.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtkeucdwmq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigufen.top/gtlpkeiere.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtzjaqkoda.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenjidiqi.icu/gteadokfxv.html

while (std::getline(in, line)) { }
来源：http://hz.hfpthk.cn/gtvupmtjfe.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtewwqlvuf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shzxlz.cn/gtmibmykkx.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gtwrtzclhv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnxiangtu.top/gtxmdvejlq.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtemqunnti.html

static_cast<double>(a) / b
来源：http://hz.ppjwa.cn/gtysljneyo.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gtszoknaua.html

int size() const noexcept { return n_; }
来源：http://hz.xuanzx.com/gtaxnjtvgz.html

[S53] C++：移动语义
来源：http://hz.yueranfly.top/gtrootrlhw.html

std::vector<int> w = std::move(v);
来源：http://hz.xuanzx.com/gtnxjotjaa.html

[S54] C++：异常处理
来源：http://hz.sysykeji.top/gtgaywfdte.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtrkkgfknr.html

[S55] C++：结构化绑定
来源：http://hz.tian-w.cn/gtwponqgej.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.andypj.xyz/gtwroxwlgu.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtvnoaeykf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gtogotukxs.html

[S57] C++：编译期常量
来源：http://hz.jqgfzy.top/gtufdebxlt.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtvneghqyl.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gturtjkbuz.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtxzcuxdtt.html

[S59] C++：静态断言
来源：http://hz.aibaodan.cn/gtggtkoydz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ehwqpu.com/gtayahorzh.html

[S60] C++：遍历并删除元素
来源：http://hz.ppjwa.cn/gtnaizwnqd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gtdxtcirfr.html

================================================================================
来源：http://hz.sufxvd.cn/gtqdbidlaf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtpbtxdjdf.html

================================================================================
来源：http://hz.ydzc1.top/gtoegfagcf.html

[T01] Kotlin：Hello World
来源：http://hz.pycfn.com/gtglerjvdx.html

println("Hello")
来源：http://hz.0kj1m.cn/gthrccdfds.html

[T02] Kotlin：变量
来源：http://hz.aibaodan.cn/gtvdgacmro.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.birdmap.top/gtqudwosii.html

[T03] Kotlin：字符串模板
来源：http://hz.xuetiantiany.cn/gtdndifjjs.html

"值: $b"
来源：http://hz.redwolf501.top/gtnutwkyhd.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtowkzbrhr.html

val n: String? = null;  n?.length
来源：http://hz.gzhubu.top/gttppyzxfi.html

[T05] Kotlin：when 表达式
来源：http://hz.redwolf501.top/gtmbcdtakn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yangfankeji.com/gtjuivdgan.html

[T06] Kotlin：集合映射
来源：http://hz.xziqi.cn/gtbtubfmvh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtthwzdqfj.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtskerbdle.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yvedp.cn/gtdlnxtqrb.html

[T08] Kotlin：数据类
来源：http://hz.andypj.xyz/gtzswacjaf.html

data class User(val name: String, val age: Int)
来源：http://hz.zhixingplan.top/gtfkxvznhe.html

[T09] Kotlin：扩展函数
来源：http://hz.shuidangran.top/gtkeehtndh.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtxbmkbflz.html

[T10] Kotlin：默认参数
来源：http://hz.aizwys.cn/gtuaehcqfo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ivvv.top/gtrqlefgjj.html

[T11] Kotlin：协程
来源：http://hz.jinyuanbaomall.cn/gtgtowkjwo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtlmjdkwor.html

[T12] Kotlin：解构声明
来源：http://hz.wangshuangyany.cn/gtcweqlxqu.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinghuilouyu.cn/gtzbirokzo.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtxgbczopc.html

val m = mapOf("a" to 1)
来源：http://hz.chenlongwang.top/gthjkxrkyg.html

[T14] Kotlin：循环
来源：http://hz.redwolf501.top/gtjbyqjbar.html

for (i in 1..10) println(i)
来源：http://hz.quarkkingdee.top/gtdumekngf.html

[T15] Kotlin：接口
来源：http://hz.yonumen.top/gtbwwcfesk.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtytfyurbj.html

[T16] Swift：Hello World
来源：http://hz.bjfxy.top/gtolmnapjm.html

print("Hello")
来源：http://hz.yueranfly.top/gtoeancgoj.html

[T17] Swift：变量与常量
来源：http://hz.cucudq.cn/gtuafbsmhg.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtrhfxllon.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtgjbmfjqx.html

"值: \(b)"
来源：http://hz.pycfn.com/gtbndquhbm.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtigwwgiwe.html

if let n = opt { print(n) }
来源：http://hz.hongshengwenyu.top/gtyzqjifqy.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gthyoabmun.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhengqikj.top/gtczymkwwv.html

[T21] Swift：遍历
来源：http://hz.yj20258888.top/gtzgstfjek.html

for x in a { print(x) }
来源：http://hz.kuanghao11.cn/gtkavfiics.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gteywjmmtj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtlvvuyfie.html

[T23] Swift：函数
来源：http://hz.ybcxt.top/gtldjmlowr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.meibo888.top/gtojoxlvqi.html

[T24] Swift：闭包
来源：http://hz.svipenyu.cn/gtaafzedhj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sufxvd.cn/gtrnkwsdco.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtnveylgdm.html

struct P { var x: Int }
来源：http://hz.shzxlz.cn/gtnpvrvemg.html

[T26] Swift：类与重写
来源：http://hz.vqdsnc.cn/gtbbxaignr.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtjezlkvpj.html

[T27] Swift：错误处理
来源：http://hz.guannengcc.top/gtvayqypzq.html

do { try f() } catch { print(error) }
来源：http://hz.hammf.cn/gtlsjrmmve.html

[T28] Swift：枚举
来源：http://hz.ydjk.org.cn/gthmteyusp.html

enum Color { case red, green }
来源：http://hz.guowangkeji.top/gtpryevtix.html

[T29] Swift：guard 提前返回
来源：http://hz.yvedp.cn/gtioijjlkh.html

guard let x = opt else { return }
来源：http://hz.c1oappe.top/gtvbuxghro.html

[T30] Swift：协议
来源：http://hz.zhengqikj.top/gtwfjjmjbg.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtwepbcppb.html

[T31] Lua：Hello World
来源：http://hz.ivvv.top/gturgqjaml.html

print("Hello")
来源：http://hz.ybcxt.top/gtxqlqnbiv.html

[T32] Lua：局部变量
来源：http://hz.jinqigufen.top/gtwropejge.html

local a = 1
来源：http://hz.quarkkingdee.top/gtzpfnqoaz.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtcchfylzs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yonumen.top/gtpzzhynwj.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtgxocwxxa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hywenlv.cn/gtsrmecvmo.html

[T35] Lua：字典表
来源：http://hz.0kj1m.cn/gtpxysmypr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gthpvsfbit.html

[T36] Lua：函数
来源：http://hz.jianghu66.top/gtcswvkaty.html

function add(a, b) return a + b end
来源：http://hz.jinqigfzy.top/gtaqwgfztv.html

[T37] Lua：字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtmcukpggo.html

"a" .. "b"
来源：http://hz.ywan-chungtsiang.top/gtgydxozpe.html

[T38] Lua：条件
来源：http://hz.xylfe.cn/gtwbbhpbja.html

if x > 0 then print("正") end
来源：http://hz.yuanzhike.top/gtjrmaswfk.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gtbuxeyghm.html

string.find(s, "%d+")
来源：http://hz.0kj1m.cn/gtihdaivvp.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtzjnqynnl.html

setmetatable({}, { __index = base })
来源：http://hz.meibo888.top/gtxrtogrsa.html

[T41] Perl：Hello World
来源：http://hz.yuanzhike.top/gteacecyvp.html

print "Hello\n";
来源：http://hz.sxryk.cn/gthzayzjgu.html

[T42] Perl：变量类型
来源：http://hz.pengpengdd.cyou/gtoraoowkv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cheryme.top/gtjjjkohmd.html

[T43] Perl：字符串插值
来源：http://hz.jianghu66.top/gtmrayzwyn.html

"值: $a"
来源：http://hz.xuetiantiany.cn/gtijmwzlxz.html

[T44] Perl：条件
来源：http://hz.zhoulong.xyz/gtqbkxqbxw.html

if ($a > 0) { print "正"; }
来源：http://hz.bjfxy.top/gtzdpensaq.html

[T45] Perl：数组遍历
来源：http://hz.shuidangran.top/gtwsasydmi.html

for my $x (@arr) { print $x; }
来源：http://hz.jyoumei.cn/gtsjnmnmjy.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gtzmcxxaba.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuxming.cn/gtpusedjlz.html

[T47] Perl：正则捕获
来源：http://hz.fzhhl.top/gtwidvazud.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtyftotjgz.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtqyxegjmq.html

$s =~ s/old/new/g;
来源：http://hz.bjfxy.top/gtyvdezxad.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gtxocqffuz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.52xcode.cn/gtdyodbetg.html

[T50] Perl：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtudlftedk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cqqwz.cn/gtwjexebfv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.andypj.xyz/gtdgbkjiss.html

[T51] Scala：Hello World
来源：http://hz.gotoacloud.top/gtaulkasef.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gttwlazezg.html

[T52] Scala：变量
来源：http://hz.nanxinkj.top/gtjavfchtx.html

val a = 1;  var b = 2
来源：http://hz.zhiwuduotai.top/gtcotdhumc.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangtech.top/gtbkfeqwsd.html

s"值: $b"
来源：http://hz.hfpthk.cn/gtvvvwpoyp.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtfbmqyrju.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fengsongda.top/gtjofggwmy.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtudtdryct.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.daria6918.cn/gtlqligvfu.html

[T56] Scala：样例类
来源：http://hz.yanxiufei.cn/gtqoioujdz.html

case class User(name: String, age: Int)
来源：http://hz.cucudq.cn/gtpecorfoj.html

[T57] Scala：模式匹配
来源：http://hz.xinyue.icu/gtanmzcmiv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cqqwz.cn/gtxlitcezu.html

[T58] Scala：函数定义
来源：http://hz.316326.xyz/gtdfhcjwzi.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhiwuduotai.top/gtakvmhvqc.html

[T59] Scala：循环
来源：http://hz.zhaomingkeji.xyz/gtkmymzxfd.html

for (i <- 1 to 10) println(i)
来源：http://hz.tian-w.cn/gtbpnymgoz.html

[T60] Scala：折叠
来源：http://hz.aizwys.cn/gtuayueban.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhixingplan.top/gtqjqzxsie.html

================================================================================
来源：http://hz.bjfxy.top/gtyymilirn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gtzrkecydz.html

================================================================================
来源：http://hz.xinyue.icu/gtjmctjjtp.html

[U01] Py：创建虚拟环境
来源：http://hz.quarkkingdee.top/gtnizuirwb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hysaishi.cn/gtikqqyfhj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhongyouzk.top/gtlkeunrwn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.mhx1999.top/gtippxcqhz.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtficakgcm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shuidangran.top/gtknrybpnj.html

[U04] Py：变量调试打印
来源：http://hz.pycfn.com/gtjkocmruz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxuanxn.top/gtaqqcxklm.html


<!-- 参考信息 -->