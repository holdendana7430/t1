代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangkeji.top/gtubvmxruh.html

[R52] 统计行数
来源：http://hz.yongpay.top/gtiygmekvn.html

wc -l a.txt
来源：http://hz.jianghu66.top/gtpqghswup.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtokvoscfz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sysykeji.top/gtpbuxydqt.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtlkljccsd.html

diff a.txt b.txt
来源：http://hz.kuanghao11.cn/gterrsjxrn.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtqoicdvzj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.haohaochexian.top/gtsgabhbuo.html

[R56] 远程拷贝
来源：http://hz.zhengqikj.top/gtxgnqoama.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtcfqdhyoe.html

[R57] 远程执行命令
来源：http://hz.smart0.xyz/gtxwiablgu.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gthuyzhmsj.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtoxkamnen.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gtlpyvrhxa.html

[R59] 发 POST JSON
来源：http://hz.jianghu66.top/gtpaneoahm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zycfv.cn/gtuzkrieak.html

[R60] 只看 HTTP 状态码
来源：http://hz.xinyue.icu/gtikokaqqc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.mhx1999.top/gtjrsaxnwi.html

[R61] 磁盘占用
来源：http://hz.zhaomingkeji.xyz/gtapsuqrtm.html

df -h;  du -sh *
来源：http://hz.xuetiantiany.cn/gtwjvcfozc.html

[R62] 找最占空间的文件
来源：http://hz.hfpthk.cn/gtogavqqdt.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gthfobwtbp.html

[R63] 内存与进程
来源：http://hz.tianlin.xyz/gtlmbmwotn.html

free -h;  ps aux | grep nginx
来源：http://hz.xuetiantiany.cn/gtyftfwaav.html

[R64] 结束进程
来源：http://hz.hywenlv.cn/gtjwnrvlct.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gtzqaiiydx.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtaqadbowq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sweek.top/gtdtapwxfj.html

[R66] 定时任务
来源：http://hz.havefunace.top/gtbpncoeah.html

crontab -e;  crontab -l
来源：http://hz.tanke756.top/gtplqipnqt.html

[R67] 生成随机十六进制串
来源：http://hz.fzhhl.top/gthqiycqlh.html

openssl rand -hex 16
来源：http://hz.zhiwuduotai.top/gtepaabvpg.html

[R68] 计算文件校验值
来源：http://hz.aizwys.cn/gthetxpxez.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.haohaochexian.top/gttbqzyvbw.html

[R69] 生成随机密码
来源：http://hz.52xcode.cn/gtkxtgbkco.html

head -c 16 /dev/urandom | base64
来源：http://hz.guowangkeji.top/gtdijmhinl.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtjppuzrml.html

date +%s;  date -d @1700000000
来源：http://hz.zhiwuduotai.top/gtchsuolfi.html

[R71] 日期格式化
来源：http://hz.9152youxi.cn/gtlwrbwiyo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yvedp.cn/gtpvvlswjd.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtqfpdcvjf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fengsongda.top/gtmpihucsu.html

[R73] 分割大日志
来源：http://hz.yvedp.cn/gtbvdenims.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtaqbwvfpd.html

[R74] 批量重命名
来源：http://hz.sysykeji.top/gtytzpbfns.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ybcxt.top/gtcfgqyequ.html

[R75] 导出环境变量
来源：http://hz.cqqwz.cn/gtcdwnqqii.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtuklzekfl.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gtpkvlosbl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtpguotivm.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtimujifcu.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gtfrhyfpqr.html

[R78] 交互式菜单
来源：http://hz.dianchejie.cn/gtodehovdw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinyuanbaomall.cn/gtikekubit.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtwffqcdgw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gtupvbojlz.html

[R80] 查看脚本执行耗时
来源：http://hz.bjfxy.top/gthsnxihif.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtpzntmcck.html

================================================================================
来源：http://hz.iojbl.cn/gtvpegxyzh.html

S. C / C++ 专题
来源：http://hz.yj20258888.top/gtlvxllcfg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwlnxuhsu.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gtxbcgygmm.html

