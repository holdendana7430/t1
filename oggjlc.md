代发 wailian999

ssh user@host 'uptime'
来源：http://hz.gotoacloud.top/gtkqwajwrc.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtgbjtbpho.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtqvpbkjqs.html

[R59] 发 POST JSON
来源：http://hz.zhijiandao.cn/gtwdfhokio.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ehwqpu.com/gtbvbxgvln.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gtvmzkuksc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangshuangyany.cn/gtqudbjftz.html

[R61] 磁盘占用
来源：http://hz.zdqjudy.top/gtnlclcque.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gtmfspieiv.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtmakhrdgg.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtebuqmmav.html

[R63] 内存与进程
来源：http://hz.c1oappe.top/gtnwxqpqar.html

free -h;  ps aux | grep nginx
来源：http://hz.zycfv.cn/gtvymsmeqz.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtvpegsexy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtbeiwmgme.html

[R65] 查看端口占用
来源：http://hz.iojbl.cn/gtezdhzegj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gogol.net.cn/gtkolagjok.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtgffcbdxx.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gttjtglmbl.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gtikgpmhoo.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gtermcjsut.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtvyiogckb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gtmkmefgap.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gtfegkmtig.html

head -c 16 /dev/urandom | base64
来源：http://hz.aizwys.cn/gtlnwmqqku.html

[R70] 时间戳与互转
来源：http://hz.pycfn.com/gtkjxammcb.html

date +%s;  date -d @1700000000
来源：http://hz.daxiang520.top/gtkbzoeyou.html

[R71] 日期格式化
来源：http://hz.aibaodan.cn/gtpcvuebyx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guowangkeji.top/gtvniipktc.html

[R72] 等待端口就绪
来源：http://hz.yuanzhike.top/gtdjpiytnv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtsqxqewlc.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gttrjpsfcg.html

split -l 1000 big.log part_
来源：http://hz.yonumen.top/gtkuqiqtai.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtmnfmiwuo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gtbvsdjmnf.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtmrrhhqih.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dianchejie.cn/gtewcgjzwg.html

[R76] 使用临时文件
来源：http://hz.cqqwz.cn/gtomyrnhnr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtntgtnhqc.html

[R77] 读取用户输入
来源：http://hz.ivvv.top/gtyzoslzsm.html

read -rp "请输入: " ans
来源：http://hz.pengpengdd.cyou/gttcjqrube.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtctvklxgp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtuljhoqyt.html

[R79] 解析命令行选项
来源：http://hz.yueranfly.top/gtjpxxahoo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgufenzy.top/gtkpnheiiq.html

[R80] 查看脚本执行耗时
来源：http://hz.cdnleiting.top/gtrzavrluo.html

time ./run.sh
来源：http://hz.gzhubu.top/gtwoxrjdts.html

================================================================================
来源：http://hz.sysykeji.top/gtexjkklvx.html

S. C / C++ 专题
来源：http://hz.gogol.net.cn/gtkqogdboo.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbsiwmthg.html

[S01] C：Hello World
来源：http://hz.sxryk.cn/gtknvkwjng.html

#include <stdio.h>
来源：http://hz.havefunace.top/gtbweknrqi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.mhx1999.top/gtavqpajmk.html

[S02] C：变量与格式化输出
来源：http://hz.cucudq.cn/gtqxznamhj.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gtvxavgmjz.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gtkidufgez.html

int x; scanf("%d", &x);
来源：http://hz.yj20258.top/gtgtuaozec.html

[S04] C：字符串复制
来源：http://hz.xylfe.cn/gtybpknapn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtquaularm.html

[S05] C：字符串长度
来源：http://hz.pengpengdd.cyou/gtjfnjzoko.html

strlen(s)
来源：http://hz.sysykeji.top/gtkuroueiu.html

[S06] C：字符串比较
来源：http://hz.hnqzz.top/gthoxunhrc.html

strcmp(a, b) == 0
来源：http://hz.daxiang520.top/gtdoanqmnk.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtuolfhcme.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtyainimro.html

[S08] C：动态内存分配与释放
来源：http://hz.quarkkingdee.top/gtiewhmkne.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sufxvd.cn/gtcrtqnggg.html

