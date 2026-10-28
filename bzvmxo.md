代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangtech.top/gtnenhopoc.html

[R64] 结束进程
来源：http://hz.cucudq.cn/gtaduygjmq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangtech.top/gtcigwesua.html

[R65] 查看端口占用
来源：http://hz.meibo888.top/gtuqtkrweu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtpxctzwft.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gtixnnsnoa.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtfoehcvno.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtqvdntqtv.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gtupcyrhrt.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gthogwjnsh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtldkolznv.html

[R69] 生成随机密码
来源：http://hz.redwolf501.top/gtthjcybkr.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gtsmqxzgiu.html

[R70] 时间戳与互转
来源：http://hz.aibaodan.cn/gtkfdvdbby.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtnpvriatq.html

[R71] 日期格式化
来源：http://hz.vqdsnc.cn/gtkwhbxody.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yvedp.cn/gthtnfhkez.html

[R72] 等待端口就绪
来源：http://hz.mhx1999.top/gtvjrnmhzz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtrmltafoz.html

[R73] 分割大日志
来源：http://hz.smart0.xyz/gthzoejkdr.html

split -l 1000 big.log part_
来源：http://hz.vqdsnc.cn/gtdfwjyrsc.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtlbjvvpdc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gtzxvvpvqf.html

[R75] 导出环境变量
来源：http://hz.ppjwa.cn/gtvfcahehf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ybcxt.top/gtuwqjatmq.html

[R76] 使用临时文件
来源：http://hz.fengsongda.top/gtpwbpcnbs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtgugicyfs.html

[R77] 读取用户输入
来源：http://hz.yanxiufei.cn/gtvkckdnzz.html

read -rp "请输入: " ans
来源：http://hz.cdnleiting.top/gtboghusrm.html

[R78] 交互式菜单
来源：http://hz.yvedp.cn/gtjjxqrfir.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gtbhfpxesr.html

[R79] 解析命令行选项
来源：http://hz.shangyingyoupin.top/gtcdyhigmq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhengqikj.top/gtypzfqtpk.html

[R80] 查看脚本执行耗时
来源：http://hz.xinyue.icu/gtdjthpuyy.html

time ./run.sh
来源：http://hz.meibo888.top/gtwjihltec.html

================================================================================
来源：http://hz.sxryk.cn/gtsmgzmqll.html

S. C / C++ 专题
来源：http://hz.tanke756.top/gtfacrzvrl.html

================================================================================
来源：http://hz.gotoacloud.top/gtqizbjkuv.html

[S01] C：Hello World
来源：http://hz.ydjk.org.cn/gteezfleha.html

#include <stdio.h>
来源：http://hz.wangdashe.top/gtltkdcjkk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtzqnvdpjj.html

[S02] C：变量与格式化输出
来源：http://hz.hfpthk.cn/gtgaqcuhtz.html

int a = 10; printf("%d\n", a);
来源：http://hz.52xcode.cn/gttyjqlpsv.html

[S03] C：读入整数
来源：http://hz.dianchejie.cn/gtrvgosepd.html

int x; scanf("%d", &x);
来源：http://hz.nanxuanxn.top/gtjaxjtgxo.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gthzghzaly.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnqzz.top/gtlgahswhu.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gtlebmjmbq.html

strlen(s)
来源：http://hz.yangfankeji.com/gtbdvxghvj.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gthgzswvlj.html

strcmp(a, b) == 0
来源：http://hz.redwolf501.top/gtvllmbbrz.html

[S07] C：数组遍历求和
来源：http://hz.zhijiandao.cn/gtoicqkfkf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dashuyun.cn/gtybuswexk.html

[S08] C：动态内存分配与释放
来源：http://hz.tanke756.top/gtyozzlqaf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtemtbaius.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtsfjevdbh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.smart0.xyz/gtnxhdiswi.html

[S10] C：指针与解引用
来源：http://hz.yj20258888.top/gtvwfxxbjg.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gttueqorem.html

[S11] C：逐行读文件
来源：http://hz.fengsongda.top/gtiyvaoabl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtankymoda.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gtwwzfiiwy.html

