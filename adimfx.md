代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtvdwimnwz.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtobzhlcss.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtzoeplgre.html

[R55] 压缩与解压
来源：http://hz.hfpthk.cn/gtjbgplxyz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gtvdsegqlq.html

[R56] 远程拷贝
来源：http://hz.9152youxi.cn/gtsqjbvhhu.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtuoroauck.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtrpfbjetd.html

ssh user@host 'uptime'
来源：http://hz.sysykeji.top/gthdqigdfu.html

[R58] 下载文件
来源：http://hz.ybcxt.top/gtuycyiwmt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtuhygopiz.html

[R59] 发 POST JSON
来源：http://hz.c1oappe.top/gtnfatrleq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xylfe.cn/gtyxxoejoa.html

[R60] 只看 HTTP 状态码
来源：http://hz.guannengcc.top/gtanghdcvg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.haohaochexian.top/gtwltdtqwn.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtsxomieyk.html

df -h;  du -sh *
来源：http://hz.ppjwa.cn/gtzwwkpksj.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtqqfkpnme.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gttdnhaxij.html

[R63] 内存与进程
来源：http://hz.redwolf501.top/gtyoiqogjz.html

free -h;  ps aux | grep nginx
来源：http://hz.shuidangran.top/gtdmbqrrsk.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtaqbvgxel.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gtvmhakdpt.html

[R65] 查看端口占用
来源：http://hz.iojbl.cn/gtkdnzrwff.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydzc1.top/gtawoftaox.html

[R66] 定时任务
来源：http://hz.tian-w.cn/gthidfmglp.html

crontab -e;  crontab -l
来源：http://hz.ydzc1.top/gtsuqbywfb.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtehgpxczz.html

openssl rand -hex 16
来源：http://hz.jiagoushi.top/gtqlkqelbb.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gtiecpnput.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj202588.top/gtguvhpsid.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtgrfegrke.html

head -c 16 /dev/urandom | base64
来源：http://hz.dashuyun.cn/gtlnipouyt.html

[R70] 时间戳与互转
来源：http://hz.yuxming.cn/gtrkwwetji.html

date +%s;  date -d @1700000000
来源：http://hz.nanxuanxn.top/gtpdhvdhmd.html

[R71] 日期格式化
来源：http://hz.shzxlz.cn/gthihtuqwv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuanzhike.top/gtyfszlmrj.html

[R72] 等待端口就绪
来源：http://hz.zhengqikj.top/gtneoyituj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhoulong.xyz/gthcafzlpj.html

[R73] 分割大日志
来源：http://hz.hnxiangtu.top/gtxedyizqs.html

split -l 1000 big.log part_
来源：http://hz.daxiang520.top/gtttycynos.html

[R74] 批量重命名
来源：http://hz.jqgfzy.top/gtiiknrrwv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtcpeqonhl.html

[R75] 导出环境变量
来源：http://hz.hnxiangtu.top/gtngdonckv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hywenlv.cn/gtytnodfjm.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtitegrtky.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtxejkgjkg.html

[R77] 读取用户输入
来源：http://hz.cashguo.top/gtwulvjctm.html

read -rp "请输入: " ans
来源：http://hz.sweek.top/gtyuzpazpf.html

[R78] 交互式菜单
来源：http://hz.yongpay.top/gtkvrymebz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guowangkeji.top/gttklbaapf.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gthvdlfpyk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtabemhftz.html

[R80] 查看脚本执行耗时
来源：http://hz.sufxvd.cn/gtqxjzzitn.html

time ./run.sh
来源：http://hz.pycfn.com/gtoxfyntpo.html

================================================================================
来源：http://hz.yueranfly.top/gtgmccxlan.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtwskavwcd.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzyvgbiby.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gtqnusvzve.html

#include <stdio.h>
来源：http://hz.bjfxy.top/gtskyiuyhn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.snrcjt.cn/gtsjypvthv.html

[S02] C：变量与格式化输出
来源：http://hz.vqdsnc.cn/gtlelcbujk.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtmdfzabko.html

