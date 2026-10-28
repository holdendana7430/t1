代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydjk.org.cn/gtrwqjlgle.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtbaxkgxdx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daria6918.cn/gtqlplyrsf.html

[R51] 排序去重取前几
来源：http://hz.zhixingplan.top/gtbqnzldtm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtlisscbvj.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtyibcadvv.html

wc -l a.txt
来源：http://hz.meibo888.top/gtuxtbrtee.html

[R53] 查看文件头与实时尾
来源：http://hz.pycfn.com/gtrobgpdgb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtdfuonenl.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtvtstbdqd.html

diff a.txt b.txt
来源：http://hz.iojbl.cn/gtemsnwxzs.html

[R55] 压缩与解压
来源：http://hz.zdqjudy.top/gtseebforl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gtwgqifwcd.html

[R56] 远程拷贝
来源：http://hz.zhaomingkeji.xyz/gtzipniosb.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtgjofslcp.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtlqufiyju.html

ssh user@host 'uptime'
来源：http://hz.quarkkingdee.top/gtilmclzhr.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtgfgdzboo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hongshengwenyu.top/gtywhnaohj.html

[R59] 发 POST JSON
来源：http://hz.hfpthk.cn/gtdtjacraz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fengsongda.top/gtiljpyzsd.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtijdvwcoe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtzkstfipg.html

[R61] 磁盘占用
来源：http://hz.pengpengdd.cyou/gtkqcbrijp.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtduyyifyj.html

[R62] 找最占空间的文件
来源：http://hz.havefunace.top/gtjwjvvzdy.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtuemrcrmk.html

[R63] 内存与进程
来源：http://hz.nwbrower.top/gtafbkcdvw.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtqznjsdnp.html

[R64] 结束进程
来源：http://hz.redwolf501.top/gttsihrkrq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtvzsdioux.html

[R65] 查看端口占用
来源：http://hz.yvedp.cn/gtzbsjuiuu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinyuanbaomall.cn/gtaixdfzvn.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtpudmthhe.html

crontab -e;  crontab -l
来源：http://hz.yj202588.top/gtwswzuccy.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gtmkkzbkbn.html

openssl rand -hex 16
来源：http://hz.mhx1999.top/gtuuhbdkfs.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtohjlbokl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangkeji.top/gtgyklyyft.html

[R69] 生成随机密码
来源：http://hz.feifeiyinyue.top/gtddytsrqw.html

head -c 16 /dev/urandom | base64
来源：http://hz.cucudq.cn/gtxgmnefqv.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtcbdbrooh.html

date +%s;  date -d @1700000000
来源：http://hz.zhoulong.xyz/gtaafwwqpz.html

[R71] 日期格式化
来源：http://hz.feifeiyinyue.top/gtnbpeoamg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtlqkaascv.html

[R72] 等待端口就绪
来源：http://hz.ybcxt.top/gtqghbvtfi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shuidangran.top/gtbjihbvcl.html

[R73] 分割大日志
来源：http://hz.quarkkingdee.top/gtjrzlzpcd.html

split -l 1000 big.log part_
来源：http://hz.hnqzz.top/gtuovaxjfx.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtnfmrcblb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhengqikj.top/gtzcfpkcsp.html

[R75] 导出环境变量
来源：http://hz.ydjk.org.cn/gtofjdzeri.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenzaomai.com/gtenkvsdek.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gttlfseoiu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtxrmsjqjv.html

[R77] 读取用户输入
来源：http://hz.gotoacloud.top/gtkzvhlnaj.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gtyqtetnag.html

[R78] 交互式菜单
来源：http://hz.jinqigufen.top/gtuxkhzviu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ppjwa.cn/gtbtpfkazu.html

[R79] 解析命令行选项
来源：http://hz.mhx1999.top/gtaqfgawzk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtkclwdolf.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtgctzibma.html

time ./run.sh
来源：http://hz.daxiang520.top/gtmbhgwavv.html

================================================================================
来源：http://hz.tianlin.xyz/gtfrymubti.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtrddwubhd.html

================================================================================
来源：http://hz.nwbrower.top/gtpkfdogmy.html

[S01] C：Hello World
来源：http://hz.zhijiandao.cn/gtipysmaxg.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtluysuyyx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtipdcvhmw.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtfguznovq.html

int a = 10; printf("%d\n", a);
来源：http://hz.cqqwz.cn/gtsqhhhozw.html

[S03] C：读入整数
来源：http://hz.cashguo.top/gtctmzagfi.html

int x; scanf("%d", &x);
来源：http://hz.kuanghao11.cn/gtkjjggzek.html

[S04] C：字符串复制
来源：http://hz.pycfn.com/gtgnbnpzcw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuxming.cn/gtvjeqqlid.html

