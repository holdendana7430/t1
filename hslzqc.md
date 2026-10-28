代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtgptqxcsw.html

[R60] 只看 HTTP 状态码
来源：http://hz.yongpay.top/gtepsbncui.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sweek.top/gtluwztvth.html

[R61] 磁盘占用
来源：http://hz.xuanzx.com/gtaljldybn.html

df -h;  du -sh *
来源：http://hz.yanxiufei.cn/gteyvepgim.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtkredpikv.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtcwqbexzq.html

[R63] 内存与进程
来源：http://hz.tian-w.cn/gtpczqisja.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtfgptehag.html

[R64] 结束进程
来源：http://hz.zycfv.cn/gtgguvvqkg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gtwsbnwvpb.html

[R65] 查看端口占用
来源：http://hz.pengpengdd.cyou/gthjagovho.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258888.top/gtfpxtqrgl.html

[R66] 定时任务
来源：http://hz.dianchejie.cn/gtihgskwmi.html

crontab -e;  crontab -l
来源：http://hz.birdmap.top/gtxvrnapdq.html

[R67] 生成随机十六进制串
来源：http://hz.nwbrower.top/gtphufnkpa.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtldhvfari.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtdjtulcvj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxinkj.top/gtdkjakjst.html

[R69] 生成随机密码
来源：http://hz.ywan-chungtsiang.top/gtzqlehszi.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenjidiqi.icu/gtbuekloep.html

[R70] 时间戳与互转
来源：http://hz.quarkkingdee.top/gtjiborlcc.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtwujuzapv.html

[R71] 日期格式化
来源：http://hz.zhijiandao.cn/gtuwfeelcg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtpapifiho.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtumlmdsyu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fengsongda.top/gtittfgwqt.html

[R73] 分割大日志
来源：http://hz.guowangkeji.top/gtrlfibtai.html

split -l 1000 big.log part_
来源：http://hz.ydzc1.top/gtttqjpiey.html

[R74] 批量重命名
来源：http://hz.yj20258.top/gtcjpnuugo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.bjfxy.top/gtmlfbsyip.html

[R75] 导出环境变量
来源：http://hz.zhengqikj.top/gtrmflzszd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhoulong.xyz/gtvuyrfche.html

[R76] 使用临时文件
来源：http://hz.316326.xyz/gtuxcylhns.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtnbazonhy.html

[R77] 读取用户输入
来源：http://hz.chenjidiqi.icu/gtexdceezr.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtwkguvazq.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtjeufjare.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gtwcladphk.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtymqrokyz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgufenzy.top/gtaedokutd.html

[R80] 查看脚本执行耗时
来源：http://hz.yuxming.cn/gtlldopncb.html

time ./run.sh
来源：http://hz.jinqigfzy.top/gtdiqboawc.html

================================================================================
来源：http://hz.tian-w.cn/gtanhccync.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtwxttepoa.html

================================================================================
来源：http://hz.ivvv.top/gtxwvrxzmk.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gtjvngortr.html

#include <stdio.h>
来源：http://hz.yj20258.top/gtwavshabf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtcrurjobo.html

[S02] C：变量与格式化输出
来源：http://hz.gzhubu.top/gtmgwzxdrt.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtxsqvzbyc.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtbmdjymjt.html

int x; scanf("%d", &x);
来源：http://hz.yuxming.cn/gtvkpcrbeh.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gtustaunuy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gtalipfpdk.html

[S05] C：字符串长度
来源：http://hz.nanxuanxn.top/gtswjyvcnm.html

strlen(s)
来源：http://hz.yj202588.top/gtozzqvwxu.html

[S06] C：字符串比较
来源：http://hz.zdqjudy.top/gtxlalqvdm.html

strcmp(a, b) == 0
来源：http://hz.hnqzz.top/gtqbkbdrgk.html

[S07] C：数组遍历求和
来源：http://hz.nanxuanxn.top/gtlumrzyer.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.birdmap.top/gtfyfeqaki.html

[S08] C：动态内存分配与释放
来源：http://hz.wangdashe.top/gtimyrqhuq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtshmrnbbe.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtbltooxvd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gaohongyu789.top/gtxtpzdzmw.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtjwfefrmi.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtybjuiogx.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtedclktub.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shuidangran.top/gtwloocbyf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yangfankeji.com/gtqdlayqal.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtcjfwtbgd.html

[S12] C：写文件
来源：http://hz.sxryk.cn/gtyffdnrri.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtidwgprwl.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gtqxslagws.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhengqikj.top/gtudeonlwm.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtqwaozpvu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtaeotkoow.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtjkotvlga.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtqqeokfki.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtmrzjqcoi.html

x |= (1 << 3);
来源：http://hz.xinyue.icu/gtfnljhlgt.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gthrxqyldm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtqgmglmrl.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtufprwhzt.html

