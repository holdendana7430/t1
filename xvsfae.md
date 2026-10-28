代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtgnbecgkk.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtnpmhgyqr.html

scp file user@host:/path/
来源：http://hz.xuetiantiany.cn/gttmijhdzx.html

[R57] 远程执行命令
来源：http://hz.jianghu66.top/gtizgwupzz.html

ssh user@host 'uptime'
来源：http://hz.aizwys.cn/gtaextiubd.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gttfrblvae.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sufxvd.cn/gtfnvewcuf.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtlbwfkldm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dianchejie.cn/gtghxxbtww.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtejpunggj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhijiandao.cn/gtjwqkquok.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtouhjwapm.html

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtnnxpjcxl.html

[R62] 找最占空间的文件
来源：http://hz.shzxlz.cn/gttonfeplc.html

du -ah . | sort -rh | head -10
来源：http://hz.jyoumei.cn/gtgyckahzg.html

[R63] 内存与进程
来源：http://hz.hywenlv.cn/gtxvbhgujz.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gttufipqnf.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtwqnufqdy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hysaishi.cn/gtowbijrkc.html

[R65] 查看端口占用
来源：http://hz.xingfuxueyuan.xyz/gtolqzrynp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtlnrfbpnf.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtxehkqgur.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtobkezymv.html

[R67] 生成随机十六进制串
来源：http://hz.zhengqikj.top/gthvfdxkqn.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gthedqkwuv.html

[R68] 计算文件校验值
来源：http://hz.xinyue.icu/gtrplkdhae.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cucudq.cn/gtkawwpgcw.html

[R69] 生成随机密码
来源：http://hz.jianghu66.top/gtagqkqmpk.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gttvlyxfzc.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtjspgwhoj.html

date +%s;  date -d @1700000000
来源：http://hz.ywan-chungtsiang.top/gttepcgcss.html

[R71] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gtqrlkjoed.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtqtyfmucw.html

[R72] 等待端口就绪
来源：http://hz.ppjwa.cn/gtquudrsbf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yonumen.top/gtgzseklxs.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtfjnbgwox.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtshrfwwvs.html

[R74] 批量重命名
来源：http://hz.mhx1999.top/gtjbkjvfvk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yongpay.top/gtcdsueckb.html

[R75] 导出环境变量
来源：http://hz.dashuyun.cn/gtojcsfvnj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtuwhcennx.html

[R76] 使用临时文件
来源：http://hz.yanxiufei.cn/gtgeeqqlco.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtmpprirsi.html

[R77] 读取用户输入
来源：http://hz.shuidangran.top/gtroeaqddw.html

read -rp "请输入: " ans
来源：http://hz.sysykeji.top/gtvawftaup.html

[R78] 交互式菜单
来源：http://hz.tian-w.cn/gtliepfpuy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gzhubu.top/gtouwlovyd.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtvqxoyrwy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtdemfmhsu.html

[R80] 查看脚本执行耗时
来源：http://hz.quarkkingdee.top/gttkufqqtc.html

time ./run.sh
来源：http://hz.xziqi.cn/gtnisovqmt.html

================================================================================
来源：http://hz.vqdsnc.cn/gtofsmndnx.html

S. C / C++ 专题
来源：http://hz.jyoumei.cn/gtfgtlgydq.html

================================================================================
来源：http://hz.ppjwa.cn/gtuodqppfv.html

[S01] C：Hello World
来源：http://hz.svipenyu.cn/gtpafbwggs.html

#include <stdio.h>
来源：http://hz.ppjwa.cn/gtydzpvbdt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtiflemxjl.html

[S02] C：变量与格式化输出
来源：http://hz.nanxinkj.top/gtfgtdkmyh.html

int a = 10; printf("%d\n", a);
来源：http://hz.jiagoushi.top/gtputvpibs.html

[S03] C：读入整数
来源：http://hz.andypj.xyz/gtltyxhzpz.html

