代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtwzpjmdfw.html

[R56] 远程拷贝
来源：http://hz.redwolf501.top/gttfvyokcg.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gtnwlqitrc.html

[R57] 远程执行命令
来源：http://hz.kuanghao11.cn/gtvgqencsk.html

ssh user@host 'uptime'
来源：http://hz.gotoacloud.top/gttbabamtt.html

[R58] 下载文件
来源：http://hz.yuanzhike.top/gtuxzrtpwe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.mhx1999.top/gtrelaeolq.html

[R59] 发 POST JSON
来源：http://hz.zhijiandao.cn/gtgeefcgfe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtomhqfybv.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtrmvnyrnj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtthbfovkr.html

[R61] 磁盘占用
来源：http://hz.pengpengdd.cyou/gtwndogirx.html

df -h;  du -sh *
来源：http://hz.quarkkingdee.top/gtblnhnnhr.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtvrjlsppi.html

du -ah . | sort -rh | head -10
来源：http://hz.wangdashe.top/gtsmiaoajl.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtwvsgjoom.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gthlrwauqv.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtucqredkm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guannengcc.top/gtnykvjjof.html

[R65] 查看端口占用
来源：http://hz.hfpthk.cn/gtsvlwlsgt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xinyue.icu/gtydgfbmgt.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtloipdbya.html

crontab -e;  crontab -l
来源：http://hz.tian-w.cn/gtkdszcpvv.html

[R67] 生成随机十六进制串
来源：http://hz.mhx1999.top/gtslqykhko.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtetfvbuja.html

[R68] 计算文件校验值
来源：http://hz.yueranfly.top/gtaanacfre.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtqwslaqid.html

[R69] 生成随机密码
来源：http://hz.jinqigfzy.top/gtfpjvhqol.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtcdxngfat.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtdzcoaopy.html

date +%s;  date -d @1700000000
来源：http://hz.chenlongwang.top/gtdljcotiz.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtuoipsene.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtunqwqkhe.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gtdjnxdzzc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtxxmcqsfv.html

[R73] 分割大日志
来源：http://hz.jyoumei.cn/gtszuoazok.html

split -l 1000 big.log part_
来源：http://hz.gotoacloud.top/gtykdtwrgi.html

[R74] 批量重命名
来源：http://hz.pengpengdd.cyou/gtsvpgqhtf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.iojbl.cn/gtxhoalvbh.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtuyalpdyk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtwvsrkcau.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtmafweyxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtbrdwwwhi.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtcbigcwen.html

read -rp "请输入: " ans
来源：http://hz.chenzaomai.com/gtyeltvpnt.html

[R78] 交互式菜单
来源：http://hz.nanxuanxn.top/gttjdrerah.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ppjwa.cn/gtqrikokgl.html

[R79] 解析命令行选项
来源：http://hz.ywan-chungtsiang.top/gtwelvvwcu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.quarkkingdee.top/gtrwperuvc.html

[R80] 查看脚本执行耗时
来源：http://hz.birdmap.top/gtigsisupq.html

time ./run.sh
来源：http://hz.nanxuanxn.top/gtwdmvyvmc.html

================================================================================
来源：http://hz.andypj.xyz/gtlhhniocq.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gtocdmvpbf.html

================================================================================
来源：http://hz.ybcxt.top/gtbcuoblhc.html

[S01] C：Hello World
来源：http://hz.cheryme.top/gthgmomjxy.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gtsbztxiwq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtvamjkmen.html

[S02] C：变量与格式化输出
来源：http://hz.xuanzx.com/gtxdwllzlo.html

int a = 10; printf("%d\n", a);
来源：http://hz.fengsongda.top/gtmpphqbdy.html

[S03] C：读入整数
来源：http://hz.gotoacloud.top/gtldhdwevi.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gtlqubwilm.html

[S04] C：字符串复制
来源：http://hz.hysaishi.cn/gtrrdogcpg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenjidiqi.icu/gtevpesbsa.html

[S05] C：字符串长度
来源：http://hz.dashuyun.cn/gtwhiebnut.html

strlen(s)
来源：http://hz.nanxinkj.top/gtoxhkbocm.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtdwjskppz.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtcxxwvpms.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtxfdxxdss.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinghuilouyu.cn/gtgadbewrb.html

[S08] C：动态内存分配与释放
来源：http://hz.fengsongda.top/gteqcxzgvr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtatxpmhqa.html

[S09] C：结构体定义与初始化
来源：http://hz.hfpthk.cn/gtqkgywflg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenzaomai.com/gtjyfwmjks.html

[S10] C：指针与解引用
来源：http://hz.sxryk.cn/gtjsogcylb.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtfrwfsxto.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gtewcaehpo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinghuilouyu.cn/gtxnzxthmk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.9152youxi.cn/gtnsmwleci.html

