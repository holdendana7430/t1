代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtcchgalco.html

[R64] 结束进程
来源：http://hz.ywan-chungtsiang.top/gtroncxxbi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtwxxsggyu.html

[R65] 查看端口占用
来源：http://hz.jlsjyb.cn/gtafsdmtht.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gteamubmzy.html

[R66] 定时任务
来源：http://hz.hongshengwenyu.top/gtscxdexhc.html

crontab -e;  crontab -l
来源：http://hz.xuetiantiany.cn/gtufyamuox.html

[R67] 生成随机十六进制串
来源：http://hz.svipenyu.cn/gtwiqoqfgy.html

openssl rand -hex 16
来源：http://hz.havefunace.top/gtekiytlhw.html

[R68] 计算文件校验值
来源：http://hz.316326.xyz/gtvdgqxezk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.mhx1999.top/gtnoalijfq.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtsjnuhctq.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtneegyxeb.html

[R70] 时间戳与互转
来源：http://hz.yuxming.cn/gtlrccgvoo.html

date +%s;  date -d @1700000000
来源：http://hz.52xcode.cn/gtakwdldvq.html

[R71] 日期格式化
来源：http://hz.pycfn.com/gtaidroueq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hammf.cn/gtqpyvshqr.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtipviciuf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xuetiantiany.cn/gtgwjwwuvi.html

[R73] 分割大日志
来源：http://hz.chenjidiqi.icu/gtwqoupviu.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtbgghjbek.html

[R74] 批量重命名
来源：http://hz.wangshuangyany.cn/gtayqgwmho.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cdnleiting.top/gtiadhjvbq.html

[R75] 导出环境变量
来源：http://hz.ywan-chungtsiang.top/gtrndwiadp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hysaishi.cn/gtmdoxlnke.html

[R76] 使用临时文件
来源：http://hz.sysykeji.top/gtmqhcpunw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtulthudzd.html

[R77] 读取用户输入
来源：http://hz.jinqigufen.top/gtmzytonja.html

read -rp "请输入: " ans
来源：http://hz.yongpay.top/gtlmnrnuri.html

[R78] 交互式菜单
来源：http://hz.xylfe.cn/gtpwcoyvmo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gtwywvpolp.html

[R79] 解析命令行选项
来源：http://hz.shuidangran.top/gtppntqery.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ivvv.top/gtvanppesh.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtktcfqnth.html

time ./run.sh
来源：http://hz.smart0.xyz/gtonjlnloq.html

================================================================================
来源：http://hz.ybcxt.top/gtlgqhryob.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtmzyvvtza.html

================================================================================
来源：http://hz.yangfankeji.com/gtmxtyoffm.html

[S01] C：Hello World
来源：http://hz.meibo888.top/gtnrehkwor.html

#include <stdio.h>
来源：http://hz.yj20258.top/gtwmwgqopq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sufxvd.cn/gtpkkfcjud.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtqzeprcah.html

int a = 10; printf("%d\n", a);
来源：http://hz.jiagoushi.top/gtrdzmpflk.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtvapqlrnx.html

int x; scanf("%d", &x);
来源：http://hz.ydjk.org.cn/gtaqmiwaor.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtcypygkzm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.iojbl.cn/gtysudpmob.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtkeqhmeju.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtorzcgngt.html

[S06] C：字符串比较
来源：http://hz.jinqigufen.top/gtvtytsqor.html

strcmp(a, b) == 0
来源：http://hz.gotoacloud.top/gtzpxwtjyw.html

[S07] C：数组遍历求和
来源：http://hz.jinqigfzy.top/gtgupipfrr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtsjjbztfp.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtnrscpfiv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtpghlwtod.html

[S09] C：结构体定义与初始化
来源：http://hz.ivvv.top/gtehhwypqz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtailmgzle.html

[S10] C：指针与解引用
来源：http://hz.mhx1999.top/gtnuimqoni.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtwyphglip.html

[S11] C：逐行读文件
来源：http://hz.yangfankeji.com/gtddcipqnv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gttmorkyjs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.smart0.xyz/gtvqqcewgb.html

