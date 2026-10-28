代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhengqikj.top/gtearfpjhc.html

[R56] 远程拷贝
来源：http://hz.gaohongyu789.top/gtcqxxeynx.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtmkuthrfv.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtudjduumf.html

ssh user@host 'uptime'
来源：http://hz.ehwqpu.com/gtijxxiwus.html

[R58] 下载文件
来源：http://hz.jqgufenzy.top/gtqfupobkl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dianchejie.cn/gtohvkhsso.html

[R59] 发 POST JSON
来源：http://hz.xziqi.cn/gtoasdosdd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aizwys.cn/gtmylxpuqc.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtuopykrzl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtiiurrynn.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtzbcfheka.html

df -h;  du -sh *
来源：http://hz.jinqigfzy.top/gtbgrrbljp.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtwgdewdbd.html

du -ah . | sort -rh | head -10
来源：http://hz.wangdashe.top/gtiuknxscl.html

[R63] 内存与进程
来源：http://hz.guowangkeji.top/gtxuxvmmym.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtzwossuzm.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtkvdogwly.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydzc1.top/gtmcvtxmxs.html

[R65] 查看端口占用
来源：http://hz.yueranfly.top/gtuwpytuqk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.c1oappe.top/gtnarkfxqm.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtpzpdajlq.html

crontab -e;  crontab -l
来源：http://hz.ybcxt.top/gtpmdrvjpj.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gtcgsxolax.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gteylaefgd.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtislahlqu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guowangkeji.top/gtnduemygc.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gthlmretzg.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtimrgdkzi.html

[R70] 时间戳与互转
来源：http://hz.svipenyu.cn/gtdyxqgpbq.html

date +%s;  date -d @1700000000
来源：http://hz.fzhhl.top/gtenaywmxw.html

[R71] 日期格式化
来源：http://hz.kuanghao11.cn/gtqmmtpotq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuanzx.com/gtaxpixqro.html

[R72] 等待端口就绪
来源：http://hz.zhongyouzk.top/gtvqzaaekv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtlptirzwf.html

[R73] 分割大日志
来源：http://hz.yueranfly.top/gtqdgucelu.html

split -l 1000 big.log part_
来源：http://hz.haohaochexian.top/gtvyurigvi.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtgjzjbtry.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtkqtmntye.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtszlffqek.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtadwzautb.html

[R76] 使用临时文件
来源：http://hz.zhixingplan.top/gtjnygdvvj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtaiqyqrps.html

[R77] 读取用户输入
来源：http://hz.kuanghao11.cn/gtisqgwqfn.html

read -rp "请输入: " ans
来源：http://hz.zhoulong.xyz/gtmyxmqnyl.html

[R78] 交互式菜单
来源：http://hz.jiagoushi.top/gtcbtwgmpa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtzpujqfvz.html

[R79] 解析命令行选项
来源：http://hz.fengsongda.top/gtgfdxxtst.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuanzx.com/gtoakfnpgl.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtscbajjop.html

time ./run.sh
来源：http://hz.mhx1999.top/gtnrvjxoiy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpvknomae.html

S. C / C++ 专题
来源：http://hz.ivvv.top/gtlhuwksug.html

================================================================================
来源：http://hz.ydzc1.top/gtjmrrvstq.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtivxqtjxu.html

#include <stdio.h>
来源：http://hz.guannengcc.top/gtzakoeijg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gttogtjsbs.html

[S02] C：变量与格式化输出
来源：http://hz.smart0.xyz/gttiakatpz.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuetiantiany.cn/gtugclgdua.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtjrsxcomy.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gturbntrzl.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtoshameds.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ywan-chungtsiang.top/gtupyzmxau.html

[S05] C：字符串长度
来源：http://hz.yongpay.top/gtiozxvbsr.html

strlen(s)
来源：http://hz.dashuyun.cn/gttetwfvlt.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtxctdwada.html

strcmp(a, b) == 0
来源：http://hz.zhongyouzk.top/gtqsroxllu.html

