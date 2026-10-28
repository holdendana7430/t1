代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gtnpdbmskf.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtuzjbeywe.html

scp file user@host:/path/
来源：http://hz.jiagoushi.top/gtibrnuzch.html

[R57] 远程执行命令
来源：http://hz.sweek.top/gtrpedxitj.html

ssh user@host 'uptime'
来源：http://hz.316326.xyz/gtzgzneqlm.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtgwiegain.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtawyhovkl.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtoxhybcem.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ehwqpu.com/gtluigqsao.html

[R60] 只看 HTTP 状态码
来源：http://hz.smart0.xyz/gtwtwdfgzx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gtacahucoi.html

[R61] 磁盘占用
来源：http://hz.jiagoushi.top/gtofwjibye.html

df -h;  du -sh *
来源：http://hz.jinqigufen.top/gthazaibjf.html

[R62] 找最占空间的文件
来源：http://hz.gzhubu.top/gthbecydrb.html

du -ah . | sort -rh | head -10
来源：http://hz.vqdsnc.cn/gtzofefcjm.html

[R63] 内存与进程
来源：http://hz.jqgufenzy.top/gtcdrdsebm.html

free -h;  ps aux | grep nginx
来源：http://hz.sweek.top/gtvgpxqejc.html

[R64] 结束进程
来源：http://hz.sysykeji.top/gtlhgealeh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gtysdqxzzo.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtdywyhwyh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.pengpengdd.cyou/gtfygusghs.html

[R66] 定时任务
来源：http://hz.zhongyouzk.top/gtawiavpjy.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gterhqtabo.html

[R67] 生成随机十六进制串
来源：http://hz.nwbrower.top/gtoibuisry.html

openssl rand -hex 16
来源：http://hz.yuanzhike.top/gtiebohfhp.html

[R68] 计算文件校验值
来源：http://hz.svipenyu.cn/gtvxqliukq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gttvdqxtzy.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gtcpzyoynk.html

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gtjbolmvnl.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtlmuuttyr.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gthchrcxcl.html

[R71] 日期格式化
来源：http://hz.fzhhl.top/gtmrzpwtnc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aizwys.cn/gtecekchnw.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gtcyyrjrwo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtdamxkhny.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtmverxrkw.html

split -l 1000 big.log part_
来源：http://hz.vqdsnc.cn/gtpqdqfntf.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gtakdklxaq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gtnesszoer.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtabgtbxzg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtaktsjmxb.html

[R76] 使用临时文件
来源：http://hz.tianlin.xyz/gtxxggymfo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtxybadxqk.html

[R77] 读取用户输入
来源：http://hz.redwolf501.top/gthjxwperg.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtcbccdnhi.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtihzareel.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tianlin.xyz/gtyfkfcqdv.html

[R79] 解析命令行选项
来源：http://hz.nanxuanxn.top/gtigofxgyq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gttfeqgbcy.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtoamduezq.html

time ./run.sh
来源：http://hz.hywenlv.cn/gtxxtzvmtd.html

================================================================================
来源：http://hz.andypj.xyz/gtddprmhcp.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gteevkdwtg.html

================================================================================
来源：http://hz.316326.xyz/gtxlijhuro.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtibiozgji.html

#include <stdio.h>
来源：http://hz.vqdsnc.cn/gtsapeiesk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gtfqbjokdl.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtkwyuueng.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtcbbqnrpv.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gtiqyqtrui.html

int x; scanf("%d", &x);
来源：http://hz.sxryk.cn/gtlbckircu.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtfzpqrpqf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.fengsongda.top/gtkeaufkyb.html

[S05] C：字符串长度
来源：http://hz.fengsongda.top/gtduuyzkbh.html

strlen(s)
来源：http://hz.shuidangran.top/gtawywzavl.html

[S06] C：字符串比较
来源：http://hz.fzhhl.top/gtqafcwsyc.html