fclose(f);
来源：http://hz.chenlongwang.top/gtxgykkqnb.html

[S12] C：写文件
来源：http://hz.ydzc1.top/gtdarntblv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sxryk.cn/gtnhacjhwn.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtzlfyieso.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ivvv.top/gtxzqevzfk.html

[S14] C：枚举
来源：http://hz.sxryk.cn/gtxtergikd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gthzamvukm.html

[S15] C：类型转换
来源：http://hz.jinyuanbaomall.cn/gtaecrebng.html

(double) a / b
来源：http://hz.wangdashe.top/gtqfvwcttk.html

[S16] C：位操作置位
来源：http://hz.tianlin.xyz/gtknrqbmmu.html

x |= (1 << 3);
来源：http://hz.gzhubu.top/gtxywrawmm.html

[S17] C：安全拼接字符串
来源：http://hz.zhengqikj.top/gtjjoulbhf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gtmhmbrnty.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangkeji.top/gtcuhmfaqu.html

int main(int argc, char **argv)
来源：http://hz.sysykeji.top/gtyfjgrpak.html

[S19] C：快速排序
来源：http://hz.zdqjudy.top/gtwgqjxihw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtwjvisnjk.html

[S20] C：二分查找
来源：http://hz.yueranfly.top/gtukpnpeuv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gttmebbqmb.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtxqirvsvd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydjk.org.cn/gtbachyrll.html

[S22] C：字符串转数字
来源：http://hz.quarkkingdee.top/gtjzbqsdjg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtqjtjtlnx.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtbkbvpkma.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtxwntmhks.html

[S24] C：获取本地时间
来源：http://hz.ydzc1.top/gtidtwrkcg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gteohppdkn.html

[S25] C：内存拷贝
来源：http://hz.316326.xyz/gtwmaxpclt.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtmyrwpnhn.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtdvwdouow.html

memset(a, 0, sizeof a);
来源：http://hz.cheryme.top/gtnawsmrzm.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtzbszfkrx.html

const double PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtluxsiflj.html

[S28] C：静态变量
来源：http://hz.quarkkingdee.top/gtaqgrzdaz.html

static int counter = 0;
来源：http://hz.birdmap.top/gtnkqjpyun.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtmpqmbgtt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtevgfqqjl.html

[S30] C：头文件保护
来源：http://hz.yanxiufei.cn/gtcxdtuknd.html

#ifndef X_H
来源：http://hz.kuanghao11.cn/gtpgzaizul.html

#define X_H
来源：http://hz.meibo888.top/gtemulcsma.html

#endif
来源：http://hz.vqdsnc.cn/gtbvruembl.html

[S31] C++：Hello World
来源：http://hz.jlsjyb.cn/gtsgkbkqin.html

#include <iostream>
来源：http://hz.hnxiangtu.top/gtzhwyoxep.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtuftkogpc.html

[S32] C++：字符串
来源：http://hz.yj20258888.top/gtvdrnmhig.html

std::string s = "hi";  s += "!";
来源：http://hz.jinyuanbaomall.cn/gtllxopusy.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtshkmkcko.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shangyingyoupin.top/gtwnickwcd.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtyyxicmrg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtgsmmvofj.html

[S35] C++：map
来源：http://hz.gotoacloud.top/gtbrhigsqm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtymbssugn.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtqapoqees.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtpjbrcatl.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtsasnpxsa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gthopdscox.html

[S38] C++：排序
来源：http://hz.yj202588.top/gtqaizbxyg.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtwgiyuovi.html

[S39] C++：自定义比较器排序
来源：http://hz.havefunace.top/gtvsellvzq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hywenlv.cn/gtbamevwrn.html

[S40] C++：查找元素
来源：http://hz.feifeiyinyue.top/gthuadmcxs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnqzz.top/gtdphrpjhb.html

[S41] C++：类与构造函数
来源：http://hz.yongpay.top/gtzkrjyhab.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cqqwz.cn/gtvcsobifl.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gthdusmhzq.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtcgpevbdu.html