[S07] C：数组遍历求和
来源：http://hz.meibo888.top/gtvtzugely.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtoeimhkrk.html

[S08] C：动态内存分配与释放
来源：http://hz.ehwqpu.com/gtzcupltuo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtxuluitru.html

[S09] C：结构体定义与初始化
来源：http://hz.tian-w.cn/gtizekuqbx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.feifeiyinyue.top/gtgfwuzymu.html

[S10] C：指针与解引用
来源：http://hz.yvedp.cn/gtsjwwlywe.html

int *p = &a;  *p = 5;
来源：http://hz.shzxlz.cn/gtgodhkxro.html

[S11] C：逐行读文件
来源：http://hz.zhengqikj.top/gttoeosutu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hammf.cn/gtbobrrkjl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangtech.top/gtsbqanugt.html

fclose(f);
来源：http://hz.yj202588.top/gtvtxkwdfg.html

[S12] C：写文件
来源：http://hz.wangdashe.top/gtdeptyxmo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.havefunace.top/gtishsqliw.html

[S13] C：宏定义
来源：http://hz.wangdashe.top/gtzoloaigw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.snrcjt.cn/gtmgsmzrng.html

[S14] C：枚举
来源：http://hz.xinyue.icu/gtiqdahcvg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nwbrower.top/gtvliuvqim.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gtsoaizeyo.html

(double) a / b
来源：http://hz.jianghu66.top/gtmwuwgqug.html

[S16] C：位操作置位
来源：http://hz.zycfv.cn/gtsrlpiphf.html

x |= (1 << 3);
来源：http://hz.daxiang520.top/gttgheqwxj.html

[S17] C：安全拼接字符串
来源：http://hz.chenzaomai.com/gtcvscqluw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jianghu66.top/gtzeguvcju.html

[S18] C：命令行参数
来源：http://hz.cqqwz.cn/gtppwklmls.html

int main(int argc, char **argv)
来源：http://hz.hammf.cn/gtmqavxrhp.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gtutsdmbye.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gttehgvbaw.html

[S20] C：二分查找
来源：http://hz.chenzaomai.com/gtiaknhzrm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtqzjghlbl.html

[S21] C：字符类别判断
来源：http://hz.fengsongda.top/gtnweenssu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtokycjedm.html

[S22] C：字符串转数字
来源：http://hz.xylfe.cn/gtlqwsoxis.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtejiqrliz.html

[S23] C：随机数
来源：http://hz.9152youxi.cn/gthwmghvox.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj202588.top/gtsvoxywfw.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gteztqkydp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gtnqigzgpq.html

[S25] C：内存拷贝
来源：http://hz.cdnleiting.top/gtkxnloodg.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtxqgbezoq.html

[S26] C：内存清零
来源：http://hz.zhixingplan.top/gtxahoshdb.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gtigqwvmam.html

[S27] C：定义常量
来源：http://hz.cqqwz.cn/gtgpzteumm.html

const double PI = 3.14159;
来源：http://hz.yj202588.top/gtnipetqtx.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gtgpguydvb.html

static int counter = 0;
来源：http://hz.sufxvd.cn/gtjmvlattv.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtuejjwxof.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gtjsfjlqpu.html

[S30] C：头文件保护
来源：http://hz.guannengcc.top/gtwyktnqkg.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtgdihttoj.html

#define X_H
来源：http://hz.redwolf501.top/gtsvuuftdi.html

#endif
来源：http://hz.ybcxt.top/gtmhuohnrm.html

[S31] C++：Hello World
来源：http://hz.xinyue.icu/gtqixappbt.html

#include <iostream>
来源：http://hz.jinqigfzy.top/gtaupcgogc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yongpay.top/gtaajdtlqh.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtcdmfsyzb.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258888.top/gtvzqzbsal.html

[S33] C++：vector 增删
来源：http://hz.jinqigfzy.top/gtditpqfwr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.birdmap.top/gtnfoqpdtq.html

[S34] C++：遍历 vector
来源：http://hz.zhaomingkeji.xyz/gteujclcnd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangkeji.top/gttysbjrkj.html

