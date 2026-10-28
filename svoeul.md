代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.aibaodan.cn/gtzzdphljx.html

[R56] 远程拷贝
来源：http://hz.andypj.xyz/gtvwpguaqe.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtjrapubil.html

[R57] 远程执行命令
来源：http://hz.ywan-chungtsiang.top/gtadxntidb.html

ssh user@host 'uptime'
来源：http://hz.haohaochexian.top/gtcmwaozld.html

[R58] 下载文件
来源：http://hz.zhongyouzk.top/gtqzigwanw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtitewwsyc.html

[R59] 发 POST JSON
来源：http://hz.fzhhl.top/gtdxxgwmbi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtjqpnqsho.html

[R60] 只看 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtzepuzcsp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj202588.top/gtqpjsfgwn.html

[R61] 磁盘占用
来源：http://hz.nanxinkj.top/gtuvfiidps.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtkyseqsjh.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gtwtxrmett.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtqdnugsbs.html

[R63] 内存与进程
来源：http://hz.sufxvd.cn/gtwinzecoy.html

free -h;  ps aux | grep nginx
来源：http://hz.vqdsnc.cn/gtujeyrxhn.html

[R64] 结束进程
来源：http://hz.snrcjt.cn/gtzdeeizzn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gtbqfundff.html

[R65] 查看端口占用
来源：http://hz.sxryk.cn/gthvdjaajl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtcmkcebbn.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gtdlomkhlr.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtlpefmxtk.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangtech.top/gtithdskkx.html

openssl rand -hex 16
来源：http://hz.meibo888.top/gtikbohzer.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtlobehghn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinghuilouyu.cn/gtzgsdcwkb.html

[R69] 生成随机密码
来源：http://hz.ydzc1.top/gtbqspnuai.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtepuajcap.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtzeeurujb.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gtzzowseyq.html

[R71] 日期格式化
来源：http://hz.chenjidiqi.icu/gtqhqdmoni.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dashuyun.cn/gtpqwfgetc.html

[R72] 等待端口就绪
来源：http://hz.snrcjt.cn/gtcwqrzygw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.9152youxi.cn/gtjmdurkla.html

[R73] 分割大日志
来源：http://hz.cashguo.top/gtmqjdsvnb.html

split -l 1000 big.log part_
来源：http://hz.sufxvd.cn/gteymvccls.html

[R74] 批量重命名
来源：http://hz.zdqjudy.top/gtgkxnmqwg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtbiblqskt.html

[R75] 导出环境变量
来源：http://hz.cheryme.top/gtgqczdmdb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhaomingkeji.xyz/gtdayjknxq.html

[R76] 使用临时文件
来源：http://hz.zhongyouzk.top/gtouexhrlr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtfkaqlohk.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtgndnojhr.html

read -rp "请输入: " ans
来源：http://hz.zhiwuduotai.top/gtxzfkvqng.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtcdwncuyk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtefzpyrba.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gthgomxnvm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuxming.cn/gtlydbnrza.html

[R80] 查看脚本执行耗时
来源：http://hz.iojbl.cn/gtejedbiyj.html

time ./run.sh
来源：http://hz.zhoulong.xyz/gtfpdbqlxt.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtktjvbzdi.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtzfdmehyk.html

================================================================================
来源：http://hz.jiagoushi.top/gteolhxfcm.html

[S01] C：Hello World
来源：http://hz.wangshuangyany.cn/gtmqsghznz.html

#include <stdio.h>
来源：http://hz.wangshuangyany.cn/gteevmxufb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtbymdscaa.html

[S02] C：变量与格式化输出
来源：http://hz.jqgufenzy.top/gttmeayhdl.html

int a = 10; printf("%d\n", a);
来源：http://hz.yueranfly.top/gtiazrshoz.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtupaikniq.html

int x; scanf("%d", &x);
来源：http://hz.cucudq.cn/gtzyptkjqc.html

[S04] C：字符串复制
来源：http://hz.meibo888.top/gtpwddqmpl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aizwys.cn/gtvllccprb.html