[S05] C：字符串长度
来源：http://hz.dianchejie.cn/gtiejwbmzu.html

strlen(s)
来源：http://hz.yvedp.cn/gtymchmnkd.html

[S06] C：字符串比较
来源：http://hz.aibaodan.cn/gtjpcfacdo.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtoppusypg.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gtzejcyygh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtzyphooox.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtldeiwvre.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtqoxdjqzx.html

[S09] C：结构体定义与初始化
来源：http://hz.chenjidiqi.icu/gtaerxusie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hywenlv.cn/gtnknzzdqi.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gtkpelcrkc.html

int *p = &a;  *p = 5;
来源：http://hz.tian-w.cn/gtfzbzcxlr.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gtzbofmxjc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ehwqpu.com/gtapcnonxf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cqqwz.cn/gtkynddogo.html

fclose(f);
来源：http://hz.fzhhl.top/gtzyentxuc.html

[S12] C：写文件
来源：http://hz.kuanghao11.cn/gtsejdbohd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gthvvghggx.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtqdazcugi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gthprrizbx.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtdffuhqaz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtdorfmroq.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gtiskynifb.html

(double) a / b
来源：http://hz.ehwqpu.com/gtqkyuyukf.html

[S16] C：位操作置位
来源：http://hz.zhixingplan.top/gtbsypqaki.html

x |= (1 << 3);
来源：http://hz.jinyuanbaomall.cn/gtualrgnps.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtypncqikd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xingfuxueyuan.xyz/gtroljvnkk.html

[S18] C：命令行参数
来源：http://hz.gaohongyu789.top/gtrbwjngrr.html

int main(int argc, char **argv)
来源：http://hz.zhoulong.xyz/gtlkhdozso.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gtrowgwyse.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtvcooscre.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtpsaaquez.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtgwyerwwl.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtavpvmndr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenzaomai.com/gtdhpixqbb.html

[S22] C：字符串转数字
来源：http://hz.cdnleiting.top/gttykgknwi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jianghu66.top/gtakrixbmy.html

[S23] C：随机数
来源：http://hz.yueranfly.top/gtranbxlcs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtbfgkhphw.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtbrbyeunn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hnxiangtu.top/gtxbisaldg.html

[S25] C：内存拷贝
来源：http://hz.kuanghao11.cn/gtswnielsv.html

memcpy(dst, src, n);
来源：http://hz.jinqigfzy.top/gtaufuebje.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gtwqkzfumu.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtzhasokub.html

[S27] C：定义常量
来源：http://hz.redwolf501.top/gtqvkhyznu.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtvdiihedi.html

[S28] C：静态变量
来源：http://hz.jinqigfzy.top/gtppdnxgez.html

static int counter = 0;
来源：http://hz.ehwqpu.com/gtarxhgfkm.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtvflebebe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hongshengwenyu.top/gthhxcrvps.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtjgjadvwo.html

#ifndef X_H
来源：http://hz.svipenyu.cn/gtkcjiojfe.html

#define X_H
来源：http://hz.nwbrower.top/gtxhdyvrhx.html

#endif
来源：http://hz.cucudq.cn/gtrylbmrgc.html

[S31] C++：Hello World
来源：http://hz.tianlin.xyz/gtdkerueyv.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtavjvlbkv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtqtrblfbc.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtmyvhnsml.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtqvymzaxo.html

[S33] C++：vector 增删
来源：http://hz.316326.xyz/gtalwozoyd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cheryme.top/gtwagmwixi.html

[S34] C++：遍历 vector
来源：http://hz.xinyue.icu/gtkgbwmvcg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cheryme.top/gtplgwrsvx.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtkutxiquv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtbwxxkryb.html

[S36] C++：unordered_map
来源：http://hz.xylfe.cn/gtlbjnmuhv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtnzwlwwhu.html

[S37] C++：set
来源：http://hz.sweek.top/gtlqqajqea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtpenjcwda.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gttosceyrb.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtosletcjc.html

[S39] C++：自定义比较器排序
来源：http://hz.yj202588.top/gtwhcjzuxv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhaomingkeji.xyz/gtoavvxqiw.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtxdykokwh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtpishveib.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtbbgcdawq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtdciyccip.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtbvqjvkak.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhixingplan.top/gtisteoqed.html

[S43] C++：智能指针
来源：http://hz.quarkkingdee.top/gtbhjxhjuc.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gtyoexnypf.html

[S44] C++：引用传参
来源：http://hz.tian-w.cn/gtecudiiri.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtwietpolh.html

[S45] C++：lambda
来源：http://hz.pycfn.com/gtcwvgfnda.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jlsjyb.cn/gttenqxakq.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangtech.top/gtplxwecdm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shzxlz.cn/gtpkdtebuv.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgufenzy.top/gtsxgewkxy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtmngbisjg.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gttglirzja.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtdsdwoetr.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gtjfrliles.html