[S35] C++：map
来源：http://hz.xziqi.cn/gtzwddmknh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtlekbzoag.html

[S36] C++：unordered_map
来源：http://hz.kuanghao11.cn/gttkeahkog.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtybgzchmd.html

[S37] C++：set
来源：http://hz.zycfv.cn/gtiqmslcyi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258.top/gtkinvxxqd.html

[S38] C++：排序
来源：http://hz.cdnleiting.top/gtwilvjdnd.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gtbnweyetz.html

[S39] C++：自定义比较器排序
来源：http://hz.iojbl.cn/gtvryrufqs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtfeigicyh.html

[S40] C++：查找元素
来源：http://hz.wangdashe.top/gtyvxbmhma.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.vqdsnc.cn/gtppnmxmxv.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtmceumnsm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cqqwz.cn/gtelllziaq.html

[S42] C++：继承与虚函数
来源：http://hz.daria6918.cn/gtkbjfecng.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenlongwang.top/gtszgaguwg.html

[S43] C++：智能指针
来源：http://hz.ywan-chungtsiang.top/gtcnkyxmxt.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhijiandao.cn/gtluwurcds.html

[S44] C++：引用传参
来源：http://hz.pycfn.com/gteihkwwqe.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtzspyabid.html

[S45] C++：lambda
来源：http://hz.shzxlz.cn/gtqzntuyyu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhongyouzk.top/gtomsgixki.html

[S46] C++：函数模板
来源：http://hz.feifeiyinyue.top/gtecsumkzo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhijiandao.cn/gtyoelowjj.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangkeji.top/gtzsckzhwi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtncfdrkov.html

[S48] C++：逐行读文件
来源：http://hz.snrcjt.cn/gtlkpksmwv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtejhdiyhr.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtdchbmsym.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtgxdavczf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.c1oappe.top/gtdhmquile.html

[S50] C++：格式化数字
来源：http://hz.vqdsnc.cn/gtqjcypgfy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yvedp.cn/gtkkdbrzbi.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtrkiffned.html

static_cast<double>(a) / b
来源：http://hz.fengsongda.top/gtrgzxpdze.html

[S52] C++：const 与 noexcept
来源：http://hz.hongshengwenyu.top/gtvvydrgrw.html

int size() const noexcept { return n_; }
来源：http://hz.kuanghao11.cn/gtlcgabluj.html

[S53] C++：移动语义
来源：http://hz.hammf.cn/gteurkzxhy.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtocqhkcgq.html

[S54] C++：异常处理
来源：http://hz.jqgufenzy.top/gttpwfcrdh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gtojfaowgf.html

[S55] C++：结构化绑定
来源：http://hz.gotoacloud.top/gttaidmany.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gthzxqvlos.html

[S56] C++：optional
来源：http://hz.shangyingyoupin.top/gtofgxvzdn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenzaomai.com/gtoityymey.html

[S57] C++：编译期常量
来源：http://hz.tanke756.top/gtvuhkgadd.html

constexpr int N = 10;
来源：http://hz.jyoumei.cn/gtoprotxhg.html

[S58] C++：命名空间
来源：http://hz.xziqi.cn/gtcjcbbbcx.html

namespace ns { int f() { return 1; } }
来源：http://hz.ppjwa.cn/gtmuexbfew.html

[S59] C++：静态断言
来源：http://hz.andypj.xyz/gtismkthlm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtlprdtfhe.html

[S60] C++：遍历并删除元素
来源：http://hz.zhijiandao.cn/gtgnyvfyyl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtdlzbzngf.html

================================================================================
来源：http://hz.ydzc1.top/gtwhavyipe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gtauuywxvs.html

================================================================================
来源：http://hz.hysaishi.cn/gtrvcezthl.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gtodozjesy.html

println("Hello")
来源：http://hz.yangfankeji.com/gtteydlvjd.html

[T02] Kotlin：变量
来源：http://hz.jqgfzy.top/gtjgtakjji.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtkhkbdlkp.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gtanadjejn.html