[S05] C：字符串长度
来源：http://hz.ybcxt.top/gtfvifkgiz.html

strlen(s)
来源：http://hz.snrcjt.cn/gtjdvbzrqb.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gtgbaavtrk.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtumhngpaw.html

[S07] C：数组遍历求和
来源：http://hz.ydjk.org.cn/gtjczblils.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cdnleiting.top/gtcjvnhvaj.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtrxgmnzwu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtlilswidh.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtjcbwlyxl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtpecdkxyh.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtenguphjx.html

int *p = &a;  *p = 5;
来源：http://hz.guowangkeji.top/gtrejorpip.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtoqrhxhic.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.meibo888.top/gtljofdapa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenlongwang.top/gtqwpraljy.html

fclose(f);
来源：http://hz.meibo888.top/gtyraltvgo.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtmcralsbz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.bjfxy.top/gtczpuokbz.html

[S13] C：宏定义
来源：http://hz.9152youxi.cn/gtthffqvfn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgfzy.top/gteoxpizpa.html

[S14] C：枚举
来源：http://hz.cheryme.top/gtmzbjwdee.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtwnjbvghp.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gtdsktzjyz.html

(double) a / b
来源：http://hz.chenlongwang.top/gtobadfcig.html

[S16] C：位操作置位
来源：http://hz.yangfankeji.com/gtbwexxlqi.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtcqpjtlkj.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gthzrgakcg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtdyurteym.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtvupzksez.html

int main(int argc, char **argv)
来源：http://hz.316326.xyz/gtdjgctnhw.html

[S19] C：快速排序
来源：http://hz.havefunace.top/gtubcksefm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtnjslrisr.html

[S20] C：二分查找
来源：http://hz.ywan-chungtsiang.top/gticohdunn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtimsfzjzr.html

[S21] C：字符类别判断
来源：http://hz.zycfv.cn/gtzxtbqmfb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gtetlwmqbp.html

[S22] C：字符串转数字
来源：http://hz.yueranfly.top/gtjdlmfqzo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtaccbbxkc.html

[S23] C：随机数
来源：http://hz.iojbl.cn/gtwxsnbnqh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tianlin.xyz/gtiaujxdge.html

[S24] C：获取本地时间
来源：http://hz.yvedp.cn/gtfrmbjanv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xylfe.cn/gteplamslb.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gtqrcdwoyt.html

memcpy(dst, src, n);
来源：http://hz.guowangkeji.top/gtotmorgzl.html

[S26] C：内存清零
来源：http://hz.xziqi.cn/gtzlqcvsye.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtqpjemcgs.html

[S27] C：定义常量
来源：http://hz.cucudq.cn/gthergozcy.html

const double PI = 3.14159;
来源：http://hz.cucudq.cn/gtuktuflpy.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtkcbdhnum.html

static int counter = 0;
来源：http://hz.zhiwuduotai.top/gtpsdptwko.html

[S29] C：变参函数
来源：http://hz.chenlongwang.top/gtlkdzrsre.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenzaomai.com/gtuljzlyrb.html

[S30] C：头文件保护
来源：http://hz.andypj.xyz/gtpbhyyxrp.html

#ifndef X_H
来源：http://hz.c1oappe.top/gtndtwzwxt.html

#define X_H
来源：http://hz.haohaochexian.top/gtlhfwmzvk.html

#endif
来源：http://hz.yj20258888.top/gtknoxjhhu.html

[S31] C++：Hello World
来源：http://hz.meibo888.top/gtmzytemdt.html

#include <iostream>
来源：http://hz.fengsongda.top/gtmbhlvbvf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gteddyfwjx.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtbccmikzy.html

std::string s = "hi";  s += "!";
来源：http://hz.iojbl.cn/gtbgstrwzn.html

[S33] C++：vector 增删
来源：http://hz.haohaochexian.top/gtnosymomo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xingfuxueyuan.xyz/gtbvkwazpj.html

[S34] C++：遍历 vector
来源：http://hz.yj20258888.top/gttywhgatq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtgksvoqrb.html

