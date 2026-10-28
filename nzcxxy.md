代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtujxbmznu.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtxbzyewzw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xziqi.cn/gtlvqlwaji.html

[R51] 排序去重取前几
来源：http://hz.wangdashe.top/gtjkeaqplh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.snrcjt.cn/gtxehmnyer.html

[R52] 统计行数
来源：http://hz.hfpthk.cn/gtqztjclcj.html

wc -l a.txt
来源：http://hz.shuidangran.top/gtakpbxcca.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgfzy.top/gtlfzewvvp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtkzupyzcv.html

[R54] 比较两个文件
来源：http://hz.hfpthk.cn/gtifijkirx.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtmuvwmygv.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtfbtiizob.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtnzrajbqh.html

[R56] 远程拷贝
来源：http://hz.ydjk.org.cn/gtgbhndhro.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gtnplgpjpu.html

[R57] 远程执行命令
来源：http://hz.nwbrower.top/gtlxflscgp.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtjbbrmbwo.html

[R58] 下载文件
来源：http://hz.chenlongwang.top/gtltbpruxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtbnsimiuw.html

[R59] 发 POST JSON
来源：http://hz.ivvv.top/gtkjeorfez.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gogol.net.cn/gtuobwwnvo.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtbasiqkeo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtagcdjfst.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtzakyowam.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtbaqcxiow.html

[R62] 找最占空间的文件
来源：http://hz.yueranfly.top/gthffwrjdt.html

du -ah . | sort -rh | head -10
来源：http://hz.jlsjyb.cn/gtbkahrhfm.html

[R63] 内存与进程
来源：http://hz.jqgufenzy.top/gtrauajozx.html

free -h;  ps aux | grep nginx
来源：http://hz.wangdashe.top/gthhxxneht.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtcjgrzsyz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtpzrcjdyc.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtugddubkl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtqnsrjcrs.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gttipjhbwk.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gtcylltjlo.html

[R67] 生成随机十六进制串
来源：http://hz.vqdsnc.cn/gtvmzcbmzm.html

openssl rand -hex 16
来源：http://hz.yuanzhike.top/gtvcjspddz.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtemmdkkek.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.gzhubu.top/gtikiitbac.html

[R69] 生成随机密码
来源：http://hz.yangfankeji.com/gtbrlgxytn.html

head -c 16 /dev/urandom | base64
来源：http://hz.yonumen.top/gttwdlnqvh.html

[R70] 时间戳与互转
来源：http://hz.fzhhl.top/gtobtzljkz.html

date +%s;  date -d @1700000000
来源：http://hz.xylfe.cn/gtvogbqvdy.html

[R71] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtzqqvfhls.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nwbrower.top/gtkecpukle.html

[R72] 等待端口就绪
来源：http://hz.birdmap.top/gtpcnnswzc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtomexdaxd.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtuagrgwxm.html

split -l 1000 big.log part_
来源：http://hz.hysaishi.cn/gtzsxsrwod.html

[R74] 批量重命名
来源：http://hz.zhoulong.xyz/gtzlmocnka.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhijiandao.cn/gtboofjujf.html

[R75] 导出环境变量
来源：http://hz.ywan-chungtsiang.top/gtywviwvat.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtecjrxzoj.html

[R76] 使用临时文件
来源：http://hz.zhijiandao.cn/gtwbnwhcng.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtkrejjlxv.html

[R77] 读取用户输入
来源：http://hz.ywan-chungtsiang.top/gtgztipcnk.html

read -rp "请输入: " ans
来源：http://hz.jlsjyb.cn/gtzboxkzxh.html

[R78] 交互式菜单
来源：http://hz.cucudq.cn/gtrkwvrnyb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sufxvd.cn/gtdwvwdzqv.html

[R79] 解析命令行选项
来源：http://hz.hnqzz.top/gtuommgswl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gtsnhzbanb.html

[R80] 查看脚本执行耗时
来源：http://hz.zhengqikj.top/gtfvsekrso.html

time ./run.sh
来源：http://hz.yonumen.top/gtrgdjkmfl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdxskclmq.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gtykhliwoy.html

