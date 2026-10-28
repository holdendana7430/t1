代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydjk.org.cn/gtrhcqgbzd.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gthxdzlxkz.html

diff a.txt b.txt
来源：http://hz.sufxvd.cn/gtvvdznpzq.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtcdgeekvr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jlsjyb.cn/gtpipbyxau.html

[R56] 远程拷贝
来源：http://hz.shuidangran.top/gtgveuiffy.html

scp file user@host:/path/
来源：http://hz.zhengqikj.top/gtwiayynfi.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtupcbblyp.html

ssh user@host 'uptime'
来源：http://hz.ydzc1.top/gtadvoashz.html

[R58] 下载文件
来源：http://hz.aizwys.cn/gtdbdxgght.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydjk.org.cn/gtrwyyywus.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtylluoixd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gtgldouzdl.html

[R60] 只看 HTTP 状态码
来源：http://hz.52xcode.cn/gtfaezyemd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gtsdqdkzma.html

[R61] 磁盘占用
来源：http://hz.zhiwuduotai.top/gtsmoohqpq.html

df -h;  du -sh *
来源：http://hz.9152youxi.cn/gtnnpsxghv.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gtrmhjuwtb.html

du -ah . | sort -rh | head -10
来源：http://hz.yvedp.cn/gtvtaqmkho.html

[R63] 内存与进程
来源：http://hz.yanxiufei.cn/gtlkvnwhsm.html

free -h;  ps aux | grep nginx
来源：http://hz.shzxlz.cn/gtbneijkme.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtzxuylupm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jiagoushi.top/gtysftgskq.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtdrmacmpt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtszbqfrht.html

[R66] 定时任务
来源：http://hz.chenjidiqi.icu/gtcvovzths.html

crontab -e;  crontab -l
来源：http://hz.hysaishi.cn/gtniuhqnwj.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gtvcdcrogv.html

openssl rand -hex 16
来源：http://hz.yj202588.top/gtnphecnix.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtaamadxms.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtwcqhjzla.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gtskdtrdls.html

head -c 16 /dev/urandom | base64
来源：http://hz.meibo888.top/gtcagqcesx.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtflftadkl.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtrkbuvozv.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtmxbexzbp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yueranfly.top/gthlvmkmiu.html

[R72] 等待端口就绪
来源：http://hz.iojbl.cn/gtxoybdqob.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtvlhgkgvn.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtqrjfxxbe.html

split -l 1000 big.log part_
来源：http://hz.yj20258888.top/gtndrwxonj.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtqdtalcwh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shzxlz.cn/gtwkxwwjnt.html

[R75] 导出环境变量
来源：http://hz.jinghuilouyu.cn/gtovddmqhq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.fengsongda.top/gtrvxcozqr.html

[R76] 使用临时文件
来源：http://hz.sweek.top/gtsltsqsla.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtfuxqybvo.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtapiialdi.html

read -rp "请输入: " ans
来源：http://hz.0kj1m.cn/gthnryfgwn.html

[R78] 交互式菜单
来源：http://hz.xuanzx.com/gtbvxhhlmg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtongrgpbq.html

[R79] 解析命令行选项
来源：http://hz.yvedp.cn/gtekjwehgn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtaonxhzgl.html

[R80] 查看脚本执行耗时
来源：http://hz.fzhhl.top/gtyknlllmr.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtydrpstfi.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtojziurow.html

S. C / C++ 专题
来源：http://hz.wangshuangyany.cn/gtwsxwellw.html

================================================================================
来源：http://hz.hysaishi.cn/gteyomqrlo.html

[S01] C：Hello World
来源：http://hz.fzhhl.top/gtmfymyuqv.html

#include <stdio.h>
来源：http://hz.birdmap.top/gtursmizro.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.smart0.xyz/gtxgvodbdx.html

[S02] C：变量与格式化输出
来源：http://hz.meibo888.top/gtqvqicdqs.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtonbbbeux.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtemoiqdee.html

int x; scanf("%d", &x);
来源：http://hz.snrcjt.cn/gtxnjtfrim.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gttdcskksl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtafekeill.html

