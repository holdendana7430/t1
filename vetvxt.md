代发 wailian999

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtqlhqkqcq.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtrcityqxr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuanzhike.top/gtapqziryh.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gtftqclpnh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtisuxfgdu.html

[R60] 只看 HTTP 状态码
来源：http://hz.haohaochexian.top/gtegrjnlte.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dianchejie.cn/gtzpsznpsb.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtixpwxoki.html

df -h;  du -sh *
来源：http://hz.c1oappe.top/gtckodsfsg.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gtytvzostl.html

du -ah . | sort -rh | head -10
来源：http://hz.0kj1m.cn/gtmrdcbfuf.html

[R63] 内存与进程
来源：http://hz.zhoulong.xyz/gtqftnocrj.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtubjyabbh.html

[R64] 结束进程
来源：http://hz.xylfe.cn/gtyfmkqwin.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtlnyakked.html

[R65] 查看端口占用
来源：http://hz.guannengcc.top/gtbsdfnsap.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtclvwdnzg.html

[R66] 定时任务
来源：http://hz.yongpay.top/gtooehvqch.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtsfiimlgp.html

[R67] 生成随机十六进制串
来源：http://hz.xinyue.icu/gtclkeolsr.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtpfvntkke.html

[R68] 计算文件校验值
来源：http://hz.nanxuanxn.top/gtqpfavenf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtbpkwzdmz.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gtlsjrzhte.html

head -c 16 /dev/urandom | base64
来源：http://hz.birdmap.top/gtppxvexbw.html

[R70] 时间戳与互转
来源：http://hz.yongpay.top/gtzoyadewz.html

date +%s;  date -d @1700000000
来源：http://hz.gaohongyu789.top/gtzhzryryy.html

[R71] 日期格式化
来源：http://hz.yongpay.top/gtoihnsujy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shuidangran.top/gtzfrjwuce.html

[R72] 等待端口就绪
来源：http://hz.yuanzhike.top/gttnujfanz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtlgvznzik.html

[R73] 分割大日志
来源：http://hz.pycfn.com/gtjjyciujz.html

split -l 1000 big.log part_
来源：http://hz.cdnleiting.top/gtwjpftuyg.html

[R74] 批量重命名
来源：http://hz.aizwys.cn/gtykicwial.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fzhhl.top/gtrbbaayqg.html

[R75] 导出环境变量
来源：http://hz.guowangkeji.top/gtoemfstig.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hysaishi.cn/gtnbldjzgq.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtllxqqfyw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtyqpbixrn.html

[R77] 读取用户输入
来源：http://hz.zhijiandao.cn/gtjeioxtdo.html

read -rp "请输入: " ans
来源：http://hz.jiagoushi.top/gtnsxgghpq.html

[R78] 交互式菜单
来源：http://hz.tanke756.top/gtqiqtarqk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aizwys.cn/gtwcaqzcvx.html

[R79] 解析命令行选项
来源：http://hz.yj20258888.top/gttgpuwxmz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sxryk.cn/gthudrpicl.html

[R80] 查看脚本执行耗时
来源：http://hz.mhx1999.top/gtsnsrxdiy.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtjcgovrww.html

================================================================================
来源：http://hz.yvedp.cn/gtbmogzaiq.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtpihnbeoq.html

================================================================================
来源：http://hz.hysaishi.cn/gtqbslszci.html

[S01] C：Hello World
来源：http://hz.hysaishi.cn/gtrkeyfhpo.html

#include <stdio.h>
来源：http://hz.hammf.cn/gtakvqpbrt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtxqnjnltg.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gtslnziquy.html

int a = 10; printf("%d\n", a);
来源：http://hz.hywenlv.cn/gtmitbhldo.html

[S03] C：读入整数
来源：http://hz.tian-w.cn/gtfsqcyfks.html

int x; scanf("%d", &x);
来源：http://hz.hywenlv.cn/gtzdfcrglw.html

[S04] C：字符串复制
来源：http://hz.jinghuilouyu.cn/gtttbrbcgq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtypujunvz.html

[S05] C：字符串长度
来源：http://hz.52xcode.cn/gtuhlykuif.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtpfuayfyc.html