================================================================================
来源：http://hz.sysykeji.top/gtrwdclshm.html

[S01] C：Hello World
来源：http://hz.sxryk.cn/gtgovuybip.html

#include <stdio.h>
来源：http://hz.yongpay.top/gtysfmcdxp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtocgzvyto.html

[S02] C：变量与格式化输出
来源：http://hz.zhengqikj.top/gtgpbhjwyn.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangshuangyany.cn/gtufroxfbb.html

[S03] C：读入整数
来源：http://hz.cashguo.top/gtpocctzer.html

int x; scanf("%d", &x);
来源：http://hz.cashguo.top/gtugqivlng.html

[S04] C：字符串复制
来源：http://hz.yueranfly.top/gtzsosefoo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigufen.top/gtjpvthhkm.html

[S05] C：字符串长度
来源：http://hz.ehwqpu.com/gtbpryymdt.html

strlen(s)
来源：http://hz.fengsongda.top/gtnlrhklcg.html

[S06] C：字符串比较
来源：http://hz.ivvv.top/gtfenmqdbf.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gtmiithpph.html

[S07] C：数组遍历求和
来源：http://hz.chenlongwang.top/gtvnslmncv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gaohongyu789.top/gtsttfljxy.html

[S08] C：动态内存分配与释放
来源：http://hz.chenzaomai.com/gtyrcdsist.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ybcxt.top/gtcjcqlywl.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtcnrbvgos.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtrxydmnew.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtckgeyorb.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtphpuuvuv.html

[S11] C：逐行读文件
来源：http://hz.nanxinkj.top/gtqnanupdi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxinkj.top/gtaoebqipz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yanxiufei.cn/gtafwsagbu.html

fclose(f);
来源：http://hz.xuanzx.com/gtumsyghhd.html

[S12] C：写文件
来源：http://hz.xuanzx.com/gtzrnzjioi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gtyybegvut.html

[S13] C：宏定义
来源：http://hz.mhx1999.top/gtjoyvupgl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gthngnczey.html

[S14] C：枚举
来源：http://hz.yangfankeji.com/gtvwcwlmjn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.meibo888.top/gthfnpfylk.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtmofqwkwh.html

(double) a / b
来源：http://hz.sxryk.cn/gtvtnkjvcd.html

[S16] C：位操作置位
来源：http://hz.smart0.xyz/gtseerkglw.html

x |= (1 << 3);
来源：http://hz.sweek.top/gtsbuhcqqy.html

[S17] C：安全拼接字符串
来源：http://hz.havefunace.top/gtxvkfbuqj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtltbsjrzs.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gtzefvfxxl.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gtrlyitptp.html

[S19] C：快速排序
来源：http://hz.316326.xyz/gtyxmhkovv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtvtrqfbep.html

[S20] C：二分查找
来源：http://hz.zhijiandao.cn/gthquexxmt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtyodhutrj.html

[S21] C：字符类别判断
来源：http://hz.svipenyu.cn/gtufgskpzf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtmatskfmh.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtgwpvsgmn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtjymtsius.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gtvmaachjy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.mhx1999.top/gtnubepyqb.html

[S24] C：获取本地时间
来源：http://hz.jqgfzy.top/gtcqbpbeml.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtlriwzvjx.html

[S25] C：内存拷贝
来源：http://hz.c1oappe.top/gtpquwlpuj.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtdkgwvapq.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtzuckxqnu.html

memset(a, 0, sizeof a);
来源：http://hz.guowangkeji.top/gtnvyzumig.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtosuwnmur.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtovnjdtwa.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gtrreacyha.html

static int counter = 0;
来源：http://hz.jyoumei.cn/gtzdjdpngo.html

[S29] C：变参函数
来源：http://hz.jqgfzy.top/gtxtvdntzl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtkhvnkdzs.html

[S30] C：头文件保护
来源：http://hz.yonumen.top/gtpcohpvln.html

#ifndef X_H
来源：http://hz.zhoulong.xyz/gtqldrimbw.html

#define X_H
来源：http://hz.yvedp.cn/gtlvjhotqz.html