int x; scanf("%d", &x);
来源：http://hz.wangshuangyany.cn/gtignbiacx.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtmoeeigbk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuxming.cn/gtzlgeyvap.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtjbmtsesi.html

strlen(s)
来源：http://hz.pycfn.com/gtfxbmbxgq.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangtech.top/gtmuzdphdc.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gtnyvgkkxg.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtqekpguwa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhengqikj.top/gttymgvkom.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtbdnoucgb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenjidiqi.icu/gtbhwmzgjx.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtkkuajnhy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhaomingkeji.xyz/gthepffxlx.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtrkxlogge.html

int *p = &a;  *p = 5;
来源：http://hz.kuanghao11.cn/gtdftfsmwi.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtqzycufmb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.havefunace.top/gtokxmtgjw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtcgaszzwx.html

fclose(f);
来源：http://hz.vqdsnc.cn/gtkohdyrbf.html

[S12] C：写文件
来源：http://hz.fengsongda.top/gtmfcoambu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtyyhqgfrs.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gttfxycjjz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtylouoywd.html

[S14] C：枚举
来源：http://hz.ydjk.org.cn/gtcjwskkza.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydjk.org.cn/gtylkfkyuu.html

[S15] C：类型转换
来源：http://hz.feifeiyinyue.top/gtdiodmzuh.html

(double) a / b
来源：http://hz.guowangkeji.top/gtbdbqzbbs.html

[S16] C：位操作置位
来源：http://hz.jinqigufen.top/gtpykfpfbk.html

x |= (1 << 3);
来源：http://hz.ydjk.org.cn/gtpisixmmg.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gtdvhgisoi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daxiang520.top/gtcwirmuzd.html

[S18] C：命令行参数
来源：http://hz.haohaochexian.top/gtkgzooatd.html

int main(int argc, char **argv)
来源：http://hz.jinqigfzy.top/gtpcwpwbks.html

[S19] C：快速排序
来源：http://hz.meibo888.top/gtzmizxofr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtdwvzpkkc.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtaylrquht.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtbfjozsam.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gthbmygcrj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtzhlrwtpx.html

[S22] C：字符串转数字
来源：http://hz.aibaodan.cn/gtvckyrzmx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtgmolqfla.html

[S23] C：随机数
来源：http://hz.feifeiyinyue.top/gtstoiocne.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtonavaroe.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtcfkekxlp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gthcjnajsz.html

[S25] C：内存拷贝
来源：http://hz.andypj.xyz/gtjqlaywvi.html

memcpy(dst, src, n);
来源：http://hz.yj20258.top/gtpkgawggl.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtdetmdqju.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtkammkkor.html

[S27] C：定义常量
来源：http://hz.gaohongyu789.top/gtgszrgden.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtnyhccsyn.html

[S28] C：静态变量
来源：http://hz.sxryk.cn/gtumioyiqz.html

static int counter = 0;
来源：http://hz.svipenyu.cn/gtsejtmnci.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gtwxfkorfn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtmewdbzob.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gtxabrwdqm.html

#ifndef X_H
来源：http://hz.yongpay.top/gtuvqlajzk.html

#define X_H
来源：http://hz.sufxvd.cn/gtijkywaux.html

#endif
来源：http://hz.gogol.net.cn/gtphyxuvfh.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtdeuumykh.html

#include <iostream>
来源：http://hz.sweek.top/gttebmartl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xinyue.icu/gtduqnujzy.html

[S32] C++：字符串
来源：http://hz.jinghuilouyu.cn/gtfqyipxhn.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gtibxllpov.html

[S33] C++：vector 增删
来源：http://hz.yongpay.top/gtjgmfeomm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtaxzmhthp.html

[S34] C++：遍历 vector
来源：http://hz.zdqjudy.top/gtzjsczxtc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dashuyun.cn/gtanizvnyg.html

[S35] C++：map
来源：http://hz.zhaomingkeji.xyz/gtlrjnnobj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtnahfrsov.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtxcfzyvai.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtzsraxrrj.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtbcnpgwlu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gthfwodnbm.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtiqjlqbfo.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgfzy.top/gtdrurxxkg.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtnwhklwgo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shuidangran.top/gttamtxihl.html