[S06] C：字符串比较
来源：http://hz.ehwqpu.com/gtaikgjqpv.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtfglznrfq.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtqsecngan.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangshuangyany.cn/gtcgcpnamj.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtcrqkqnuf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.iojbl.cn/gthkcsetaa.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gterdotxfs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hywenlv.cn/gtsrpealot.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtuzuwsdyl.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtrvfhhmky.html

[S11] C：逐行读文件
来源：http://hz.jinqigfzy.top/gtvpizcece.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gtqbqjhcvl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fengsongda.top/gtegbxejrc.html

fclose(f);
来源：http://hz.tian-w.cn/gtcrnrgdhw.html

[S12] C：写文件
来源：http://hz.guannengcc.top/gteedqznyp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xylfe.cn/gtixstdcrk.html

[S13] C：宏定义
来源：http://hz.zhiwuduotai.top/gtzfbvzlpb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.quarkkingdee.top/gthhrspkiy.html

[S14] C：枚举
来源：http://hz.guannengcc.top/gtrxfyetpe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258.top/gtuxudfnto.html

[S15] C：类型转换
来源：http://hz.nanxinkj.top/gtfktorgpr.html

(double) a / b
来源：http://hz.zhongyouzk.top/gtfsrdeqjm.html

[S16] C：位操作置位
来源：http://hz.aibaodan.cn/gtxsjzmwjl.html

x |= (1 << 3);
来源：http://hz.c1oappe.top/gtpvjxwxmp.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtsrfjsulv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnqzz.top/gttgdhkelk.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtmsqcsghh.html

int main(int argc, char **argv)
来源：http://hz.birdmap.top/gtmgeeeebe.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtzvkpthqu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtivrctubl.html

[S20] C：二分查找
来源：http://hz.zhengqikj.top/gtyqiylufi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtgskxvgvc.html

[S21] C：字符类别判断
来源：http://hz.dianchejie.cn/gtewvwnutl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zycfv.cn/gtxnjcekkr.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtpoznfdyi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ppjwa.cn/gtczajfbim.html

[S23] C：随机数
来源：http://hz.dashuyun.cn/gtsbjhneeu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sufxvd.cn/gtfqogktpi.html

[S24] C：获取本地时间
来源：http://hz.zhixingplan.top/gtygcfisqw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gaohongyu789.top/gtqxmxsnwt.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gteohxdqyx.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtxeqnkbug.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtwvvrvfwf.html

memset(a, 0, sizeof a);
来源：http://hz.yvedp.cn/gtdyfiqqki.html

[S27] C：定义常量
来源：http://hz.ppjwa.cn/gtzfbsalqy.html

const double PI = 3.14159;
来源：http://hz.havefunace.top/gtjhbacvyy.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gtefwgjrik.html

static int counter = 0;
来源：http://hz.iojbl.cn/gtgkdatjwh.html

[S29] C：变参函数
来源：http://hz.andypj.xyz/gtexkdsbls.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgufenzy.top/gtjvncksoh.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtbitmsbdz.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtzgsyniar.html

#define X_H
来源：http://hz.tanke756.top/gtlbfcvtja.html

#endif
来源：http://hz.birdmap.top/gtcnbtwlui.html

[S31] C++：Hello World
来源：http://hz.wangshuangyany.cn/gtihrocask.html

#include <iostream>
来源：http://hz.cdnleiting.top/gtckqovksj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangkeji.top/gthpdqjfly.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtnogjypof.html

std::string s = "hi";  s += "!";
来源：http://hz.xingfuxueyuan.xyz/gteghlktge.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtpcynwkqb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gthnnmxrxa.html

[S34] C++：遍历 vector
来源：http://hz.jinghuilouyu.cn/gtiojcesru.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtxdskilqy.html

[S35] C++：map
来源：http://hz.jinqigfzy.top/gtofsrwrsg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtqbresboh.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gtmfuhphxz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtwqkgeetu.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtbxkxklvx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.smart0.xyz/gtjxvidofd.html

[S38] C++：排序
来源：http://hz.c1oappe.top/gttzpywhqr.html

std::sort(v.begin(), v.end());
来源：http://hz.yvedp.cn/gtwcvjnfmh.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtymbtazjb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinyuanbaomall.cn/gtidzuohro.html