#include <stdio.h>
来源：http://hz.yonumen.top/gtbeeokmcv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sweek.top/gtixrsfgmv.html

[S02] C：变量与格式化输出
来源：http://hz.cashguo.top/gtpzjmqyxf.html

int a = 10; printf("%d\n", a);
来源：http://hz.tian-w.cn/gtnnqzenge.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gthsgicsxr.html

int x; scanf("%d", &x);
来源：http://hz.sufxvd.cn/gtabovqegd.html

[S04] C：字符串复制
来源：http://hz.snrcjt.cn/gtpslhzczh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.wangshuangyany.cn/gtakcwcknp.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtomtpixhq.html

strlen(s)
来源：http://hz.yuanzhike.top/gtqprwjcjl.html

[S06] C：字符串比较
来源：http://hz.daria6918.cn/gtrlqmvbyd.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtpuhmgvuj.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtishdqsvb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj202588.top/gtpjuqfnit.html

[S08] C：动态内存分配与释放
来源：http://hz.xuetiantiany.cn/gthcjtbgjr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtsyhchgwg.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gtiiekvisq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gtgvnmwmlg.html

[S10] C：指针与解引用
来源：http://hz.chenlongwang.top/gtmcpoozvt.html

int *p = &a;  *p = 5;
来源：http://hz.bjfxy.top/gtmvjzsczd.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtrgazqxrh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigfzy.top/gtrropffhd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxinkj.top/gtogmzjrqx.html

fclose(f);
来源：http://hz.sufxvd.cn/gtmehylaxj.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtzwibgkts.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gthdtsngmc.html

[S13] C：宏定义
来源：http://hz.shzxlz.cn/gtwlafxgjz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtkcifnmod.html

[S14] C：枚举
来源：http://hz.yj20258888.top/gtglajhjyr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinyuanbaomall.cn/gtbhymqygr.html

[S15] C：类型转换
来源：http://hz.zhixingplan.top/gtnsagrmrd.html

(double) a / b
来源：http://hz.hammf.cn/gtljvnfwvy.html

[S16] C：位操作置位
来源：http://hz.yanxiufei.cn/gtxivlfmlb.html

x |= (1 << 3);
来源：http://hz.cdnleiting.top/gtfgohkhzz.html

[S17] C：安全拼接字符串
来源：http://hz.mhx1999.top/gttwahlkem.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gthlxefflm.html

[S18] C：命令行参数
来源：http://hz.tanke756.top/gtlqfssrli.html

int main(int argc, char **argv)
来源：http://hz.redwolf501.top/gtvgjesvln.html

[S19] C：快速排序
来源：http://hz.ppjwa.cn/gthbgspfmm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtxwvzblkz.html

[S20] C：二分查找
来源：http://hz.nwbrower.top/gttfjqzhoc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gtfxynkzax.html

[S21] C：字符类别判断
来源：http://hz.yanxiufei.cn/gtgnsbnxwi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtlhmbkgzb.html

[S22] C：字符串转数字
来源：http://hz.52xcode.cn/gthtefvjwb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gtkjjhzezk.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtohwwixnf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.0kj1m.cn/gtowargwvb.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtlppykdrs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shzxlz.cn/gtmadvggmt.html

[S25] C：内存拷贝
来源：http://hz.ppjwa.cn/gtmnwgzepy.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtadladpeo.html

[S26] C：内存清零
来源：http://hz.cucudq.cn/gtfmsovtkr.html

memset(a, 0, sizeof a);
来源：http://hz.ppjwa.cn/gtyricfrty.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtzqepayhd.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtndlqdkxt.html

[S28] C：静态变量
来源：http://hz.hnqzz.top/gtlvmpyftw.html

static int counter = 0;
来源：http://hz.gzhubu.top/gtojstzuyp.html

[S29] C：变参函数
来源：http://hz.zhengqikj.top/gtpmzxglmn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shzxlz.cn/gtebbtzwaz.html

[S30] C：头文件保护
来源：http://hz.nanxinkj.top/gtlnwnqtfv.html

#ifndef X_H
来源：http://hz.yanxiufei.cn/gtznurbzrk.html

