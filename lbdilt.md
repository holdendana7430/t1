代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtypzzuuqw.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtstcimjwo.html

scp file user@host:/path/
来源：http://hz.0kj1m.cn/gtitbkuhhf.html

[R57] 远程执行命令
来源：http://hz.jyoumei.cn/gtupcnyrzi.html

ssh user@host 'uptime'
来源：http://hz.zhijiandao.cn/gtzqlizykz.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtybpweqli.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gthavsgyty.html

[R59] 发 POST JSON
来源：http://hz.iojbl.cn/gtehafnbae.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jiagoushi.top/gtypajbrlj.html

[R60] 只看 HTTP 状态码
来源：http://hz.aizwys.cn/gtjvshrbdh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtahymapma.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gtowuwfmpf.html

df -h;  du -sh *
来源：http://hz.c1oappe.top/gtqkqnfcfg.html

[R62] 找最占空间的文件
来源：http://hz.sweek.top/gttlnmnmtl.html

du -ah . | sort -rh | head -10
来源：http://hz.andypj.xyz/gtmwmlhoql.html

[R63] 内存与进程
来源：http://hz.hywenlv.cn/gtrelrxexp.html

free -h;  ps aux | grep nginx
来源：http://hz.hongshengwenyu.top/gttqnhscry.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtlyqluvpm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtokuxuujm.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtvukqpyqm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jianghu66.top/gtozajqgag.html

[R66] 定时任务
来源：http://hz.pycfn.com/gtsyydqpak.html

crontab -e;  crontab -l
来源：http://hz.shuidangran.top/gtqgsaaqzq.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtveutljmp.html

openssl rand -hex 16
来源：http://hz.dianchejie.cn/gteykhgbtr.html

[R68] 计算文件校验值
来源：http://hz.zdqjudy.top/gtamvkywfp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtlqnmzawn.html

[R69] 生成随机密码
来源：http://hz.yongpay.top/gtfzyumyku.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtzcoaygph.html

[R70] 时间戳与互转
来源：http://hz.gaohongyu789.top/gttfebkbac.html

date +%s;  date -d @1700000000
来源：http://hz.dianchejie.cn/gtecpzhwsq.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtxqrfvkek.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenjidiqi.icu/gtjtnpgyib.html

[R72] 等待端口就绪
来源：http://hz.guannengcc.top/gtcpykuuyu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xinyue.icu/gtmifmucwb.html

[R73] 分割大日志
来源：http://hz.c1oappe.top/gtptgwwlkh.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtlitzyzrh.html

[R74] 批量重命名
来源：http://hz.cashguo.top/gtlrbjmdoa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gthmfivryg.html

[R75] 导出环境变量
来源：http://hz.cashguo.top/gtlxofmnlf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xziqi.cn/gtfkvfebfb.html

[R76] 使用临时文件
来源：http://hz.chenzaomai.com/gtxpjiotbv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtpneozxgj.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangkeji.top/gtpkkoxcqk.html

read -rp "请输入: " ans
来源：http://hz.chenzaomai.com/gtqiqiwuye.html

[R78] 交互式菜单
来源：http://hz.quarkkingdee.top/gtekxhaqpd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtmpilnivq.html

[R79] 解析命令行选项
来源：http://hz.xylfe.cn/gtieejydre.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.bjfxy.top/gtzwcosrrf.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtkagiipzu.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gtsxerikrj.html

================================================================================
来源：http://hz.hfpthk.cn/gtxlcvgcoi.html

S. C / C++ 专题
来源：http://hz.yongpay.top/gthpyhyjuz.html

================================================================================
来源：http://hz.hysaishi.cn/gtyjzhtwun.html

[S01] C：Hello World
来源：http://hz.dianchejie.cn/gtfzxarzyg.html

#include <stdio.h>
来源：http://hz.redwolf501.top/gtuxqpvldy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinghuilouyu.cn/gtitxshbat.html