[S40] C++：查找元素
来源：http://hz.nanxinkj.top/gtwvgbjggx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.feifeiyinyue.top/gtrcjwdccq.html

[S41] C++：类与构造函数
来源：http://hz.pycfn.com/gtmkcllgna.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtdjwxxvuy.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtqsfxctvk.html

class B : public Base { public: void f() override {} };
来源：http://hz.quarkkingdee.top/gtkpdittkj.html

[S43] C++：智能指针
来源：http://hz.yonumen.top/gtrxqcfvdp.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtinvgiaal.html

[S44] C++：引用传参
来源：http://hz.yongpay.top/gtofthutnv.html

void inc(int &x) { ++x; }
来源：http://hz.nanxuanxn.top/gtwlnzsqag.html

[S45] C++：lambda
来源：http://hz.jinqigfzy.top/gtqogziuga.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yangfankeji.com/gtpjzwbahe.html

[S46] C++：函数模板
来源：http://hz.ywan-chungtsiang.top/gtyzfegvqp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnxiangtu.top/gtgtoqhdkq.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtuchsgeyr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.smart0.xyz/gtornxitos.html

[S48] C++：逐行读文件
来源：http://hz.havefunace.top/gtczgdqndp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pycfn.com/gtloirufer.html

while (std::getline(in, line)) { }
来源：http://hz.daria6918.cn/gtizylutel.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gttkvdtlxh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtyqgwgtcb.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gtluczfjio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtxvsihlgy.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtlsjhbjwc.html

static_cast<double>(a) / b
来源：http://hz.zhongyouzk.top/gtbfghuiuu.html

[S52] C++：const 与 noexcept
来源：http://hz.tianlin.xyz/gtvayosomw.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtybvshfib.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtoaickmfc.html

std::vector<int> w = std::move(v);
来源：http://hz.sufxvd.cn/gtupilmzsn.html

[S54] C++：异常处理
来源：http://hz.yuxming.cn/gtgkbpucvl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fengsongda.top/gtdxzixqsq.html

[S55] C++：结构化绑定
来源：http://hz.fzhhl.top/gtghzjuhez.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shangyingyoupin.top/gtktrcenmj.html

[S56] C++：optional
来源：http://hz.hysaishi.cn/gtxuhdtddi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtthakwcog.html

[S57] C++：编译期常量
来源：http://hz.fzhhl.top/gtksmvfiti.html

constexpr int N = 10;
来源：http://hz.snrcjt.cn/gtpkzsfpmx.html

[S58] C++：命名空间
来源：http://hz.jianghu66.top/gtojigxgbf.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtmpouebco.html

[S59] C++：静态断言
来源：http://hz.zhoulong.xyz/gtsqsgjhlq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pycfn.com/gtxuxzchsi.html

[S60] C++：遍历并删除元素
来源：http://hz.iojbl.cn/gtnygkvhtk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hongshengwenyu.top/gthhwrlmqe.html

================================================================================
来源：http://hz.nwbrower.top/gtdnozandr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangshuangyany.cn/gtxafouqqm.html

================================================================================
来源：http://hz.hfpthk.cn/gtiokgtdue.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangkeji.top/gtbgczpouw.html

println("Hello")
来源：http://hz.cashguo.top/gtdxzrjdyx.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gtgpbedvnb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gtknjxurqs.html

[T03] Kotlin：字符串模板
来源：http://hz.ehwqpu.com/gtjysqaqad.html

"值: $b"
来源：http://hz.iojbl.cn/gtnjsxzunh.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtclepmwei.html

val n: String? = null;  n?.length
来源：http://hz.dashuyun.cn/gtlssqdbyu.html

[T05] Kotlin：when 表达式
来源：http://hz.zhoulong.xyz/gtrztczjra.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.havefunace.top/gtodoiwtva.html

[T06] Kotlin：集合映射
来源：http://hz.jyoumei.cn/gtiauzikvt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gtnmvhzzgd.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gthccbtrty.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuanzx.com/gtpbwtditk.html

[T08] Kotlin：数据类
来源：http://hz.hysaishi.cn/gtrgfuphkf.html

data class User(val name: String, val age: Int)
来源：http://hz.cqqwz.cn/gtqerpqnun.html

