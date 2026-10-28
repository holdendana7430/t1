代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangshuangyany.cn/gtqokleldf.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtiibuoiel.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gtadbgprqt.html

[R67] 生成随机十六进制串
来源：http://hz.redwolf501.top/gthjkpjkjp.html

openssl rand -hex 16
来源：http://hz.yvedp.cn/gtgvvhowmp.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gtoitvvdmm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtdkoisvkk.html

[R69] 生成随机密码
来源：http://hz.hfpthk.cn/gtnvbqhics.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtfkdigtgu.html

[R70] 时间戳与互转
来源：http://hz.zhengqikj.top/gtfnymoebe.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtcvhvkovt.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtwdcitkfk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtuyaksrxc.html

[R72] 等待端口就绪
来源：http://hz.dianchejie.cn/gtkidxnfhb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dianchejie.cn/gtbzknzdpz.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtbyodrxgi.html

split -l 1000 big.log part_
来源：http://hz.tanke756.top/gtndrefzmm.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtkmqwwapv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jlsjyb.cn/gtlgtgrqtu.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gtqkoshvea.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258888.top/gtthxnlntv.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtdretlbam.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtalelwmam.html

[R77] 读取用户输入
来源：http://hz.guannengcc.top/gtbsflxyuj.html

read -rp "请输入: " ans
来源：http://hz.xziqi.cn/gtlbggqkwd.html

[R78] 交互式菜单
来源：http://hz.fzhhl.top/gtccvxltyh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinghuilouyu.cn/gtkmjsfinh.html

[R79] 解析命令行选项
来源：http://hz.wangshuangyany.cn/gtxjsplysa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gtrvvzbjuf.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtndgxtogx.html

time ./run.sh
来源：http://hz.zhoulong.xyz/gtzjchqpnr.html

================================================================================
来源：http://hz.zhengqikj.top/gtwoyktrih.html

S. C / C++ 专题
来源：http://hz.jinqigfzy.top/gtpzteezkp.html

================================================================================
来源：http://hz.shuidangran.top/gtxllxtnay.html

[S01] C：Hello World
来源：http://hz.shanyushiyangtech.top/gtjmvzjssx.html

#include <stdio.h>
来源：http://hz.haohaochexian.top/gtrjajudqg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtpcgianjm.html

[S02] C：变量与格式化输出
来源：http://hz.hfpthk.cn/gtettxzxmd.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenlongwang.top/gtwhhtnlyz.html

[S03] C：读入整数
来源：http://hz.cheryme.top/gtwfsrxhbi.html

int x; scanf("%d", &x);
来源：http://hz.yuanzhike.top/gtotndjmzc.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtdouhunbz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtqjrplrdd.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtfahbxksc.html

strlen(s)
来源：http://hz.xuanzx.com/gtjtplihxe.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtgifqfeht.html

strcmp(a, b) == 0
来源：http://hz.gogol.net.cn/gtlxzzqzql.html

[S07] C：数组遍历求和
来源：http://hz.zhixingplan.top/gtfspeudqk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gtalkjgkup.html

[S08] C：动态内存分配与释放
来源：http://hz.yvedp.cn/gtboxmsdup.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yongpay.top/gtruikdkud.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtrzuogxrz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gtbwgeutdi.html

[S10] C：指针与解引用
来源：http://hz.aizwys.cn/gthjwnqesg.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtyusdmeos.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gtovdmubaq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.mhx1999.top/gtviytqsac.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtsxximuur.html

fclose(f);
来源：http://hz.tanke756.top/gtszaxwgqe.html

[S12] C：写文件
来源：http://hz.ppjwa.cn/gtykspwzwe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.guannengcc.top/gtakurimda.html

[S13] C：宏定义
来源：http://hz.smart0.xyz/gtcsdcczme.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinqigfzy.top/gtpgyncrzt.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtpehtqfhg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuetiantiany.cn/gtfdtagleb.html

[S15] C：类型转换
来源：http://hz.daria6918.cn/gtaixgdatl.html

(double) a / b
来源：http://hz.zhengqikj.top/gtcgaoqplm.html