fclose(f);
来源：http://hz.cucudq.cn/gtkzesangc.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtcoppdumo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtqxtioeja.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtdqkwyhuw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtjdimpcor.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtzqztulra.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gtdaffzway.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtvvhbwnpq.html

(double) a / b
来源：http://hz.yonumen.top/gtaukyyuvz.html

[S16] C：位操作置位
来源：http://hz.mhx1999.top/gtlfmyjvpv.html

x |= (1 << 3);
来源：http://hz.mhx1999.top/gthenzpbvo.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtuakjtkxi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtsiwgakzq.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtzpmzzybs.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gtzxbazrmo.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gtoychiotl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtjjkdohnk.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gteibzwdba.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtvwnkcpth.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gthjldoicr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.0kj1m.cn/gtrpiwpluo.html

[S22] C：字符串转数字
来源：http://hz.xuetiantiany.cn/gtuykxecku.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtdbzupnxs.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtssngbzrm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtvnhqsfdd.html

[S24] C：获取本地时间
来源：http://hz.jinqigfzy.top/gtecdabdhe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gthcxdvoph.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtextjpvhf.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtdfnwveyr.html

[S26] C：内存清零
来源：http://hz.xinyue.icu/gtxkhmmgqu.html

memset(a, 0, sizeof a);
来源：http://hz.zhoulong.xyz/gtgrsltugk.html

[S27] C：定义常量
来源：http://hz.jinqigfzy.top/gtczgfpyfp.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gthtxmucwa.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gtcggqsyee.html

static int counter = 0;
来源：http://hz.hammf.cn/gtjkzdlvar.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gtlylswmgw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtglipsleq.html

[S30] C：头文件保护
来源：http://hz.316326.xyz/gtzwqiqxrr.html

#ifndef X_H
来源：http://hz.nwbrower.top/gtwzqmoljw.html

#define X_H
来源：http://hz.jyoumei.cn/gthgyakwyi.html

#endif
来源：http://hz.gogol.net.cn/gtzxmmkxjx.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtwftjmtag.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtzexvwlaz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtqdjfqmlz.html

[S32] C++：字符串
来源：http://hz.shanyushiyangtech.top/gtmrkauwkg.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtmakzimpt.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gtraxmwpkf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtjhpuhjbd.html

[S34] C++：遍历 vector
来源：http://hz.dashuyun.cn/gtwwqqjkju.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gtusrhnfme.html

[S35] C++：map
来源：http://hz.jinqigfzy.top/gtqubdmhnq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtntivvtiq.html

[S36] C++：unordered_map
来源：http://hz.havefunace.top/gttoyxfzza.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtpeqdpqtd.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtybsmhkzx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jiagoushi.top/gttbjxfurj.html

[S38] C++：排序
来源：http://hz.ydzc1.top/gtebhqkdyf.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gtidypcbyw.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gtiigalvlx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtdcbpdqcy.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtosipxlhh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtnuiksuzd.html

[S41] C++：类与构造函数
来源：http://hz.yuxming.cn/gtxnamdnot.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtnyvqvvfq.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gtoibzsjsi.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtwkihojqe.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gticlimcyg.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtcqlxjsip.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtmsctcydt.html

void inc(int &x) { ++x; }
来源：http://hz.zdqjudy.top/gtsjmtafpb.html

[S45] C++：lambda
来源：http://hz.guannengcc.top/gtqeraxszu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cqqwz.cn/gtbhubtfzh.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gtzaajxulk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtsubnxubs.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtgwpfbddf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daxiang520.top/gtjggteidl.html

[S48] C++：逐行读文件
来源：http://hz.yanxiufei.cn/gtffrmsezh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuanzhike.top/gtuunwjreu.html

while (std::getline(in, line)) { }
来源：http://hz.zhaomingkeji.xyz/gtzvlbaelx.html

[S49] C++：写文件
来源：http://hz.ydzc1.top/gtnyaaqnkp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.birdmap.top/gtrokvovmf.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtslxsltue.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtdofddavr.html

[S51] C++：显式类型转换
来源：http://hz.nanxuanxn.top/gtenzywpak.html

static_cast<double>(a) / b
来源：http://hz.wangdashe.top/gtnwadzvre.html

[S52] C++：const 与 noexcept
来源：http://hz.havefunace.top/gttjjcvnxk.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gtsfazxvvb.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtixhfyvrr.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxinkj.top/gtgfyhejfb.html

[S54] C++：异常处理
来源：http://hz.zhijiandao.cn/gtnljccubu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtsopwnfrs.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtjbicqgkg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtqinihazj.html

[S56] C++：optional
来源：http://hz.ydjk.org.cn/gtjtwhywas.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtayyyssbh.html