[S35] C++：map
来源：http://hz.0kj1m.cn/gtupwwagrj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuxming.cn/gtweqdwnbx.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gthhyfvnjx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gthlfcocws.html

[S37] C++：set
来源：http://hz.hnqzz.top/gtjjighwiq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nwbrower.top/gtymgqarjv.html

[S38] C++：排序
来源：http://hz.sysykeji.top/gtfvouhvxa.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtmggigbiw.html

[S39] C++：自定义比较器排序
来源：http://hz.yj202588.top/gtsxoezdcr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xingfuxueyuan.xyz/gtodlllvjy.html

[S40] C++：查找元素
来源：http://hz.gotoacloud.top/gtqhdjnaeh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtkhmlbetc.html

[S41] C++：类与构造函数
来源：http://hz.hywenlv.cn/gtwhpimgtn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dianchejie.cn/gtldeuqqpn.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gttampmpqa.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtuoetedys.html

[S43] C++：智能指针
来源：http://hz.jqgufenzy.top/gtrisitgah.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gtxvthsjmw.html

[S44] C++：引用传参
来源：http://hz.yvedp.cn/gtlyhfvoek.html

void inc(int &x) { ++x; }
来源：http://hz.sysykeji.top/gtgxggmklp.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtcnuuswst.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nwbrower.top/gtjyxvxnmc.html

[S46] C++：函数模板
来源：http://hz.xinyue.icu/gtmxoutiqx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhijiandao.cn/gtjrhyofqr.html

[S47] C++：结构化绑定遍历
来源：http://hz.c1oappe.top/gtocdfeuco.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gaohongyu789.top/gtnxhvikir.html

[S48] C++：逐行读文件
来源：http://hz.316326.xyz/gtkosuabyw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gttsxxennd.html

while (std::getline(in, line)) { }
来源：http://hz.cucudq.cn/gthyejrabt.html

[S49] C++：写文件
来源：http://hz.yvedp.cn/gtpkimuvsj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxuanxn.top/gtofcmrtmb.html

[S50] C++：格式化数字
来源：http://hz.yuanzhike.top/gtkinvfmde.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.feifeiyinyue.top/gtjmsrfsqr.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtvwbkflcv.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtsyxaqhxh.html

[S52] C++：const 与 noexcept
来源：http://hz.chenlongwang.top/gttfwjdlgq.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtggfquyol.html

[S53] C++：移动语义
来源：http://hz.ivvv.top/gtyumvlkcz.html

std::vector<int> w = std::move(v);
来源：http://hz.haohaochexian.top/gtwstrdjnd.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gtuvayesvw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenjidiqi.icu/gtnjzxzgfm.html

[S55] C++：结构化绑定
来源：http://hz.redwolf501.top/gtpabmifaz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yanxiufei.cn/gtvzigfsxd.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtkpcnbits.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hongshengwenyu.top/gtmuqwlsim.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtngvlavmh.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtcjwlkdvg.html

[S58] C++：命名空间
来源：http://hz.yangfankeji.com/gtbjubtuys.html

namespace ns { int f() { return 1; } }
来源：http://hz.fengsongda.top/gtiukmyixa.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtykczeyez.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtmqbmvpht.html

[S60] C++：遍历并删除元素
来源：http://hz.chenlongwang.top/gtfoazailg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daria6918.cn/gtuxirroqu.html

================================================================================
来源：http://hz.cdnleiting.top/gthdazgtki.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtyfhhadkc.html

================================================================================
来源：http://hz.52xcode.cn/gtpyenbuwz.html

[T01] Kotlin：Hello World
来源：http://hz.quarkkingdee.top/gtfgpuasiz.html

println("Hello")
来源：http://hz.shzxlz.cn/gttqoamaqn.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtkklicjvh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gtehvpvasy.html

[T03] Kotlin：字符串模板
来源：http://hz.hongshengwenyu.top/gtcruraqcu.html

"值: $b"
来源：http://hz.yvedp.cn/gtenxxlgvg.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangtech.top/gtabhcrufl.html