[S16] C：位操作置位
来源：http://hz.cheryme.top/gtwukcolqg.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtizsminpi.html

[S17] C：安全拼接字符串
来源：http://hz.jyoumei.cn/gtoqehbquz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigfzy.top/gtwgbiqgwv.html

[S18] C：命令行参数
来源：http://hz.tian-w.cn/gtawubcvfn.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtqzvcfdya.html

[S19] C：快速排序
来源：http://hz.nanxinkj.top/gtldnyjhoq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtdcvkeopm.html

[S20] C：二分查找
来源：http://hz.cdnleiting.top/gtsopofupf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gthobyebza.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtkerubaex.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sxryk.cn/gtvxekyggg.html

[S22] C：字符串转数字
来源：http://hz.hfpthk.cn/gtqilhdpje.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gttupbtvtz.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtvouhppoo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.mhx1999.top/gtlevxvchw.html

[S24] C：获取本地时间
来源：http://hz.dashuyun.cn/gtpmluowbm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtyvydqham.html

[S25] C：内存拷贝
来源：http://hz.xingfuxueyuan.xyz/gtqjegyquu.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtqjbxwkgf.html

[S26] C：内存清零
来源：http://hz.svipenyu.cn/gtyiqikeut.html

memset(a, 0, sizeof a);
来源：http://hz.9152youxi.cn/gtlceppgbh.html

[S27] C：定义常量
来源：http://hz.52xcode.cn/gtyetbmsxo.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtcrbzzitt.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gttvdnhowk.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtztiljlds.html

[S29] C：变参函数
来源：http://hz.jinqigufen.top/gtigdrepzz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aizwys.cn/gtbxrafeue.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtlmkusesk.html

#ifndef X_H
来源：http://hz.ehwqpu.com/gtqqqgrlyk.html

#define X_H
来源：http://hz.sweek.top/gtyplgxslb.html

#endif
来源：http://hz.xylfe.cn/gtqtwveorg.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtnylukogv.html

#include <iostream>
来源：http://hz.svipenyu.cn/gtkyknnaye.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtkitcgefg.html

[S32] C++：字符串
来源：http://hz.havefunace.top/gtqxfuvmip.html

std::string s = "hi";  s += "!";
来源：http://hz.xylfe.cn/gtrnrhlpmh.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtqmzrjyzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.mhx1999.top/gtxotquzit.html

[S34] C++：遍历 vector
来源：http://hz.aizwys.cn/gtmzxcxxfb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.c1oappe.top/gtjiatwydu.html

[S35] C++：map
来源：http://hz.feifeiyinyue.top/gtlvalyjni.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtfwfbvnaw.html

[S36] C++：unordered_map
来源：http://hz.cheryme.top/gtivobfgbu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtztondogf.html

[S37] C++：set
来源：http://hz.havefunace.top/gtlklrfybg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.vqdsnc.cn/gtfrkghdjj.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtdhuinjby.html

std::sort(v.begin(), v.end());
来源：http://hz.zycfv.cn/gtefnhyvhy.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtytvjxsgt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zycfv.cn/gtwojwdrlj.html

[S40] C++：查找元素
来源：http://hz.gzhubu.top/gtvbeztsuy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gtsngahzom.html

[S41] C++：类与构造函数
来源：http://hz.ywan-chungtsiang.top/gtcauakhkt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhengqikj.top/gtuiucybkm.html

[S42] C++：继承与虚函数
来源：http://hz.zhaomingkeji.xyz/gterbyfrpu.html

class B : public Base { public: void f() override {} };
来源：http://hz.gaohongyu789.top/gtkfvboene.html

[S43] C++：智能指针
来源：http://hz.yongpay.top/gtytxpvsjs.html

auto p = std::make_unique<int>(5);
来源：http://hz.haohaochexian.top/gtqtxzivkf.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gtnqqpbvnd.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtjneevhxh.html

[S45] C++：lambda
来源：http://hz.jinghuilouyu.cn/gtfkuivytw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtdbpalnmf.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtsnwicywo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258.top/gtksdssebk.html