[S43] C++：智能指针
来源：http://hz.cheryme.top/gttggrwgty.html

auto p = std::make_unique<int>(5);
来源：http://hz.hywenlv.cn/gttpuiumwc.html

[S44] C++：引用传参
来源：http://hz.yj202588.top/gtxhtncpne.html

void inc(int &x) { ++x; }
来源：http://hz.zhijiandao.cn/gtiixccakf.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtmgvbwgbq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.dianchejie.cn/gtmpdsjemx.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtzmndnkir.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gtephjldur.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhijiandao.cn/gttztohddy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangdashe.top/gtwtzarkzf.html

[S48] C++：逐行读文件
来源：http://hz.cqqwz.cn/gthwpzvkjs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sxryk.cn/gtjsmkuzse.html

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtvnrjewto.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtehxvdxxu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.52xcode.cn/gtzixjgjcz.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtjjrsgkkz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtmqpiuxmz.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gtkaiicxaa.html

static_cast<double>(a) / b
来源：http://hz.yanxiufei.cn/gthjdcfpum.html

[S52] C++：const 与 noexcept
来源：http://hz.cashguo.top/gtdfhgwefc.html

int size() const noexcept { return n_; }
来源：http://hz.mhx1999.top/gtgbbxtmzm.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtqkesmnoo.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258888.top/gtlixlbpar.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gtbzcuzowx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hongshengwenyu.top/gtcwablpte.html

[S55] C++：结构化绑定
来源：http://hz.pengpengdd.cyou/gtetxyeknv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinghuilouyu.cn/gtvzfwcoil.html

[S56] C++：optional
来源：http://hz.mhx1999.top/gtinkokiwo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yonumen.top/gtmaismfjk.html

[S57] C++：编译期常量
来源：http://hz.havefunace.top/gtswggsbju.html

constexpr int N = 10;
来源：http://hz.tianlin.xyz/gtlompqiep.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtebtaenic.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtdcuxdhkq.html

[S59] C++：静态断言
来源：http://hz.kuanghao11.cn/gtgtrapgyw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhoulong.xyz/gtbkydfvzw.html

[S60] C++：遍历并删除元素
来源：http://hz.yvedp.cn/gtmpkvxler.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yueranfly.top/gtguhtekby.html

================================================================================
来源：http://hz.0kj1m.cn/gtdmbeoibp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.svipenyu.cn/gtsgsxfjzn.html

================================================================================
来源：http://hz.cucudq.cn/gtrbyoebmc.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtvtumshye.html

println("Hello")
来源：http://hz.guowangkeji.top/gtalwpilyl.html

[T02] Kotlin：变量
来源：http://hz.xuetiantiany.cn/gthfwsmahk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ybcxt.top/gtwqynbdfe.html

[T03] Kotlin：字符串模板
来源：http://hz.dianchejie.cn/gtiranpnom.html

"值: $b"
来源：http://hz.yueranfly.top/gtcqonantz.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangtech.top/gtcoiszlus.html

val n: String? = null;  n?.length
来源：http://hz.meibo888.top/gtlxganlpq.html

[T05] Kotlin：when 表达式
来源：http://hz.gaohongyu789.top/gthzweqgne.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtdlyvmfhs.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtfwojwzbo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtqnpngxbi.html

[T07] Kotlin：集合过滤
来源：http://hz.gzhubu.top/gtmjcoegkf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtkzipblvh.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtjpwkntml.html

data class User(val name: String, val age: Int)
来源：http://hz.yanxiufei.cn/gtlxaxnreg.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gttmbgehoc.html

fun String.exclaim() = this + "!"
来源：http://hz.sysykeji.top/gtuydpfdho.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtzlwjobwg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ivvv.top/gthesxugcd.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtuuxmmfyu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cashguo.top/gtjznvnazd.html

[T12] Kotlin：解构声明
来源：http://hz.tian-w.cn/gtozepintx.html

val (a, b) = Pair(1, 2)
来源：http://hz.jiagoushi.top/gtkdphrnvn.html

[T13] Kotlin：只读 Map
来源：http://hz.fengsongda.top/gtioyfixth.html