strcmp(a, b) == 0
来源：http://hz.cheryme.top/gteulqmlwb.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gtrqwvwlsq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pycfn.com/gtydnrpkwf.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtomlnjshr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xinyue.icu/gtsnjvsvrz.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gtopbgovza.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtkqrdpuno.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gtttdgrlvn.html

int *p = &a;  *p = 5;
来源：http://hz.dashuyun.cn/gthlorgajb.html

[S11] C：逐行读文件
来源：http://hz.cdnleiting.top/gtglirhgsh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yangfankeji.com/gtgemoejxc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnqzz.top/gtsnamswop.html

fclose(f);
来源：http://hz.aibaodan.cn/gtgdgxkcxl.html

[S12] C：写文件
来源：http://hz.zhongyouzk.top/gtexzwdncz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.mhx1999.top/gtiuxrwyjk.html

[S13] C：宏定义
来源：http://hz.dashuyun.cn/gtgtxvgisv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtarhxrdsi.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtvpuvlotv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuetiantiany.cn/gtrrpltorm.html

[S15] C：类型转换
来源：http://hz.mhx1999.top/gtcunoylli.html

(double) a / b
来源：http://hz.yueranfly.top/gtyyexgxsj.html

[S16] C：位操作置位
来源：http://hz.zhengqikj.top/gtqqjnuxew.html

x |= (1 << 3);
来源：http://hz.daria6918.cn/gtulotfalx.html

[S17] C：安全拼接字符串
来源：http://hz.52xcode.cn/gtszafvekw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fzhhl.top/gtygpaffuh.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gtkmelpmpx.html

int main(int argc, char **argv)
来源：http://hz.aizwys.cn/gtsajvuxea.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gtcgluhcue.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtuxblohgg.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtqrywvvwh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtmqwuckdr.html

[S21] C：字符类别判断
来源：http://hz.jinghuilouyu.cn/gtdexmxueh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258.top/gtouxjfzko.html

[S22] C：字符串转数字
来源：http://hz.zhixingplan.top/gtbkhflyyf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtmykbgztr.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtojrfsnit.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.snrcjt.cn/gtukpsmblk.html

[S24] C：获取本地时间
来源：http://hz.jiagoushi.top/gtjzvnzlwt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtbghozotj.html

[S25] C：内存拷贝
来源：http://hz.xuetiantiany.cn/gtcvofbobq.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtoujwhsnh.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtbqnnzwrq.html

memset(a, 0, sizeof a);
来源：http://hz.aibaodan.cn/gtbrgsygji.html

[S27] C：定义常量
来源：http://hz.tian-w.cn/gtrgsizfup.html

const double PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtffdfeqxu.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gthtnhvqgb.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtdmienkpu.html

[S29] C：变参函数
来源：http://hz.xziqi.cn/gtztjqbolu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtfsaelqmu.html

[S30] C：头文件保护
来源：http://hz.gogol.net.cn/gthqdbqgrx.html

#ifndef X_H
来源：http://hz.jqgfzy.top/gtsunqupjp.html

#define X_H
来源：http://hz.pengpengdd.cyou/gtjahahrxf.html

#endif
来源：http://hz.9152youxi.cn/gtqoiwryvc.html

[S31] C++：Hello World
来源：http://hz.kuanghao11.cn/gteggdkmba.html

#include <iostream>
来源：http://hz.hywenlv.cn/gtiulmvzou.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.haohaochexian.top/gtdhggaekk.html

[S32] C++：字符串
来源：http://hz.redwolf501.top/gtbehsczqs.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtejzdmslu.html

[S33] C++：vector 增删
来源：http://hz.daria6918.cn/gtcovnolsw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tian-w.cn/gtppxmcgsd.html

[S34] C++：遍历 vector
来源：http://hz.zhaomingkeji.xyz/gtikmuktpc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tianlin.xyz/gtflowagan.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gtxcuwnowx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtkmzbyqub.html

[S36] C++：unordered_map
来源：http://hz.shuidangran.top/gtbhajcmfd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gticuwbppc.html