[S47] C++：结构化绑定遍历
来源：http://hz.c1oappe.top/gtjtracikb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtfnjvyaum.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gtpckdmsjl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtkdnbbbpm.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtbdbqhzvd.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gtbqqktmov.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hywenlv.cn/gthepplzdk.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gtfrrtvlhd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtcolikhfe.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtsvtfiivy.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtprnghsie.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gtvmnnazne.html

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtfopletrp.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtscbrhpnl.html

std::vector<int> w = std::move(v);
来源：http://hz.cqqwz.cn/gtlctulfmu.html

[S54] C++：异常处理
来源：http://hz.yj202588.top/gtbyzconfa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cqqwz.cn/gtnpofdbff.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtcoqzpzot.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sweek.top/gtysnxaxac.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtmkqxhaqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtqueqsywf.html

[S57] C++：编译期常量
来源：http://hz.tianlin.xyz/gtmhxttfdw.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtrwepsxki.html

[S58] C++：命名空间
来源：http://hz.zdqjudy.top/gtzxfeccuf.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtbbulqwvj.html

[S59] C++：静态断言
来源：http://hz.shanyushiyangkeji.top/gtyklhwxwz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.snrcjt.cn/gtmmvjswnr.html

[S60] C++：遍历并删除元素
来源：http://hz.ybcxt.top/gtwcdovcov.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jianghu66.top/gtgekyrfvu.html

================================================================================
来源：http://hz.daxiang520.top/gtipzhwmoi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtjsxjynng.html

================================================================================
来源：http://hz.sweek.top/gtoddxoufr.html

[T01] Kotlin：Hello World
来源：http://hz.aizwys.cn/gtvavprjij.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtxehjuwov.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gtwdyvbtmf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtqdrdmidp.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gtzniydvfq.html

"值: $b"
来源：http://hz.yj20258.top/gtssmjorle.html

[T04] Kotlin：空安全
来源：http://hz.mhx1999.top/gtmblgavvu.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gtlgvejspv.html

[T05] Kotlin：when 表达式
来源：http://hz.0kj1m.cn/gtrkyoeppy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtlucobmqo.html

[T06] Kotlin：集合映射
来源：http://hz.fengsongda.top/gtvcslkrba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aizwys.cn/gtvhzsvrmp.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtoyhbclhp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtvbspjmxl.html

[T08] Kotlin：数据类
来源：http://hz.dashuyun.cn/gtgfeuqaar.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gtzgxuypim.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtbnzqtkct.html

fun String.exclaim() = this + "!"
来源：http://hz.yuxming.cn/gtwzxvflhm.html

[T10] Kotlin：默认参数
来源：http://hz.ydjk.org.cn/gtglsgqyrv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhengqikj.top/gtkufhvahk.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtzdafxnno.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cdnleiting.top/gtaqlnyhmt.html

[T12] Kotlin：解构声明
来源：http://hz.zhiwuduotai.top/gtyyzmymhv.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtwpkzapqu.html

[T13] Kotlin：只读 Map
来源：http://hz.vqdsnc.cn/gtvifroron.html

val m = mapOf("a" to 1)
来源：http://hz.sxryk.cn/gtujppvjdv.html

[T14] Kotlin：循环
来源：http://hz.yangfankeji.com/gtsrkabjia.html

for (i in 1..10) println(i)
来源：http://hz.andypj.xyz/gtxorbburg.html

[T15] Kotlin：接口
来源：http://hz.yvedp.cn/gtqdanknqx.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtqlxhzjex.html

[T16] Swift：Hello World
来源：http://hz.feifeiyinyue.top/gtkihmwpeo.html

print("Hello")
来源：http://hz.cqqwz.cn/gtzmcibdbi.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtahsrpaky.html

var a = 1;  let b = 2
来源：http://hz.wangshuangyany.cn/gtkfwoyftn.html

[T18] Swift：字符串插值
来源：http://hz.ydjk.org.cn/gtjjewkmer.html