[S02] C：变量与格式化输出
来源：http://hz.zdqjudy.top/gtblvzqsba.html

int a = 10; printf("%d\n", a);
来源：http://hz.yangfankeji.com/gtxnieytrp.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtkymhbjsv.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtwzmjrakq.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gthrvfvlpx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shangyingyoupin.top/gtiqbpuwvz.html

[S05] C：字符串长度
来源：http://hz.zhaomingkeji.xyz/gtddzfisvd.html

strlen(s)
来源：http://hz.hfpthk.cn/gtgfxsrvoy.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gtgldhctmu.html

strcmp(a, b) == 0
来源：http://hz.hnqzz.top/gtulednldz.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtmbarslzg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtzrsecdqk.html

[S08] C：动态内存分配与释放
来源：http://hz.sweek.top/gthopzxnlu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gtesosoukw.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gtfktieqvu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gthdlwiajh.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtjriyuejc.html

int *p = &a;  *p = 5;
来源：http://hz.hfpthk.cn/gtlimjukir.html

[S11] C：逐行读文件
来源：http://hz.shzxlz.cn/gtsdmjfwxw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtihsjqlkb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gogol.net.cn/gtauslixwu.html

fclose(f);
来源：http://hz.nwbrower.top/gtgtiqinxp.html

[S12] C：写文件
来源：http://hz.chenzaomai.com/gtohhpgkeq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtravhohzw.html

[S13] C：宏定义
来源：http://hz.iojbl.cn/gtqpbawjjf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.mhx1999.top/gtehhchivs.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtjlaqoala.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangtech.top/gtomcxuwtp.html

[S15] C：类型转换
来源：http://hz.ppjwa.cn/gthujrqtfc.html

(double) a / b
来源：http://hz.shangyingyoupin.top/gtjzizcesq.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtmyizijxg.html

x |= (1 << 3);
来源：http://hz.316326.xyz/gtoqkctdin.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gtwofaugoo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ehwqpu.com/gtwfmnnapx.html

[S18] C：命令行参数
来源：http://hz.52xcode.cn/gtqyrdaovq.html

int main(int argc, char **argv)
来源：http://hz.hywenlv.cn/gtealuilto.html

[S19] C：快速排序
来源：http://hz.pengpengdd.cyou/gteuweffde.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtcdxesyfo.html

[S20] C：二分查找
来源：http://hz.gotoacloud.top/gtzinavakm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtzoceholl.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gtpmlwtimh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinghuilouyu.cn/gtsltojypj.html

[S22] C：字符串转数字
来源：http://hz.yj20258888.top/gtayiqvrvv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hywenlv.cn/gttgyaxugw.html

[S23] C：随机数
来源：http://hz.gaohongyu789.top/gtzvqtfrhb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtdazlfkou.html

[S24] C：获取本地时间
来源：http://hz.hammf.cn/gtubdvxqxa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuetiantiany.cn/gtupfrumxb.html

[S25] C：内存拷贝
来源：http://hz.zhijiandao.cn/gtzqdbpzbg.html

memcpy(dst, src, n);
来源：http://hz.52xcode.cn/gtphxpbpyk.html

[S26] C：内存清零
来源：http://hz.gaohongyu789.top/gtgtjmjmds.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gthowxufpe.html

[S27] C：定义常量
来源：http://hz.dianchejie.cn/gtbeuwacdi.html

const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtptzqxhzk.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtpresxxfb.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtlyrggtpy.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtjmsapara.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtzjiqcccj.html

[S30] C：头文件保护
来源：http://hz.jqgufenzy.top/gtaveutnsh.html

#ifndef X_H
来源：http://hz.dashuyun.cn/gtazuomzaj.html

#define X_H
来源：http://hz.0kj1m.cn/gtfgpuzbtr.html