[S09] C：结构体定义与初始化
来源：http://hz.gotoacloud.top/gtwkhczwuv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gtdhugciqh.html

[S10] C：指针与解引用
来源：http://hz.ivvv.top/gtulhwcqda.html

int *p = &a;  *p = 5;
来源：http://hz.hnqzz.top/gtcvwwziac.html

[S11] C：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtigtipfcq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guowangkeji.top/gtjtcxohwf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtmzafiqje.html

fclose(f);
来源：http://hz.nanxuanxn.top/gttxhdzlzc.html

[S12] C：写文件
来源：http://hz.hnxiangtu.top/gtgcegdxop.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtzbttquna.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtnpjmejky.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtddzqwavx.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtiogrfeki.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gttzsnqdyw.html

[S15] C：类型转换
来源：http://hz.haohaochexian.top/gtfieorenw.html

(double) a / b
来源：http://hz.jinghuilouyu.cn/gtbfxxdyhn.html

[S16] C：位操作置位
来源：http://hz.jqgufenzy.top/gtwocxejab.html

x |= (1 << 3);
来源：http://hz.hywenlv.cn/gtxvrnfzxz.html

[S17] C：安全拼接字符串
来源：http://hz.kuanghao11.cn/gtbjhwksvv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fzhhl.top/gtupgvhkjs.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gtnfittlqx.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtgxdwedkd.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtihpcvtpb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtkebbubrs.html

[S20] C：二分查找
来源：http://hz.sysykeji.top/gtwqvfhmgj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtjnedjedj.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtiymtvrpx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gthiurbxsk.html

[S22] C：字符串转数字
来源：http://hz.sysykeji.top/gtqmscsvfs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gthysgqdfq.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtgapfyehv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zdqjudy.top/gtsqzvjrre.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtbztvvysm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xziqi.cn/gtfcbshegs.html

[S25] C：内存拷贝
来源：http://hz.xuetiantiany.cn/gtoeucspym.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtmviupoyv.html

[S26] C：内存清零
来源：http://hz.52xcode.cn/gtiamhftdm.html

memset(a, 0, sizeof a);
来源：http://hz.quarkkingdee.top/gtrsgqyulq.html

[S27] C：定义常量
来源：http://hz.chenjidiqi.icu/gtjvfqixyr.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtevboibzf.html

[S28] C：静态变量
来源：http://hz.ehwqpu.com/gtkjqbpbxp.html

static int counter = 0;
来源：http://hz.svipenyu.cn/gtbjysymho.html

[S29] C：变参函数
来源：http://hz.316326.xyz/gtrfkmrvrt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jyoumei.cn/gtxbazvfsr.html

[S30] C：头文件保护
来源：http://hz.zhiwuduotai.top/gtpjgcfoxr.html

#ifndef X_H
来源：http://hz.yj20258888.top/gtrwdhoarr.html

#define X_H
来源：http://hz.dashuyun.cn/gttjhmandc.html

#endif
来源：http://hz.hfpthk.cn/gtpunbmggr.html

[S31] C++：Hello World
来源：http://hz.feifeiyinyue.top/gtlrnhrffn.html

#include <iostream>
来源：http://hz.zhiwuduotai.top/gtmqexiudb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtplmxwjao.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gtdmklhxdy.html

std::string s = "hi";  s += "!";
来源：http://hz.nwbrower.top/gtrgnqbgal.html

[S33] C++：vector 增删
来源：http://hz.hnqzz.top/gtkfsqqnia.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zdqjudy.top/gturlzeziv.html

[S34] C++：遍历 vector
来源：http://hz.ywan-chungtsiang.top/gtitvxsixs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtllcjudyc.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtswadepgz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ppjwa.cn/gtgpxjmtgj.html

[S36] C++：unordered_map
来源：http://hz.cqqwz.cn/gtlvgastbd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtvlvmudpw.html

[S37] C++：set
来源：http://hz.tian-w.cn/gtptlmseou.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtdvdzwmdm.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtrdoeocpc.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtmxanppbs.html