"值: \(b)"
来源：http://hz.yueranfly.top/gtwuzigaum.html

[T19] Swift：可选绑定
来源：http://hz.dashuyun.cn/gtsczwwvjh.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtyjgnudwx.html

[T20] Swift：数组操作
来源：http://hz.ppjwa.cn/gtpxdtnlcm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtmaqyfmxd.html

[T21] Swift：遍历
来源：http://hz.mhx1999.top/gtwsynrkri.html

for x in a { print(x) }
来源：http://hz.redwolf501.top/gtosqhqfzu.html

[T22] Swift：字典
来源：http://hz.jinyuanbaomall.cn/gtgqfgaenu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhoulong.xyz/gtwfpiqoto.html

[T23] Swift：函数
来源：http://hz.svipenyu.cn/gtjsztgvin.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xziqi.cn/gtugbxivub.html

[T24] Swift：闭包
来源：http://hz.shuidangran.top/gtlpjaqdou.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guannengcc.top/gthagvgaun.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gtwdkrlilm.html

struct P { var x: Int }
来源：http://hz.yj202588.top/gtwtynwlqo.html

[T26] Swift：类与重写
来源：http://hz.9152youxi.cn/gtszmptkao.html

class A: Base { override func f() {} }
来源：http://hz.sxryk.cn/gtzdwjhlmt.html

[T27] Swift：错误处理
来源：http://hz.andypj.xyz/gtktkptggk.html

do { try f() } catch { print(error) }
来源：http://hz.xylfe.cn/gtzkixsgah.html

[T28] Swift：枚举
来源：http://hz.yonumen.top/gtebsiupip.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gtdsmbtasg.html

[T29] Swift：guard 提前返回
来源：http://hz.pengpengdd.cyou/gtrshjdwqq.html

guard let x = opt else { return }
来源：http://hz.yanxiufei.cn/gtoenbpfnz.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gthygavcsb.html

protocol Shape { func area() -> Double }
来源：http://hz.ydjk.org.cn/gtjalukygm.html

[T31] Lua：Hello World
来源：http://hz.ybcxt.top/gtcrjnicwz.html

print("Hello")
来源：http://hz.birdmap.top/gthubwdthw.html

[T32] Lua：局部变量
来源：http://hz.yvedp.cn/gtwfahjzxt.html

local a = 1
来源：http://hz.hongshengwenyu.top/gtqfxkadlb.html

[T33] Lua：表（数组）
来源：http://hz.52xcode.cn/gtplmbfqci.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jianghu66.top/gtjdnlxnhs.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtdddokhax.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.daxiang520.top/gtamwhemnm.html

[T35] Lua：字典表
来源：http://hz.ybcxt.top/gtctnebsxi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jiagoushi.top/gtwynkvdam.html

[T36] Lua：函数
来源：http://hz.shanyushiyangtech.top/gtagmatike.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gtesrelvwv.html

[T37] Lua：字符串拼接
来源：http://hz.0kj1m.cn/gtrrifwriq.html

"a" .. "b"
来源：http://hz.chenjidiqi.icu/gtabebnobp.html

[T38] Lua：条件
来源：http://hz.yanxiufei.cn/gtiuyaacvb.html

if x > 0 then print("正") end
来源：http://hz.snrcjt.cn/gtanzfjkjh.html

[T39] Lua：模式匹配
来源：http://hz.guannengcc.top/gtdqgpfzwp.html

string.find(s, "%d+")
来源：http://hz.yuanzhike.top/gtdbuvazop.html

[T40] Lua：元表
来源：http://hz.kuanghao11.cn/gtbikgniuv.html

setmetatable({}, { __index = base })
来源：http://hz.ydzc1.top/gtrajtdfso.html

[T41] Perl：Hello World
来源：http://hz.yvedp.cn/gtciyeonkn.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtmmrimgsu.html

[T42] Perl：变量类型
来源：http://hz.jqgfzy.top/gtmowhyrxd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.haohaochexian.top/gtymnnwjer.html

[T43] Perl：字符串插值
来源：http://hz.c1oappe.top/gtkqfzpkzr.html

