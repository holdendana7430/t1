代发 wailian999

find . -name "*.log" -type f
来源：http://hz.mhx1999.top/gttxjfvpkn.html

[R44] 按修改时间查找
来源：http://hz.cheryme.top/gtilprsilq.html

find . -mtime -7 -type f
来源：http://hz.cucudq.cn/gtegwxequw.html

[R45] 批量删除
来源：http://hz.xuetiantiany.cn/gtenacljzy.html

find . -name "*.tmp" -delete
来源：http://hz.chenzaomai.com/gtsatwqyij.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gttmbazinq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.svipenyu.cn/gtihedsyoa.html

[R47] sed 单行替换
来源：http://hz.ivvv.top/gtczmrobse.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.snrcjt.cn/gtqavagofz.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtydphlsal.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gtmxzeipfu.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtlbzkjhdn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.vqdsnc.cn/gtuvhtymwh.html

[R50] awk 求和
来源：http://hz.wangshuangyany.cn/gtmbwyhoos.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenzaomai.com/gttkdfkaoz.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtbkujdxbc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtkvlolwjo.html

[R52] 统计行数
来源：http://hz.jiagoushi.top/gtmkfncizb.html

wc -l a.txt
来源：http://hz.guannengcc.top/gtevaugfzo.html

[R53] 查看文件头与实时尾
来源：http://hz.hnqzz.top/gteffrkcxq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.svipenyu.cn/gtnfbqtfhg.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gtoruvaycc.html

diff a.txt b.txt
来源：http://hz.c1oappe.top/gthmezjbrg.html

[R55] 压缩与解压
来源：http://hz.jinqigfzy.top/gtkhqbwkdx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gtngyppvfi.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gtaogaqjkk.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gttpkmxwdf.html

[R57] 远程执行命令
来源：http://hz.hfpthk.cn/gtstoddwnf.html

ssh user@host 'uptime'
来源：http://hz.shuidangran.top/gtdxrpvnfc.html

[R58] 下载文件
来源：http://hz.zhongyouzk.top/gtsjgifzbk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sxryk.cn/gtlmhgpcad.html

[R59] 发 POST JSON
来源：http://hz.xylfe.cn/gtimdliiim.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenzaomai.com/gtvvoecfvz.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhixingplan.top/gtqglzgyoz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhengqikj.top/gtiefvzmqy.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtswuzbvcr.html

df -h;  du -sh *
来源：http://hz.yvedp.cn/gtrdopfvkp.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtfhqxkxjh.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gthwaacopo.html

[R63] 内存与进程
来源：http://hz.gzhubu.top/gtxltjymhb.html

free -h;  ps aux | grep nginx
来源：http://hz.yongpay.top/gtpshlqowk.html

[R64] 结束进程
来源：http://hz.cashguo.top/gtbsiwhocx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtnzjpgmdk.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtruzkudpq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cucudq.cn/gtmxuixdjo.html

[R66] 定时任务
来源：http://hz.zycfv.cn/gtdeuzjyan.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtngcjragz.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gtnmmylvnd.html

openssl rand -hex 16
来源：http://hz.gaohongyu789.top/gthoxkmygl.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gttqdtrcsx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtacxihiwe.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gtqwltskhq.html

head -c 16 /dev/urandom | base64
来源：http://hz.smart0.xyz/gtawmhtxke.html

[R70] 时间戳与互转
来源：http://hz.tanke756.top/gtmeqyywzk.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtfikkakqe.html

[R71] 日期格式化
来源：http://hz.cqqwz.cn/gtisfixlha.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtirwnbmtk.html

[R72] 等待端口就绪
来源：http://hz.shuidangran.top/gtdgmwvzbn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ppjwa.cn/gtjdemxlsu.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtppnbykda.html

split -l 1000 big.log part_
来源：http://hz.bjfxy.top/gtjvkssqce.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtakqcitqm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gtxfuloyzs.html

[R75] 导出环境变量
来源：http://hz.aizwys.cn/gtoyzjixei.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenzaomai.com/gtjydrocwm.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangtech.top/gtilqdddco.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gteggsmcmz.html