#define X_H
来源：http://hz.cheryme.top/gtgertjnzp.html

#endif
来源：http://hz.wangshuangyany.cn/gtyyextdrc.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtizvqnfcu.html

#include <iostream>
来源：http://hz.cdnleiting.top/gterdixrac.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gotoacloud.top/gtyyrbsgco.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtuoxlwgej.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtmxdusiza.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtbaqaswdi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xziqi.cn/gtgyrfjisb.html

[S34] C++：遍历 vector
来源：http://hz.pengpengdd.cyou/gtwudkerzm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtzqtgkzuq.html

[S35] C++：map
来源：http://hz.cashguo.top/gtruhrgxku.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtxdidfdri.html

[S36] C++：unordered_map
来源：http://hz.jyoumei.cn/gtnjecwpyl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtfgsxwfci.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtipcyepzr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cucudq.cn/gtwiszwrie.html

[S38] C++：排序
来源：http://hz.hnxiangtu.top/gtgvpswduz.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtxlsckfnn.html

[S39] C++：自定义比较器排序
来源：http://hz.yanxiufei.cn/gtcvuchffc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gttukvahfk.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtkscidrbw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hysaishi.cn/gtmtwzczfc.html

[S41] C++：类与构造函数
来源：http://hz.jyoumei.cn/gtibnlslxz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gtjoscuhtx.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtyxfxpvlp.html

class B : public Base { public: void f() override {} };
来源：http://hz.aizwys.cn/gtphvrljlk.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangkeji.top/gtzhjlrtfa.html

auto p = std::make_unique<int>(5);
来源：http://hz.gaohongyu789.top/gtzniopmgk.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtbdlrxpig.html

void inc(int &x) { ++x; }
来源：http://hz.tianlin.xyz/gtgcaixuwi.html

[S45] C++：lambda
来源：http://hz.jiagoushi.top/gtdhgpgnyx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtosxvkrph.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gtmrljjftc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pycfn.com/gtcoqiztqz.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtlqszzcwk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cdnleiting.top/gtsvmikuei.html

[S48] C++：逐行读文件
来源：http://hz.aizwys.cn/gtsgvltlxt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtwqtknvvg.html

while (std::getline(in, line)) { }
来源：http://hz.snrcjt.cn/gtkwfttlgu.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtnjioutbh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.wangshuangyany.cn/gtagberegq.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtbahpwmve.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtfrezvrkg.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtfiqafgpu.html

static_cast<double>(a) / b
来源：http://hz.jinqigufen.top/gtfujklmsa.html

[S52] C++：const 与 noexcept
来源：http://hz.jyoumei.cn/gtlpaqwubk.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtlojvfida.html

[S53] C++：移动语义
来源：http://hz.hywenlv.cn/gthbskuvsw.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtzlicsupi.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtqujivhgi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sysykeji.top/gtfottzwxi.html

[S55] C++：结构化绑定
来源：http://hz.hnqzz.top/gtvciugwwx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhiwuduotai.top/gtpzgltsex.html

[S56] C++：optional
来源：http://hz.c1oappe.top/gtzbyfsdtu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yongpay.top/gtimwfpqtd.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtqkrbplrm.html

constexpr int N = 10;
来源：http://hz.yanxiufei.cn/gtdwxotyom.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtcbwusioo.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhiwuduotai.top/gtwbugpwvk.html

[S59] C++：静态断言
来源：http://hz.pengpengdd.cyou/gteyyfcrso.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zdqjudy.top/gttxxytyxe.html

[S60] C++：遍历并删除元素
来源：http://hz.bjfxy.top/gtdmzcyzcv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.meibo888.top/gtjrdfgpyy.html

================================================================================
来源：http://hz.sufxvd.cn/gtruqismfj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aizwys.cn/gtdearrjky.html

================================================================================
来源：http://hz.iojbl.cn/gtdshixyvc.html

[T01] Kotlin：Hello World
来源：http://hz.guowangkeji.top/gtruwsjnmc.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtvekwthrr.html

[T02] Kotlin：变量
来源：http://hz.gzhubu.top/gtykrfylqa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtchhghhyf.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258888.top/gtvkjqsvvr.html