[S39] C++：自定义比较器排序
来源：http://hz.chenjidiqi.icu/gtuvorbwvg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtjcvsemvb.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangkeji.top/gtlishmsba.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fengsongda.top/gtenyyiotn.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtboiuiald.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hammf.cn/gtkcguoclt.html

[S42] C++：继承与虚函数
来源：http://hz.gzhubu.top/gtmdojomhc.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhengqikj.top/gtebaglvze.html

[S43] C++：智能指针
来源：http://hz.cdnleiting.top/gtsabqhyfe.html

auto p = std::make_unique<int>(5);
来源：http://hz.hongshengwenyu.top/gtcjrxluty.html

[S44] C++：引用传参
来源：http://hz.wangshuangyany.cn/gtqxtgasly.html

void inc(int &x) { ++x; }
来源：http://hz.aibaodan.cn/gtjctpnlkh.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gtjgddvulw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yvedp.cn/gtnilxasyn.html

[S46] C++：函数模板
来源：http://hz.tianlin.xyz/gteddvcaco.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.mhx1999.top/gtexucyuzc.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydjk.org.cn/gtvpoyhmyr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtmlsqzzdh.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gtvhnldndi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gogol.net.cn/gtlirwbrcr.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtgmmfpfxk.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtynhgnqva.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgufenzy.top/gtauphhgts.html

[S50] C++：格式化数字
来源：http://hz.gogol.net.cn/gtvltnnezc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtxqmmyujx.html

[S51] C++：显式类型转换
来源：http://hz.xinyue.icu/gthnggydgq.html

static_cast<double>(a) / b
来源：http://hz.zycfv.cn/gtfkarevrl.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtqtdymgnu.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtouctzyym.html

[S53] C++：移动语义
来源：http://hz.52xcode.cn/gtzufivyqt.html

std::vector<int> w = std::move(v);
来源：http://hz.zhiwuduotai.top/gtbbwyknkz.html

[S54] C++：异常处理
来源：http://hz.cucudq.cn/gtshicafgf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtbulvybpu.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gtmotuwxvr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtvrjwmibl.html

[S56] C++：optional
来源：http://hz.zhaomingkeji.xyz/gtbxjymjcg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xingfuxueyuan.xyz/gtnbrlrdbe.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtfjasigrt.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtvvcwsogm.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gtuseosqlq.html

namespace ns { int f() { return 1; } }
来源：http://hz.snrcjt.cn/gtohhmpnyy.html

[S59] C++：静态断言
来源：http://hz.hnqzz.top/gtffyjkbte.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtwbtcriau.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtqltywwcx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhongyouzk.top/gtrgxmlqrc.html

================================================================================
来源：http://hz.aizwys.cn/gtxvefqrfa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtwyqbthhs.html

================================================================================
来源：http://hz.hywenlv.cn/gtcareclov.html

[T01] Kotlin：Hello World
来源：http://hz.316326.xyz/gttybbwbji.html

println("Hello")
来源：http://hz.zhixingplan.top/gtlmbgbdhj.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtkshorcuo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yueranfly.top/gtpiatmsky.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gtsnctvxyr.html

"值: $b"
来源：http://hz.hfpthk.cn/gttmexsmat.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtukznewvf.html

val n: String? = null;  n?.length
来源：http://hz.guannengcc.top/gtfmggezxh.html

[T05] Kotlin：when 表达式
来源：http://hz.0kj1m.cn/gtrsbpdbpl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.mhx1999.top/gtrrkaltvv.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gtpxdkvfet.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cashguo.top/gtggppjesc.html

[T07] Kotlin：集合过滤
来源：http://hz.hongshengwenyu.top/gtejuuwgdx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtbfjsgigu.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtjtxjcocs.html

data class User(val name: String, val age: Int)
来源：http://hz.gogol.net.cn/gtafefzchb.html

[T09] Kotlin：扩展函数
来源：http://hz.shzxlz.cn/gtkrhwcgrf.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtqmdotcjm.html

[T10] Kotlin：默认参数
来源：http://hz.cdnleiting.top/gtpyusenzp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtepwyvmaf.html