[R77] 读取用户输入
来源：http://hz.fzhhl.top/gtafvjbjof.html

read -rp "请输入: " ans
来源：http://hz.nwbrower.top/gtohgrbttp.html

[R78] 交互式菜单
来源：http://hz.sufxvd.cn/gthbxnytgy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuetiantiany.cn/gtvtnxbspa.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtamcccswf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cdnleiting.top/gtyicjspfo.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtdtbqanve.html

time ./run.sh
来源：http://hz.jiagoushi.top/gtlprfdfhw.html

================================================================================
来源：http://hz.jqgfzy.top/gtaoriddsg.html

S. C / C++ 专题
来源：http://hz.iojbl.cn/gtmpetrrhv.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtlwsjrksj.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtrfqsaryj.html

#include <stdio.h>
来源：http://hz.havefunace.top/gtbmmuewif.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnxiangtu.top/gtvfvqlutb.html

[S02] C：变量与格式化输出
来源：http://hz.zhaomingkeji.xyz/gtvppvntrv.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangdashe.top/gtfxqmtgbe.html

[S03] C：读入整数
来源：http://hz.hywenlv.cn/gtiiohmjqm.html

int x; scanf("%d", &x);
来源：http://hz.iojbl.cn/gtpfsnscaa.html

[S04] C：字符串复制
来源：http://hz.52xcode.cn/gtmyvndevk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gthykvjxle.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtxkibpvsg.html

strlen(s)
来源：http://hz.redwolf501.top/gtmgeynmnf.html

[S06] C：字符串比较
来源：http://hz.haohaochexian.top/gtlnkewtci.html

strcmp(a, b) == 0
来源：http://hz.pengpengdd.cyou/gtfvgybvaq.html

[S07] C：数组遍历求和
来源：http://hz.guannengcc.top/gtlwpawrrx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gtbafgxslx.html

[S08] C：动态内存分配与释放
来源：http://hz.jlsjyb.cn/gtqomervnm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtjrqgpskp.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtkgknqisg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jianghu66.top/gtbwgiuazi.html

[S10] C：指针与解引用
来源：http://hz.hongshengwenyu.top/gtqjrfiaum.html

int *p = &a;  *p = 5;
来源：http://hz.yongpay.top/gtmxrhhwcm.html

[S11] C：逐行读文件
来源：http://hz.ybcxt.top/gtmnlfqdza.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnqzz.top/gtpunlaovn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cdnleiting.top/gtolsamizn.html

fclose(f);
来源：http://hz.ppjwa.cn/gtvoazstzk.html

[S12] C：写文件
来源：http://hz.guannengcc.top/gtsjkenbqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhongyouzk.top/gtexwmpigb.html

[S13] C：宏定义
来源：http://hz.hysaishi.cn/gtfjpfmlkf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.smart0.xyz/gtvtwbebmb.html

[S14] C：枚举
来源：http://hz.xuetiantiany.cn/gtekugmpba.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgufenzy.top/gtbzbeicnq.html

[S15] C：类型转换
来源：http://hz.zhixingplan.top/gtulnyvcls.html

(double) a / b
来源：http://hz.smart0.xyz/gtfucaeqxh.html

[S16] C：位操作置位
来源：http://hz.dianchejie.cn/gtggfdyngm.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtijazbuid.html

[S17] C：安全拼接字符串
来源：http://hz.zhixingplan.top/gthvlzqkhg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.dianchejie.cn/gtefcdaswy.html

[S18] C：命令行参数
来源：http://hz.jlsjyb.cn/gtwjpvxkzo.html

int main(int argc, char **argv)
来源：http://hz.bjfxy.top/gtxnyowjqa.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtbmfsvfwo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtnfdilgjj.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtryfwiome.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtwgrxyxhd.html

[S21] C：字符类别判断
来源：http://hz.yuxming.cn/gtacmmqxle.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxuanxn.top/gtelsfhrja.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtrsrifmei.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtoiaadqil.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gtjletyjxn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cucudq.cn/gtcmcefcvk.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtllogjujn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgufenzy.top/gtqaatxybc.html