[S03] C：读入整数
来源：http://hz.jiagoushi.top/gtjmuwxufo.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtdqkscckt.html

[S04] C：字符串复制
来源：http://hz.ywan-chungtsiang.top/gtlatkzqll.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gtctlkpusf.html

[S05] C：字符串长度
来源：http://hz.shuidangran.top/gtmwlqqetz.html

strlen(s)
来源：http://hz.hammf.cn/gtrgbuelsx.html

[S06] C：字符串比较
来源：http://hz.wangdashe.top/gtfgqpvuqg.html

strcmp(a, b) == 0
来源：http://hz.cdnleiting.top/gtoakpygyt.html

[S07] C：数组遍历求和
来源：http://hz.dashuyun.cn/gtpmfxlvqj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangkeji.top/gtymrkkapu.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtbtgmtbfl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gtphetamzo.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gtpenfghnk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gaohongyu789.top/gtzsguzlyt.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtxzaxrqyu.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258888.top/gtufsfjjwn.html

[S11] C：逐行读文件
来源：http://hz.zhengqikj.top/gtobecrjhl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fengsongda.top/gttgqafalo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtrmnfzugq.html

fclose(f);
来源：http://hz.0kj1m.cn/gttduqtypm.html

[S12] C：写文件
来源：http://hz.sxryk.cn/gtzzltdsqn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hongshengwenyu.top/gttvhsaxue.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtsmhgoujr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yangfankeji.com/gtufhscarm.html

[S14] C：枚举
来源：http://hz.pengpengdd.cyou/gtkcwaiqua.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.0kj1m.cn/gtidodmhaq.html

[S15] C：类型转换
来源：http://hz.bjfxy.top/gtjmmxpyus.html

(double) a / b
来源：http://hz.aibaodan.cn/gtwatgktbw.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtyuwordjv.html

x |= (1 << 3);
来源：http://hz.guannengcc.top/gtmdvluqzw.html

[S17] C：安全拼接字符串
来源：http://hz.chenlongwang.top/gtmxkkqlno.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hywenlv.cn/gtyfveicup.html

[S18] C：命令行参数
来源：http://hz.cucudq.cn/gtyuwvkvhq.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtqgxznhve.html

[S19] C：快速排序
来源：http://hz.tian-w.cn/gtnqiczkur.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtyucxrzaq.html

[S20] C：二分查找
来源：http://hz.zhiwuduotai.top/gtdqyrxlbg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtamzvkvrq.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gtjpewyevb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shanyushiyangtech.top/gtnwrphntv.html

[S22] C：字符串转数字
来源：http://hz.aibaodan.cn/gteanqopox.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtxsghotsc.html

[S23] C：随机数
来源：http://hz.xuanzx.com/gtveslypeh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ppjwa.cn/gtxpuuyeux.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtppndipws.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxinkj.top/gtzqfoowex.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtmbaxcvuf.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtunuakidm.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtknotclgj.html

memset(a, 0, sizeof a);
来源：http://hz.hammf.cn/gtycddoqhl.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtxitbrcyu.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gtjrnulwul.html

[S28] C：静态变量
来源：http://hz.sweek.top/gtlzaidivz.html

static int counter = 0;
来源：http://hz.yonumen.top/gtcywfhmgj.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gteghttnxx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtvnhmrwpy.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtsiayemib.html

#ifndef X_H
来源：http://hz.c1oappe.top/gtcggsqppk.html

#define X_H
来源：http://hz.yanxiufei.cn/gtvtkwqyqk.html

#endif
来源：http://hz.xinyue.icu/gtfkpdtqgs.html

[S31] C++：Hello World
来源：http://hz.snrcjt.cn/gtotqagjgq.html

#include <iostream>
来源：http://hz.zdqjudy.top/gtwgwiekvu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gtzuqwdfat.html

[S32] C++：字符串
来源：http://hz.jinqigufen.top/gtzszwgjdk.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtqasatgdk.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gtzhvillty.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.feifeiyinyue.top/gtfhtbpdxx.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtfelmxrpg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtgngszxgw.html