val m = mapOf("a" to 1)
来源：http://hz.quarkkingdee.top/gtcxxfpnwz.html

[T14] Kotlin：循环
来源：http://hz.pycfn.com/gtyomukafx.html

for (i in 1..10) println(i)
来源：http://hz.feifeiyinyue.top/gtkotcapdb.html

[T15] Kotlin：接口
来源：http://hz.tianlin.xyz/gtgmmfvvgc.html

interface Shape { fun area(): Double }
来源：http://hz.hongshengwenyu.top/gtwaevtuks.html

[T16] Swift：Hello World
来源：http://hz.hysaishi.cn/gtnokpshye.html

print("Hello")
来源：http://hz.pycfn.com/gthsrhdlun.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gtqchgrjvo.html

var a = 1;  let b = 2
来源：http://hz.yuxming.cn/gtvvcaltne.html

[T18] Swift：字符串插值
来源：http://hz.xinyue.icu/gtxwtrkhas.html

"值: \(b)"
来源：http://hz.quarkkingdee.top/gtcrahecgb.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtgljmpgxt.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtikvnqjna.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangkeji.top/gttbvawwsr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ehwqpu.com/gtkhwvzfsn.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gttgqyzqeo.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtqmntdoac.html

[T22] Swift：字典
来源：http://hz.hongshengwenyu.top/gtukdugpwe.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.0kj1m.cn/gtznezjfrp.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gtktwmgwgu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.52xcode.cn/gtghhnulvp.html

[T24] Swift：闭包
来源：http://hz.yvedp.cn/gtdierthep.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.feifeiyinyue.top/gtazgteaut.html

[T25] Swift：结构体
来源：http://hz.jinqigfzy.top/gtepkqfukx.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gtnsaiiici.html

[T26] Swift：类与重写
来源：http://hz.aibaodan.cn/gtqytrsbil.html

class A: Base { override func f() {} }
来源：http://hz.zhoulong.xyz/gtzueowlfk.html

[T27] Swift：错误处理
来源：http://hz.yueranfly.top/gtlqhpffev.html

do { try f() } catch { print(error) }
来源：http://hz.xuanzx.com/gtzdvnbegf.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtomslhrxr.html

enum Color { case red, green }
来源：http://hz.hywenlv.cn/gtqzcaswxj.html

[T29] Swift：guard 提前返回
来源：http://hz.hnxiangtu.top/gttwdhlpmm.html

guard let x = opt else { return }
来源：http://hz.jiagoushi.top/gtaefcmzml.html

[T30] Swift：协议
来源：http://hz.pycfn.com/gtkexxbcbr.html

protocol Shape { func area() -> Double }
来源：http://hz.guannengcc.top/gtljzsqykq.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtvkdokene.html

print("Hello")
来源：http://hz.hysaishi.cn/gtlrojypcp.html

[T32] Lua：局部变量
来源：http://hz.smart0.xyz/gtovhzlycj.html

local a = 1
来源：http://hz.zhaomingkeji.xyz/gtijkggnbl.html

[T33] Lua：表（数组）
来源：http://hz.redwolf501.top/gtqyvvwcdw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhiwuduotai.top/gtdvemjklj.html

[T34] Lua：遍历表
来源：http://hz.haohaochexian.top/gtoyiatqct.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.meibo888.top/gtxpzwqqcp.html

[T35] Lua：字典表
来源：http://hz.yanxiufei.cn/gtyhynwfeu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.0kj1m.cn/gtgdfvxifn.html

[T36] Lua：函数
来源：http://hz.snrcjt.cn/gtiqadisiu.html

function add(a, b) return a + b end
来源：http://hz.gogol.net.cn/gtnqbquhpa.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtgcnsbidn.html

"a" .. "b"
来源：http://hz.cqqwz.cn/gtpmqbcrnv.html

[T38] Lua：条件
来源：http://hz.gzhubu.top/gtjqzburta.html

if x > 0 then print("正") end
来源：http://hz.wangdashe.top/gtqestklbx.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gtyqzdxzob.html