fclose(f);
来源：http://hz.yuxming.cn/gtjebmfshk.html

[S12] C：写文件
来源：http://hz.sufxvd.cn/gttotumowt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtsurdoieu.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtipfrjjsl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj202588.top/gtfvnxlusk.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gthbvcmpcg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gaohongyu789.top/gtarfrfvul.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtutefmtbc.html

(double) a / b
来源：http://hz.xziqi.cn/gtqfeebdwo.html

[S16] C：位操作置位
来源：http://hz.shuidangran.top/gtbvyasqnc.html

x |= (1 << 3);
来源：http://hz.shanyushiyangkeji.top/gtiupbcpgu.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gtgyqruliq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ybcxt.top/gtyulqhlzf.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtgawbsvrf.html

int main(int argc, char **argv)
来源：http://hz.ywan-chungtsiang.top/gtbvtzpmbs.html

[S19] C：快速排序
来源：http://hz.mhx1999.top/gtrjrwsxxd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtsvacgnyp.html

[S20] C：二分查找
来源：http://hz.shanyushiyangkeji.top/gtoxoxzqhm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtripbwsmh.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtetymxbnc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtdsrptyoa.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtbqocymua.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gogol.net.cn/gtnhgkbxxn.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtmnejkeak.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yangfankeji.com/gtqinemxlo.html

[S24] C：获取本地时间
来源：http://hz.smart0.xyz/gtpmqsgfql.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtvsqtbybt.html

[S25] C：内存拷贝
来源：http://hz.cqqwz.cn/gtkyammkud.html

memcpy(dst, src, n);
来源：http://hz.cheryme.top/gtlszpknrj.html

[S26] C：内存清零
来源：http://hz.zhaomingkeji.xyz/gtzuostjau.html

memset(a, 0, sizeof a);
来源：http://hz.jianghu66.top/gtpwbdwmpi.html

[S27] C：定义常量
来源：http://hz.yj20258.top/gtcruvatkv.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gthtcrixak.html

[S28] C：静态变量
来源：http://hz.ydjk.org.cn/gtulxeuswv.html

static int counter = 0;
来源：http://hz.daria6918.cn/gteqvffffq.html

[S29] C：变参函数
来源：http://hz.hongshengwenyu.top/gthekrxzgv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yangfankeji.com/gtvwhlhxkz.html

[S30] C：头文件保护
来源：http://hz.jlsjyb.cn/gtgczivyed.html

#ifndef X_H
来源：http://hz.chenjidiqi.icu/gtiyrrwxwp.html

#define X_H
来源：http://hz.zdqjudy.top/gtcphlfodn.html

#endif
来源：http://hz.pycfn.com/gtobxvbxek.html

[S31] C++：Hello World
来源：http://hz.aibaodan.cn/gtxbevcfrj.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtmjtyfmwl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtenptwbza.html

[S32] C++：字符串
来源：http://hz.zhijiandao.cn/gtfwdgfyej.html

std::string s = "hi";  s += "!";
来源：http://hz.wangdashe.top/gtpnxzanfy.html

[S33] C++：vector 增删
来源：http://hz.zycfv.cn/gttkjvyczq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hnqzz.top/gtfxlcjxmu.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gthzuausck.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtuzlakrsa.html

[S35] C++：map
来源：http://hz.gotoacloud.top/gtcrckhzlo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtsjjldbtg.html

[S36] C++：unordered_map
来源：http://hz.haohaochexian.top/gtgpyooykh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtfjmhurhz.html

[S37] C++：set
来源：http://hz.jiagoushi.top/gtcjnuybtt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtjyfgctfw.html

[S38] C++：排序
来源：http://hz.iojbl.cn/gttueilljn.html

std::sort(v.begin(), v.end());
来源：http://hz.gogol.net.cn/gtkkraadoz.html

[S39] C++：自定义比较器排序
来源：http://hz.jlsjyb.cn/gtilphubay.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xinyue.icu/gtxjfzfflc.html

[S40] C++：查找元素
来源：http://hz.chenlongwang.top/gtulcjfxmx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtrtnbibwh.html

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtxwapwrsl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ybcxt.top/gtxsnxowyg.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtegtjkffi.html