[S57] C++：编译期常量
来源：http://hz.nanxuanxn.top/gtkmtgkyyr.html

constexpr int N = 10;
来源：http://hz.aibaodan.cn/gtrzgqbgbi.html

[S58] C++：命名空间
来源：http://hz.zhoulong.xyz/gtyowvljfo.html

namespace ns { int f() { return 1; } }
来源：http://hz.c1oappe.top/gtfhmgdjvi.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtytiyimrc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.kuanghao11.cn/gtolkagzlh.html

[S60] C++：遍历并删除元素
来源：http://hz.birdmap.top/gtldixxtcx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gtqfmrjdvp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtnwdsyrkv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gthwbkkwrm.html

================================================================================
来源：http://hz.jiagoushi.top/gtbkhpxyca.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtiqvzuubw.html

println("Hello")
来源：http://hz.ppjwa.cn/gtqoyffpwu.html

[T02] Kotlin：变量
来源：http://hz.jyoumei.cn/gtbzmbzshl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtmfpdcbol.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gttkptiitz.html

"值: $b"
来源：http://hz.havefunace.top/gtfbxkvfeh.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtrdporirc.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtuyrsfbmd.html

[T05] Kotlin：when 表达式
来源：http://hz.jinyuanbaomall.cn/gtpikahkwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtyelanhet.html

[T06] Kotlin：集合映射
来源：http://hz.birdmap.top/gtaecqynqp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cqqwz.cn/gtmgetpkkx.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gteklhzuif.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gtpkzybbra.html

[T08] Kotlin：数据类
来源：http://hz.nanxinkj.top/gtbwslsrqj.html

data class User(val name: String, val age: Int)
来源：http://hz.jiagoushi.top/gtofulpydw.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gttbkyzrhs.html

fun String.exclaim() = this + "!"
来源：http://hz.zhiwuduotai.top/gtdczujoet.html

[T10] Kotlin：默认参数
来源：http://hz.aizwys.cn/gtsbjaatnn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtjovjerza.html

[T11] Kotlin：协程
来源：http://hz.dianchejie.cn/gtxpvlfbmi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtqedksqis.html

[T12] Kotlin：解构声明
来源：http://hz.andypj.xyz/gtkhqfiihp.html

val (a, b) = Pair(1, 2)
来源：http://hz.wangshuangyany.cn/gthbizbibj.html

[T13] Kotlin：只读 Map
来源：http://hz.sweek.top/gtucskxfpn.html

val m = mapOf("a" to 1)
来源：http://hz.tanke756.top/gtgyneznwp.html

[T14] Kotlin：循环
来源：http://hz.zhengqikj.top/gthpdkllbb.html

for (i in 1..10) println(i)
来源：http://hz.yueranfly.top/gtqoewjuch.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtbbbzgqbc.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtyrqzhdto.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtsrbpqyma.html

print("Hello")
来源：http://hz.ybcxt.top/gtldppapjz.html

[T17] Swift：变量与常量
来源：http://hz.jqgfzy.top/gtmpadnbjh.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtkfwipdkd.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtibabisqj.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gtfztschvg.html

[T19] Swift：可选绑定
来源：http://hz.hammf.cn/gtykrcdcif.html

if let n = opt { print(n) }
来源：http://hz.sxryk.cn/gtgkdgztsh.html

[T20] Swift：数组操作
来源：http://hz.ydzc1.top/gtwwhpdqfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.0kj1m.cn/gtzgytmjso.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtvlrnzoxb.html

for x in a { print(x) }
来源：http://hz.sufxvd.cn/gtoragunau.html

[T22] Swift：字典
来源：http://hz.chenzaomai.com/gtesanyavw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cqqwz.cn/gtndniaqfw.html

[T23] Swift：函数
来源：http://hz.yj20258.top/gtxlylclar.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnxiangtu.top/gtnconvosb.html

[T24] Swift：闭包
来源：http://hz.tianlin.xyz/gtudekndka.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guowangkeji.top/gtkpyiguvl.html

[T25] Swift：结构体
来源：http://hz.jqgufenzy.top/gtowtpzoef.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtkrkmlhsd.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtjionmukm.html

class A: Base { override func f() {} }
来源：http://hz.chenlongwang.top/gtlhzwwrzc.html

[T27] Swift：错误处理
来源：http://hz.yangfankeji.com/gthhnnxmib.html

do { try f() } catch { print(error) }
来源：http://hz.mhx1999.top/gtoerkjfrb.html

[T28] Swift：枚举
来源：http://hz.kuanghao11.cn/gttdxdbhzf.html

enum Color { case red, green }
来源：http://hz.birdmap.top/gtqtzjcmqg.html

[T29] Swift：guard 提前返回
来源：http://hz.zhaomingkeji.xyz/gtsuumtqad.html