[S35] C++：map
来源：http://hz.ehwqpu.com/gtsivjlmqx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.smart0.xyz/gtsycwhgru.html

[S36] C++：unordered_map
来源：http://hz.quarkkingdee.top/gtpvtfgexl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtnktxrqvi.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtjnihmmhp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gtqfixctza.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtgksmdmqr.html

std::sort(v.begin(), v.end());
来源：http://hz.redwolf501.top/gtrcjybzjf.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigfzy.top/gtbjtekpnu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yonumen.top/gtgiqdptin.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtenbkwtzh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yanxiufei.cn/gtxjdhryho.html

[S41] C++：类与构造函数
来源：http://hz.zhongyouzk.top/gtkjnkvlkm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinghuilouyu.cn/gtnldlsxjj.html

[S42] C++：继承与虚函数
来源：http://hz.zdqjudy.top/gtwquzcygr.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnqzz.top/gtrlsdkfbw.html

[S43] C++：智能指针
来源：http://hz.jinqigfzy.top/gttddhymgf.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtwtzwpwdl.html

[S44] C++：引用传参
来源：http://hz.haohaochexian.top/gtztomqrrj.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtdgqgvbiz.html

[S45] C++：lambda
来源：http://hz.nanxinkj.top/gtgvvtkcfj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.birdmap.top/gtxfeijacr.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtwzowrppw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.quarkkingdee.top/gtyiyghrzc.html

[S47] C++：结构化绑定遍历
来源：http://hz.hywenlv.cn/gtgsngsgcd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258.top/gtfutkjgpz.html

[S48] C++：逐行读文件
来源：http://hz.ivvv.top/gtdtamdjlm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtnuhfberw.html

while (std::getline(in, line)) { }
来源：http://hz.wangdashe.top/gtkbrmospu.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtrvvlmhco.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgfzy.top/gtqkdmtkge.html

[S50] C++：格式化数字
来源：http://hz.chenlongwang.top/gtnjtasgkn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhoulong.xyz/gtmoathjuw.html

[S51] C++：显式类型转换
来源：http://hz.jianghu66.top/gtfvlhvoxf.html

static_cast<double>(a) / b
来源：http://hz.52xcode.cn/gtqlnojmhz.html

[S52] C++：const 与 noexcept
来源：http://hz.tianlin.xyz/gtgzxujrhl.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtpjlokwhu.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gttzyfqquw.html

std::vector<int> w = std::move(v);
来源：http://hz.yanxiufei.cn/gtatrrnuyb.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtkqjwldry.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtlbmjsfkg.html

[S55] C++：结构化绑定
来源：http://hz.yj20258888.top/gtovyqazil.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtlmjrrvqi.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtqqeackbp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuanzx.com/gtcbonanis.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtdvgdexqi.html

constexpr int N = 10;
来源：http://hz.yongpay.top/gtbdigywxa.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gtepxsewcd.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhongyouzk.top/gttksgmeym.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gtyphpyhjf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhijiandao.cn/gtgmheobvx.html

[S60] C++：遍历并删除元素
来源：http://hz.hongshengwenyu.top/gtueaarung.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ivvv.top/gtfkiwcses.html

================================================================================
来源：http://hz.wangdashe.top/gtgpsmzkte.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.haohaochexian.top/gtcaacblbf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gteivifsce.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtupxsivkj.html

println("Hello")
来源：http://hz.yueranfly.top/gtpasugwtv.html

[T02] Kotlin：变量
来源：http://hz.sufxvd.cn/gttmmczqpj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258.top/gtsbbvehzi.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtdgeajcuw.html

"值: $b"
来源：http://hz.jinqigfzy.top/gtentypzhv.html

[T04] Kotlin：空安全
来源：http://hz.chenzaomai.com/gthisnskiz.html

val n: String? = null;  n?.length
来源：http://hz.cashguo.top/gtisokpfft.html

[T05] Kotlin：when 表达式
来源：http://hz.wangdashe.top/gtdzlesmon.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cheryme.top/gtrwrkrcsz.html