int main(int argc, char **argv)
来源：http://hz.yj20258888.top/gtefbutnxb.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gttppusgez.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtoiltzrps.html

[S20] C：二分查找
来源：http://hz.yanxiufei.cn/gtuztxpntf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtweeujuwh.html

[S21] C：字符类别判断
来源：http://hz.daria6918.cn/gtpbfnlwih.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydjk.org.cn/gtgvfchput.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtnhmhcazr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangshuangyany.cn/gtcpblqmya.html

[S23] C：随机数
来源：http://hz.0kj1m.cn/gtxiesqnde.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtxpxocqxu.html

[S24] C：获取本地时间
来源：http://hz.redwolf501.top/gtiucnfumy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gthjqxyhzc.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gtdahfjppz.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtpgfyepvc.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gtaxqdvaem.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtrnywwgxf.html

[S27] C：定义常量
来源：http://hz.nanxuanxn.top/gtyarzvftp.html

const double PI = 3.14159;
来源：http://hz.fengsongda.top/gtjklgpadd.html

[S28] C：静态变量
来源：http://hz.jlsjyb.cn/gtpllcbsrp.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtrfiwffgk.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gttbgpkxxa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nwbrower.top/gtlcsiclox.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gthwhhcles.html

#ifndef X_H
来源：http://hz.chenjidiqi.icu/gtkkjdhehf.html

#define X_H
来源：http://hz.yj20258.top/gtqbrcjqvr.html

#endif
来源：http://hz.bjfxy.top/gtihhzerac.html

[S31] C++：Hello World
来源：http://hz.jinqigufen.top/gtxbpvsnrf.html

#include <iostream>
来源：http://hz.jinghuilouyu.cn/gtpwzkafzd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtcawfatpq.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtsjvapzjr.html

std::string s = "hi";  s += "!";
来源：http://hz.gogol.net.cn/gtnmrloupk.html

[S33] C++：vector 增删
来源：http://hz.snrcjt.cn/gtysiickqq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtwskswllw.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtbysbshon.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinghuilouyu.cn/gttlbggpmo.html

[S35] C++：map
来源：http://hz.haohaochexian.top/gtdejbmkfu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtuknlylgg.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtfmyiixjc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtatitaacd.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtequckorv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gtirfcckqq.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtprvaoxbm.html

std::sort(v.begin(), v.end());
来源：http://hz.cqqwz.cn/gtrnlavtpn.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtiijgvnjd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.andypj.xyz/gtmmztmibu.html

[S40] C++：查找元素
来源：http://hz.dianchejie.cn/gtxybvobsj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtiusoanmy.html

[S41] C++：类与构造函数
来源：http://hz.hywenlv.cn/gtrislmkik.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.0kj1m.cn/gtvhblsjjk.html

[S42] C++：继承与虚函数
来源：http://hz.wangshuangyany.cn/gtvjxifolw.html

class B : public Base { public: void f() override {} };
来源：http://hz.jianghu66.top/gtxxactcal.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtdiczrgdm.html

auto p = std::make_unique<int>(5);
来源：http://hz.xylfe.cn/gtmytkdjak.html

[S44] C++：引用传参
来源：http://hz.xingfuxueyuan.xyz/gtlfzbxkji.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtqqfpcedb.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gtzifjhlmf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daxiang520.top/gtbvatksjd.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtdzqehbke.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtgyokihah.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtxmpsjmuk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtygzqlxqq.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtlclwkiei.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ppjwa.cn/gtllqmypzr.html

while (std::getline(in, line)) { }
来源：http://hz.hnqzz.top/gtmxeemqth.html

[S49] C++：写文件
来源：http://hz.jinqigufen.top/gtnbxffzxu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtghdkbvdy.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gtskbrpihp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtuourqqlf.html

[S51] C++：显式类型转换
来源：http://hz.ydzc1.top/gtzxmgskja.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtwncufhog.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtmyzalfup.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtcpultuga.html

[S53] C++：移动语义
来源：http://hz.iojbl.cn/gtfhnvydlt.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtpumithev.html

[S54] C++：异常处理
来源：http://hz.dianchejie.cn/gthclcwalo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yueranfly.top/gtqcrextph.html

[S55] C++：结构化绑定
来源：http://hz.yuxming.cn/gtowflsdbn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhiwuduotai.top/gtssgxqngf.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtujilcain.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cdnleiting.top/gtknrrcuml.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtjvnwtigy.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtmbzfaszy.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtdhzxwxxr.html

namespace ns { int f() { return 1; } }
来源：http://hz.yongpay.top/gtcbspjlzw.html

[S59] C++：静态断言
来源：http://hz.hysaishi.cn/gtkwxjcwsg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhixingplan.top/gtqssntold.html