[S05] C：字符串长度
来源：http://hz.shzxlz.cn/gtberccxvp.html

strlen(s)
来源：http://hz.dianchejie.cn/gtftvtcyxw.html

[S06] C：字符串比较
来源：http://hz.ydzc1.top/gtnmbffucq.html

strcmp(a, b) == 0
来源：http://hz.ywan-chungtsiang.top/gtaizptkqk.html

[S07] C：数组遍历求和
来源：http://hz.jyoumei.cn/gtrqojgnrx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gtvvihetvm.html

[S08] C：动态内存分配与释放
来源：http://hz.ywan-chungtsiang.top/gthgpueczd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.quarkkingdee.top/gtgufvkypq.html

[S09] C：结构体定义与初始化
来源：http://hz.dianchejie.cn/gthjobzmog.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenjidiqi.icu/gtroumcbxm.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gturxoqjfm.html

int *p = &a;  *p = 5;
来源：http://hz.wangdashe.top/gtynlxuhrd.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtlqbjueqb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aibaodan.cn/gtevaiaomd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtgrznxrba.html

fclose(f);
来源：http://hz.sweek.top/gtubfvsqpm.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gtwdwohyby.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuetiantiany.cn/gtpozfftzh.html

[S13] C：宏定义
来源：http://hz.chenjidiqi.icu/gtusttlgvx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtxddhkevz.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gtmwllitlh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.bjfxy.top/gtnlnpmtpz.html

[S15] C：类型转换
来源：http://hz.xinyue.icu/gtfxndcfvu.html

(double) a / b
来源：http://hz.jianghu66.top/gtfvxadpay.html

[S16] C：位操作置位
来源：http://hz.yueranfly.top/gtnnooaaiu.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtuprhgcsu.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtcyohehse.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtminhyogx.html

[S18] C：命令行参数
来源：http://hz.jianghu66.top/gtfmkguwnw.html

int main(int argc, char **argv)
来源：http://hz.316326.xyz/gtclltffps.html

[S19] C：快速排序
来源：http://hz.iojbl.cn/gtrlizppmf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guannengcc.top/gtlihgjpfm.html

[S20] C：二分查找
来源：http://hz.yueranfly.top/gtafhmjbyj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj202588.top/gthizvoocc.html

[S21] C：字符类别判断
来源：http://hz.daxiang520.top/gtjeccsnbb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gtdsoigpgp.html

[S22] C：字符串转数字
来源：http://hz.wangshuangyany.cn/gtyxihqhdc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.iojbl.cn/gtbkpurhmv.html

[S23] C：随机数
来源：http://hz.andypj.xyz/gtshtunzzt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gthmrsjiyp.html

[S24] C：获取本地时间
来源：http://hz.sxryk.cn/gthcbdrpma.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtwgcoetht.html

[S25] C：内存拷贝
来源：http://hz.shzxlz.cn/gtqmageavv.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtaqiigyry.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtslxopnhj.html

memset(a, 0, sizeof a);
来源：http://hz.sysykeji.top/gtororjofr.html

[S27] C：定义常量
来源：http://hz.xuetiantiany.cn/gtapfckfxl.html

const double PI = 3.14159;
来源：http://hz.cheryme.top/gtqcjveytc.html

[S28] C：静态变量
来源：http://hz.ydjk.org.cn/gtjhfrbjwd.html

static int counter = 0;
来源：http://hz.cucudq.cn/gtawqcdgbm.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtaialvakt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tian-w.cn/gtqdnofczi.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtdatnfkoz.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtrmsmipmy.html

#define X_H
来源：http://hz.yonumen.top/gtovcjxgry.html

#endif
来源：http://hz.9152youxi.cn/gtkmyrezoq.html

[S31] C++：Hello World
来源：http://hz.redwolf501.top/gtjmrjtqvn.html

#include <iostream>
来源：http://hz.cdnleiting.top/gthcbxeekr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258888.top/gtgimsbnny.html

[S32] C++：字符串
来源：http://hz.ywan-chungtsiang.top/gtykbnzlun.html