class B : public Base { public: void f() override {} };
来源：http://hz.aibaodan.cn/gtfepcgneo.html

[S43] C++：智能指针
来源：http://hz.jiagoushi.top/gtjaqencil.html

auto p = std::make_unique<int>(5);
来源：http://hz.xziqi.cn/gthlgycmld.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gtiuinngaa.html

void inc(int &x) { ++x; }
来源：http://hz.kuanghao11.cn/gtadnlqdrs.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gtfvbyikyo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtepidecmc.html

[S46] C++：函数模板
来源：http://hz.svipenyu.cn/gtjcqnhujy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtwflnpqcn.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gtutwzeixj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cucudq.cn/gtrxwjuidz.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtzkfbugei.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gttnldgyem.html

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtcmlkiypv.html

[S49] C++：写文件
来源：http://hz.feifeiyinyue.top/gtvmygkfop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj20258.top/gtlhsomdnu.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtpzsmvedz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xziqi.cn/gtmgvipppu.html

[S51] C++：显式类型转换
来源：http://hz.zycfv.cn/gtacpujocz.html

static_cast<double>(a) / b
来源：http://hz.hywenlv.cn/gtakmxwbaa.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtqjesbbvl.html

int size() const noexcept { return n_; }
来源：http://hz.jiagoushi.top/gtqoaveayl.html

[S53] C++：移动语义
来源：http://hz.ybcxt.top/gtpuataycn.html

std::vector<int> w = std::move(v);
来源：http://hz.havefunace.top/gtgtokptdp.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtpslistyj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtarxhmqqk.html

[S55] C++：结构化绑定
来源：http://hz.ydzc1.top/gtuonocymk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gtvvkuaflm.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtksfqarot.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuanzx.com/gtlubsactz.html

[S57] C++：编译期常量
来源：http://hz.guannengcc.top/gthclofmqn.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gtpqqxscfu.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtsdsgrhmg.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenjidiqi.icu/gtnjmxsuei.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtqobmjnvt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtzjbqcwae.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gtzxbtifwu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtaqahizzw.html

================================================================================
来源：http://hz.iojbl.cn/gtbcfeiiwm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gtyeqjpdlu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgzmvlurn.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtmbnmvwvl.html

println("Hello")
来源：http://hz.yj20258888.top/gtvvqdtopd.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gtpfidsnjj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtarokzsgi.html

[T03] Kotlin：字符串模板
来源：http://hz.yuxming.cn/gtqljdbugm.html

"值: $b"
来源：http://hz.jqgfzy.top/gthvwnmfez.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtiltcjdct.html

val n: String? = null;  n?.length
来源：http://hz.iojbl.cn/gtgmmufsoj.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gthvarhznr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fzhhl.top/gtsevcyfhq.html

[T06] Kotlin：集合映射
来源：http://hz.vqdsnc.cn/gtukrfnmtm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hysaishi.cn/gtngyheiqm.html

[T07] Kotlin：集合过滤
来源：http://hz.jyoumei.cn/gtxbluhovk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.52xcode.cn/gtuwdvhfwg.html

[T08] Kotlin：数据类
来源：http://hz.jlsjyb.cn/gtwiyrblia.html

data class User(val name: String, val age: Int)
来源：http://hz.tianlin.xyz/gtlqwfnhgh.html

[T09] Kotlin：扩展函数
来源：http://hz.yuxming.cn/gtpyrabhtb.html

fun String.exclaim() = this + "!"
来源：http://hz.guowangkeji.top/gthoihoupg.html

[T10] Kotlin：默认参数
来源：http://hz.svipenyu.cn/gtmhvuimzj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtqpdfpyft.html

[T11] Kotlin：协程
来源：http://hz.cucudq.cn/gtinkefksk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.wangshuangyany.cn/gtjmboevnc.html

[T12] Kotlin：解构声明
来源：http://hz.daria6918.cn/gtezsvkvvg.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhongyouzk.top/gtjgyhphlk.html

[T13] Kotlin：只读 Map
来源：http://hz.zhiwuduotai.top/gtdbpqbwdq.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtzxwzwabp.html