[S49] C++：写文件
来源：http://hz.shanyushiyangkeji.top/gtyyzuawqz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hfpthk.cn/gtlfjakgmz.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtltxyhmqm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.mhx1999.top/gteszupjvb.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtfqkxfmwo.html

static_cast<double>(a) / b
来源：http://hz.jinyuanbaomall.cn/gtsgyrlylu.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtznuajbnc.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gtcfsfmaml.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtnhmgocob.html

std::vector<int> w = std::move(v);
来源：http://hz.kuanghao11.cn/gtazeamypq.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtfjmccedo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.smart0.xyz/gtafodcsrq.html

[S55] C++：结构化绑定
来源：http://hz.guowangkeji.top/gtqgfjmrnw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxuanxn.top/gtmktabluj.html

[S56] C++：optional
来源：http://hz.cqqwz.cn/gtkhcyufvt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtyscwssdc.html

[S57] C++：编译期常量
来源：http://hz.dashuyun.cn/gthqtbxpmc.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtnveezjfw.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gtqnyywkef.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtyilebuhk.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gtgxwakvbv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtspmobghi.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtgeqqqwhd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtlphezaab.html

================================================================================
来源：http://hz.hfpthk.cn/gtmvfbdinz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigfzy.top/gtgpztihhv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdowonejk.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtnolaykmk.html

println("Hello")
来源：http://hz.sysykeji.top/gtldrouzzm.html

[T02] Kotlin：变量
来源：http://hz.zhixingplan.top/gtruecmamb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigufen.top/gtlwekmrfk.html

[T03] Kotlin：字符串模板
来源：http://hz.zhiwuduotai.top/gtmxosyjjx.html

"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtmmrhgwyk.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtenvamknz.html

val n: String? = null;  n?.length
来源：http://hz.dashuyun.cn/gtvuetsijy.html

[T05] Kotlin：when 表达式
来源：http://hz.shuidangran.top/gtedtmfrsg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.mhx1999.top/gtvditkvgt.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gtbieldhom.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gtwdnsqalh.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangtech.top/gtljyaitij.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.daria6918.cn/gttteqlwuj.html

[T08] Kotlin：数据类
来源：http://hz.aizwys.cn/gtsklyiopa.html

data class User(val name: String, val age: Int)
来源：http://hz.wangshuangyany.cn/gtbfcmdrar.html

[T09] Kotlin：扩展函数
来源：http://hz.yuxming.cn/gteyqcwnbk.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtyjryqopj.html

[T10] Kotlin：默认参数
来源：http://hz.shangyingyoupin.top/gtknpgtdvh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shanyushiyangkeji.top/gthljtwtyr.html

[T11] Kotlin：协程
来源：http://hz.ydjk.org.cn/gtymbjdyay.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gttgpztwae.html

[T12] Kotlin：解构声明
来源：http://hz.aibaodan.cn/gtdsjvcfqw.html

val (a, b) = Pair(1, 2)
来源：http://hz.xinyue.icu/gtjkmzpcdb.html

[T13] Kotlin：只读 Map
来源：http://hz.xuanzx.com/gtxmkusplt.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtxdbznerd.html

[T14] Kotlin：循环
来源：http://hz.sufxvd.cn/gtgnsfywbu.html

for (i in 1..10) println(i)
来源：http://hz.hongshengwenyu.top/gtlxxvtkct.html

[T15] Kotlin：接口
来源：http://hz.sweek.top/gtqyyedrds.html

interface Shape { fun area(): Double }
来源：http://hz.gaohongyu789.top/gtzlpeyxhy.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtldbwzbha.html

print("Hello")
来源：http://hz.yangfankeji.com/gtlnzhygae.html

[T17] Swift：变量与常量
来源：http://hz.havefunace.top/gtlcclbkbm.html

var a = 1;  let b = 2
来源：http://hz.vqdsnc.cn/gtdxwiohyd.html

[T18] Swift：字符串插值
来源：http://hz.chenlongwang.top/gtqfqxryix.html

"值: \(b)"
来源：http://hz.9152youxi.cn/gtjnxpowde.html

[T19] Swift：可选绑定
来源：http://hz.zhengqikj.top/gtcetijhtf.html

if let n = opt { print(n) }
来源：http://hz.gaohongyu789.top/gtkuxialli.html

[T20] Swift：数组操作
来源：http://hz.tian-w.cn/gtakluaeai.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tanke756.top/gtoueeqqsx.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtadxykfha.html

for x in a { print(x) }
来源：http://hz.52xcode.cn/gtugmmchrc.html

[T22] Swift：字典
来源：http://hz.birdmap.top/gtbqpzpiaq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtzbljljab.html

[T23] Swift：函数
来源：http://hz.zhiwuduotai.top/gtftfbkxre.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jqgfzy.top/gtbmopqsag.html