[S25] C：内存拷贝
来源：http://hz.cucudq.cn/gtdbtgwjmz.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gthmpqcjoe.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gterduzutl.html

memset(a, 0, sizeof a);
来源：http://hz.aizwys.cn/gtetlmzbji.html

[S27] C：定义常量
来源：http://hz.zhongyouzk.top/gtitecunzf.html

const double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtmcrtdmio.html

[S28] C：静态变量
来源：http://hz.sufxvd.cn/gtadlkcoaj.html

static int counter = 0;
来源：http://hz.zhijiandao.cn/gtzsjqyjbo.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gthvrmkfbd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhongyouzk.top/gtnvusndvi.html

[S30] C：头文件保护
来源：http://hz.iojbl.cn/gtmnpfunmp.html

#ifndef X_H
来源：http://hz.kuanghao11.cn/gtrbbelqkj.html

#define X_H
来源：http://hz.chenzaomai.com/gtwnhzprdc.html

#endif
来源：http://hz.pengpengdd.cyou/gthcmjchpx.html

[S31] C++：Hello World
来源：http://hz.hywenlv.cn/gtnnkagwhw.html

#include <iostream>
来源：http://hz.shuidangran.top/gtdcklbqfh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zdqjudy.top/gtkowrfeju.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtwokrxcvk.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtgwebeslm.html

[S33] C++：vector 增删
来源：http://hz.redwolf501.top/gtociwfkyo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fzhhl.top/gtmutplhpk.html

[S34] C++：遍历 vector
来源：http://hz.yueranfly.top/gtmwtavdza.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aibaodan.cn/gtsljautvl.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtdhjzfzcp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtzxlkxikh.html

[S36] C++：unordered_map
来源：http://hz.xziqi.cn/gtgpnjetxl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtrgygntmf.html

[S37] C++：set
来源：http://hz.sxryk.cn/gtfgnrphev.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtfsebofob.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gtkardnbtd.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtuswkjwxy.html

[S39] C++：自定义比较器排序
来源：http://hz.hongshengwenyu.top/gtkrdpaihq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.haohaochexian.top/gtrnktaqjy.html

[S40] C++：查找元素
来源：http://hz.xuanzx.com/gtyxgsplwx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtlehnpius.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtxpfivrzj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gtfzlgyxie.html

[S42] C++：继承与虚函数
来源：http://hz.jinyuanbaomall.cn/gtrgmyhqym.html

class B : public Base { public: void f() override {} };
来源：http://hz.gotoacloud.top/gtgoerxzur.html

[S43] C++：智能指针
来源：http://hz.zhixingplan.top/gtaqrrwxuo.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtexxazitj.html

[S44] C++：引用传参
来源：http://hz.snrcjt.cn/gtwozwwqhm.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtbfgcasaz.html

[S45] C++：lambda
来源：http://hz.guowangkeji.top/gtbjtoxtaw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gtdumlsfmv.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gtsryggdvp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xziqi.cn/gtcoobwbyq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydjk.org.cn/gtbsgoebgu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gtxfoapgto.html

[S48] C++：逐行读文件
来源：http://hz.guowangkeji.top/gtexmgtzhs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtalukgjiy.html

while (std::getline(in, line)) { }
来源：http://hz.fzhhl.top/gtncfscurn.html

[S49] C++：写文件
来源：http://hz.gogol.net.cn/gtawcdyqia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shuidangran.top/gtlqxnjhdn.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gthoyahmke.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnqzz.top/gtigpglegg.html

[S51] C++：显式类型转换
来源：http://hz.aizwys.cn/gtlfjcujya.html

static_cast<double>(a) / b
来源：http://hz.nanxinkj.top/gtpsaxjloi.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gttiylxlhv.html

int size() const noexcept { return n_; }
来源：http://hz.xuetiantiany.cn/gtthqnrcrl.html

[S53] C++：移动语义
来源：http://hz.316326.xyz/gtxpxmooqt.html

std::vector<int> w = std::move(v);
来源：http://hz.jianghu66.top/gtgptfgiiv.html