"值: $b"
来源：http://hz.kuanghao11.cn/gtexrwprbs.html

[T04] Kotlin：空安全
来源：http://hz.jiagoushi.top/gtyrcjlpyr.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtdkiibkzn.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtzygqkpbs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dashuyun.cn/gtrynmtdic.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtlktzbbyj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtzyeetphy.html

[T07] Kotlin：集合过滤
来源：http://hz.yueranfly.top/gthyilmrhj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtizechdbx.html

[T08] Kotlin：数据类
来源：http://hz.ivvv.top/gtawzwvhod.html

data class User(val name: String, val age: Int)
来源：http://hz.meibo888.top/gtwhltgkpw.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtfmzcqebw.html

fun String.exclaim() = this + "!"
来源：http://hz.jianghu66.top/gtntzekptl.html

[T10] Kotlin：默认参数
来源：http://hz.chenlongwang.top/gtbwwymkkv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gotoacloud.top/gtnkuvolwn.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gtkkocwsfc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cucudq.cn/gtdzsavjun.html

[T12] Kotlin：解构声明
来源：http://hz.yueranfly.top/gtcuircgsw.html

val (a, b) = Pair(1, 2)
来源：http://hz.daria6918.cn/gthuwgsxfq.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258888.top/gtdrljvfld.html

val m = mapOf("a" to 1)
来源：http://hz.fzhhl.top/gtitxknsft.html

[T14] Kotlin：循环
来源：http://hz.9152youxi.cn/gteyyzewmv.html

for (i in 1..10) println(i)
来源：http://hz.gotoacloud.top/gtuzqrpzep.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtwfquneff.html

interface Shape { fun area(): Double }
来源：http://hz.c1oappe.top/gtuxyctnhl.html

[T16] Swift：Hello World
来源：http://hz.jyoumei.cn/gtlpaupnef.html

print("Hello")
来源：http://hz.birdmap.top/gtcwrxnriw.html

[T17] Swift：变量与常量
来源：http://hz.haohaochexian.top/gtmqhnnnts.html

var a = 1;  let b = 2
来源：http://hz.wangdashe.top/gtdvzitlnw.html

[T18] Swift：字符串插值
来源：http://hz.hysaishi.cn/gtrsdvauwt.html

"值: \(b)"
来源：http://hz.52xcode.cn/gtyssfsvom.html

[T19] Swift：可选绑定
来源：http://hz.hnxiangtu.top/gtgkhdurpl.html

if let n = opt { print(n) }
来源：http://hz.yuanzhike.top/gtbqsjjegf.html

[T20] Swift：数组操作
来源：http://hz.hysaishi.cn/gtrfvnllkn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yangfankeji.com/gtzlmejntx.html

[T21] Swift：遍历
来源：http://hz.vqdsnc.cn/gtnrjccizq.html

for x in a { print(x) }
来源：http://hz.xuetiantiany.cn/gtexhozicc.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtjzkzepdh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj20258888.top/gtdoqdhksi.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtjlamgqee.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtjzkbhrgr.html

[T24] Swift：闭包
来源：http://hz.hnqzz.top/gtxkomvpzv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gtwwbcgbwt.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtfcaemgmf.html

struct P { var x: Int }
来源：http://hz.mhx1999.top/gtlzikzidk.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtebuqhvmf.html

class A: Base { override func f() {} }
来源：http://hz.gogol.net.cn/gtxbftoqus.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtedneoclh.html

do { try f() } catch { print(error) }
来源：http://hz.hysaishi.cn/gtgtmxyecl.html

[T28] Swift：枚举
来源：http://hz.zhijiandao.cn/gtkaflczmv.html

enum Color { case red, green }
来源：http://hz.sysykeji.top/gtckptrgba.html

[T29] Swift：guard 提前返回
来源：http://hz.pengpengdd.cyou/gtbjgdslwl.html

guard let x = opt else { return }
来源：http://hz.snrcjt.cn/gtueuayixw.html

[T30] Swift：协议
来源：http://hz.zhijiandao.cn/gtijxtgppx.html