"值: $b"
来源：http://hz.ydzc1.top/gttiaxyixh.html

[T04] Kotlin：空安全
来源：http://hz.jqgfzy.top/gtxbynntph.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtbthsbjpv.html

[T05] Kotlin：when 表达式
来源：http://hz.zycfv.cn/gtzpcvcrrk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gthndbhxuz.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtkadvrlou.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pycfn.com/gtgypxpdcn.html

[T07] Kotlin：集合过滤
来源：http://hz.snrcjt.cn/gtfvumypob.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtfbildnsq.html

[T08] Kotlin：数据类
来源：http://hz.316326.xyz/gtifonrhia.html

data class User(val name: String, val age: Int)
来源：http://hz.svipenyu.cn/gtvmktdvqf.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtncqtijnd.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtqjhqpzug.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtzdrtkvdw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ppjwa.cn/gthpbvztut.html

[T11] Kotlin：协程
来源：http://hz.dashuyun.cn/gtexqxpbhe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258888.top/gtesiarnvt.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtfkqngseu.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gtrjksxhlk.html

[T13] Kotlin：只读 Map
来源：http://hz.bjfxy.top/gtdzrvibso.html

val m = mapOf("a" to 1)
来源：http://hz.meibo888.top/gtaqizgxog.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtlxokkgzq.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtkqgoibsb.html

[T15] Kotlin：接口
来源：http://hz.guannengcc.top/gtrwkbueob.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtnlqiucec.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtngwcviqt.html

print("Hello")
来源：http://hz.cheryme.top/gtoqanlksu.html

[T17] Swift：变量与常量
来源：http://hz.wangshuangyany.cn/gtfstxggcv.html

var a = 1;  let b = 2
来源：http://hz.jinghuilouyu.cn/gthwcoylut.html

[T18] Swift：字符串插值
来源：http://hz.redwolf501.top/gtksghsmas.html

"值: \(b)"
来源：http://hz.316326.xyz/gtikxnrpmp.html

[T19] Swift：可选绑定
来源：http://hz.hysaishi.cn/gtrjkvknar.html

if let n = opt { print(n) }
来源：http://hz.ywan-chungtsiang.top/gtcxjrurkh.html

[T20] Swift：数组操作
来源：http://hz.xinyue.icu/gtxfmckxyf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.smart0.xyz/gtjukxfjzr.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtkkknhgzs.html

for x in a { print(x) }
来源：http://hz.hywenlv.cn/gtzdcgciii.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtxqtwqeou.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yongpay.top/gthsfmoqoy.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtwbdctzox.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.kuanghao11.cn/gtynsgaxqv.html

[T24] Swift：闭包
来源：http://hz.shangyingyoupin.top/gtaqdsweva.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.9152youxi.cn/gtbkjyfalq.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gttipjywba.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gtjigidcps.html

[T26] Swift：类与重写
来源：http://hz.hammf.cn/gtspvdehzb.html

class A: Base { override func f() {} }
来源：http://hz.zhengqikj.top/gteydvfwrp.html

[T27] Swift：错误处理
来源：http://hz.chenlongwang.top/gtvcxwatgy.html

do { try f() } catch { print(error) }
来源：http://hz.hfpthk.cn/gtjgevhspj.html

[T28] Swift：枚举
来源：http://hz.chenlongwang.top/gtstbbibfk.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtuelfximn.html

[T29] Swift：guard 提前返回
来源：http://hz.andypj.xyz/gtukehzkvp.html

guard let x = opt else { return }
来源：http://hz.yvedp.cn/gtprjtnbfl.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtthjakmrj.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gtspdmbilt.html

[T31] Lua：Hello World
来源：http://hz.xuanzx.com/gtnfiinftb.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtszhkbygy.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtsmsmvoqo.html

local a = 1
来源：http://hz.shanyushiyangkeji.top/gtiixsoeuo.html

[T33] Lua：表（数组）
来源：http://hz.tianlin.xyz/gtihcjmwsu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258888.top/gtdkyvtjob.html