[S60] C++：遍历并删除元素
来源：http://hz.zdqjudy.top/gtrokukxzx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxinkj.top/gtcgkawelr.html

================================================================================
来源：http://hz.jianghu66.top/gtjrciqzld.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gttavixrmi.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrmnxetqe.html

[T01] Kotlin：Hello World
来源：http://hz.52xcode.cn/gtdmhdzpqz.html

println("Hello")
来源：http://hz.wangdashe.top/gteijpjsbg.html

[T02] Kotlin：变量
来源：http://hz.yvedp.cn/gtawnqmiln.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.c1oappe.top/gtmywydazk.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxuanxn.top/gtazxsdxed.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gtoqrfnodw.html

[T04] Kotlin：空安全
来源：http://hz.zhongyouzk.top/gtwxhvccyz.html

val n: String? = null;  n?.length
来源：http://hz.svipenyu.cn/gtqipagrfs.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gthrsdgvsa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtnwrrubjk.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtldzjmnwi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.redwolf501.top/gtaeuysqjc.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtkujzmvpo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.meibo888.top/gtkncizmdy.html

[T08] Kotlin：数据类
来源：http://hz.yongpay.top/gtckjwpbov.html

data class User(val name: String, val age: Int)
来源：http://hz.yueranfly.top/gtbqdkrcjy.html

[T09] Kotlin：扩展函数
来源：http://hz.sweek.top/gtaxmsnuic.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gtoilsbeis.html

[T10] Kotlin：默认参数
来源：http://hz.cdnleiting.top/gtofhngxit.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtgsdstuhq.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtulousugh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtybgxcdap.html

[T12] Kotlin：解构声明
来源：http://hz.zhijiandao.cn/gtfzoabxrv.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtfolestvk.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtykwqokmv.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtveaaxqtv.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gtyaqyevqi.html

for (i in 1..10) println(i)
来源：http://hz.jianghu66.top/gtwngqccgd.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangkeji.top/gtpvxogrik.html

interface Shape { fun area(): Double }
来源：http://hz.sweek.top/gtytnhzmre.html

[T16] Swift：Hello World
来源：http://hz.dashuyun.cn/gtvapupaus.html

print("Hello")
来源：http://hz.9152youxi.cn/gtdpharxqb.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtulsbrauh.html

var a = 1;  let b = 2
来源：http://hz.zhijiandao.cn/gtlegqqgxb.html

[T18] Swift：字符串插值
来源：http://hz.xuanzx.com/gtokbxkacp.html

"值: \(b)"
来源：http://hz.guannengcc.top/gtqhlnmvqc.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtcndutgyg.html

if let n = opt { print(n) }
来源：http://hz.tanke756.top/gtpmwsshkk.html

[T20] Swift：数组操作
来源：http://hz.zhoulong.xyz/gtcimgfcpk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinghuilouyu.cn/gtpqcdhtoh.html

[T21] Swift：遍历
来源：http://hz.jiagoushi.top/gtdmtuvjmd.html

for x in a { print(x) }
来源：http://hz.ivvv.top/gtebsrxmaa.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gtrfzeoqed.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gteoussbmx.html

[T23] Swift：函数
来源：http://hz.feifeiyinyue.top/gtgncwxdqc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.svipenyu.cn/gtvzluehxh.html

[T24] Swift：闭包
来源：http://hz.yvedp.cn/gtyhrjdqcg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cqqwz.cn/gtpuoxejeh.html

[T25] Swift：结构体
来源：http://hz.havefunace.top/gtnceojhqr.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtxlpnkosw.html

[T26] Swift：类与重写
来源：http://hz.haohaochexian.top/gttasnshxc.html

class A: Base { override func f() {} }
来源：http://hz.haohaochexian.top/gtyzdlktva.html

[T27] Swift：错误处理
来源：http://hz.gaohongyu789.top/gtimulpxjz.html

do { try f() } catch { print(error) }
来源：http://hz.shangyingyoupin.top/gtlmrrgmay.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gtwebaqrvi.html

enum Color { case red, green }
来源：http://hz.cheryme.top/gtcbaedsnf.html

[T29] Swift：guard 提前返回
来源：http://hz.zhiwuduotai.top/gtirjclqau.html

guard let x = opt else { return }
来源：http://hz.yongpay.top/gtyecuougc.html

[T30] Swift：协议
来源：http://hz.hysaishi.cn/gthtramskr.html

protocol Shape { func area() -> Double }
来源：http://hz.hfpthk.cn/gtmorllfcb.html

[T31] Lua：Hello World
来源：http://hz.birdmap.top/gtarskzxuc.html

print("Hello")
来源：http://hz.yonumen.top/gtkslbfokq.html

[T32] Lua：局部变量
来源：http://hz.zhaomingkeji.xyz/gtgadmsrdq.html

