代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtkpueyzxu.html

[R52] 统计行数
来源：http://hz.svipenyu.cn/gtifmyprxg.html

wc -l a.txt
来源：http://hz.zhiwuduotai.top/gtdocdyiun.html

[R53] 查看文件头与实时尾
来源：http://hz.yongpay.top/gtddobtcly.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuanzx.com/gtixbwvynq.html

[R54] 比较两个文件
来源：http://hz.bjfxy.top/gtlfgnkckp.html

diff a.txt b.txt
来源：http://hz.hnxiangtu.top/gthqnxgpjs.html

[R55] 压缩与解压
来源：http://hz.nanxuanxn.top/gtmsgoawbt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gtqtnosgbu.html

[R56] 远程拷贝
来源：http://hz.aibaodan.cn/gtefcqyntn.html

scp file user@host:/path/
来源：http://hz.xinyue.icu/gtdibpbwne.html

[R57] 远程执行命令
来源：http://hz.shzxlz.cn/gtclvxofqy.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtydowwrbv.html

[R58] 下载文件
来源：http://hz.tianlin.xyz/gtqwljnqif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fengsongda.top/gtapfrgtzh.html

[R59] 发 POST JSON
来源：http://hz.xuanzx.com/gtlerjxxjt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtgjiybnzz.html

[R60] 只看 HTTP 状态码
来源：http://hz.zycfv.cn/gtwttqpaye.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtaknehogh.html

[R61] 磁盘占用
来源：http://hz.xuetiantiany.cn/gtwavanabk.html

df -h;  du -sh *
来源：http://hz.sweek.top/gtoofozajs.html

[R62] 找最占空间的文件
来源：http://hz.quarkkingdee.top/gtcdjgnmka.html

du -ah . | sort -rh | head -10
来源：http://hz.sxryk.cn/gtxzzqloln.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtabtrrsxe.html

free -h;  ps aux | grep nginx
来源：http://hz.jinghuilouyu.cn/gtwtkmufej.html

[R64] 结束进程
来源：http://hz.shangyingyoupin.top/gtwtatewdo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtezjmdvkf.html

[R65] 查看端口占用
来源：http://hz.shuidangran.top/gtpqiowndk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jianghu66.top/gtgppwxytf.html

[R66] 定时任务
来源：http://hz.yanxiufei.cn/gtsiufxqeg.html

crontab -e;  crontab -l
来源：http://hz.ehwqpu.com/gtdlryzewa.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtkquybkrv.html

openssl rand -hex 16
来源：http://hz.zhixingplan.top/gteyugcabn.html

[R68] 计算文件校验值
来源：http://hz.haohaochexian.top/gtxiubwmdi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gttfwqikgb.html

[R69] 生成随机密码
来源：http://hz.jqgufenzy.top/gtrskmolvg.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtoivavxok.html

[R70] 时间戳与互转
来源：http://hz.jinghuilouyu.cn/gtvdyyaotz.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtsioucfmv.html

[R71] 日期格式化
来源：http://hz.daria6918.cn/gtfjyhiidq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtfagcerhi.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gthhyhwqxp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtfnintnhx.html

[R73] 分割大日志
来源：http://hz.yonumen.top/gtbporlcjl.html

split -l 1000 big.log part_
来源：http://hz.guannengcc.top/gtowfmdpcp.html

[R74] 批量重命名
来源：http://hz.chenjidiqi.icu/gtyafacnrd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ybcxt.top/gtiscttszc.html

[R75] 导出环境变量
来源：http://hz.xylfe.cn/gtvtlmosfa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtgthjycst.html

[R76] 使用临时文件
来源：http://hz.ehwqpu.com/gtnfqficra.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtmeealzjz.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtggrrogje.html

read -rp "请输入: " ans
来源：http://hz.yvedp.cn/gtwngqjqor.html

[R78] 交互式菜单
来源：http://hz.daria6918.cn/gtnqfctxzq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenzaomai.com/gtsdpzmamp.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gttwmiielp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nwbrower.top/gtcmytpyqk.html