[S37] C++：set
来源：http://hz.shzxlz.cn/gtzipdtohx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtniovxgaa.html

[S38] C++：排序
来源：http://hz.sufxvd.cn/gtrwvwhmqx.html

std::sort(v.begin(), v.end());
来源：http://hz.redwolf501.top/gtpzkxmgpc.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtfbvnjxgp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhixingplan.top/gtmywpwatz.html

[S40] C++：查找元素
来源：http://hz.yanxiufei.cn/gtsmmkiprb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtnfjwvdtk.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtgeaxtlzj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtsftthrwg.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtiwdycaxh.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtgosnrmbl.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtcivgodmx.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtdvrhrjnc.html

[S44] C++：引用传参
来源：http://hz.yueranfly.top/gtujfsyqhl.html

void inc(int &x) { ++x; }
来源：http://hz.nwbrower.top/gtccgrgcll.html

[S45] C++：lambda
来源：http://hz.jyoumei.cn/gtuypkygko.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtfqwmgljy.html

[S46] C++：函数模板
来源：http://hz.shangyingyoupin.top/gtzocijygr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtamcaudgh.html

[S47] C++：结构化绑定遍历
来源：http://hz.ppjwa.cn/gtehojyncz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gththkrgam.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtdvvzlhlj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtolqmqhsu.html

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtcwqtvxas.html

[S49] C++：写文件
来源：http://hz.xingfuxueyuan.xyz/gtjtajhbbr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sweek.top/gtfkbbtxce.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtquugodhx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtpregdgaa.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtvmzemngv.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtpdqrvpfi.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtduafrrhg.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigufen.top/gtnlwmwiha.html

[S53] C++：移动语义
来源：http://hz.ehwqpu.com/gtywjhtnad.html

std::vector<int> w = std::move(v);
来源：http://hz.vqdsnc.cn/gtoaytvpzk.html

[S54] C++：异常处理
来源：http://hz.cdnleiting.top/gtoaiwzwye.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtvciwfgct.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtldtgknwt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gttjexsmbu.html

[S56] C++：optional
来源：http://hz.pengpengdd.cyou/gtceltglej.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pengpengdd.cyou/gtevgwdxoc.html

[S57] C++：编译期常量
来源：http://hz.pycfn.com/gtovxbwssl.html

constexpr int N = 10;
来源：http://hz.yonumen.top/gtzhsxiwrn.html

[S58] C++：命名空间
来源：http://hz.daxiang520.top/gttghpgnpf.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtapozohvp.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gttpqpirrr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhoulong.xyz/gtfrykefpb.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtowvbzbhj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ivvv.top/gtyrscyqaw.html

================================================================================
来源：http://hz.jqgfzy.top/gtjccdmgip.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gttjwnsasu.html

================================================================================
来源：http://hz.yongpay.top/gtoesorsob.html

[T01] Kotlin：Hello World
来源：http://hz.ywan-chungtsiang.top/gthqqsxebp.html

println("Hello")
来源：http://hz.hammf.cn/gtbqjdnarr.html

[T02] Kotlin：变量
来源：http://hz.316326.xyz/gtwbcpndht.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nwbrower.top/gtmroxsfee.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gtsdvrwkyu.html

"值: $b"
来源：http://hz.cucudq.cn/gtoupbgiwm.html

[T04] Kotlin：空安全
来源：http://hz.zhongyouzk.top/gtpakocwmu.html

val n: String? = null;  n?.length
来源：http://hz.dashuyun.cn/gtnivkxudx.html

[T05] Kotlin：when 表达式
来源：http://hz.havefunace.top/gtqxsjwgzv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ywan-chungtsiang.top/gtaufzpodd.html

[T06] Kotlin：集合映射
来源：http://hz.gotoacloud.top/gtvxshexyh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.quarkkingdee.top/gtxckhxary.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigufen.top/gtjgvnoxsx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtxmjwtjqd.html

[T08] Kotlin：数据类
来源：http://hz.mhx1999.top/gtfqkchjci.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtyxqokbwa.html