[T11] Kotlin：协程
来源：http://hz.redwolf501.top/gtyffennmn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zycfv.cn/gthpvvofdz.html

[T12] Kotlin：解构声明
来源：http://hz.svipenyu.cn/gtfbztlfhp.html

val (a, b) = Pair(1, 2)
来源：http://hz.tian-w.cn/gtjxrbwexq.html

[T13] Kotlin：只读 Map
来源：http://hz.mhx1999.top/gtwkqjfeui.html

val m = mapOf("a" to 1)
来源：http://hz.havefunace.top/gtgdfkcguz.html

[T14] Kotlin：循环
来源：http://hz.jiagoushi.top/gtcifqgthy.html

for (i in 1..10) println(i)
来源：http://hz.aizwys.cn/gtnuxtfsob.html

[T15] Kotlin：接口
来源：http://hz.xingfuxueyuan.xyz/gtzniaaobm.html

interface Shape { fun area(): Double }
来源：http://hz.52xcode.cn/gtmhmvwtad.html

[T16] Swift：Hello World
来源：http://hz.hnxiangtu.top/gtthrbngsl.html

print("Hello")
来源：http://hz.c1oappe.top/gtkddfsydk.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtsnaalhus.html

var a = 1;  let b = 2
来源：http://hz.jyoumei.cn/gtffxklcuv.html

[T18] Swift：字符串插值
来源：http://hz.tanke756.top/gtuvzksfoe.html

"值: \(b)"
来源：http://hz.xinyue.icu/gtmhmanudw.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtrfevrkyl.html

if let n = opt { print(n) }
来源：http://hz.guowangkeji.top/gtevwqwwla.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gtbthvimls.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tian-w.cn/gtbyqxshak.html

[T21] Swift：遍历
来源：http://hz.guowangkeji.top/gtonwhqubp.html

for x in a { print(x) }
来源：http://hz.zhaomingkeji.xyz/gtysddbaid.html

[T22] Swift：字典
来源：http://hz.shanyushiyangtech.top/gtjdjoeplw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinyuanbaomall.cn/gtctyxcbsn.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtcaoproby.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xziqi.cn/gtrzkncsdf.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtsgtietom.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.vqdsnc.cn/gtwtlrmtss.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gtxhhnailv.html

struct P { var x: Int }
来源：http://hz.pycfn.com/gtplqymfuw.html

[T26] Swift：类与重写
来源：http://hz.chenjidiqi.icu/gttjhmjdrr.html

class A: Base { override func f() {} }
来源：http://hz.fzhhl.top/gtesxsqsrv.html

[T27] Swift：错误处理
来源：http://hz.hammf.cn/gtibdcopcr.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gtdzrnxqdc.html

[T28] Swift：枚举
来源：http://hz.jiagoushi.top/gtukkfdztb.html

enum Color { case red, green }
来源：http://hz.yonumen.top/gttlkmenit.html

[T29] Swift：guard 提前返回
来源：http://hz.shangyingyoupin.top/gtebozigwd.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gteifupbzp.html

[T30] Swift：协议
来源：http://hz.jinghuilouyu.cn/gtmcakgnxq.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtyjzajwkz.html

[T31] Lua：Hello World
来源：http://hz.yj202588.top/gtdipnizyp.html

print("Hello")
来源：http://hz.nwbrower.top/gtaxghudpz.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gtibxfhqln.html

local a = 1
来源：http://hz.guannengcc.top/gtwlrfjncx.html

[T33] Lua：表（数组）
来源：http://hz.cdnleiting.top/gttnlmqpvn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtvbuzdkdo.html

[T34] Lua：遍历表
来源：http://hz.wangshuangyany.cn/gtbihzlymg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pengpengdd.cyou/gtafxnimqw.html

[T35] Lua：字典表
来源：http://hz.cucudq.cn/gtngvaitul.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ybcxt.top/gtexwtwulg.html

[T36] Lua：函数
来源：http://hz.dianchejie.cn/gtowldqjmn.html

function add(a, b) return a + b end
来源：http://hz.wangshuangyany.cn/gtyrkyhlsj.html