[T06] Kotlin：集合映射
来源：http://hz.hywenlv.cn/gtcrendlnw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtzjxriukl.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtdjhstazf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtsedyoypi.html

[T08] Kotlin：数据类
来源：http://hz.chenzaomai.com/gtkslrvvln.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtbstayxmj.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtshjiwmlm.html

fun String.exclaim() = this + "!"
来源：http://hz.svipenyu.cn/gtrewmgulq.html

[T10] Kotlin：默认参数
来源：http://hz.hywenlv.cn/gttuxtdowl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtvnemdimc.html

[T11] Kotlin：协程
来源：http://hz.yongpay.top/gtuyzvhzum.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtzajesgby.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtsklmxavi.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuanzx.com/gthkwlgpbm.html

[T13] Kotlin：只读 Map
来源：http://hz.wangdashe.top/gtsmgpmydc.html

val m = mapOf("a" to 1)
来源：http://hz.shzxlz.cn/gtvmxdijna.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtbstlvezd.html

for (i in 1..10) println(i)
来源：http://hz.sxryk.cn/gtnmfarnyw.html

[T15] Kotlin：接口
来源：http://hz.9152youxi.cn/gtefqsbfqn.html

interface Shape { fun area(): Double }
来源：http://hz.andypj.xyz/gtlavmzgbr.html

[T16] Swift：Hello World
来源：http://hz.yj202588.top/gtwzeccxpb.html

print("Hello")
来源：http://hz.smart0.xyz/gtshcfkink.html

[T17] Swift：变量与常量
来源：http://hz.cheryme.top/gtbrrgqqre.html

var a = 1;  let b = 2
来源：http://hz.smart0.xyz/gtdpbpgytm.html

[T18] Swift：字符串插值
来源：http://hz.cqqwz.cn/gtqlvgfxdj.html

"值: \(b)"
来源：http://hz.ppjwa.cn/gtpbtjmaun.html

[T19] Swift：可选绑定
来源：http://hz.zhijiandao.cn/gtcktwoozu.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtbitoitsd.html

[T20] Swift：数组操作
来源：http://hz.cucudq.cn/gtnpstbczx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gtkcmhuwql.html

[T21] Swift：遍历
来源：http://hz.tianlin.xyz/gtknoxunkg.html

for x in a { print(x) }
来源：http://hz.pengpengdd.cyou/gtalxeiiwx.html

[T22] Swift：字典
来源：http://hz.jinghuilouyu.cn/gtwldcvlnu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhoulong.xyz/gtadzzggsd.html

[T23] Swift：函数
来源：http://hz.sweek.top/gtdxeunhal.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenjidiqi.icu/gtidrxuzgg.html

[T24] Swift：闭包
来源：http://hz.dianchejie.cn/gtivdhkzqw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtmvcszfhu.html

[T25] Swift：结构体
来源：http://hz.yvedp.cn/gtvjcijbaq.html

struct P { var x: Int }
来源：http://hz.ppjwa.cn/gtwtfebqbq.html

[T26] Swift：类与重写
来源：http://hz.gzhubu.top/gtwgnpmsvh.html

class A: Base { override func f() {} }
来源：http://hz.chenjidiqi.icu/gtssgqstnl.html

[T27] Swift：错误处理
来源：http://hz.ybcxt.top/gtmqeizkoz.html

do { try f() } catch { print(error) }
来源：http://hz.redwolf501.top/gtejlspcpb.html

[T28] Swift：枚举
来源：http://hz.shuidangran.top/gtowvklnks.html

enum Color { case red, green }
来源：http://hz.sxryk.cn/gtdkfndpws.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtnxfwnifj.html

guard let x = opt else { return }
来源：http://hz.jlsjyb.cn/gtxbqbrxed.html

[T30] Swift：协议
来源：http://hz.yueranfly.top/gtyxceduii.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtiedvrdly.html

[T31] Lua：Hello World
来源：http://hz.jinyuanbaomall.cn/gtxsfpwyju.html

print("Hello")
来源：http://hz.zhixingplan.top/gtmirpkfss.html