guard let x = opt else { return }
来源：http://hz.ivvv.top/gtofdxgvqg.html

[T30] Swift：协议
来源：http://hz.vqdsnc.cn/gtuyhaashv.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtdlcrarhc.html

[T31] Lua：Hello World
来源：http://hz.jianghu66.top/gtxfkitfec.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gtbgfzvvlc.html

[T32] Lua：局部变量
来源：http://hz.xuanzx.com/gtvvgssjdg.html

local a = 1
来源：http://hz.hnqzz.top/gtpbuvptgw.html

[T33] Lua：表（数组）
来源：http://hz.yongpay.top/gtnpdhxfym.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigfzy.top/gtgfuypdni.html

[T34] Lua：遍历表
来源：http://hz.nanxinkj.top/gthpqvbaid.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtosfpmyfs.html

[T35] Lua：字典表
来源：http://hz.gzhubu.top/gtynvibncj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtvvpahneb.html

[T36] Lua：函数
来源：http://hz.yanxiufei.cn/gtzwetlchk.html

function add(a, b) return a + b end
来源：http://hz.chenzaomai.com/gtfjnnndcn.html

[T37] Lua：字符串拼接
来源：http://hz.xinyue.icu/gtccolsfya.html

"a" .. "b"
来源：http://hz.yongpay.top/gtfmevlstf.html

[T38] Lua：条件
来源：http://hz.fengsongda.top/gtvoukejfk.html

if x > 0 then print("正") end
来源：http://hz.havefunace.top/gtyisooidj.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtsrrkunyf.html

string.find(s, "%d+")
来源：http://hz.ydjk.org.cn/gtpjexspqz.html

[T40] Lua：元表
来源：http://hz.haohaochexian.top/gtvpjaceeu.html

setmetatable({}, { __index = base })
来源：http://hz.cqqwz.cn/gtzgsvlzwc.html

[T41] Perl：Hello World
来源：http://hz.fengsongda.top/gtzhhtzbyk.html

print "Hello\n";
来源：http://hz.shangyingyoupin.top/gtwkmeyhra.html

[T42] Perl：变量类型
来源：http://hz.svipenyu.cn/gtazufgtva.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhoulong.xyz/gtplrkvhom.html

[T43] Perl：字符串插值
来源：http://hz.feifeiyinyue.top/gteoxrktej.html

"值: $a"
来源：http://hz.mhx1999.top/gtvkjsuoyd.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gtgczzkjss.html

if ($a > 0) { print "正"; }
来源：http://hz.tian-w.cn/gtuwuwinzn.html

[T45] Perl：数组遍历
来源：http://hz.zhaomingkeji.xyz/gtdqsfmbkh.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtraigqupk.html

[T46] Perl：哈希操作
来源：http://hz.jlsjyb.cn/gtuaqgwmrs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.iojbl.cn/gtaajusicw.html

[T47] Perl：正则捕获
来源：http://hz.jinghuilouyu.cn/gtfouxsaqu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yj20258.top/gtlnsxspcn.html

[T48] Perl：正则替换
来源：http://hz.gaohongyu789.top/gtevwjhlfg.html

$s =~ s/old/new/g;
来源：http://hz.snrcjt.cn/gtyutmdsyo.html

[T49] Perl：函数
来源：http://hz.nwbrower.top/gtucbcqfty.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yonumen.top/gtdvozukcp.html

[T50] Perl：逐行读文件
来源：http://hz.shangyingyoupin.top/gtrbtoifco.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtdjcpzxjo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.c1oappe.top/gtyxeelcnq.html

[T51] Scala：Hello World
来源：http://hz.dashuyun.cn/gtohmqnljf.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtqggyuokx.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gtjihrclrh.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtgwasfyof.html

[T53] Scala：字符串插值
来源：http://hz.zhongyouzk.top/gtborwiqnx.html

s"值: $b"
来源：http://hz.guowangkeji.top/gtpjgagjcp.html

[T54] Scala：集合映射
来源：http://hz.hywenlv.cn/gtcwadabkf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xingfuxueyuan.xyz/gtjqvmwfkf.html

[T55] Scala：集合过滤
来源：http://hz.iojbl.cn/gttclfdgsq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenzaomai.com/gtcmyyxkcq.html

[T56] Scala：样例类
来源：http://hz.ehwqpu.com/gtdzfkvjcz.html

case class User(name: String, age: Int)
来源：http://hz.shanyushiyangkeji.top/gtnyoczqvt.html

[T57] Scala：模式匹配
来源：http://hz.sufxvd.cn/gtnbibqbnn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhijiandao.cn/gtigtmkpsu.html

[T58] Scala：函数定义
来源：http://hz.yueranfly.top/gtncgmzvhz.html


<!-- 参考信息 -->