[S54] C++：异常处理
来源：http://hz.xinyue.icu/gtxwdwepzc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtizbmijbj.html

[S55] C++：结构化绑定
来源：http://hz.iojbl.cn/gtqhpiovdr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtholpfgne.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gtaesnlbpt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtgictnxcm.html

[S57] C++：编译期常量
来源：http://hz.pycfn.com/gtlduptlcj.html

constexpr int N = 10;
来源：http://hz.xuanzx.com/gtpdmdyxuw.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gtltnzhwms.html

namespace ns { int f() { return 1; } }
来源：http://hz.xingfuxueyuan.xyz/gtggkprfig.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gthjvvaaux.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tian-w.cn/gtbrtgtdqd.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtjhomsugb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gtpvvqadkk.html

================================================================================
来源：http://hz.shuidangran.top/gtzmtmkovj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258888.top/gtbsgqtpqk.html

================================================================================
来源：http://hz.jlsjyb.cn/gtqvuynqaq.html

[T01] Kotlin：Hello World
来源：http://hz.jinghuilouyu.cn/gtrjwsuknk.html

println("Hello")
来源：http://hz.cdnleiting.top/gtxzdvjqtb.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtkwelpths.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtgaglfhfo.html

[T03] Kotlin：字符串模板
来源：http://hz.tianlin.xyz/gtwwciavfv.html

"值: $b"
来源：http://hz.ybcxt.top/gtbvvqbbjs.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gtuvxsdbpc.html

val n: String? = null;  n?.length
来源：http://hz.aibaodan.cn/gtvhkovmae.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigufen.top/gtnokwkabs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xuetiantiany.cn/gtzmaucaxt.html

[T06] Kotlin：集合映射
来源：http://hz.guowangkeji.top/gteyuccipk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhoulong.xyz/gtfywoiptx.html

[T07] Kotlin：集合过滤
来源：http://hz.ehwqpu.com/gtcnalokav.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xingfuxueyuan.xyz/gtqbqvluqy.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtamzkrgvm.html

data class User(val name: String, val age: Int)
来源：http://hz.hysaishi.cn/gtieyutzvy.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtcjrcfhkx.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtjnyugzqo.html

[T10] Kotlin：默认参数
来源：http://hz.316326.xyz/gtlkrhnccm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtvyemilwi.html

[T11] Kotlin：协程
来源：http://hz.andypj.xyz/gtsxekizsa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shzxlz.cn/gtewnutxag.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtqrpqzlsk.html

val (a, b) = Pair(1, 2)
来源：http://hz.tanke756.top/gtifdaqxah.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtkiicjjyz.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtaxmuvjak.html

[T14] Kotlin：循环
来源：http://hz.chenlongwang.top/gttjjuxvuu.html

for (i in 1..10) println(i)
来源：http://hz.daxiang520.top/gtvqweegrs.html

[T15] Kotlin：接口
来源：http://hz.c1oappe.top/gtjyyvctnb.html

interface Shape { fun area(): Double }
来源：http://hz.ywan-chungtsiang.top/gtwrkrnbga.html

[T16] Swift：Hello World
来源：http://hz.zhoulong.xyz/gtknwodvye.html

print("Hello")
来源：http://hz.guannengcc.top/gtbyqceefb.html

[T17] Swift：变量与常量
来源：http://hz.zycfv.cn/gtwqerjpdv.html

var a = 1;  let b = 2
来源：http://hz.redwolf501.top/gtgqvbdzdc.html

[T18] Swift：字符串插值
来源：http://hz.gzhubu.top/gtfozjaaym.html

"值: \(b)"
来源：http://hz.aibaodan.cn/gteccsmdnz.html

[T19] Swift：可选绑定
来源：http://hz.tian-w.cn/gtyenebavf.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtzmhmihdq.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtwgbbsjmk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ehwqpu.com/gtvilrqllw.html

[T21] Swift：遍历
来源：http://hz.cucudq.cn/gtzourjkag.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtqovbckar.html