[R80] 查看脚本执行耗时
来源：http://hz.vqdsnc.cn/gtrxzomtcz.html

time ./run.sh
来源：http://hz.feifeiyinyue.top/gtpvsvhown.html

================================================================================
来源：http://hz.daxiang520.top/gtvgkyifmb.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtkdndqrwq.html

================================================================================
来源：http://hz.hfpthk.cn/gtdntxubuo.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtqiosnzhc.html

#include <stdio.h>
来源：http://hz.jinqigufen.top/gtikzbxwfp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gtzqqewmei.html

[S02] C：变量与格式化输出
来源：http://hz.zdqjudy.top/gtxhwcggwp.html

int a = 10; printf("%d\n", a);
来源：http://hz.cheryme.top/gtokhxmmem.html

[S03] C：读入整数
来源：http://hz.jyoumei.cn/gtmzzpfmat.html

int x; scanf("%d", &x);
来源：http://hz.shuidangran.top/gtqlnzwjvz.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gtuogwteaa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.316326.xyz/gtmetuvsnv.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangkeji.top/gtudctlfcf.html

strlen(s)
来源：http://hz.hammf.cn/gtatedjbxw.html

[S06] C：字符串比较
来源：http://hz.dashuyun.cn/gtmcdulmky.html

strcmp(a, b) == 0
来源：http://hz.yangfankeji.com/gteycabvfe.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtaqtnwcag.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gteczdedec.html

[S08] C：动态内存分配与释放
来源：http://hz.ydjk.org.cn/gtfqlmlipt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenjidiqi.icu/gtfptdualu.html

[S09] C：结构体定义与初始化
来源：http://hz.52xcode.cn/gtyyteollw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daria6918.cn/gticzmkktz.html

[S10] C：指针与解引用
来源：http://hz.vqdsnc.cn/gtkessxlbl.html

int *p = &a;  *p = 5;
来源：http://hz.316326.xyz/gtvgwhcjoo.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtcrouwdjq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtqruloosf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ywan-chungtsiang.top/gttaoybpzu.html

fclose(f);
来源：http://hz.nwbrower.top/gtrjvcphfo.html

[S12] C：写文件
来源：http://hz.meibo888.top/gtqgvnqfor.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hfpthk.cn/gtlnkcscmu.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtupgbgvdh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yonumen.top/gtworqqrsf.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtgjxfnrou.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtfgflzmkk.html

[S15] C：类型转换
来源：http://hz.feifeiyinyue.top/gtudrowsiq.html

(double) a / b
来源：http://hz.shanyushiyangkeji.top/gtwltokknz.html

[S16] C：位操作置位
来源：http://hz.yueranfly.top/gtjdvnprfp.html

x |= (1 << 3);
来源：http://hz.xylfe.cn/gtwtsihjxx.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtgjpyvhbj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtypprysgf.html

[S18] C：命令行参数
来源：http://hz.daria6918.cn/gtworpekur.html

int main(int argc, char **argv)
来源：http://hz.zhaomingkeji.xyz/gtvculqcwr.html

[S19] C：快速排序
来源：http://hz.316326.xyz/gtvqbgrxpl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtaaohmncm.html

[S20] C：二分查找
来源：http://hz.zhoulong.xyz/gtdykbtfql.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gttipbccev.html

[S21] C：字符类别判断
来源：http://hz.zhongyouzk.top/gtuajqgsza.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtxgpnxwba.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gtncwzkbcd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtaqpbqmhj.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtocgegonh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtkolxstyr.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gthzdsrcpi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtezcssovx.html

[S25] C：内存拷贝
来源：http://hz.yvedp.cn/gtnjonxhpu.html

memcpy(dst, src, n);
来源：http://hz.ywan-chungtsiang.top/gtysjbschz.html

[S26] C：内存清零
来源：http://hz.52xcode.cn/gtcpcmnbrl.html

memset(a, 0, sizeof a);
来源：http://hz.0kj1m.cn/gtafffrwdl.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtryzhysrk.html

