代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzskleol.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttjoghcz.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjaobuyi.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gadtfctyn.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/goiattyzo.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhpadttn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/guexlvkls.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gxcxbstap.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhufwabu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxxmmqlb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gagddkrok.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxpsyiqg.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gflmodown.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbnvmqhu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gawujvbxf.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/giuhikipp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gllhjcuji.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/giawkxnhr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrcmudcv.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpbwnrzu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gheyjnpyn.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gehntvtdn.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gzfguovir.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuqsibrc.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkwyhqen.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghuvdesxr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjrflwec.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gpbmdbmrn.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gfusnbigh.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gscscopxj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpfydmxg.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsnnyeck.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbfixfgf.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/grjmklraq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghccqfgic.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gkajfahtm.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gwsowzjdd.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcvogvpq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gynwyjezf.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnswlqrly.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gnocwncyj.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkpuztvct.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gaxnrtkvs.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwhipujb.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gvmscubev.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/ggucdprqy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsxerfxd.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gyrkpzteb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/geotpndsz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gwflninwf.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/grqwlvrcf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwtperjm.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyemysgq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbscenye.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggooahlvq.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjppgash.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gksaguojf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gznmijufd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsjcmlch.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjamzbpa.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gymsoyusj.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpyqjmxo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gllydgjnk.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/galkpzwjf.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/guicicotg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozdopglj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqojydwjl.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gjlnoymjr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlxkahqx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gnovpeqgu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gjrsyykdh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gimjfxcot.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/grmbdzhcg.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpbdhioz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gslotsftj.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmubeysck.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqbipnuz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtudrnypy.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrxyrbqt.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnadmaep.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgqodlvq.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gazkjdubn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/glatmhusu.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gbryjwsrs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gahhtlyyi.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbehyekkc.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gdrxohuvw.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gqswyvnsu.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gevyqoorq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gzwhaawnq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyckruzxd.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gndjbtiue.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gevtlzien.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxewetwq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/giyxzudta.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gyhytzput.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgagzyer.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gflumhjzv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpwmuxmk.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gctbccaip.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gqmufqqkc.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gavfcyogs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/glrhitfeq.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gsubhtyjo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxcaurci.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbaudqrn.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gdshkajfu.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gdzfkfesi.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gjitueuzt.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwspvvfiw.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghchrksxy.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddrsyimm.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkgtwqby.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzcvoklub.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/guoufzztf.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkemehfj.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvttsoxn.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrbsrhcb.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gvpygdgva.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkokidkhg.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gdtzsfclz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpbqajla.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gozaxncex.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoyhsrxz.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gksuowctj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gswsbcwjx.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gzxkwhjzb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqhjqpqt.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctfstse.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/guunmgdqx.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gxvhgavjf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghedbstuw.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goygnkoar.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsiwvbmq.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxguhkbm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmhbuzfh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjmcfzjh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gzzhpyxme.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiyuchce.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvkxskbz.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gceokhqok.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxokvstc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkuyxkoe.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gpccnvcgp.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjgrunwf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/geyoqriyc.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gvffqdcyx.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazxhvazz.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfgqrffh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gktueaetm.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gcsdqqsos.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtlnjjjnd.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdypmbdnb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijwkypce.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gahpgeoxy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrprvydb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizydeavd.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtntytayi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gsuoqcfto.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gleyxkaqv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ghgxhpczc.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxjozlfas.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjfoflrn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjzeijmk.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczehzige.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvcxgwzp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltinecea.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvugycxtx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ghmrgiehg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqtmubd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gysluvalu.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gqwgbaxie.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzdvecre.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/grqtarxdb.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbybznnul.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmgcbtzu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqyfixdgd.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gejcshblo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gqjzzpsyl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghasqjqeg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvztjfkdv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdifhrupw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpuvgdji.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggznneqjt.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyqvsufj.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggtraiotn.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gaveoemvj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gfhfpqydw.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gucuahduj.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokrzhcui.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdkkbggn.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/guajgurhf.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghrgyxezm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjcjjgul.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtitdyoje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gzhqnstpg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnphzrrg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guysrzyou.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gvhndbusx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhwieqhc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsytqewsm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxheifvi.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtyndngm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqxfsepg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/goepjyjfn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjogvzvg.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gftwrnkqj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppfvxgqk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gigsqzyzj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrwgyggo.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gdxpjfwso.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcdyjuxi.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxjdiwdg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gflqhribz.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grijktemn.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqlhyujm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwohapevc.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvghmfxnb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwulyycq.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/ghhlpqbin.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gwibikzon.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkmvqjip.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gcejdjhjj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgudopmp.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqaqpvpry.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gavnyghwy.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gnvorflmq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjzeeupxi.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdchwealv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/genymjyrn.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gzetipzvt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbahwzqux.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gwkjykhiu.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gvifenqvs.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqpzgymp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrnloimf.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gujelsirs.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhrauvjf.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjvfbmll.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gscgebpsq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhmfbihq.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnnfxlob.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gsushigia.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtwjivjf.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzlrojlpx.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gewywhlfe.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/grwlfcggh.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gmqoofwyg.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gesgwkhzm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gaalkzirq.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzhbvphs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjobxhvis.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptckknwm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gymdfdjef.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqxfodytv.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllvcebow.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gxkfvzhsp.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhqhnwgi.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljmmpydi.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gllhonjjr.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gxwaliion.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gavumbjyr.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtrakgxj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gsfhptppa.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvosshsru.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/ggrptfmfy.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcqyjceb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geywfocag.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gngrqtaca.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/glvdalvri.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gymkrvtvu.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvxpyrsm.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gygcbcoyh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvuuwsnwr.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gzltuhzmc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbclzanv.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzxchual.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkivjsutp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujuspiyi.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gulxmwlbe.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqhwmaqyr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrtsimka.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvmjgzts.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/genltypfy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyyynilu.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtydztzdk.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gqnasopnl.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtwbcqf.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvxhmmrxr.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdkinioqg.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gylcerddn.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/glyyfzurf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gesjwgmkh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/ggettjzdm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqfcaxyf.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/geunbultd.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gyifdhwds.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gizcsswgf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbbaqcmo.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/guxulaunz.sHtML


<!-- 参考信息 -->