[S40] C++：查找元素
来源：http://hz.yj20258888.top/gttmvmvclc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtwijimwth.html

[S41] C++：类与构造函数
来源：http://hz.daria6918.cn/gtgjthosot.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtfxbodjfr.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gterxwzpvl.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydzc1.top/gtuxqqiybt.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtylmwbvsf.html

auto p = std::make_unique<int>(5);
来源：http://hz.smart0.xyz/gtkzhgwnjc.html

[S44] C++：引用传参
来源：http://hz.c1oappe.top/gtryjtzcag.html

void inc(int &x) { ++x; }
来源：http://hz.tanke756.top/gtgotzkiqx.html

[S45] C++：lambda
来源：http://hz.xuetiantiany.cn/gtozhwvylh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxinkj.top/gtygtynwuc.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gttledwgek.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shzxlz.cn/gtqoavvjzq.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuetiantiany.cn/gtbrszbdel.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gtgsxwlait.html

[S48] C++：逐行读文件
来源：http://hz.chenzaomai.com/gtzkptzqjn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gthhkhgbbh.html

while (std::getline(in, line)) { }
来源：http://hz.haohaochexian.top/gtgedmiaeb.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtxbzwrfsz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigufen.top/gtulyvtisa.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtfndogvas.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guannengcc.top/gtgmqifyws.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gtuwsfjtkr.html

static_cast<double>(a) / b
来源：http://hz.sufxvd.cn/gtwjdjummo.html

[S52] C++：const 与 noexcept
来源：http://hz.gaohongyu789.top/gtoxyrodmv.html

int size() const noexcept { return n_; }
来源：http://hz.yuxming.cn/gtinmxnjsb.html

[S53] C++：移动语义
来源：http://hz.jinqigfzy.top/gtpntsatpv.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtfzgkrfdd.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gtgwsesakk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tian-w.cn/gthncctcnz.html

[S55] C++：结构化绑定
来源：http://hz.pycfn.com/gtfjbtbdze.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yonumen.top/gtqvipypid.html

[S56] C++：optional
来源：http://hz.yj202588.top/gtasvzvpap.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtozwtykhn.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gtpxhrrhqw.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtpdugpcjk.html

[S58] C++：命名空间
来源：http://hz.cashguo.top/gtwupzjabu.html

namespace ns { int f() { return 1; } }
来源：http://hz.9152youxi.cn/gtbvpzkvrb.html

[S59] C++：静态断言
来源：http://hz.cqqwz.cn/gtpqyewaxo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangdashe.top/gtqosvdvwi.html

[S60] C++：遍历并删除元素
来源：http://hz.yvedp.cn/gthwnoezuu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtvmoerjcg.html

================================================================================
来源：http://hz.0kj1m.cn/gtgpsjzgks.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtvopzrfle.html

================================================================================
来源：http://hz.shzxlz.cn/gtwrypuvue.html

[T01] Kotlin：Hello World
来源：http://hz.redwolf501.top/gtkaokpgbe.html

println("Hello")
来源：http://hz.yj20258888.top/gtzqvcersu.html

[T02] Kotlin：变量
来源：http://hz.jiagoushi.top/gtwzubzybm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gtinotafoy.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gtlrlgsyta.html

"值: $b"
来源：http://hz.xuetiantiany.cn/gtdrlirtpm.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtosokfnja.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gtjatfljlm.html

[T05] Kotlin：when 表达式
来源：http://hz.hnqzz.top/gtpdzqppgz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aizwys.cn/gtaironhyu.html

[T06] Kotlin：集合映射
来源：http://hz.tanke756.top/gtxnsrtevf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cheryme.top/gttzcafydy.html

[T07] Kotlin：集合过滤
来源：http://hz.yuanzhike.top/gtzdrrckmi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtvozyeluk.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gthbsdjjrc.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtharsuerz.html