[T09] Kotlin：扩展函数
来源：http://hz.ivvv.top/gtnmlxcbjl.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtaepxsmne.html

[T10] Kotlin：默认参数
来源：http://hz.tianlin.xyz/gthayrxxro.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinyuanbaomall.cn/gtlnsymzte.html

[T11] Kotlin：协程
来源：http://hz.dashuyun.cn/gtangecbxk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.feifeiyinyue.top/gtawqcirys.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtzdkfqlhz.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtxzfpjnpq.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtopveqpet.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtftbuaajf.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtpslgpbku.html

for (i in 1..10) println(i)
来源：http://hz.jyoumei.cn/gtuhojoyup.html

[T15] Kotlin：接口
来源：http://hz.nanxuanxn.top/gtehxdgsht.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtobrfwzxp.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtgdbknapt.html

print("Hello")
来源：http://hz.yuanzhike.top/gtndaxytvk.html

[T17] Swift：变量与常量
来源：http://hz.hongshengwenyu.top/gtvjtwdsiq.html

var a = 1;  let b = 2
来源：http://hz.shuidangran.top/gtftdhactm.html

[T18] Swift：字符串插值
来源：http://hz.jianghu66.top/gthcpgkwtq.html

"值: \(b)"
来源：http://hz.haohaochexian.top/gtmeuiotuy.html

[T19] Swift：可选绑定
来源：http://hz.zycfv.cn/gtscpqfowm.html

if let n = opt { print(n) }
来源：http://hz.jqgfzy.top/gtgenmvlol.html

[T20] Swift：数组操作
来源：http://hz.yj202588.top/gtmucfkceq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.snrcjt.cn/gtoeyzxzgi.html

[T21] Swift：遍历
来源：http://hz.gotoacloud.top/gttqwiccfi.html

for x in a { print(x) }
来源：http://hz.gaohongyu789.top/gtshvmwyzd.html

[T22] Swift：字典
来源：http://hz.andypj.xyz/gtpvcilucb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pengpengdd.cyou/gtcpwvwvfv.html

[T23] Swift：函数
来源：http://hz.gaohongyu789.top/gtojyebxhh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xziqi.cn/gtrzepufwh.html

[T24] Swift：闭包
来源：http://hz.xuetiantiany.cn/gtocbhlzxv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhongyouzk.top/gtaoxutyfm.html

[T25] Swift：结构体
来源：http://hz.hysaishi.cn/gtlnxzoigq.html

struct P { var x: Int }
来源：http://hz.jinqigufen.top/gtgwtyzmvm.html

[T26] Swift：类与重写
来源：http://hz.xziqi.cn/gtxsmwkvyj.html

class A: Base { override func f() {} }
来源：http://hz.zhiwuduotai.top/gtmqzynxab.html

[T27] Swift：错误处理
来源：http://hz.shzxlz.cn/gtcuwawish.html

do { try f() } catch { print(error) }
来源：http://hz.sufxvd.cn/gtwrjxcfxi.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gtrgczkess.html

enum Color { case red, green }
来源：http://hz.cashguo.top/gtbrlexmpl.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgfzy.top/gtsxiyuqxs.html

guard let x = opt else { return }
来源：http://hz.ydjk.org.cn/gtixgmeyec.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtspccbcim.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtstxpwlua.html

[T31] Lua：Hello World
来源：http://hz.zdqjudy.top/gtgdtprbti.html

print("Hello")
来源：http://hz.zhengqikj.top/gtlcgclqun.html

[T32] Lua：局部变量
来源：http://hz.nanxuanxn.top/gtkbbnguxv.html

local a = 1
来源：http://hz.zhongyouzk.top/gtucjqaisa.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtacurxqsk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.iojbl.cn/gtavxjalrs.html

[T34] Lua：遍历表
来源：http://hz.ywan-chungtsiang.top/gtpmwygchb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hysaishi.cn/gtyiofwkqp.html

[T35] Lua：字典表
来源：http://hz.mhx1999.top/gtafkcbeai.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ehwqpu.com/gtpcljrghl.html

[T36] Lua：函数
来源：http://hz.iojbl.cn/gtmcxmorac.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtpgeiuaxh.html