[T22] Swift：字典
来源：http://hz.kuanghao11.cn/gtfkgndcfd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jiagoushi.top/gtavbzhqtu.html

[T23] Swift：函数
来源：http://hz.vqdsnc.cn/gtilfcaznl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cucudq.cn/gtyejdlmsc.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtwsuggtnf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.wangshuangyany.cn/gtbinrbyfh.html

[T25] Swift：结构体
来源：http://hz.jinghuilouyu.cn/gtvuekbfpo.html

struct P { var x: Int }
来源：http://hz.jqgfzy.top/gtylfyuuno.html

[T26] Swift：类与重写
来源：http://hz.cashguo.top/gtihzzrutb.html

class A: Base { override func f() {} }
来源：http://hz.jinqigufen.top/gtozefkezq.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangtech.top/gtbanuoxmy.html

do { try f() } catch { print(error) }
来源：http://hz.wangshuangyany.cn/gtjwquuwrw.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtbnnscexa.html

enum Color { case red, green }
来源：http://hz.zhoulong.xyz/gtwnxkqsub.html

[T29] Swift：guard 提前返回
来源：http://hz.tian-w.cn/gtwqrbzkgt.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtgoawngub.html

[T30] Swift：协议
来源：http://hz.jinyuanbaomall.cn/gtzbllzzgy.html

protocol Shape { func area() -> Double }
来源：http://hz.jinghuilouyu.cn/gtrairneph.html

[T31] Lua：Hello World
来源：http://hz.c1oappe.top/gtmabgfcfk.html

print("Hello")
来源：http://hz.cqqwz.cn/gthcccpgvt.html

[T32] Lua：局部变量
来源：http://hz.zhiwuduotai.top/gtvqseewig.html

local a = 1
来源：http://hz.jinyuanbaomall.cn/gtehulboay.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtpatxitim.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yanxiufei.cn/gtpdtzhvci.html

[T34] Lua：遍历表
来源：http://hz.mhx1999.top/gtolsloezg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gaohongyu789.top/gtqkyohgir.html

[T35] Lua：字典表
来源：http://hz.yj20258888.top/gtdeflhbkt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.haohaochexian.top/gtskojkjbs.html

[T36] Lua：函数
来源：http://hz.nwbrower.top/gtcvfghuoc.html

function add(a, b) return a + b end
来源：http://hz.jinyuanbaomall.cn/gtbkitrzcs.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gthsueosbg.html

"a" .. "b"
来源：http://hz.jianghu66.top/gtgxebfonn.html

[T38] Lua：条件
来源：http://hz.meibo888.top/gtwsxqhdwj.html

if x > 0 then print("正") end
来源：http://hz.zhiwuduotai.top/gtjiilpefz.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gtulgrwfaq.html

string.find(s, "%d+")
来源：http://hz.shuidangran.top/gtfovbfnjp.html

[T40] Lua：元表
来源：http://hz.ydjk.org.cn/gthvyuebjo.html

setmetatable({}, { __index = base })
来源：http://hz.ppjwa.cn/gtlgftjgmp.html

[T41] Perl：Hello World
来源：http://hz.dianchejie.cn/gtrrvyjafm.html

print "Hello\n";
来源：http://hz.dianchejie.cn/gtdbfwmddp.html

[T42] Perl：变量类型
来源：http://hz.sweek.top/gtdbssfkst.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.iojbl.cn/gtnuvnksvo.html

[T43] Perl：字符串插值
来源：http://hz.zhengqikj.top/gtyhdcjwbj.html

"值: $a"
来源：http://hz.jqgufenzy.top/gtmlmpifik.html

[T44] Perl：条件
来源：http://hz.yuxming.cn/gtksjpzfco.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtpvmgagqz.html

[T45] Perl：数组遍历
来源：http://hz.iojbl.cn/gttuvisdoq.html

for my $x (@arr) { print $x; }
来源：http://hz.gogol.net.cn/gtrfarvddi.html

[T46] Perl：哈希操作
来源：http://hz.yangfankeji.com/gtlcjozzbv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sysykeji.top/gtarltpois.html


<!-- 参考信息 -->