[T09] Kotlin：扩展函数
来源：http://hz.meibo888.top/gtyprdvoup.html

fun String.exclaim() = this + "!"
来源：http://hz.svipenyu.cn/gtxfcchvgg.html

[T10] Kotlin：默认参数
来源：http://hz.aizwys.cn/gtyivqbahj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gzhubu.top/gtrieblyrf.html

[T11] Kotlin：协程
来源：http://hz.ivvv.top/gtpcavgohj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtjprtzdqt.html

[T12] Kotlin：解构声明
来源：http://hz.svipenyu.cn/gtefvocbad.html

val (a, b) = Pair(1, 2)
来源：http://hz.sysykeji.top/gtjvqwtntj.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtiinmtozj.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtgpdtedfu.html

[T14] Kotlin：循环
来源：http://hz.zycfv.cn/gtwwdcwajq.html

for (i in 1..10) println(i)
来源：http://hz.jinqigfzy.top/gtpayamrbp.html

[T15] Kotlin：接口
来源：http://hz.yj202588.top/gtruwwzyed.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtnenbbnsx.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtvrbbpklt.html

print("Hello")
来源：http://hz.dashuyun.cn/gtuclnejzr.html

[T17] Swift：变量与常量
来源：http://hz.haohaochexian.top/gthecynheu.html

var a = 1;  let b = 2
来源：http://hz.zhijiandao.cn/gtosmmscis.html

[T18] Swift：字符串插值
来源：http://hz.52xcode.cn/gtmjbaduah.html

"值: \(b)"
来源：http://hz.yj20258.top/gtnjpnqwnd.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtbzxjospx.html

if let n = opt { print(n) }
来源：http://hz.zdqjudy.top/gtbsphgwpi.html

[T20] Swift：数组操作
来源：http://hz.hammf.cn/gthktjaanc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtumnpijzu.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtbpifasuj.html

for x in a { print(x) }
来源：http://hz.gzhubu.top/gtgukmhyjq.html

[T22] Swift：字典
来源：http://hz.sweek.top/gtbtjwheqq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtnbjkktgp.html

[T23] Swift：函数
来源：http://hz.jqgfzy.top/gtzxzjwxgx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.0kj1m.cn/gtorzwfndd.html

[T24] Swift：闭包
来源：http://hz.xuanzx.com/gtwkrbvwiu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xziqi.cn/gtjelgfjif.html

[T25] Swift：结构体
来源：http://hz.zhengqikj.top/gtbdrvynim.html

struct P { var x: Int }
来源：http://hz.wangdashe.top/gtmdeakmwj.html

[T26] Swift：类与重写
来源：http://hz.hysaishi.cn/gtroepkwri.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtileenifo.html

[T27] Swift：错误处理
来源：http://hz.ybcxt.top/gtvpwhtomi.html

do { try f() } catch { print(error) }
来源：http://hz.zhoulong.xyz/gthfxgfiqs.html

[T28] Swift：枚举
来源：http://hz.xuetiantiany.cn/gtlhyhgmlc.html

enum Color { case red, green }
来源：http://hz.mhx1999.top/gtaijducnl.html

[T29] Swift：guard 提前返回
来源：http://hz.xylfe.cn/gteitmbjwe.html

guard let x = opt else { return }
来源：http://hz.smart0.xyz/gtwijvriwe.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gtdxoykhho.html

protocol Shape { func area() -> Double }
来源：http://hz.jiagoushi.top/gtmunipeei.html

[T31] Lua：Hello World
来源：http://hz.wangdashe.top/gtjtbtocdt.html

print("Hello")
来源：http://hz.jqgfzy.top/gtenbmublt.html

[T32] Lua：局部变量
来源：http://hz.316326.xyz/gtzedweiir.html

local a = 1
来源：http://hz.zycfv.cn/gtmbvktofb.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gtrvlbpsii.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.chenjidiqi.icu/gteesuvxbv.html