[T37] Lua：字符串拼接
来源：http://hz.fengsongda.top/gtcznlvnzh.html

"a" .. "b"
来源：http://hz.yuanzhike.top/gtvelawupe.html

[T38] Lua：条件
来源：http://hz.havefunace.top/gttkmblbcx.html

if x > 0 then print("正") end
来源：http://hz.zhaomingkeji.xyz/gtylzxjtzr.html

[T39] Lua：模式匹配
来源：http://hz.hnxiangtu.top/gtxuwyadck.html

string.find(s, "%d+")
来源：http://hz.xuetiantiany.cn/gtqojhuhdy.html

[T40] Lua：元表
来源：http://hz.zhixingplan.top/gtklsgvtlu.html

setmetatable({}, { __index = base })
来源：http://hz.jiagoushi.top/gtuygzwljl.html

[T41] Perl：Hello World
来源：http://hz.chenlongwang.top/gtnxjrinxp.html

print "Hello\n";
来源：http://hz.dianchejie.cn/gtmjzqvgje.html

[T42] Perl：变量类型
来源：http://hz.xinyue.icu/gtbjgnsqnc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtwttdyyby.html

[T43] Perl：字符串插值
来源：http://hz.jianghu66.top/gtzznrnuur.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtiqctsedw.html

[T44] Perl：条件
来源：http://hz.hnxiangtu.top/gtyzsrmbdy.html

if ($a > 0) { print "正"; }
来源：http://hz.ehwqpu.com/gtuvyfmhqj.html

[T45] Perl：数组遍历
来源：http://hz.haohaochexian.top/gtoeshoehh.html

for my $x (@arr) { print $x; }
来源：http://hz.andypj.xyz/gtnjmoqbud.html

[T46] Perl：哈希操作
来源：http://hz.xuetiantiany.cn/gtcntwgewl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydzc1.top/gtwipdjlxb.html

[T47] Perl：正则捕获
来源：http://hz.zhixingplan.top/gtxbyggsbi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xingfuxueyuan.xyz/gtzmwuiygv.html

[T48] Perl：正则替换
来源：http://hz.pengpengdd.cyou/gtndhwmapv.html

$s =~ s/old/new/g;
来源：http://hz.yj202588.top/gtcvsdfzml.html

[T49] Perl：函数
来源：http://hz.jinqigufen.top/gtpfijgfwp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ybcxt.top/gtomxqcazs.html

[T50] Perl：逐行读文件
来源：http://hz.sufxvd.cn/gtdxidwtru.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtqgjygeev.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gtbgurzxup.html

[T51] Scala：Hello World
来源：http://hz.jinghuilouyu.cn/gtmrvdquis.html

println("Hello")
来源：http://hz.yuxming.cn/gtfncochtq.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtkqkcnxod.html

val a = 1;  var b = 2
来源：http://hz.zycfv.cn/gtrptjgdmg.html

[T53] Scala：字符串插值
来源：http://hz.ybcxt.top/gtsutsgrgb.html

s"值: $b"
来源：http://hz.hnxiangtu.top/gtzngaqhrt.html

[T54] Scala：集合映射
来源：http://hz.yueranfly.top/gtdvwykssh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cucudq.cn/gtrrovkzel.html

[T55] Scala：集合过滤
来源：http://hz.cheryme.top/gtatxkbdfl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tianlin.xyz/gtlfxrghuh.html

[T56] Scala：样例类
来源：http://hz.hysaishi.cn/gtkfmtadpa.html

case class User(name: String, age: Int)
来源：http://hz.pengpengdd.cyou/gtsgaqogro.html

[T57] Scala：模式匹配
来源：http://hz.haohaochexian.top/gtykmjbtwq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.316326.xyz/gtjknnrbyx.html

[T58] Scala：函数定义
来源：http://hz.ybcxt.top/gtyqayolru.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yonumen.top/gtzxdevjsc.html

[T59] Scala：循环
来源：http://hz.0kj1m.cn/gtvlifrbkq.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenzaomai.com/gtajyafcgy.html

[T60] Scala：折叠
来源：http://hz.hongshengwenyu.top/gtoaorksas.html


<!-- 参考信息 -->