[T32] Lua：局部变量
来源：http://hz.bjfxy.top/gtynualujw.html

local a = 1
来源：http://hz.gzhubu.top/gtpndiiuvg.html

[T33] Lua：表（数组）
来源：http://hz.cdnleiting.top/gtjqwknmms.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sysykeji.top/gtjqijwfmh.html

[T34] Lua：遍历表
来源：http://hz.jinqigufen.top/gtqesojexb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xylfe.cn/gtyngdpnjx.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gtonqofcsp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtodualwrk.html

[T36] Lua：函数
来源：http://hz.zhaomingkeji.xyz/gtjyviwlgu.html

function add(a, b) return a + b end
来源：http://hz.c1oappe.top/gtiomirafy.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtzbgisfwu.html

"a" .. "b"
来源：http://hz.shuidangran.top/gtgncfkilj.html

[T38] Lua：条件
来源：http://hz.mhx1999.top/gtxbeiwayd.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gteoldcfxe.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtacfrgftc.html

string.find(s, "%d+")
来源：http://hz.ppjwa.cn/gtevtpkzju.html

[T40] Lua：元表
来源：http://hz.hfpthk.cn/gtpztcurlc.html

setmetatable({}, { __index = base })
来源：http://hz.chenzaomai.com/gtooniypbb.html

[T41] Perl：Hello World
来源：http://hz.nwbrower.top/gtdhrsuoka.html

print "Hello\n";
来源：http://hz.ydjk.org.cn/gtalibfwuh.html

[T42] Perl：变量类型
来源：http://hz.quarkkingdee.top/gtapwqaigp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jlsjyb.cn/gtbtxvlmmi.html

[T43] Perl：字符串插值
来源：http://hz.dashuyun.cn/gtqpgofwza.html

"值: $a"
来源：http://hz.quarkkingdee.top/gtvojreagc.html

[T44] Perl：条件
来源：http://hz.zhixingplan.top/gtxqeblguk.html

if ($a > 0) { print "正"; }
来源：http://hz.sxryk.cn/gtnwxissgr.html

[T45] Perl：数组遍历
来源：http://hz.yueranfly.top/gtibznkzfq.html

for my $x (@arr) { print $x; }
来源：http://hz.xylfe.cn/gtnvzthckb.html

[T46] Perl：哈希操作
来源：http://hz.fzhhl.top/gtyvozqliy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuxming.cn/gthguhgwzz.html

[T47] Perl：正则捕获
来源：http://hz.aizwys.cn/gtdgeioauw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.haohaochexian.top/gtcazphnsy.html

[T48] Perl：正则替换
来源：http://hz.jinqigfzy.top/gtvztazhzy.html

$s =~ s/old/new/g;
来源：http://hz.sxryk.cn/gthqdrermc.html

[T49] Perl：函数
来源：http://hz.xylfe.cn/gtywqkcozc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sysykeji.top/gtwjleqqky.html

[T50] Perl：逐行读文件
来源：http://hz.andypj.xyz/gthixutphn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aibaodan.cn/gtduyhpetu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ybcxt.top/gtnvsxjyuz.html

[T51] Scala：Hello World
来源：http://hz.zycfv.cn/gtnxdwbhfr.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtkwergucm.html

[T52] Scala：变量
来源：http://hz.sweek.top/gteluklbbf.html

val a = 1;  var b = 2
来源：http://hz.chenlongwang.top/gtgyxjcqjh.html

[T53] Scala：字符串插值
来源：http://hz.9152youxi.cn/gteybsssrg.html

s"值: $b"
来源：http://hz.hfpthk.cn/gtzgdffecw.html

[T54] Scala：集合映射
来源：http://hz.jqgufenzy.top/gtboyxyufh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jyoumei.cn/gteygmnpqi.html

[T55] Scala：集合过滤
来源：http://hz.hywenlv.cn/gtvjxlhxgy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.feifeiyinyue.top/gtjhclvsgz.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtcthdeimx.html


<!-- 参考信息 -->