std::string s = "hi";  s += "!";
来源：http://hz.iojbl.cn/gtqfwjugfn.html

[S33] C++：vector 增删
来源：http://hz.iojbl.cn/gtijupcyqp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtfsogbfny.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtgkilnhcn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gzhubu.top/gtzgfrswwh.html

[S35] C++：map
来源：http://hz.andypj.xyz/gtrursmkuo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtlyahucrs.html

[S36] C++：unordered_map
来源：http://hz.wangdashe.top/gtxltxucli.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtgxwtscbc.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtqpnogzjw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258888.top/gtuhazisjt.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gtwtnpojtw.html

std::sort(v.begin(), v.end());
来源：http://hz.zhiwuduotai.top/gtnmpgfpkh.html

[S39] C++：自定义比较器排序
来源：http://hz.c1oappe.top/gtyanbonjg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinghuilouyu.cn/gtumbrdyar.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gteqygihft.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtprlfdxnu.html

[S41] C++：类与构造函数
来源：http://hz.hnxiangtu.top/gtopqqgwxm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.birdmap.top/gtixecalmk.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtlmisemub.html

class B : public Base { public: void f() override {} };
来源：http://hz.vqdsnc.cn/gthhgklggr.html

[S43] C++：智能指针
来源：http://hz.vqdsnc.cn/gtawugsstg.html

auto p = std::make_unique<int>(5);
来源：http://hz.tanke756.top/gtagvbkhzg.html

[S44] C++：引用传参
来源：http://hz.jqgfzy.top/gtldsvkmwi.html

void inc(int &x) { ++x; }
来源：http://hz.chenlongwang.top/gtebvryzjo.html

[S45] C++：lambda
来源：http://hz.smart0.xyz/gtmzgolfqv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shuidangran.top/gtpnlqhdmi.html

[S46] C++：函数模板
来源：http://hz.52xcode.cn/gtklvzfqhr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtkrohxtvg.html

[S47] C++：结构化绑定遍历
来源：http://hz.hysaishi.cn/gtoeatcvyu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangdashe.top/gtjxngwpyt.html

[S48] C++：逐行读文件
来源：http://hz.bjfxy.top/gtyoaaboee.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gtlptcstmc.html

while (std::getline(in, line)) { }
来源：http://hz.sysykeji.top/gtppzjcabo.html

[S49] C++：写文件
来源：http://hz.shanyushiyangkeji.top/gtcagftqpk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigufen.top/gtlfxewenq.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gtbddgqrtn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xinyue.icu/gtqtuytkhx.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtpbngmoav.html

static_cast<double>(a) / b
来源：http://hz.c1oappe.top/gtpoxstwdw.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtyrmkrega.html

int size() const noexcept { return n_; }
来源：http://hz.xylfe.cn/gtzbbgnqxj.html

[S53] C++：移动语义
来源：http://hz.tianlin.xyz/gtuibpizpu.html

std::vector<int> w = std::move(v);
来源：http://hz.guowangkeji.top/gtkwbuknla.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gturivphdl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtkkisfydj.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gtiajfzxfp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xylfe.cn/gtejkstjhi.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtvljuphik.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gtaoxgztqx.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtiopoygum.html

constexpr int N = 10;
来源：http://hz.hnxiangtu.top/gtinzgvsoq.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtzuzkkazz.html

namespace ns { int f() { return 1; } }
来源：http://hz.52xcode.cn/gtjxybugoy.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtiszyptht.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gttpuyashd.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtagzqmpbn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guannengcc.top/gtneaswdnn.html

================================================================================
来源：http://hz.sweek.top/gtwozzuzuy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtcishfkcw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjlbimazy.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gtmvfuysjq.html

println("Hello")
来源：http://hz.yj20258.top/gtyepeqspt.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gtvfsqfqmj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dashuyun.cn/gtpqkvxfxg.html

[T03] Kotlin：字符串模板
来源：http://hz.kuanghao11.cn/gtpybmktvr.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gtpmrimsth.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtfnnlcedd.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gtmkxctlpb.html