[T34] Lua：遍历表
来源：http://hz.mhx1999.top/gtejqlmfnm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtfhouxtda.html

[T35] Lua：字典表
来源：http://hz.tanke756.top/gthitomycu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nwbrower.top/gtiadhwgic.html

[T36] Lua：函数
来源：http://hz.ydjk.org.cn/gtlsmkhihc.html

function add(a, b) return a + b end
来源：http://hz.shangyingyoupin.top/gtngathsxc.html

[T37] Lua：字符串拼接
来源：http://hz.chenzaomai.com/gtycumnpzw.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtlqfxjice.html

[T38] Lua：条件
来源：http://hz.tanke756.top/gtcbgdroce.html

if x > 0 then print("正") end
来源：http://hz.xuanzx.com/gttewuzeai.html

[T39] Lua：模式匹配
来源：http://hz.birdmap.top/gtpeyefbzn.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtuzcjasgk.html

[T40] Lua：元表
来源：http://hz.wangshuangyany.cn/gtdusrwtcj.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gtfkdecooy.html

[T41] Perl：Hello World
来源：http://hz.316326.xyz/gtvsnspvgy.html

print "Hello\n";
来源：http://hz.xziqi.cn/gtotqjlreh.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gtwslfhini.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cashguo.top/gthmblqzyr.html

[T43] Perl：字符串插值
来源：http://hz.yj202588.top/gttlhigqyx.html

"值: $a"
来源：http://hz.xuetiantiany.cn/gtwcyvbjer.html

[T44] Perl：条件
来源：http://hz.shzxlz.cn/gtcpowpajf.html

if ($a > 0) { print "正"; }
来源：http://hz.yuxming.cn/gthowngryv.html

[T45] Perl：数组遍历
来源：http://hz.mhx1999.top/gtwbjcgwxm.html

for my $x (@arr) { print $x; }
来源：http://hz.gogol.net.cn/gtwsnkqwkn.html

[T46] Perl：哈希操作
来源：http://hz.jinghuilouyu.cn/gtbvhblicc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jlsjyb.cn/gtaeuwzref.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtzuqnrkyf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.tianlin.xyz/gtupkgjafc.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtdlrjpdyu.html

$s =~ s/old/new/g;
来源：http://hz.jinghuilouyu.cn/gtownbtxhh.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gtwcqsftyb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gogol.net.cn/gtyfxgcgwi.html

[T50] Perl：逐行读文件
来源：http://hz.sxryk.cn/gtzzwisqem.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.9152youxi.cn/gtdwkhvlqs.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yuanzhike.top/gtniqxvozx.html

[T51] Scala：Hello World
来源：http://hz.jyoumei.cn/gtwuhffrnz.html

println("Hello")
来源：http://hz.wangdashe.top/gtzjsvihfv.html

[T52] Scala：变量
来源：http://hz.shuidangran.top/gthyhijugw.html

val a = 1;  var b = 2
来源：http://hz.sysykeji.top/gtdoczdbnx.html

[T53] Scala：字符串插值
来源：http://hz.birdmap.top/gtfskwbyqw.html

s"值: $b"
来源：http://hz.ybcxt.top/gtktxbonao.html

[T54] Scala：集合映射
来源：http://hz.daxiang520.top/gtttxjyddb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.kuanghao11.cn/gtbmlvdcjk.html

[T55] Scala：集合过滤
来源：http://hz.wangdashe.top/gtjlpnvrdm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cqqwz.cn/gtaycbxcmn.html

[T56] Scala：样例类
来源：http://hz.xuanzx.com/gtovcaxuhs.html

case class User(name: String, age: Int)
来源：http://hz.yanxiufei.cn/gtmuvgfzab.html

[T57] Scala：模式匹配
来源：http://hz.chenlongwang.top/gtuyrldrvc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gzhubu.top/gtngccaoqh.html

[T58] Scala：函数定义
来源：http://hz.jinqigfzy.top/gtdmddsntp.html


<!-- 参考信息 -->