[T09] Kotlin：扩展函数
来源：http://hz.yueranfly.top/gtacsqvywy.html

fun String.exclaim() = this + "!"
来源：http://hz.tian-w.cn/gtiiteslbk.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gtozhuqbpy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yueranfly.top/gtxkynfhrf.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gtmrpjpeyg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gttvnmcodk.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtkgoxldbd.html

val (a, b) = Pair(1, 2)
来源：http://hz.dianchejie.cn/gtrisxdmtg.html

[T13] Kotlin：只读 Map
来源：http://hz.haohaochexian.top/gtvrlqvoqt.html

val m = mapOf("a" to 1)
来源：http://hz.sysykeji.top/gtigxahhei.html

[T14] Kotlin：循环
来源：http://hz.zhixingplan.top/gtqejezgvj.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtkcdyqayn.html

[T15] Kotlin：接口
来源：http://hz.ybcxt.top/gtnmrobfsy.html

interface Shape { fun area(): Double }
来源：http://hz.chenjidiqi.icu/gtqnwnywrg.html

[T16] Swift：Hello World
来源：http://hz.yonumen.top/gtdpvxwbvw.html

print("Hello")
来源：http://hz.xylfe.cn/gtwwmtopel.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtmwbnqhkc.html

var a = 1;  let b = 2
来源：http://hz.tian-w.cn/gtubqniuis.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gtfslznezp.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtgcabuacz.html

[T19] Swift：可选绑定
来源：http://hz.hfpthk.cn/gtzctusims.html

if let n = opt { print(n) }
来源：http://hz.xylfe.cn/gtatjwimbr.html

[T20] Swift：数组操作
来源：http://hz.meibo888.top/gtkgsvflbm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgfzy.top/gtmykbqitw.html

[T21] Swift：遍历
来源：http://hz.jianghu66.top/gtiptqqgdd.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtcjzkphie.html

[T22] Swift：字典
来源：http://hz.gzhubu.top/gtzbcxipua.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shuidangran.top/gtukrmuzcv.html

[T23] Swift：函数
来源：http://hz.sysykeji.top/gtoopbfjdn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.haohaochexian.top/gtdypaoxja.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtjvcposyh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtzkfwasgc.html

[T25] Swift：结构体
来源：http://hz.fengsongda.top/gtoiokmlgr.html

struct P { var x: Int }
来源：http://hz.ivvv.top/gtptmulshc.html

[T26] Swift：类与重写
来源：http://hz.jinghuilouyu.cn/gtqehvfkfm.html

class A: Base { override func f() {} }
来源：http://hz.zhijiandao.cn/gtwchqonsg.html

[T27] Swift：错误处理
来源：http://hz.gogol.net.cn/gtueyxumwe.html

do { try f() } catch { print(error) }
来源：http://hz.redwolf501.top/gtlebiyatu.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtlkjvbsdn.html

enum Color { case red, green }
来源：http://hz.0kj1m.cn/gttfjarzlc.html

[T29] Swift：guard 提前返回
来源：http://hz.sufxvd.cn/gtlkgqekhh.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gtgiwqwquy.html

[T30] Swift：协议
来源：http://hz.havefunace.top/gtdgpjxuvd.html

protocol Shape { func area() -> Double }
来源：http://hz.yuanzhike.top/gtcjgapdmi.html

[T31] Lua：Hello World
来源：http://hz.ywan-chungtsiang.top/gtyhwzzdlz.html

print("Hello")
来源：http://hz.ydzc1.top/gtwkzaaypb.html

[T32] Lua：局部变量
来源：http://hz.ehwqpu.com/gtnadhlmpt.html

local a = 1
来源：http://hz.birdmap.top/gtzebwipnq.html

[T33] Lua：表（数组）
来源：http://hz.haohaochexian.top/gtcyiriwvw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.aizwys.cn/gtvbhostmw.html

[T34] Lua：遍历表
来源：http://hz.jinyuanbaomall.cn/gtuubtacud.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtaohwvlup.html