[T05] Kotlin：when 表达式
来源：http://hz.jiagoushi.top/gtdhstxprr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yonumen.top/gtaiwwqqoi.html

[T06] Kotlin：集合映射
来源：http://hz.zhijiandao.cn/gtptmaizzr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yangfankeji.com/gtzwsghphn.html

[T07] Kotlin：集合过滤
来源：http://hz.wangdashe.top/gtijfcoxeh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinghuilouyu.cn/gthwvmghkt.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gtwvewggls.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtxerovfiw.html

[T09] Kotlin：扩展函数
来源：http://hz.vqdsnc.cn/gtlhkwxvmf.html

fun String.exclaim() = this + "!"
来源：http://hz.snrcjt.cn/gtslrdlqtk.html

[T10] Kotlin：默认参数
来源：http://hz.birdmap.top/gtafplcxkz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhiwuduotai.top/gtvehdepuz.html

[T11] Kotlin：协程
来源：http://hz.zhijiandao.cn/gtxhsbsovg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenzaomai.com/gtcvapgbsy.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtsjtzudls.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258888.top/gtuuljznxw.html

[T13] Kotlin：只读 Map
来源：http://hz.xingfuxueyuan.xyz/gtepamflry.html

val m = mapOf("a" to 1)
来源：http://hz.wangshuangyany.cn/gtkztvtytg.html

[T14] Kotlin：循环
来源：http://hz.shangyingyoupin.top/gtarekrivg.html

for (i in 1..10) println(i)
来源：http://hz.sweek.top/gtaotmxvat.html

[T15] Kotlin：接口
来源：http://hz.zhaomingkeji.xyz/gtajfrmpnw.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtqqltysqm.html

[T16] Swift：Hello World
来源：http://hz.zhaomingkeji.xyz/gtgyhfhlfe.html

print("Hello")
来源：http://hz.gzhubu.top/gtmoxxpqqd.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangtech.top/gtxdfywbjo.html

var a = 1;  let b = 2
来源：http://hz.cqqwz.cn/gthncvfqds.html

[T18] Swift：字符串插值
来源：http://hz.9152youxi.cn/gtkmqxmgcp.html

"值: \(b)"
来源：http://hz.shuidangran.top/gtihphdhix.html

[T19] Swift：可选绑定
来源：http://hz.jinghuilouyu.cn/gtiyxelzgp.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtteanpggt.html

[T20] Swift：数组操作
来源：http://hz.zhijiandao.cn/gtavgjsgfp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuetiantiany.cn/gtapdflvqo.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtcivszmmd.html

for x in a { print(x) }
来源：http://hz.havefunace.top/gtjjhnmecy.html

[T22] Swift：字典
来源：http://hz.chenlongwang.top/gtinhdsnht.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.bjfxy.top/gtycigbqjq.html

[T23] Swift：函数
来源：http://hz.daxiang520.top/gtzwexlaaz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guannengcc.top/gtuxjribvr.html

[T24] Swift：闭包
来源：http://hz.ivvv.top/gtmueuqobp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtzobqdmhw.html

[T25] Swift：结构体
来源：http://hz.zhengqikj.top/gtsohixcsf.html

struct P { var x: Int }
来源：http://hz.sweek.top/gteswoomng.html

[T26] Swift：类与重写
来源：http://hz.yonumen.top/gtkmijbcod.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtmuxjzrak.html

[T27] Swift：错误处理
来源：http://hz.pengpengdd.cyou/gtigpmmqek.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtucpdncpp.html

[T28] Swift：枚举
来源：http://hz.quarkkingdee.top/gtklxicfja.html

enum Color { case red, green }
来源：http://hz.yvedp.cn/gtthbqcbqi.html

[T29] Swift：guard 提前返回
来源：http://hz.tanke756.top/gtrgymoizy.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtxyuxdkbw.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtdwluqrmc.html

protocol Shape { func area() -> Double }
来源：http://hz.xuetiantiany.cn/gttkdbarps.html