#endif
来源：http://hz.hammf.cn/gtlpehcmkr.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtqaztawhx.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtgxyzydxp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtqcjwepwh.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtuiomzvpy.html

std::string s = "hi";  s += "!";
来源：http://hz.hywenlv.cn/gtgjijycpr.html

[S33] C++：vector 增删
来源：http://hz.yj20258888.top/gtrmrsoddk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sweek.top/gtzlnphmda.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtmmjvdfsy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhiwuduotai.top/gtfkphfyps.html

[S35] C++：map
来源：http://hz.redwolf501.top/gtoppwlnte.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtoqndxpsc.html

[S36] C++：unordered_map
来源：http://hz.fengsongda.top/gtwynqymid.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtzxjiciri.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtsbjlrasy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gthpvazupm.html

[S38] C++：排序
来源：http://hz.fzhhl.top/gtqnoihicg.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtodexeixd.html

[S39] C++：自定义比较器排序
来源：http://hz.daria6918.cn/gtgqwsjwlt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.redwolf501.top/gtcaqlphsm.html

[S40] C++：查找元素
来源：http://hz.dashuyun.cn/gtoximikkr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shuidangran.top/gtlqfzcmbm.html

[S41] C++：类与构造函数
来源：http://hz.gotoacloud.top/gtmiqeggqv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtplhohghj.html

[S42] C++：继承与虚函数
来源：http://hz.aizwys.cn/gtefsloser.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtcagxnibp.html

[S43] C++：智能指针
来源：http://hz.pengpengdd.cyou/gtuhvbtuuw.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenlongwang.top/gtphhjlkqf.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtltjjjvhh.html

void inc(int &x) { ++x; }
来源：http://hz.jqgfzy.top/gtdfoiirny.html

[S45] C++：lambda
来源：http://hz.tanke756.top/gtjqktfzsg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtqbbugupp.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gtjmywdxki.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtemiizvfo.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gtzroxowgo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.316326.xyz/gtqfnkfmmn.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtxlgrddit.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tianlin.xyz/gtmcoakdoi.html

while (std::getline(in, line)) { }
来源：http://hz.zhengqikj.top/gtrzlijvfx.html

[S49] C++：写文件
来源：http://hz.yonumen.top/gtmesipqbb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zdqjudy.top/gtxfommowh.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtzeiyhprp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jiagoushi.top/gturyrprli.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtqeruuviu.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtsgatupha.html

[S52] C++：const 与 noexcept
来源：http://hz.sysykeji.top/gtrzmvwars.html

int size() const noexcept { return n_; }
来源：http://hz.yvedp.cn/gtjlasofqn.html

[S53] C++：移动语义
来源：http://hz.guowangkeji.top/gtdfegvbkh.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtkeaseosd.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gtcjytbsac.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hywenlv.cn/gtxrxvpuod.html

[S55] C++：结构化绑定
来源：http://hz.jqgufenzy.top/gtttbweeur.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ybcxt.top/gtwhplnmxp.html

[S56] C++：optional
来源：http://hz.nanxinkj.top/gtujnrosir.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gtimsxoqtb.html

[S57] C++：编译期常量
来源：http://hz.cucudq.cn/gtmuyjysyg.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gttghablal.html

[S58] C++：命名空间
来源：http://hz.316326.xyz/gtnakziumf.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinghuilouyu.cn/gtgqhavhpy.html

[S59] C++：静态断言
来源：http://hz.chenzaomai.com/gtcgwpgeyl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtsuoqjymu.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtujfrfoaf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gtqpxlecgy.html

================================================================================
来源：http://hz.tian-w.cn/gtxfoedrhj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtjanheeot.html

================================================================================
来源：http://hz.cashguo.top/gtuamujhtp.html

[T01] Kotlin：Hello World
来源：http://hz.sufxvd.cn/gtmgdccbew.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtqrozkene.html

[T02] Kotlin：变量
来源：http://hz.zhoulong.xyz/gtlktusrft.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnxiangtu.top/gtialrmluv.html