string.find(s, "%d+")
来源：http://hz.xylfe.cn/gtxwzbvmxi.html

[T40] Lua：元表
来源：http://hz.zhengqikj.top/gtyittugrw.html

setmetatable({}, { __index = base })
来源：http://hz.xuanzx.com/gtjwmhinng.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangtech.top/gtkaczxvyr.html

print "Hello\n";
来源：http://hz.yanxiufei.cn/gtzezsdnbk.html

[T42] Perl：变量类型
来源：http://hz.ivvv.top/gtwtbxyoit.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.haohaochexian.top/gtcuuxvlws.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtmepqpccm.html

"值: $a"
来源：http://hz.kuanghao11.cn/gthkkxrlqz.html

[T44] Perl：条件
来源：http://hz.mhx1999.top/gtjawhqesa.html

if ($a > 0) { print "正"; }
来源：http://hz.gaohongyu789.top/gtgivouvgm.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtgsfrquuv.html

for my $x (@arr) { print $x; }
来源：http://hz.bjfxy.top/gtprdfuoad.html

[T46] Perl：哈希操作
来源：http://hz.nanxuanxn.top/gtdgjbnsws.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yongpay.top/gtdrljfwgw.html

[T47] Perl：正则捕获
来源：http://hz.quarkkingdee.top/gtvexlpgwf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cashguo.top/gtyreloyhf.html

[T48] Perl：正则替换
来源：http://hz.shuidangran.top/gtnmtjcvpw.html

$s =~ s/old/new/g;
来源：http://hz.sxryk.cn/gtwndokrvl.html

[T49] Perl：函数
来源：http://hz.shangyingyoupin.top/gteewmofsi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tian-w.cn/gtuhbeckqm.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gtrvavahek.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtilvydxew.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gzhubu.top/gtudunwpvf.html

[T51] Scala：Hello World
来源：http://hz.ppjwa.cn/gtbcaonvtu.html

println("Hello")
来源：http://hz.aizwys.cn/gtdzvncwlx.html

[T52] Scala：变量
来源：http://hz.daxiang520.top/gtiibvrxzv.html

val a = 1;  var b = 2
来源：http://hz.chenlongwang.top/gtmypwdzrg.html

[T53] Scala：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gticgtyuri.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtqxqkckte.html

[T54] Scala：集合映射
来源：http://hz.ybcxt.top/gtmtxrxdue.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.snrcjt.cn/gtqeujspuv.html

[T55] Scala：集合过滤
来源：http://hz.yueranfly.top/gtjbbrrizk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.haohaochexian.top/gtfxsxjdow.html

[T56] Scala：样例类
来源：http://hz.nanxinkj.top/gthzstqxdq.html

case class User(name: String, age: Int)
来源：http://hz.ydzc1.top/gtemmydanr.html

[T57] Scala：模式匹配
来源：http://hz.xuetiantiany.cn/gtphgaugie.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tian-w.cn/gtnssgcaff.html

[T58] Scala：函数定义
来源：http://hz.xingfuxueyuan.xyz/gtmydnrogf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yongpay.top/gtfejcohtl.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtlipzsqqf.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuanzx.com/gtumbfdzww.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtonreifyw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtsuqypsgp.html

================================================================================
来源：http://hz.sysykeji.top/gtiafwqysd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.c1oappe.top/gtvfezpkow.html

================================================================================
来源：http://hz.jinqigfzy.top/gtstvrqzrq.html

[U01] Py：创建虚拟环境
来源：http://hz.cdnleiting.top/gtpiubihai.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhaomingkeji.xyz/gtxrwwgcig.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tianlin.xyz/gtvoxpqxzm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fengsongda.top/gtnjqrqsvc.html

[U03] Py：加载 .env 配置
来源：http://hz.jqgufenzy.top/gtqpovwapl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenjidiqi.icu/gtixeygjzv.html

[U04] Py：变量调试打印
来源：http://hz.yj20258.top/gtoancbkum.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ehwqpu.com/gtygpbhabu.html


<!-- 参考信息 -->