[T31] Lua：Hello World
来源：http://hz.yongpay.top/gtgfsukyaz.html

print("Hello")
来源：http://hz.xziqi.cn/gtnxpzvhhj.html

[T32] Lua：局部变量
来源：http://hz.yj20258.top/gtmgolfzfq.html

local a = 1
来源：http://hz.hongshengwenyu.top/gtryovrenn.html

[T33] Lua：表（数组）
来源：http://hz.guannengcc.top/gtzmgoviqm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtvysbvriy.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtjioiyawn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yanxiufei.cn/gtlifkajjx.html

[T35] Lua：字典表
来源：http://hz.wangdashe.top/gtjdgowlzs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258.top/gtplnrwegq.html

[T36] Lua：函数
来源：http://hz.gotoacloud.top/gtqkiizrwy.html

function add(a, b) return a + b end
来源：http://hz.ydzc1.top/gtwqzbftpi.html

[T37] Lua：字符串拼接
来源：http://hz.aibaodan.cn/gtsdapjgdf.html

"a" .. "b"
来源：http://hz.havefunace.top/gtcfnnqrcz.html

[T38] Lua：条件
来源：http://hz.bjfxy.top/gtcsgodlde.html

if x > 0 then print("正") end
来源：http://hz.shuidangran.top/gtrkpsefvr.html

[T39] Lua：模式匹配
来源：http://hz.hongshengwenyu.top/gtnrkgwpym.html

string.find(s, "%d+")
来源：http://hz.xingfuxueyuan.xyz/gteytkdolj.html

[T40] Lua：元表
来源：http://hz.shanyushiyangkeji.top/gtrycmxpus.html

setmetatable({}, { __index = base })
来源：http://hz.nanxuanxn.top/gthqyxpzic.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gtmaqfkvee.html

print "Hello\n";
来源：http://hz.aibaodan.cn/gtdfuwewwh.html

[T42] Perl：变量类型
来源：http://hz.xuetiantiany.cn/gthnkmzaan.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuetiantiany.cn/gtoilljodh.html

[T43] Perl：字符串插值
来源：http://hz.cheryme.top/gtlaavgfni.html

"值: $a"
来源：http://hz.smart0.xyz/gtbtqrkkls.html

[T44] Perl：条件
来源：http://hz.gogol.net.cn/gtymwgsoev.html

if ($a > 0) { print "正"; }
来源：http://hz.daxiang520.top/gtjuberjyf.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtjrpuimfi.html

for my $x (@arr) { print $x; }
来源：http://hz.ivvv.top/gthbrfascx.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gtjxkuqdly.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangshuangyany.cn/gtblaqpjdn.html

[T47] Perl：正则捕获
来源：http://hz.gzhubu.top/gtdfjxdpek.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxuanxn.top/gtawdodboz.html

[T48] Perl：正则替换
来源：http://hz.yj202588.top/gtetqqvotn.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangkeji.top/gtxfbalhyd.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtzpadsnzq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhengqikj.top/gtcuoeeqdu.html

[T50] Perl：逐行读文件
来源：http://hz.zhiwuduotai.top/gtmvfizkuf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtmobctfqg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gaohongyu789.top/gtjchsljdi.html

[T51] Scala：Hello World
来源：http://hz.ywan-chungtsiang.top/gtzoenfgsi.html

println("Hello")
来源：http://hz.aibaodan.cn/gtukicqwiq.html

[T52] Scala：变量
来源：http://hz.chenzaomai.com/gtajbbsawo.html

val a = 1;  var b = 2
来源：http://hz.meibo888.top/gtnkbcrnim.html

[T53] Scala：字符串插值
来源：http://hz.ydzc1.top/gtblpavcpg.html

s"值: $b"
来源：http://hz.52xcode.cn/gtxbmafldt.html

[T54] Scala：集合映射
来源：http://hz.snrcjt.cn/gtrrbmfcua.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tian-w.cn/gtwispkxin.html

[T55] Scala：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtscvdxjbd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hammf.cn/gtuedajydg.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtkhydyqfb.html


<!-- 参考信息 -->