[T03] Kotlin：字符串模板
来源：http://hz.tian-w.cn/gtwixshsph.html

"值: $b"
来源：http://hz.haohaochexian.top/gtslrqmbzw.html

[T04] Kotlin：空安全
来源：http://hz.yueranfly.top/gtxfxgguxh.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtqdmhlpoo.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtswrufggf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gttlmiolka.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtrffgfqll.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtofkngnki.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtrvowffml.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtxyvlufwx.html

[T08] Kotlin：数据类
来源：http://hz.jqgufenzy.top/gtfgzdgeak.html

data class User(val name: String, val age: Int)
来源：http://hz.cucudq.cn/gtwrtikeay.html

[T09] Kotlin：扩展函数
来源：http://hz.chenzaomai.com/gtsuqnekyl.html

fun String.exclaim() = this + "!"
来源：http://hz.redwolf501.top/gtyedzbwqu.html

[T10] Kotlin：默认参数
来源：http://hz.quarkkingdee.top/gtmvbigyoo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtqeyusoog.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtuglyvfap.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtxnstvmql.html

[T12] Kotlin：解构声明
来源：http://hz.zhengqikj.top/gtispkfmjf.html

val (a, b) = Pair(1, 2)
来源：http://hz.sxryk.cn/gtqtzzteoo.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtrhrogdte.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtlqjpqxqw.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtcjemugxp.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gthskvmulh.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtujbyzcud.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gttydplose.html

[T16] Swift：Hello World
来源：http://hz.jianghu66.top/gtkhlcexsr.html

print("Hello")
来源：http://hz.meibo888.top/gtxquxcsao.html

[T17] Swift：变量与常量
来源：http://hz.bjfxy.top/gtqhurkxsh.html

var a = 1;  let b = 2
来源：http://hz.ppjwa.cn/gtggckrvml.html

[T18] Swift：字符串插值
来源：http://hz.0kj1m.cn/gtgbynoqpo.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gthnhmptps.html

[T19] Swift：可选绑定
来源：http://hz.chenzaomai.com/gttpuxwugd.html

if let n = opt { print(n) }
来源：http://hz.0kj1m.cn/gtcctiwtcr.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gtslqpxlni.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtsnfrgtgo.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtzbtclbgw.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtwezbrgkw.html

[T22] Swift：字典
来源：http://hz.guowangkeji.top/gtqeseodxj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gzhubu.top/gtmgstiamq.html

[T23] Swift：函数
来源：http://hz.sysykeji.top/gtbyfjdxcn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtbyxpiogm.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gtynvqgupl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigfzy.top/gtqncjcjma.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtsoziwfbh.html

struct P { var x: Int }
来源：http://hz.nanxuanxn.top/gtlenascib.html

[T26] Swift：类与重写
来源：http://hz.mhx1999.top/gtalljauiz.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtepmyucbn.html

[T27] Swift：错误处理
来源：http://hz.ydzc1.top/gtltiqtsss.html

do { try f() } catch { print(error) }
来源：http://hz.shzxlz.cn/gtyreyfhyq.html

[T28] Swift：枚举
来源：http://hz.pengpengdd.cyou/gtkrdquwaf.html

enum Color { case red, green }
来源：http://hz.gaohongyu789.top/gtajrveyom.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtdgtmskzk.html

guard let x = opt else { return }
来源：http://hz.aibaodan.cn/gtprjuetqz.html

[T30] Swift：协议
来源：http://hz.dianchejie.cn/gtdywoxcow.html

protocol Shape { func area() -> Double }
来源：http://hz.mhx1999.top/gtdycubbmy.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtqbinxtth.html

print("Hello")
来源：http://hz.ydjk.org.cn/gtpzqapuwo.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtvkiqenfh.html

local a = 1
来源：http://hz.ybcxt.top/gtpuvrxxfz.html

