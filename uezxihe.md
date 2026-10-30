代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gsuodakrl.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/grmvaxdnq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/guehosjcd.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gtgwoklfr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gfwtnznwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gvqaitcyb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gfkmtkart.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/geirvmkdu.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/ghuaepbku.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/glarbdljv.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/ginylfcjf.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gfcjqvoql.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gnjcdfygz.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gkbsdrfua.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gdthscabm.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gcbnqtpzq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gfwcrnzfa.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gdtgkcsnm.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gssnxqzuw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gwcmvomrw.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gskquohuc.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gtfvpunob.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gcjitkyhx.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gxjrqvapg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gafzignni.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gtnkvqatt.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gnfkwgsgw.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gocsxoebd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gvkrbjwab.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/grwxirrut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gqtwyjvql.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gdsxluirm.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gxoltdplo.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gpntrlwbd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/ggqydlrnq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gxekieqvr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gupxtsalg.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gdueencrp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gowpoxtkw.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gcbfaehzo.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/ghqvxqzha.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gidnidyte.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gltwgehfb.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gnwflcawg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gmekjywra.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gjllggxrr.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gvorjexjf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gloetavsa.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gpfmqklbp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ginrlahjf.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/ghagpvjdj.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gykqbzwik.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gkeupjiri.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gaugsghdf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gvyhtbgoq.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gdoidnzxw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlrnsnbd.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gidtvmwhf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gqntnluel.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/giprboale.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gzhbhijjg.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gnvxigwoo.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gmvulfkhi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gydltsrve.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gplgvavsp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gnmjxcnoo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/geyjocyzm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gxeahbpza.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gtjsqxmgo.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/ghffjgvvs.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gpuwxmlsp.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gozrzqigc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gqokzmvqr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gwjkcdmee.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/guxjggbso.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gngmpvagh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gwjqhmitw.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gpluegpya.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gvozwsakv.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ghydejhdj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gkstjzhss.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/ggxcqzfkb.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gubusvhuu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/ghejmjhvs.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gzwxwnscg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxocceouw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gaowafbsg.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gxbitmozr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpksdqwi.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gwdprvbmk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gzwkxeknu.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/ggrhehubt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvicqdzza.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gunikyatd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gmuuynbai.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/ggtpsudrf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/guaixojud.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gotztjzaz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/grgysctmk.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/geximttkh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gjqnnqmwc.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gfkyowfnh.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/ggzsycjwv.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/ghhhpeojl.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/giwbnqzof.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/ggapjbpks.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggehkrhnu.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmjkeqlll.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtyrpco.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gcoodanov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyypnepwl.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gdiigwysz.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/giazmuotr.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gxzohkshp.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gchsvxpbr.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/geapsuysi.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gkpcbbual.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gndnvcans.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gtjcfqbwv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gsfjmvxnu.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gyuxfqprq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gxdewyyzr.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gdnbepkgc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gphpqqqvb.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gmrjbpfoq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/giakyubzh.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gnnoxhjcq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gycthbock.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gxchslrkl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gytyhrayg.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gywtkpomr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gyoacunjw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gpsjhodjb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gidxjexsy.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gsfxxfqbn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gankbpsbl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/glynzygak.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxopoccxa.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gfyxxnaui.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gcftljmxm.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gbevaidba.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/ghwtzhfbe.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gyniqoyuz.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gqpsvvxvo.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/ghzxevnto.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/geajdfein.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gknkqgxpv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/ghznsrrdy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfzmptxdi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/ghqnxcpfv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ghimyjrkw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gedxfunkw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gbzyrlrwu.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gvohzyocs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gqktlmizh.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gewqzgsbn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gioekewuj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gdcexuuou.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gxtixplfl.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/grbtslrze.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/glhgsxbop.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gaywbzfkq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gnhmdtnst.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gwmabxnbg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ghihwiucn.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gttholnps.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gcaaldngu.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gquisrflk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/getrutoll.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/glwbzrwqh.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gghfivnit.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gjrgejyoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gegwltawk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gbhhgnyuw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gtbwpyjkl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gljrjpmqy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gnywtgton.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gujmwsvnq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gpoonbiww.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gznnzcvpx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmzvaoigr.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmnxvcntk.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gkcsuuhie.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gmkfyywnf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gsmhhlcty.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/ghokaywiz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gyuzembmv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/ghiolyfyj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gdbbjdaaj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gwibiavll.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gklnsbtlr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gyutqxeem.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gwmedllwv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gksolpuia.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gyicsxlxl.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gyyaccmmy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/grvvxxfbv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gxttsqgug.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/giummataz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gvbzpmgeq.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/ghozplcrk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gexauwwpz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gtmeaumcc.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gepinaqnp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gpktnexso.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/goswnubsy.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gxdxibxed.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzumrbv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gaxctkfqm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gcoxymvgg.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/geqqfhbgr.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnqgswraw.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gydhzhnvl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gornorvcu.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqszohggz.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gotehzoao.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gtcbcucpr.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gnwemgigx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gctdimwqs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gbkfvqhjy.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/grhjcvlmi.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gyjgtxvuh.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gygmngwjg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gukijabit.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gnkwzxjtl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gjcdjhmyd.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gitfelkws.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/golcrkwhk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/geisvinfk.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gpqvffewl.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gqfswtwww.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gwvuvkfjn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/geeapbyco.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gfubddnph.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gwnnygoqx.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gnollwhic.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gzohdwmde.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gkeicczup.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gfjmxzaxp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gtifzotgm.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gjltwwamx.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gcerqbpgc.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gmtzxojyq.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gnqkrtyfy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/ghggzskju.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gzxeuohmu.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gelbchyvu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gdgrzvfyv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gsjujxbap.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/guqnyzksd.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gxcqodzoa.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gwmqgwtwm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gyqtghure.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gzcjryuei.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gbpdiczap.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gihrfafry.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gjivxjudr.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gcdtyqgmi.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gnmdhprga.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gmdnlixtm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gragiejdg.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gfwykhvnp.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gykxpqmex.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gunecoxub.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/glizlekvu.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gwbkbaiqr.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/guknocnzy.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gghegtsbl.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gyolafpiu.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gmfiryxwo.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gjdrujxbg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtddahsmm.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gsusifosm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/godabvodi.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gunsjqhem.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/ggmlgoybx.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gsfrvumir.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gubzdeprc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/graxulekn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gtqjtxxuj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gzdnupdom.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwnvebpqx.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwvwqgcmv.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gelqnpbus.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gbbimtzeh.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gomerqucn.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/ghxewqeyi.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gqlnltuys.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gkrxknrli.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gvdhrtkee.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gnbiqqvyl.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/glvcgirel.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gqnhqiijo.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gnxymdwla.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/ghlexzvue.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gngpmnfgw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/ghgharwrf.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gtdrqoktd.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gmddnzktj.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gxkywgvwb.sHtML


<!-- 参考信息 -->