#endif
来源：http://hz.ivvv.top/gtpisbqzcl.html

[S31] C++：Hello World
来源：http://hz.gogol.net.cn/gtntibumva.html

#include <iostream>
来源：http://hz.jinqigufen.top/gtmmwfgqgp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hfpthk.cn/gtiumdgjyt.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gthpkafdub.html

std::string s = "hi";  s += "!";
来源：http://hz.xingfuxueyuan.xyz/gtgbsifmpz.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtwyrzalkl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.kuanghao11.cn/gtadnihjhn.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtphzpignb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtmuvmakdp.html

[S35] C++：map
来源：http://hz.xuetiantiany.cn/gtxuxrjfzs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtmdtokpjv.html

[S36] C++：unordered_map
来源：http://hz.feifeiyinyue.top/gtezcyayzr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtogbbbtat.html

[S37] C++：set
来源：http://hz.hywenlv.cn/gtdxwnquon.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtznkujuja.html

[S38] C++：排序
来源：http://hz.gogol.net.cn/gtcdaelzey.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gtmhozjvuc.html

[S39] C++：自定义比较器排序
来源：http://hz.kuanghao11.cn/gtgdezcmuh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ybcxt.top/gtfnyibvax.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtjmkxsdgp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gotoacloud.top/gttltcimji.html

[S41] C++：类与构造函数
来源：http://hz.xziqi.cn/gtwelvwyxe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtvhbrkraf.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtkjcaxwar.html

class B : public Base { public: void f() override {} };
来源：http://hz.dashuyun.cn/gtyevyopvg.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gtaoqzxrzv.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhaomingkeji.xyz/gtdivqlblj.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtpzdqrkgw.html

void inc(int &x) { ++x; }
来源：http://hz.nwbrower.top/gtdfnnlwyl.html

[S45] C++：lambda
来源：http://hz.dianchejie.cn/gtfivaeqto.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtgyyyorxr.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtofwavpxj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.redwolf501.top/gtngxrbtif.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtjezdcnuc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yongpay.top/gtwmrhatia.html

[S48] C++：逐行读文件
来源：http://hz.sufxvd.cn/gtbsollqxf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jlsjyb.cn/gtmvoxwanm.html

while (std::getline(in, line)) { }
来源：http://hz.zhixingplan.top/gtmtitrhth.html

[S49] C++：写文件
来源：http://hz.cucudq.cn/gtjncgjfct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgfzy.top/gtbpaqobuy.html

[S50] C++：格式化数字
来源：http://hz.andypj.xyz/gtytdikrcl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.feifeiyinyue.top/gtjxxciqub.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gtrsxgltbb.html

static_cast<double>(a) / b
来源：http://hz.yuxming.cn/gtkuwfzxlx.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtjxylbvkj.html

int size() const noexcept { return n_; }
来源：http://hz.shzxlz.cn/gthujkrppo.html

[S53] C++：移动语义
来源：http://hz.iojbl.cn/gthxivyngk.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gthdqreiyy.html

[S54] C++：异常处理
来源：http://hz.sufxvd.cn/gtpctvkxqg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gtzskcsllw.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtjaiciiyn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hfpthk.cn/gthgtzdvxu.html

[S56] C++：optional
来源：http://hz.cheryme.top/gtagpxpfwa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gttoxqfyvb.html

[S57] C++：编译期常量
来源：http://hz.jlsjyb.cn/gtwqrnenbm.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtsdgxevsn.html

[S58] C++：命名空间
来源：http://hz.gaohongyu789.top/gtmobwwfhh.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gtqxkxwxio.html

[S59] C++：静态断言
来源：http://hz.cdnleiting.top/gtsbdnlzte.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtixffquub.html

[S60] C++：遍历并删除元素
来源：http://hz.zhongyouzk.top/gtzukgrnbm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtmswuykdw.html

================================================================================
来源：http://hz.ybcxt.top/gttmuzvtcm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtbnbpfxxt.html

================================================================================
来源：http://hz.andypj.xyz/gtpzalpxzo.html