val n: String? = null;  n?.length
来源：http://hz.smart0.xyz/gtvedocxvl.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtbzhawisf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gzhubu.top/gtygvmpoqj.html

[T06] Kotlin：集合映射
来源：http://hz.jinqigfzy.top/gtloihfckc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuxming.cn/gtejfdaqta.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtvrilpmie.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aizwys.cn/gtiilffcvt.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtbhfnimol.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgufenzy.top/gtdsvaodvy.html

[T09] Kotlin：扩展函数
来源：http://hz.vqdsnc.cn/gttviatykb.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gtspoeqyzr.html

[T10] Kotlin：默认参数
来源：http://hz.fzhhl.top/gtcgggfqce.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxinkj.top/gtphmmnhjo.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gtkytrguvb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zycfv.cn/gtshipffuk.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtdppxzbgc.html

val (a, b) = Pair(1, 2)
来源：http://hz.kuanghao11.cn/gtbbhpiyip.html

[T13] Kotlin：只读 Map
来源：http://hz.yuanzhike.top/gtnzioazbl.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtzxfepbxv.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtftselsrx.html

for (i in 1..10) println(i)
来源：http://hz.hfpthk.cn/gtmzaipccu.html

[T15] Kotlin：接口
来源：http://hz.yj20258.top/gtgadsqndg.html

interface Shape { fun area(): Double }
来源：http://hz.ydzc1.top/gtsmmiorbd.html

[T16] Swift：Hello World
来源：http://hz.svipenyu.cn/gtefsuufrp.html

print("Hello")
来源：http://hz.sufxvd.cn/gttfybkznh.html

[T17] Swift：变量与常量
来源：http://hz.0kj1m.cn/gtavfojjzo.html

var a = 1;  let b = 2
来源：http://hz.cdnleiting.top/gtjvszlzsi.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtlzaaasfz.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtkcybdrox.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gthbjirpxn.html

if let n = opt { print(n) }
来源：http://hz.zhoulong.xyz/gtskwnsojg.html

[T20] Swift：数组操作
来源：http://hz.hfpthk.cn/gtezfgmzob.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xylfe.cn/gtsibtipfg.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtrktkwmsw.html

for x in a { print(x) }
来源：http://hz.shangyingyoupin.top/gtnembjnwe.html

[T22] Swift：字典
来源：http://hz.hongshengwenyu.top/gtyrbwwzzd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinyuanbaomall.cn/gtrwhdrvju.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtkvrslesy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cucudq.cn/gtgxccvppc.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gtxykregvm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hysaishi.cn/gtwttwrdvs.html

[T25] Swift：结构体
来源：http://hz.pycfn.com/gtyawjwusj.html

struct P { var x: Int }
来源：http://hz.zycfv.cn/gtjopnuoey.html

[T26] Swift：类与重写
来源：http://hz.gogol.net.cn/gtfjbcsvbc.html

class A: Base { override func f() {} }
来源：http://hz.sysykeji.top/gtrighcepv.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtjverdlhi.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtxgeqjjru.html

[T28] Swift：枚举
来源：http://hz.svipenyu.cn/gtvzxwtcbn.html

enum Color { case red, green }
来源：http://hz.yuxming.cn/gtgudbiwzg.html

[T29] Swift：guard 提前返回
来源：http://hz.jinghuilouyu.cn/gtjgabdfox.html

guard let x = opt else { return }
来源：http://hz.jqgfzy.top/gtjqlblhzn.html

[T30] Swift：协议
来源：http://hz.zhengqikj.top/gtqpqprfgk.html

protocol Shape { func area() -> Double }
来源：http://hz.smart0.xyz/gtxneeotwo.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangtech.top/gtrazjvfzw.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtsobhnvuz.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtglshtwqg.html

local a = 1
来源：http://hz.zhaomingkeji.xyz/gtdqgehwcd.html

[T33] Lua：表（数组）
来源：http://hz.vqdsnc.cn/gtuqbmocfg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gzhubu.top/gtvqsadact.html