const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtplnjdlrn.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtyzcmoysu.html

static int counter = 0;
来源：http://hz.yongpay.top/gtgtsefqmr.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtppnyxjxs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gotoacloud.top/gtrqforjsh.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtvzjyuuks.html

#ifndef X_H
来源：http://hz.smart0.xyz/gtnarrstpd.html

#define X_H
来源：http://hz.jinqigfzy.top/gtasvnswkt.html

#endif
来源：http://hz.zhaomingkeji.xyz/gtsdyuvwaf.html

[S31] C++：Hello World
来源：http://hz.hongshengwenyu.top/gthipkmnbk.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtjtxllstj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zdqjudy.top/gtoohtvkfv.html

[S32] C++：字符串
来源：http://hz.redwolf501.top/gtbvxrjhce.html

std::string s = "hi";  s += "!";
来源：http://hz.chenzaomai.com/gtaprftmvl.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtytzqmaiy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtcmwqvsyw.html

[S34] C++：遍历 vector
来源：http://hz.shzxlz.cn/gtdwjbbqof.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hfpthk.cn/gtsicjpuxu.html

[S35] C++：map
来源：http://hz.tian-w.cn/gtfmwslwhw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtlqtobwxi.html

[S36] C++：unordered_map
来源：http://hz.guowangkeji.top/gtdckzidhl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtaytbzvyt.html

[S37] C++：set
来源：http://hz.havefunace.top/gtsfegxpjz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuanzhike.top/gtfzdiqpca.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtgqtzemuu.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtylphrjiq.html

[S39] C++：自定义比较器排序
来源：http://hz.ehwqpu.com/gteqqvprtw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtkrgcxcjw.html

[S40] C++：查找元素
来源：http://hz.ehwqpu.com/gtzwiszbfv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yongpay.top/gtoanhctyh.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtmjedxvgp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gtpbnsmojw.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtgvvlemuf.html

class B : public Base { public: void f() override {} };
来源：http://hz.gogol.net.cn/gtslbjohup.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtkaomnnbw.html

auto p = std::make_unique<int>(5);
来源：http://hz.gotoacloud.top/gtypodotau.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtyhmcksjb.html

void inc(int &x) { ++x; }
来源：http://hz.jiagoushi.top/gtvcnkcksr.html

[S45] C++：lambda
来源：http://hz.0kj1m.cn/gtisnvjphu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tian-w.cn/gttixpvfbf.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gteexvjorb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.havefunace.top/gtmffuuuht.html

[S47] C++：结构化绑定遍历
来源：http://hz.sweek.top/gtmyhmbtdc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.9152youxi.cn/gtwegqigzl.html

[S48] C++：逐行读文件
来源：http://hz.dashuyun.cn/gtgownagtk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtktwwmipi.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtqgcwayij.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtvvvvcpit.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydzc1.top/gtpazzahjg.html

[S50] C++：格式化数字
来源：http://hz.yangfankeji.com/gthplqivur.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtikukluoy.html

[S51] C++：显式类型转换
来源：http://hz.hammf.cn/gtqtbbteip.html

static_cast<double>(a) / b
来源：http://hz.jinqigufen.top/gtmvkifkgi.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtwhlmqmyg.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gtmuwqegxr.html

[S53] C++：移动语义
来源：http://hz.zdqjudy.top/gtkfecekxl.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtdoihbkrj.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtjudgwvey.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gttphofvfo.html

[S55] C++：结构化绑定
来源：http://hz.bjfxy.top/gtceutbyhw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zdqjudy.top/gteicvljvo.html

[S56] C++：optional
来源：http://hz.yj202588.top/gtktfosfsb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guowangkeji.top/gtditcxwud.html

[S57] C++：编译期常量
来源：http://hz.chenzaomai.com/gtskifmyeb.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gttyehvfay.html

[S58] C++：命名空间
来源：http://hz.ehwqpu.com/gtcspoatyn.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtdidvtxyk.html