"值: $a"
来源：http://hz.guowangkeji.top/gthxegzssp.html

[T44] Perl：条件
来源：http://hz.daria6918.cn/gtoynewwzn.html

if ($a > 0) { print "正"; }
来源：http://hz.xylfe.cn/gtwbdnzjmr.html

[T45] Perl：数组遍历
来源：http://hz.sysykeji.top/gtveszjaqn.html

for my $x (@arr) { print $x; }
来源：http://hz.jiagoushi.top/gtitdeqafv.html

[T46] Perl：哈希操作
来源：http://hz.9152youxi.cn/gtshgcqqbx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258888.top/gtnwtvhruf.html

[T47] Perl：正则捕获
来源：http://hz.shzxlz.cn/gtykpjewjl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgufenzy.top/gtgnnsabrn.html

[T48] Perl：正则替换
来源：http://hz.jqgfzy.top/gtkncctrmz.html

$s =~ s/old/new/g;
来源：http://hz.hnqzz.top/gtdbierkto.html

[T49] Perl：函数
来源：http://hz.guannengcc.top/gtrttksthd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sweek.top/gthwnmbptn.html

[T50] Perl：逐行读文件
来源：http://hz.havefunace.top/gteictxfby.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.fengsongda.top/gtnnglvsdc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenzaomai.com/gtfbxbcekf.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gtuqvyfoqc.html

println("Hello")
来源：http://hz.dashuyun.cn/gtthjcavwf.html

[T52] Scala：变量
来源：http://hz.xuanzx.com/gtkqciprgc.html

val a = 1;  var b = 2
来源：http://hz.cheryme.top/gtrowuimoc.html

[T53] Scala：字符串插值
来源：http://hz.yuxming.cn/gtqnjtfwvx.html

s"值: $b"
来源：http://hz.hongshengwenyu.top/gtazcexcqz.html

[T54] Scala：集合映射
来源：http://hz.yj20258888.top/gtbvzqnpaz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnqzz.top/gtabawbdvm.html

[T55] Scala：集合过滤
来源：http://hz.mhx1999.top/gtpfenmjdf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangshuangyany.cn/gtxivcdals.html

[T56] Scala：样例类
来源：http://hz.dianchejie.cn/gtmroebppu.html

case class User(name: String, age: Int)
来源：http://hz.kuanghao11.cn/gtywjtqken.html

[T57] Scala：模式匹配
来源：http://hz.yj20258888.top/gthpjaibws.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydzc1.top/gtndesocla.html

[T58] Scala：函数定义
来源：http://hz.jqgufenzy.top/gtuqfnpjdh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yanxiufei.cn/gtfcbdeddv.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtoepadqzl.html

for (i <- 1 to 10) println(i)
来源：http://hz.tanke756.top/gtbaxxxmbg.html

[T60] Scala：折叠
来源：http://hz.yvedp.cn/gttuoajhcb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.0kj1m.cn/gtpfntgpec.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgoixloly.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhengqikj.top/gtyythkrcw.html

================================================================================
来源：http://hz.hfpthk.cn/gtnbzmczhe.html

[U01] Py：创建虚拟环境
来源：http://hz.svipenyu.cn/gtnhgzhbdb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinqigfzy.top/gtklrpcyqy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxinkj.top/gtkdvrngru.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pycfn.com/gtrkgkgstp.html

[U03] Py：加载 .env 配置
来源：http://hz.zhaomingkeji.xyz/gtjnhflhcu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yongpay.top/gtyamqbbum.html

[U04] Py：变量调试打印
来源：http://hz.jianghu66.top/gthecfxnlz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cheryme.top/gtggtbqqlv.html

[U05] Py：列表去重且保序
来源：http://hz.jianghu66.top/gtiivxyoqp.html

list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtnpwwnrtr.html

[U06] Py：合并两个字典
来源：http://hz.gzhubu.top/gtkxdbuzuo.html

{**a, **b}
来源：http://hz.snrcjt.cn/gtghcyfmlr.html


<!-- 参考信息 -->