protocol Shape { func area() -> Double }
来源：http://hz.yonumen.top/gtvnvtjniz.html

[T31] Lua：Hello World
来源：http://hz.shzxlz.cn/gttxbabctk.html

print("Hello")
来源：http://hz.shzxlz.cn/gtpkestqok.html

[T32] Lua：局部变量
来源：http://hz.jqgufenzy.top/gtexxvklol.html

local a = 1
来源：http://hz.andypj.xyz/gtcqwyrtbs.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangkeji.top/gtiohaekwm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.smart0.xyz/gtapkotqoj.html

[T34] Lua：遍历表
来源：http://hz.yuanzhike.top/gtvhuqsnzx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ivvv.top/gtkekxcrva.html

[T35] Lua：字典表
来源：http://hz.tanke756.top/gthpolieri.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gtkczcrjqs.html

[T36] Lua：函数
来源：http://hz.shanyushiyangtech.top/gtspsqxyrz.html

function add(a, b) return a + b end
来源：http://hz.tanke756.top/gtpcxldrgl.html

[T37] Lua：字符串拼接
来源：http://hz.andypj.xyz/gtgyjbemrd.html

"a" .. "b"
来源：http://hz.zhaomingkeji.xyz/gtixjnirmn.html

[T38] Lua：条件
来源：http://hz.hongshengwenyu.top/gtnsuuezrz.html

if x > 0 then print("正") end
来源：http://hz.hammf.cn/gthjwgooyc.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtpgenmyyn.html

string.find(s, "%d+")
来源：http://hz.wangshuangyany.cn/gtxxnffmri.html

[T40] Lua：元表
来源：http://hz.c1oappe.top/gtwguidolw.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtcmcsnfqh.html

[T41] Perl：Hello World
来源：http://hz.zhoulong.xyz/gtklzkjofq.html

print "Hello\n";
来源：http://hz.yvedp.cn/gtsznopgxk.html

[T42] Perl：变量类型
来源：http://hz.yj20258888.top/gtyixenubd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ydjk.org.cn/gtjoptnigl.html

[T43] Perl：字符串插值
来源：http://hz.daxiang520.top/gtrviaxixb.html

"值: $a"
来源：http://hz.yanxiufei.cn/gtqbmwwjmk.html

[T44] Perl：条件
来源：http://hz.nanxuanxn.top/gtsfycbmhs.html

if ($a > 0) { print "正"; }
来源：http://hz.ydzc1.top/gtngwiemta.html

[T45] Perl：数组遍历
来源：http://hz.dashuyun.cn/gtpaaojphf.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtrlmozqys.html

[T46] Perl：哈希操作
来源：http://hz.tanke756.top/gtqfuetpqu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinyuanbaomall.cn/gtoaoiweyp.html

[T47] Perl：正则捕获
来源：http://hz.cucudq.cn/gtmphlqess.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinghuilouyu.cn/gtcnammrxn.html

[T48] Perl：正则替换
来源：http://hz.feifeiyinyue.top/gtdykjawcg.html

$s =~ s/old/new/g;
来源：http://hz.hammf.cn/gttizmouoq.html

[T49] Perl：函数
来源：http://hz.zhaomingkeji.xyz/gtdzyhnzvp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj202588.top/gtnhyfpvpf.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtyvtickoc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jyoumei.cn/gtdjzkhasl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daria6918.cn/gtxofloqov.html

[T51] Scala：Hello World
来源：http://hz.dashuyun.cn/gtsgwevwbp.html

println("Hello")
来源：http://hz.sufxvd.cn/gtbvwssajx.html

[T52] Scala：变量
来源：http://hz.jqgfzy.top/gtlhgipron.html

val a = 1;  var b = 2
来源：http://hz.ybcxt.top/gtkelnrayd.html

[T53] Scala：字符串插值
来源：http://hz.zycfv.cn/gtoilfoqit.html

s"值: $b"
来源：http://hz.9152youxi.cn/gtoxlulaik.html

[T54] Scala：集合映射
来源：http://hz.aibaodan.cn/gtezivmezc.html


<!-- 参考信息 -->