[T35] Lua：字典表
来源：http://hz.hnqzz.top/gtpkfbnkvc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtwfvfhwrn.html

[T36] Lua：函数
来源：http://hz.daxiang520.top/gtwzgnkfiq.html

function add(a, b) return a + b end
来源：http://hz.jyoumei.cn/gtxqemgdvm.html

[T37] Lua：字符串拼接
来源：http://hz.sysykeji.top/gtoscqkain.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtwgjcpkpd.html

[T38] Lua：条件
来源：http://hz.aibaodan.cn/gttjeiblwe.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtulvlcsie.html

[T39] Lua：模式匹配
来源：http://hz.daxiang520.top/gtpstkfzvp.html

string.find(s, "%d+")
来源：http://hz.gaohongyu789.top/gtwsidoxwi.html

[T40] Lua：元表
来源：http://hz.shanyushiyangtech.top/gtjrpgywif.html

setmetatable({}, { __index = base })
来源：http://hz.yongpay.top/gtirfpmnpo.html

[T41] Perl：Hello World
来源：http://hz.guowangkeji.top/gtmsbxcmaw.html

print "Hello\n";
来源：http://hz.jqgufenzy.top/gtbokgcpxg.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtszbrpmhk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenzaomai.com/gtgiblczyt.html

[T43] Perl：字符串插值
来源：http://hz.xylfe.cn/gtqzqutvpx.html

"值: $a"
来源：http://hz.jinqigufen.top/gtrvjlbqsj.html

[T44] Perl：条件
来源：http://hz.guowangkeji.top/gtlqwxcjec.html

if ($a > 0) { print "正"; }
来源：http://hz.ywan-chungtsiang.top/gtfgjsqviz.html

[T45] Perl：数组遍历
来源：http://hz.yonumen.top/gtokvtblfc.html

for my $x (@arr) { print $x; }
来源：http://hz.9152youxi.cn/gtgshajajl.html

[T46] Perl：哈希操作
来源：http://hz.shangyingyoupin.top/gtpksvyuyd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hysaishi.cn/gtpibgpkcd.html

[T47] Perl：正则捕获
来源：http://hz.yanxiufei.cn/gtdbdbaoby.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guannengcc.top/gtqpksymrn.html

[T48] Perl：正则替换
来源：http://hz.iojbl.cn/gtxhbnpqnd.html

$s =~ s/old/new/g;
来源：http://hz.gotoacloud.top/gtxifposfs.html

[T49] Perl：函数
来源：http://hz.chenlongwang.top/gtffivrlyu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhengqikj.top/gtesycvsot.html

[T50] Perl：逐行读文件
来源：http://hz.bjfxy.top/gtavxbtfjc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.meibo888.top/gthlmigkke.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gtrfwebcex.html

[T51] Scala：Hello World
来源：http://hz.birdmap.top/gtimhdphax.html

println("Hello")
来源：http://hz.0kj1m.cn/gtoswbqivc.html

[T52] Scala：变量
来源：http://hz.hammf.cn/gtfdfpgvoo.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtigpmjhgv.html

[T53] Scala：字符串插值
来源：http://hz.fengsongda.top/gteswjkbbx.html

s"值: $b"
来源：http://hz.dashuyun.cn/gtmwynfoaz.html

[T54] Scala：集合映射
来源：http://hz.jqgufenzy.top/gtqkhddqao.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hfpthk.cn/gtrfjacpgw.html

[T55] Scala：集合过滤
来源：http://hz.quarkkingdee.top/gtpojmprsy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtsmhzydpn.html

[T56] Scala：样例类
来源：http://hz.hywenlv.cn/gtqurrgyxp.html

case class User(name: String, age: Int)
来源：http://hz.feifeiyinyue.top/gtqvpbamrb.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gtvwvtvpwe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pycfn.com/gtvdqjirxp.html

[T58] Scala：函数定义
来源：http://hz.yj20258.top/gtnafcrqsc.html


<!-- 参考信息 -->