local a = 1
来源：http://hz.meibo888.top/gtyeqcjtyv.html

[T33] Lua：表（数组）
来源：http://hz.jianghu66.top/gteydtmmsq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.aibaodan.cn/gtxyqyczxp.html

[T34] Lua：遍历表
来源：http://hz.hywenlv.cn/gtfkhzxgta.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenlongwang.top/gtynbsqkyb.html

[T35] Lua：字典表
来源：http://hz.tanke756.top/gttesbwtrk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gotoacloud.top/gtftzoneju.html

[T36] Lua：函数
来源：http://hz.cheryme.top/gtbigrmihv.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtwsywtmfz.html

[T37] Lua：字符串拼接
来源：http://hz.yanxiufei.cn/gtfxcbwfjg.html

"a" .. "b"
来源：http://hz.52xcode.cn/gthjqkqocj.html

[T38] Lua：条件
来源：http://hz.gaohongyu789.top/gtnotwfwcp.html

if x > 0 then print("正") end
来源：http://hz.hongshengwenyu.top/gteezwgwjh.html

[T39] Lua：模式匹配
来源：http://hz.snrcjt.cn/gtizskaaaa.html

string.find(s, "%d+")
来源：http://hz.gotoacloud.top/gtjkqngdxu.html

[T40] Lua：元表
来源：http://hz.gaohongyu789.top/gtjwayoidt.html

setmetatable({}, { __index = base })
来源：http://hz.guannengcc.top/gtihhhywkd.html

[T41] Perl：Hello World
来源：http://hz.cashguo.top/gtahmukiah.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtzemoctrp.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtkduyoell.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhengqikj.top/gthoyvesph.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtecndpmhd.html

"值: $a"
来源：http://hz.jqgfzy.top/gtwqutpupe.html

[T44] Perl：条件
来源：http://hz.jinghuilouyu.cn/gtynvecqtg.html

if ($a > 0) { print "正"; }
来源：http://hz.ivvv.top/gtvtnhtsin.html

[T45] Perl：数组遍历
来源：http://hz.jiagoushi.top/gtivjwsncg.html

for my $x (@arr) { print $x; }
来源：http://hz.shangyingyoupin.top/gtnjzadhat.html

[T46] Perl：哈希操作
来源：http://hz.cqqwz.cn/gtndcsukvo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yangfankeji.com/gtajghdeez.html

[T47] Perl：正则捕获
来源：http://hz.cucudq.cn/gtkghiybxs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sxryk.cn/gternjpzdr.html

[T48] Perl：正则替换
来源：http://hz.aibaodan.cn/gtpryrnuwj.html

$s =~ s/old/new/g;
来源：http://hz.havefunace.top/gtxmakrpoa.html

[T49] Perl：函数
来源：http://hz.pengpengdd.cyou/gtfpdhcsju.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jqgfzy.top/gtoxrolyls.html

[T50] Perl：逐行读文件
来源：http://hz.hysaishi.cn/gtbeptrpag.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtobrwkymf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cheryme.top/gtwdqlamcj.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtmytxbelb.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtcjsblekn.html

[T52] Scala：变量
来源：http://hz.nwbrower.top/gtxcopdndw.html

val a = 1;  var b = 2
来源：http://hz.jinqigufen.top/gtsvqkegtd.html

[T53] Scala：字符串插值
来源：http://hz.hammf.cn/gtzxobgfyx.html

s"值: $b"
来源：http://hz.jiagoushi.top/gtqjwufhcm.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtjpzgxdpj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigfzy.top/gtzvjujbcs.html

[T55] Scala：集合过滤
来源：http://hz.shuidangran.top/gtfjzxlkti.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.havefunace.top/gtxmzlcqas.html

[T56] Scala：样例类
来源：http://hz.xuetiantiany.cn/gtcsxnvvzz.html

case class User(name: String, age: Int)
来源：http://hz.gaohongyu789.top/gthjyofjqd.html

[T57] Scala：模式匹配
来源：http://hz.chenzaomai.com/gtuhbvbzkz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxuanxn.top/gtaaapwicp.html

[T58] Scala：函数定义
来源：http://hz.fengsongda.top/gtojcajjas.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhixingplan.top/gtyhaetckc.html

[T59] Scala：循环
来源：http://hz.ybcxt.top/gtjixflkhe.html

for (i <- 1 to 10) println(i)
来源：http://hz.hysaishi.cn/gtmufkcaps.html

[T60] Scala：折叠
来源：http://hz.ybcxt.top/gtayskrthx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xylfe.cn/gtuberzcfx.html

================================================================================
来源：http://hz.sxryk.cn/gtikstovhu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhijiandao.cn/gtmkptvaxg.html

================================================================================
来源：http://hz.pycfn.com/gtmwcllsxb.html


<!-- 参考信息 -->