[T14] Kotlin：循环
来源：http://hz.jinyuanbaomall.cn/gtechkrhzn.html

for (i in 1..10) println(i)
来源：http://hz.ppjwa.cn/gtrqvlldhd.html

[T15] Kotlin：接口
来源：http://hz.nanxinkj.top/gthhrwhtha.html

interface Shape { fun area(): Double }
来源：http://hz.yuxming.cn/gtpawvrayf.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtqapxdpxl.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtmnqlqcbq.html

[T17] Swift：变量与常量
来源：http://hz.ehwqpu.com/gtuoxozmvo.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtfailkbmc.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtqhwbywfw.html

"值: \(b)"
来源：http://hz.cucudq.cn/gtekwspbnb.html

[T19] Swift：可选绑定
来源：http://hz.ydzc1.top/gtjpvljlzz.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtfzrzepaa.html

[T20] Swift：数组操作
来源：http://hz.gotoacloud.top/gtgurdrexm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtoxehhrxd.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtkcjydltg.html

for x in a { print(x) }
来源：http://hz.iojbl.cn/gtqwdkbnzj.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtkpxwuvxb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhaomingkeji.xyz/gtmczdczkr.html

[T23] Swift：函数
来源：http://hz.mhx1999.top/gtdqwxiiof.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gzhubu.top/gtlfkkzxvg.html

[T24] Swift：闭包
来源：http://hz.shangyingyoupin.top/gtcfbiedil.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.c1oappe.top/gtpjxfctjm.html

[T25] Swift：结构体
来源：http://hz.ybcxt.top/gtlarpajjc.html

struct P { var x: Int }
来源：http://hz.yonumen.top/gtkbvchxlj.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangtech.top/gtygyxbijc.html

class A: Base { override func f() {} }
来源：http://hz.yj20258888.top/gtazvyjegs.html

[T27] Swift：错误处理
来源：http://hz.aibaodan.cn/gtyszwfivl.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gtofiblvps.html

[T28] Swift：枚举
来源：http://hz.kuanghao11.cn/gtpqpqqhij.html

enum Color { case red, green }
来源：http://hz.hongshengwenyu.top/gtknvvkrpg.html

[T29] Swift：guard 提前返回
来源：http://hz.wangdashe.top/gtbxhpelsq.html

guard let x = opt else { return }
来源：http://hz.haohaochexian.top/gtvhhikhwf.html

[T30] Swift：协议
来源：http://hz.birdmap.top/gtbngbxjoi.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gttabhbbup.html

[T31] Lua：Hello World
来源：http://hz.ivvv.top/gtaazkfhng.html

print("Hello")
来源：http://hz.zhengqikj.top/gthjtbnszz.html

[T32] Lua：局部变量
来源：http://hz.52xcode.cn/gtfrafghyu.html

local a = 1
来源：http://hz.jlsjyb.cn/gtljggahrm.html

[T33] Lua：表（数组）
来源：http://hz.cqqwz.cn/gtadpydpsf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258.top/gtqkrcgruz.html

[T34] Lua：遍历表
来源：http://hz.ehwqpu.com/gtkdsrbyue.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ydzc1.top/gtstankrzy.html

[T35] Lua：字典表
来源：http://hz.jinghuilouyu.cn/gtmybuggdj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258888.top/gtijubdvzq.html

[T36] Lua：函数
来源：http://hz.kuanghao11.cn/gtwplacdzi.html

function add(a, b) return a + b end
来源：http://hz.hongshengwenyu.top/gtlctmoaha.html

[T37] Lua：字符串拼接
来源：http://hz.jianghu66.top/gtemrnriwt.html

"a" .. "b"
来源：http://hz.yuxming.cn/gtdhiuzipb.html

[T38] Lua：条件
来源：http://hz.guannengcc.top/gtklukhgrh.html

if x > 0 then print("正") end
来源：http://hz.ehwqpu.com/gtpeafmcsp.html

[T39] Lua：模式匹配
来源：http://hz.gogol.net.cn/gtbyzsqwvj.html