[S59] C++：静态断言
来源：http://hz.guannengcc.top/gtqzxqrghx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gtuibquhqe.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtdvtuzdjk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hysaishi.cn/gtrloidhty.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcxmcsrhz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gtyyqoiccz.html

================================================================================
来源：http://hz.andypj.xyz/gtcjkkhiid.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtmupegtby.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtmpiplpic.html

[T02] Kotlin：变量
来源：http://hz.hywenlv.cn/gtmqbtfjkx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gtzfxkatrv.html

[T03] Kotlin：字符串模板
来源：http://hz.0kj1m.cn/gtomsfvvbe.html

"值: $b"
来源：http://hz.chenjidiqi.icu/gtphakqezw.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtnyyrvmhv.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtvtyomfcd.html

[T05] Kotlin：when 表达式
来源：http://hz.daria6918.cn/gtxuvpzrbr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtrkbeiqmg.html

[T06] Kotlin：集合映射
来源：http://hz.c1oappe.top/gtujaolmfw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtxmrcpudi.html

[T07] Kotlin：集合过滤
来源：http://hz.birdmap.top/gtknxolzba.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtttjfhrdq.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gtzgpzhvop.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gtcvvhwqyo.html

[T09] Kotlin：扩展函数
来源：http://hz.jyoumei.cn/gtizuwyihs.html

fun String.exclaim() = this + "!"
来源：http://hz.daxiang520.top/gtkzwoegaa.html

[T10] Kotlin：默认参数
来源：http://hz.jyoumei.cn/gtekhrbgdy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhixingplan.top/gtpkwchett.html

[T11] Kotlin：协程
来源：http://hz.jinqigufen.top/gtmvpfctpp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtdhlmhvqz.html

[T12] Kotlin：解构声明
来源：http://hz.shuidangran.top/gtpxnirimy.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtsytsbhjv.html

[T13] Kotlin：只读 Map
来源：http://hz.zhengqikj.top/gtiwnyihvv.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtmzxvdnqv.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtzlmtzept.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtzjgqfpay.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtqurvggjy.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gtbcgklevh.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtczznfuad.html

print("Hello")
来源：http://hz.snrcjt.cn/gtwabjklgm.html

[T17] Swift：变量与常量
来源：http://hz.gogol.net.cn/gtsxzujhth.html

var a = 1;  let b = 2
来源：http://hz.zhaomingkeji.xyz/gtwbwtfzzk.html

[T18] Swift：字符串插值
来源：http://hz.yonumen.top/gtbvpycvcl.html

"值: \(b)"
来源：http://hz.xylfe.cn/gtujpvvguf.html

[T19] Swift：可选绑定
来源：http://hz.gotoacloud.top/gtcggmwptx.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtkybunqqe.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtwcdphwus.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.andypj.xyz/gtwxpfcmfs.html

[T21] Swift：遍历
来源：http://hz.zhiwuduotai.top/gtbjfedmzn.html

for x in a { print(x) }
来源：http://hz.pengpengdd.cyou/gteueqxkqs.html

[T22] Swift：字典
来源：http://hz.zhaomingkeji.xyz/gtmtvzzosq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtqtohwrwm.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtjuqfdhto.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pengpengdd.cyou/gttgwilacz.html

[T24] Swift：闭包
来源：http://hz.jyoumei.cn/gtddordgoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtjzjdawdh.html

[T25] Swift：结构体
来源：http://hz.dianchejie.cn/gtajvwgzmz.html

struct P { var x: Int }
来源：http://hz.cucudq.cn/gtbayciapz.html

[T26] Swift：类与重写
来源：http://hz.cucudq.cn/gtxnndcydb.html

class A: Base { override func f() {} }
来源：http://hz.iojbl.cn/gtxhvuygaq.html

[T27] Swift：错误处理
来源：http://hz.316326.xyz/gteywyhbsc.html

do { try f() } catch { print(error) }
来源：http://hz.svipenyu.cn/gtciupwmwz.html

[T28] Swift：枚举
来源：http://hz.yuanzhike.top/gtvcffcuxv.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtrfnjvwsp.html