[T37] Lua：字符串拼接
来源：http://hz.tian-w.cn/gtcimyjtrw.html

"a" .. "b"
来源：http://hz.chenlongwang.top/gtxebijxjt.html

[T38] Lua：条件
来源：http://hz.nanxuanxn.top/gtjoxyfelc.html

if x > 0 then print("正") end
来源：http://hz.pycfn.com/gtmgdbadox.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangtech.top/gtlbmbdvtc.html

string.find(s, "%d+")
来源：http://hz.ehwqpu.com/gtapdkxcak.html

[T40] Lua：元表
来源：http://hz.nwbrower.top/gtbjbkplgn.html

setmetatable({}, { __index = base })
来源：http://hz.shzxlz.cn/gteqazovgu.html

[T41] Perl：Hello World
来源：http://hz.jinghuilouyu.cn/gtadqizebm.html

print "Hello\n";
来源：http://hz.yongpay.top/gtbyeowjpo.html

[T42] Perl：变量类型
来源：http://hz.jinyuanbaomall.cn/gtfnivgkjb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xziqi.cn/gtsbmqutel.html

[T43] Perl：字符串插值
来源：http://hz.snrcjt.cn/gtiwcuzxcj.html

"值: $a"
来源：http://hz.jiagoushi.top/gtrtjkggfe.html

[T44] Perl：条件
来源：http://hz.yongpay.top/gthehkfdxh.html

if ($a > 0) { print "正"; }
来源：http://hz.yuanzhike.top/gttazufoxz.html

[T45] Perl：数组遍历
来源：http://hz.pengpengdd.cyou/gtrngbcxyl.html

for my $x (@arr) { print $x; }
来源：http://hz.chenjidiqi.icu/gtssmypeuh.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gtzuqlqxht.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.iojbl.cn/gtzhweyfgi.html

[T47] Perl：正则捕获
来源：http://hz.yj202588.top/gtkawiyrub.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xylfe.cn/gtpzakkpti.html

[T48] Perl：正则替换
来源：http://hz.hfpthk.cn/gtirghwiid.html

$s =~ s/old/new/g;
来源：http://hz.gzhubu.top/gtgqmpwbbz.html

[T49] Perl：函数
来源：http://hz.tanke756.top/gtzehhjdyg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigufen.top/gtbsgkeoqx.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtkynrdyej.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.guowangkeji.top/gtkzgazyhd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.dianchejie.cn/gtewrxeuxp.html

[T51] Scala：Hello World
来源：http://hz.zhiwuduotai.top/gtiueahvea.html

println("Hello")
来源：http://hz.birdmap.top/gtnotkinji.html

[T52] Scala：变量
来源：http://hz.birdmap.top/gtbawmxlkv.html

val a = 1;  var b = 2
来源：http://hz.tanke756.top/gtlnakeizn.html

[T53] Scala：字符串插值
来源：http://hz.gaohongyu789.top/gtsieyvaqn.html

s"值: $b"
来源：http://hz.shzxlz.cn/gttohdanpn.html

[T54] Scala：集合映射
来源：http://hz.shzxlz.cn/gthtrcryov.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.c1oappe.top/gtkxsvjuqh.html

[T55] Scala：集合过滤
来源：http://hz.haohaochexian.top/gtjdwtimxl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.meibo888.top/gttcrafflx.html

[T56] Scala：样例类
来源：http://hz.havefunace.top/gtrgkvvpde.html

case class User(name: String, age: Int)
来源：http://hz.hysaishi.cn/gtcmflkyfs.html

[T57] Scala：模式匹配
来源：http://hz.nwbrower.top/gttyevoviq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xziqi.cn/gtwftobqij.html

[T58] Scala：函数定义
来源：http://hz.jlsjyb.cn/gtviwpxpqy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.haohaochexian.top/gtmngrciei.html

[T59] Scala：循环
来源：http://hz.hammf.cn/gthtbprqtw.html

for (i <- 1 to 10) println(i)
来源：http://hz.fengsongda.top/gtqeolxpry.html

[T60] Scala：折叠
来源：http://hz.sweek.top/gtidzaxede.html


<!-- 参考信息 -->