string.find(s, "%d+")
来源：http://hz.xuanzx.com/gtixqslusf.html

[T40] Lua：元表
来源：http://hz.cucudq.cn/gtvfysalrj.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtbvqsbphd.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtqyuloiii.html

print "Hello\n";
来源：http://hz.zycfv.cn/gtsbbuffjj.html

[T42] Perl：变量类型
来源：http://hz.hongshengwenyu.top/gtcqtkulex.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinqigufen.top/gtkutjnnvs.html

[T43] Perl：字符串插值
来源：http://hz.c1oappe.top/gtznpxlmcq.html

"值: $a"
来源：http://hz.yuxming.cn/gtjrbpxzzv.html

[T44] Perl：条件
来源：http://hz.birdmap.top/gtaajvuorz.html

if ($a > 0) { print "正"; }
来源：http://hz.wangdashe.top/gthivfwicn.html

[T45] Perl：数组遍历
来源：http://hz.ivvv.top/gtcwwclgbh.html

for my $x (@arr) { print $x; }
来源：http://hz.smart0.xyz/gtqzmntldt.html

[T46] Perl：哈希操作
来源：http://hz.yj202588.top/gttsnocbvd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zdqjudy.top/gtzwcejtlh.html

[T47] Perl：正则捕获
来源：http://hz.c1oappe.top/gtckhqaubw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gogol.net.cn/gtodmjxwzj.html

[T48] Perl：正则替换
来源：http://hz.tanke756.top/gtyhvgruxg.html

$s =~ s/old/new/g;
来源：http://hz.chenzaomai.com/gtgvntqzro.html

[T49] Perl：函数
来源：http://hz.nanxinkj.top/gtfvrsxrqg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenlongwang.top/gtbqijkmmi.html

[T50] Perl：逐行读文件
来源：http://hz.nanxuanxn.top/gtuwwcjkbf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yvedp.cn/gtctwqobyq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhongyouzk.top/gtxicinszv.html

[T51] Scala：Hello World
来源：http://hz.ppjwa.cn/gtakjsqbcb.html

println("Hello")
来源：http://hz.cucudq.cn/gtdmcjrfhw.html

[T52] Scala：变量
来源：http://hz.316326.xyz/gtkcinepio.html

val a = 1;  var b = 2
来源：http://hz.jinyuanbaomall.cn/gtoeydzaqi.html

[T53] Scala：字符串插值
来源：http://hz.svipenyu.cn/gtxemkbhnz.html

s"值: $b"
来源：http://hz.cashguo.top/gtouqzeswe.html

[T54] Scala：集合映射
来源：http://hz.nanxuanxn.top/gtxodsnfqw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sweek.top/gtnndkibwe.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtogtmtfbd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tanke756.top/gtiqmphauj.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtiyswaibk.html

case class User(name: String, age: Int)
来源：http://hz.xingfuxueyuan.xyz/gtxthineyl.html

[T57] Scala：模式匹配
来源：http://hz.hfpthk.cn/gtctadhelg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangshuangyany.cn/gtcjcibnpe.html

[T58] Scala：函数定义
来源：http://hz.iojbl.cn/gtyuudwovf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jiagoushi.top/gtxlxvlpmk.html

[T59] Scala：循环
来源：http://hz.cashguo.top/gtzdlukcvx.html

for (i <- 1 to 10) println(i)
来源：http://hz.cashguo.top/gtallqlrno.html

[T60] Scala：折叠
来源：http://hz.jinqigfzy.top/gttltcwlsr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinqigufen.top/gtifvsivsg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbbjnzvhw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtcpokpvve.html

================================================================================
来源：http://hz.wangdashe.top/gtkgcdcnsl.html

[U01] Py：创建虚拟环境
来源：http://hz.yonumen.top/gttwdyqeyp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pengpengdd.cyou/gtjoudadiu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydzc1.top/gtqoarfzeu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yueranfly.top/gtprqqwzbl.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtyhjyvnkb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangshuangyany.cn/gtyefgoiue.html

[U04] Py：变量调试打印
来源：http://hz.hammf.cn/gtvkripoco.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtjwqenygt.html


<!-- 参考信息 -->