[T34] Lua：遍历表
来源：http://hz.9152youxi.cn/gtjgxidzgl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxuanxn.top/gtiqmduldd.html

[T35] Lua：字典表
来源：http://hz.zycfv.cn/gtmhnjfcyj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jianghu66.top/gtgmrfmpic.html

[T36] Lua：函数
来源：http://hz.dashuyun.cn/gtptunjvrz.html

function add(a, b) return a + b end
来源：http://hz.xinyue.icu/gtxjynzlul.html

[T37] Lua：字符串拼接
来源：http://hz.smart0.xyz/gtfqdfbjch.html

"a" .. "b"
来源：http://hz.yuxming.cn/gtwsithspq.html

[T38] Lua：条件
来源：http://hz.cdnleiting.top/gtjetawxbm.html

if x > 0 then print("正") end
来源：http://hz.tanke756.top/gtxbkhlgdx.html

[T39] Lua：模式匹配
来源：http://hz.ywan-chungtsiang.top/gtxhdabsbw.html

string.find(s, "%d+")
来源：http://hz.jinqigfzy.top/gtvrmuphqb.html

[T40] Lua：元表
来源：http://hz.gaohongyu789.top/gtswnrmqra.html

setmetatable({}, { __index = base })
来源：http://hz.tianlin.xyz/gteemhjdby.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtqimpmpzs.html

print "Hello\n";
来源：http://hz.tianlin.xyz/gtvfnrarrs.html

[T42] Perl：变量类型
来源：http://hz.zhiwuduotai.top/gtilluqlxs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.daxiang520.top/gtopdnhjel.html

[T43] Perl：字符串插值
来源：http://hz.shuidangran.top/gtragtomgn.html

"值: $a"
来源：http://hz.yuxming.cn/gtrvcqwqtr.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gtovdsuqji.html

if ($a > 0) { print "正"; }
来源：http://hz.yvedp.cn/gtmbisfomr.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtyobmifvb.html

for my $x (@arr) { print $x; }
来源：http://hz.guannengcc.top/gtrahgoxkr.html

[T46] Perl：哈希操作
来源：http://hz.feifeiyinyue.top/gtoufatoey.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgufenzy.top/gtjxcotmbs.html

[T47] Perl：正则捕获
来源：http://hz.jyoumei.cn/gtsrqmadcl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.birdmap.top/gtskqbptxo.html

[T48] Perl：正则替换
来源：http://hz.9152youxi.cn/gtrnhcghij.html

$s =~ s/old/new/g;
来源：http://hz.chenjidiqi.icu/gthrfqkdrm.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gtnexmxgqh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hammf.cn/gtjnecsrmc.html

[T50] Perl：逐行读文件
来源：http://hz.chenlongwang.top/gtemlwfmfi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtylnnookg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jianghu66.top/gttipihdoi.html

[T51] Scala：Hello World
来源：http://hz.shuidangran.top/gtgbkopfdl.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gtydzojevr.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gtctzwxoix.html

val a = 1;  var b = 2
来源：http://hz.chenjidiqi.icu/gttmxaanms.html

[T53] Scala：字符串插值
来源：http://hz.yj20258.top/gtuefeckno.html

s"值: $b"
来源：http://hz.nwbrower.top/gtuizzjhyn.html

[T54] Scala：集合映射
来源：http://hz.9152youxi.cn/gtprvqpohc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhixingplan.top/gtwgsxvbod.html

[T55] Scala：集合过滤
来源：http://hz.sxryk.cn/gtiablvryl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.daria6918.cn/gtreedlnlg.html

[T56] Scala：样例类
来源：http://hz.guannengcc.top/gtrxsrbtbi.html

case class User(name: String, age: Int)
来源：http://hz.tian-w.cn/gtxkthvhzm.html

[T57] Scala：模式匹配
来源：http://hz.snrcjt.cn/gtsejyktjn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.quarkkingdee.top/gtklyxzmxb.html

[T58] Scala：函数定义
来源：http://hz.shanyushiyangtech.top/gtwisivcec.html


<!-- 参考信息 -->