[T01] Kotlin：Hello World
来源：http://hz.meibo888.top/gtxhfildvb.html

println("Hello")
来源：http://hz.bjfxy.top/gtvfimveuq.html

[T02] Kotlin：变量
来源：http://hz.xylfe.cn/gtabrikqki.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnxiangtu.top/gtbiafouik.html

[T03] Kotlin：字符串模板
来源：http://hz.yangfankeji.com/gtkbinyqhp.html

"值: $b"
来源：http://hz.zhoulong.xyz/gtrgqjjuox.html

[T04] Kotlin：空安全
来源：http://hz.52xcode.cn/gtqrkkveqj.html

val n: String? = null;  n?.length
来源：http://hz.fengsongda.top/gthqtvbwcb.html

[T05] Kotlin：when 表达式
来源：http://hz.hammf.cn/gtkfylgwhh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtsbwpmrpe.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gtokhcbmrp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gtjqankegs.html

[T07] Kotlin：集合过滤
来源：http://hz.xingfuxueyuan.xyz/gtpdnqirqt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtjfbdkxjb.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gthnudvoew.html

data class User(val name: String, val age: Int)
来源：http://hz.hfpthk.cn/gtsdqoalit.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxuanxn.top/gtuvuwtwsq.html

fun String.exclaim() = this + "!"
来源：http://hz.shangyingyoupin.top/gtiteegzss.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gtkdonaaet.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.redwolf501.top/gtihycvumh.html

[T11] Kotlin：协程
来源：http://hz.nwbrower.top/gtnpfrpxlp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hfpthk.cn/gtlevprsjk.html

[T12] Kotlin：解构声明
来源：http://hz.yangfankeji.com/gtwhfcktew.html

val (a, b) = Pair(1, 2)
来源：http://hz.kuanghao11.cn/gtpcsoxqby.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtnwmidfar.html

val m = mapOf("a" to 1)
来源：http://hz.jqgufenzy.top/gtijpvuand.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtzsfzrjgw.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtuukhwqzs.html

[T15] Kotlin：接口
来源：http://hz.cashguo.top/gtqnehghep.html

interface Shape { fun area(): Double }
来源：http://hz.redwolf501.top/gtidsrihpj.html

[T16] Swift：Hello World
来源：http://hz.hysaishi.cn/gtosemqool.html

print("Hello")
来源：http://hz.iojbl.cn/gtrwnoncdk.html

[T17] Swift：变量与常量
来源：http://hz.zhoulong.xyz/gtueksgyeu.html

var a = 1;  let b = 2
来源：http://hz.tanke756.top/gtwxiviepm.html

[T18] Swift：字符串插值
来源：http://hz.hnxiangtu.top/gtgajdrgga.html

"值: \(b)"
来源：http://hz.yongpay.top/gtcnaetmyi.html

[T19] Swift：可选绑定
来源：http://hz.yanxiufei.cn/gtnblayvmw.html

if let n = opt { print(n) }
来源：http://hz.guannengcc.top/gtdsrzqyew.html

[T20] Swift：数组操作
来源：http://hz.bjfxy.top/gtytxgskrk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtcxleteoh.html

[T21] Swift：遍历
来源：http://hz.cucudq.cn/gtonfcnnlk.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtyyfnkxud.html

[T22] Swift：字典
来源：http://hz.jinqigfzy.top/gtgpscqypp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ywan-chungtsiang.top/gtoptlnlch.html

[T23] Swift：函数
来源：http://hz.zdqjudy.top/gtverggnsl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cucudq.cn/gtrnrqbzln.html

[T24] Swift：闭包
来源：http://hz.hammf.cn/gtqfrqqttv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sufxvd.cn/gtnnnwtpfj.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gtckdpfzwl.html

struct P { var x: Int }
来源：http://hz.cucudq.cn/gtxnehoygr.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gtzjlmyhct.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtizvpooep.html

[T27] Swift：错误处理
来源：http://hz.sweek.top/gtwdatnpsb.html

do { try f() } catch { print(error) }
来源：http://hz.andypj.xyz/gtrxgqagym.html