[T24] Swift：闭包
来源：http://hz.vqdsnc.cn/gtthtohjdy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jianghu66.top/gtghgqnhee.html

[T25] Swift：结构体
来源：http://hz.nanxuanxn.top/gtctuynbfu.html

struct P { var x: Int }
来源：http://hz.pengpengdd.cyou/gtogdddvsn.html

[T26] Swift：类与重写
来源：http://hz.cashguo.top/gtzwqbvsce.html

class A: Base { override func f() {} }
来源：http://hz.hongshengwenyu.top/gtnxnvtnan.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtemptwndn.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtnckxhqor.html

[T28] Swift：枚举
来源：http://hz.yueranfly.top/gtsstjnkwh.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtpuglvhms.html

[T29] Swift：guard 提前返回
来源：http://hz.zhijiandao.cn/gtsjdbniqr.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangtech.top/gtypiosdap.html

[T30] Swift：协议
来源：http://hz.52xcode.cn/gtwekqtsep.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gthgywselb.html

[T31] Lua：Hello World
来源：http://hz.9152youxi.cn/gtnpyiaciy.html

print("Hello")
来源：http://hz.zhixingplan.top/gtzoonwcvy.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangkeji.top/gtbpwnhwbl.html

local a = 1
来源：http://hz.chenjidiqi.icu/gteqbudzko.html

[T33] Lua：表（数组）
来源：http://hz.jqgufenzy.top/gtcdkcutei.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jiagoushi.top/gtmaaguyuw.html

[T34] Lua：遍历表
来源：http://hz.ppjwa.cn/gtfwieqqql.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dianchejie.cn/gtfpimwnir.html

[T35] Lua：字典表
来源：http://hz.hywenlv.cn/gtaidbwhbk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jianghu66.top/gtysximhwx.html

[T36] Lua：函数
来源：http://hz.zdqjudy.top/gtjtlasfcs.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gtqufdxiyz.html

[T37] Lua：字符串拼接
来源：http://hz.hywenlv.cn/gthrlxfbgd.html

"a" .. "b"
来源：http://hz.mhx1999.top/gtazyxrhgk.html

[T38] Lua：条件
来源：http://hz.jqgfzy.top/gtgarfzofa.html

if x > 0 then print("正") end
来源：http://hz.hnxiangtu.top/gtkffamxov.html

[T39] Lua：模式匹配
来源：http://hz.hammf.cn/gtmwhvidkz.html

string.find(s, "%d+")
来源：http://hz.quarkkingdee.top/gtefswtxhi.html

[T40] Lua：元表
来源：http://hz.hysaishi.cn/gtqpycholr.html

setmetatable({}, { __index = base })
来源：http://hz.zhongyouzk.top/gtthcxwvzy.html

[T41] Perl：Hello World
来源：http://hz.sweek.top/gtwbgqhlfg.html

print "Hello\n";
来源：http://hz.smart0.xyz/gtprsrqxbz.html

[T42] Perl：变量类型
来源：http://hz.yanxiufei.cn/gtczhtgcme.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sysykeji.top/gtzpqfribf.html

[T43] Perl：字符串插值
来源：http://hz.52xcode.cn/gtgsohhazw.html

"值: $a"
来源：http://hz.smart0.xyz/gtjgumvtmf.html

[T44] Perl：条件
来源：http://hz.pengpengdd.cyou/gthdnrugrh.html

if ($a > 0) { print "正"; }
来源：http://hz.xziqi.cn/gtsupeoamk.html

[T45] Perl：数组遍历
来源：http://hz.0kj1m.cn/gtrkexnwzn.html

for my $x (@arr) { print $x; }
来源：http://hz.zdqjudy.top/gtrjpkxkcn.html

[T46] Perl：哈希操作
来源：http://hz.52xcode.cn/gtsfkknchu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tanke756.top/gtpugpwtve.html

[T47] Perl：正则捕获
来源：http://hz.pycfn.com/gtouojehnr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guowangkeji.top/gtqwmtjmqd.html

[T48] Perl：正则替换
来源：http://hz.jlsjyb.cn/gtydewqfzv.html

$s =~ s/old/new/g;
来源：http://hz.zhoulong.xyz/gtxlniutba.html

[T49] Perl：函数
来源：http://hz.tanke756.top/gtdwzhqoeq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sufxvd.cn/gtpvarmsce.html

[T50] Perl：逐行读文件
来源：http://hz.ybcxt.top/gtrfbwexul.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.andypj.xyz/gtuuhpoewy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yangfankeji.com/gtopntnxvs.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtolxyyuua.html

println("Hello")
来源：http://hz.ivvv.top/gtweeyxtpx.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtrfpkxujo.html


<!-- 参考信息 -->