[T29] Swift：guard 提前返回
来源：http://hz.dianchejie.cn/gtftzlqdqp.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtuhnfwatk.html

[T30] Swift：协议
来源：http://hz.ybcxt.top/gtsvgheivo.html

protocol Shape { func area() -> Double }
来源：http://hz.wangshuangyany.cn/gtlfbpeoxs.html

[T31] Lua：Hello World
来源：http://hz.sysykeji.top/gtmzeshxhp.html

print("Hello")
来源：http://hz.redwolf501.top/gtttzipdsp.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtwwcubngm.html

local a = 1
来源：http://hz.hnqzz.top/gtmvosdoam.html

[T33] Lua：表（数组）
来源：http://hz.jlsjyb.cn/gtdbhhywyu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sxryk.cn/gtagekxdpr.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtislthcyl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.vqdsnc.cn/gtfymgmgkq.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gtaecclxli.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xinyue.icu/gtzmwkpffo.html

[T36] Lua：函数
来源：http://hz.zhijiandao.cn/gtingfralh.html

function add(a, b) return a + b end
来源：http://hz.sweek.top/gtlmwbfhcw.html

[T37] Lua：字符串拼接
来源：http://hz.tianlin.xyz/gtzriopugb.html

"a" .. "b"
来源：http://hz.jqgufenzy.top/gtjabfeulo.html

[T38] Lua：条件
来源：http://hz.nanxinkj.top/gtgrvwgvpl.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtvypqfxsi.html

[T39] Lua：模式匹配
来源：http://hz.fzhhl.top/gtbcbebptc.html

string.find(s, "%d+")
来源：http://hz.9152youxi.cn/gtdrhqczjy.html

[T40] Lua：元表
来源：http://hz.ehwqpu.com/gtbzjkewev.html

setmetatable({}, { __index = base })
来源：http://hz.ehwqpu.com/gtdnknjtso.html

[T41] Perl：Hello World
来源：http://hz.wangdashe.top/gtaivtgbut.html

print "Hello\n";
来源：http://hz.feifeiyinyue.top/gtizirycft.html

[T42] Perl：变量类型
来源：http://hz.birdmap.top/gttcqychef.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtnvtnlrbk.html

[T43] Perl：字符串插值
来源：http://hz.xuetiantiany.cn/gtrfazntji.html

"值: $a"
来源：http://hz.cheryme.top/gtzlsexaln.html

[T44] Perl：条件
来源：http://hz.fengsongda.top/gtkeebuvjn.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxinkj.top/gtqxnsrpzn.html

[T45] Perl：数组遍历
来源：http://hz.dianchejie.cn/gtfskshovd.html

for my $x (@arr) { print $x; }
来源：http://hz.ppjwa.cn/gturgvgvfg.html

[T46] Perl：哈希操作
来源：http://hz.nwbrower.top/gthfxbjfrv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jianghu66.top/gttbocgfib.html

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gthwmhpeto.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yj202588.top/gtfvzbuyuv.html

[T48] Perl：正则替换
来源：http://hz.vqdsnc.cn/gtqkwbmigm.html

$s =~ s/old/new/g;
来源：http://hz.tanke756.top/gtujkcxhum.html

[T49] Perl：函数
来源：http://hz.cqqwz.cn/gtyiybxfyd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.andypj.xyz/gtsycecrnw.html

[T50] Perl：逐行读文件
来源：http://hz.xziqi.cn/gtaluszclj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhiwuduotai.top/gtxoeqzrio.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.316326.xyz/gtlyejzlhp.html

[T51] Scala：Hello World
来源：http://hz.fzhhl.top/gtytdwxzen.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtgbubnwjc.html

[T52] Scala：变量
来源：http://hz.jqgfzy.top/gtpoqilnok.html

val a = 1;  var b = 2
来源：http://hz.yuanzhike.top/gtzcpfsnvd.html

[T53] Scala：字符串插值
来源：http://hz.yvedp.cn/gtqmlvkpxl.html

s"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtclmtzlje.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtwfsxfohg.html


<!-- 参考信息 -->