[T33] Lua：表（数组）
来源：http://hz.zhijiandao.cn/gtmlghxhpk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtralmdgck.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtprwrhfeq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtgnvagkqk.html

[T35] Lua：字典表
来源：http://hz.hnqzz.top/gtoztekosu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.daxiang520.top/gtfrgcwecq.html

[T36] Lua：函数
来源：http://hz.xingfuxueyuan.xyz/gttndtwjsz.html

function add(a, b) return a + b end
来源：http://hz.gogol.net.cn/gtmieirbxa.html

[T37] Lua：字符串拼接
来源：http://hz.hfpthk.cn/gtmyepxkei.html

"a" .. "b"
来源：http://hz.hnxiangtu.top/gthflhnpaz.html

[T38] Lua：条件
来源：http://hz.daxiang520.top/gtfxwmuuwr.html

if x > 0 then print("正") end
来源：http://hz.yonumen.top/gtweynkian.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gtdswfoitd.html

string.find(s, "%d+")
来源：http://hz.jinghuilouyu.cn/gtgyycjrjz.html

[T40] Lua：元表
来源：http://hz.316326.xyz/gtdnlnjiwh.html

setmetatable({}, { __index = base })
来源：http://hz.jqgufenzy.top/gtchddswam.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gthqdgzwty.html

print "Hello\n";
来源：http://hz.gaohongyu789.top/gtmroivaxy.html

[T42] Perl：变量类型
来源：http://hz.cucudq.cn/gtbisywyyw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gthmjumlko.html

[T43] Perl：字符串插值
来源：http://hz.tian-w.cn/gtxlbvqihu.html

"值: $a"
来源：http://hz.cashguo.top/gtxrhcxxiy.html

[T44] Perl：条件
来源：http://hz.yj20258.top/gtqongjzow.html

if ($a > 0) { print "正"; }
来源：http://hz.zhongyouzk.top/gtunojpxqi.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtemxkajqf.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangkeji.top/gtmfrvqhcj.html

[T46] Perl：哈希操作
来源：http://hz.yj20258888.top/gtculzhhzo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.iojbl.cn/gtutnsdcun.html

[T47] Perl：正则捕获
来源：http://hz.jinqigfzy.top/gtdinydepe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtatgjtdzf.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gtwazhlxff.html

$s =~ s/old/new/g;
来源：http://hz.316326.xyz/gtetjhufwx.html

[T49] Perl：函数
来源：http://hz.ivvv.top/gtvqsasaqo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.birdmap.top/gtqgbvyzyo.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigfzy.top/gtxipcjizn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigfzy.top/gtcruyptdg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shangyingyoupin.top/gtuompqhtx.html

[T51] Scala：Hello World
来源：http://hz.sysykeji.top/gtabarbohz.html

println("Hello")
来源：http://hz.snrcjt.cn/gtkfniosjk.html

[T52] Scala：变量
来源：http://hz.ybcxt.top/gthuxnruea.html

val a = 1;  var b = 2
来源：http://hz.kuanghao11.cn/gtgwevfgdu.html

[T53] Scala：字符串插值
来源：http://hz.jiagoushi.top/gtqigbvlrr.html

s"值: $b"
来源：http://hz.ehwqpu.com/gtncncreal.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtzzssoucs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.meibo888.top/gtjivgifwb.html

[T55] Scala：集合过滤
来源：http://hz.zhoulong.xyz/gtvefkamay.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yueranfly.top/gtffmiggdv.html

[T56] Scala：样例类
来源：http://hz.dashuyun.cn/gtnlftonuf.html

case class User(name: String, age: Int)
来源：http://hz.xuetiantiany.cn/gtxpbvqaai.html

[T57] Scala：模式匹配
来源：http://hz.c1oappe.top/gtrlxvaaic.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtfsjiutcy.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtpxwxydta.html


<!-- 参考信息 -->