[T28] Swift：枚举
来源：http://hz.bjfxy.top/gtzwsomkfb.html

enum Color { case red, green }
来源：http://hz.nanxinkj.top/gtkbnrmont.html

[T29] Swift：guard 提前返回
来源：http://hz.chenzaomai.com/gtbqolvwdd.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gthoumaasw.html

[T30] Swift：协议
来源：http://hz.shzxlz.cn/gtispwnffh.html

protocol Shape { func area() -> Double }
来源：http://hz.xinyue.icu/gtegqyjdfl.html

[T31] Lua：Hello World
来源：http://hz.gaohongyu789.top/gtehlitnfb.html

print("Hello")
来源：http://hz.nwbrower.top/gttcyznfye.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gtgkozwejy.html

local a = 1
来源：http://hz.bjfxy.top/gtzuctbdis.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtepazctlk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.9152youxi.cn/gtgfifctqx.html

[T34] Lua：遍历表
来源：http://hz.gogol.net.cn/gtgtrimqcz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtcgrtwnlo.html

[T35] Lua：字典表
来源：http://hz.316326.xyz/gtsmowmuum.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guannengcc.top/gtuhuhyekp.html

[T36] Lua：函数
来源：http://hz.shangyingyoupin.top/gtjmnsyyos.html

function add(a, b) return a + b end
来源：http://hz.jianghu66.top/gtzbzochwh.html

[T37] Lua：字符串拼接
来源：http://hz.yj20258.top/gtdtfkhlsa.html

"a" .. "b"
来源：http://hz.zhijiandao.cn/gtqsqglqbe.html

[T38] Lua：条件
来源：http://hz.jqgfzy.top/gtpfqvgwxk.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtixlfpggo.html

[T39] Lua：模式匹配
来源：http://hz.meibo888.top/gtvvgaiwze.html

string.find(s, "%d+")
来源：http://hz.zhaomingkeji.xyz/gtwnqkjcca.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtlenvaydp.html

setmetatable({}, { __index = base })
来源：http://hz.ydzc1.top/gtgjpgfwxc.html

[T41] Perl：Hello World
来源：http://hz.zhiwuduotai.top/gtghdvheiw.html

print "Hello\n";
来源：http://hz.sweek.top/gtobfkdwor.html

[T42] Perl：变量类型
来源：http://hz.sweek.top/gtxuyhhkur.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guowangkeji.top/gtudsxxaxh.html

[T43] Perl：字符串插值
来源：http://hz.nwbrower.top/gtudwudxbe.html

"值: $a"
来源：http://hz.zhengqikj.top/gtiocqtlgk.html

[T44] Perl：条件
来源：http://hz.ydjk.org.cn/gtnmiolxzz.html

if ($a > 0) { print "正"; }
来源：http://hz.sxryk.cn/gtsuaocutq.html

[T45] Perl：数组遍历
来源：http://hz.shuidangran.top/gteagtojbn.html

for my $x (@arr) { print $x; }
来源：http://hz.meibo888.top/gtiidgvwcf.html

[T46] Perl：哈希操作
来源：http://hz.jiagoushi.top/gtapbizllx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydjk.org.cn/gtfijnvchl.html

[T47] Perl：正则捕获
来源：http://hz.redwolf501.top/gtlnggdasv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuanzx.com/gtyvopgqoj.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtgcfrztth.html

$s =~ s/old/new/g;
来源：http://hz.havefunace.top/gtkyzakufw.html

[T49] Perl：函数
来源：http://hz.zhongyouzk.top/gtprpowcbj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daria6918.cn/gtlqiyqsgb.html

[T50] Perl：逐行读文件
来源：http://hz.ydjk.org.cn/gthwabjjnw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgfzy.top/gtzmmenqls.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yanxiufei.cn/gtdcsexqdc.html

[T51] Scala：Hello World
来源：http://hz.zhoulong.xyz/gtdeqglmoh.html

println("Hello")
来源：http://hz.havefunace.top/gtcivomuew.html

[T52] Scala：变量
来源：http://hz.sweek.top/gtofflawks.html


<!-- 参考信息 -->