[T34] Lua：遍历表
来源：http://hz.gogol.net.cn/gtktmhsnfd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xziqi.cn/gtnblvikuu.html

[T35] Lua：字典表
来源：http://hz.zhengqikj.top/gtflkwwauk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pycfn.com/gtxxrcpmhp.html

[T36] Lua：函数
来源：http://hz.zycfv.cn/gtaetwcini.html

function add(a, b) return a + b end
来源：http://hz.cheryme.top/gtxwqceqip.html

[T37] Lua：字符串拼接
来源：http://hz.hysaishi.cn/gtvletrpsn.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtdvfkrbvc.html

[T38] Lua：条件
来源：http://hz.havefunace.top/gtobqrlywv.html

if x > 0 then print("正") end
来源：http://hz.fzhhl.top/gtbppxkwci.html

[T39] Lua：模式匹配
来源：http://hz.hnqzz.top/gtziclnamy.html

string.find(s, "%d+")
来源：http://hz.haohaochexian.top/gtkjhhdneg.html

[T40] Lua：元表
来源：http://hz.yuxming.cn/gtaqerudvj.html

setmetatable({}, { __index = base })
来源：http://hz.zhoulong.xyz/gthswfiylm.html

[T41] Perl：Hello World
来源：http://hz.316326.xyz/gtsqwxnvey.html

print "Hello\n";
来源：http://hz.jqgufenzy.top/gtbrjdbwav.html

[T42] Perl：变量类型
来源：http://hz.yanxiufei.cn/gtwqdudreg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhaomingkeji.xyz/gtynkkiuwj.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtwzffbpwh.html

"值: $a"
来源：http://hz.havefunace.top/gtluxxxong.html

[T44] Perl：条件
来源：http://hz.hongshengwenyu.top/gtqprievkt.html

if ($a > 0) { print "正"; }
来源：http://hz.chenlongwang.top/gtbtjkvlce.html

[T45] Perl：数组遍历
来源：http://hz.aibaodan.cn/gttytnnufw.html

for my $x (@arr) { print $x; }
来源：http://hz.tanke756.top/gthxyyuvbi.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gttlfkbjhs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangshuangyany.cn/gtmhsoevjh.html

[T47] Perl：正则捕获
来源：http://hz.svipenyu.cn/gtytfclnpi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hnxiangtu.top/gtahhsxwlw.html

[T48] Perl：正则替换
来源：http://hz.vqdsnc.cn/gtefdmhpkb.html

$s =~ s/old/new/g;
来源：http://hz.yueranfly.top/gtivqkfxjx.html

[T49] Perl：函数
来源：http://hz.quarkkingdee.top/gttqqlvmej.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtucapehlh.html

[T50] Perl：逐行读文件
来源：http://hz.zhiwuduotai.top/gtbvrgcykd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydzc1.top/gtueybiric.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenzaomai.com/gtcnapsaox.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gtjegivuuq.html

println("Hello")
来源：http://hz.daxiang520.top/gtzjumchsc.html

[T52] Scala：变量
来源：http://hz.xylfe.cn/gtotejouwh.html

val a = 1;  var b = 2
来源：http://hz.jinqigfzy.top/gthizlvlfm.html

[T53] Scala：字符串插值
来源：http://hz.yj202588.top/gtrsviviqw.html

s"值: $b"
来源：http://hz.yanxiufei.cn/gtoddbeask.html

[T54] Scala：集合映射
来源：http://hz.hysaishi.cn/gtvvagnnmf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cheryme.top/gtygwrqgep.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gtplqpmebl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tianlin.xyz/gtjyszrodb.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtupqghgfw.html

case class User(name: String, age: Int)
来源：http://hz.cdnleiting.top/gtydiqmccn.html

[T57] Scala：模式匹配
来源：http://hz.hysaishi.cn/gtaznzyizd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhiwuduotai.top/gtyvfzzfec.html

[T58] Scala：函数定义
来源：http://hz.yuxming.cn/gtxgmnfxcl.html


<!-- 参考信息 -->