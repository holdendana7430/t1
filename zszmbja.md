代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gccgcujdn.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gsycsruhf.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/ghonvizrh.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gffogtqkm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/ghclmeajj.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gkkjopxlo.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gqaqqpgzz.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gtiyiaggz.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/grhhgdiad.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/grggprxzg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gjwwjcpxe.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gtidimybg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gvfpdnhhm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gzyegwgzm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gbpznbile.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/grxcnynjo.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/ggjewubbi.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gthfzhnnd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gponjuwzi.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gfwivemti.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/ggetlidzp.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/guzhahhuu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gojmgjgto.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gqqvrfouy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gjpippcno.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gklpfvzsn.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/glpbuyngi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gsoapkhlj.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/grdmzgvry.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/ghuyvajsr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/glefwpqmu.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gfvzevfqe.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gcikgfaah.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gdsfmcnwh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gpkjoyuun.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gluzoylyn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gupfxvymy.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/giygwsjcv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gnyoyuyuu.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmtvntz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gwoxftpoc.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gcoygfapp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gosxjswej.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/guqalcitg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/guqmkckvn.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ggerqbzbe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gwbjgpeww.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ghvzkciiq.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/goztrrxcx.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gfofpcvkt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/grvdmdyni.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gyrppudvm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/goiycdjta.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gkzefzkbi.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gdqtdyedf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjbwbvmfk.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gfapoyokf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpnavrvef.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzttkqnvx.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gddhrlutn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gutzijoeb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gkiymfcmw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gteypjrqs.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gsgsmexco.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gniillppe.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gmflwbwpr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gkqhpmnls.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gbojyvjpc.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/ghupyvewo.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gfcynacfx.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gzmcvauhd.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gltsnqcir.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gdheamvip.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gyseqzlij.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/golamktzh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gmydgodwd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gdyjuwrda.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gxlzghntd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/giinsvlhq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gzjeyqtrg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gvjfdakas.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gzzrvmtil.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gkpluxiqy.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gszlyonjt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gpmpbimls.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gjochvfkz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/ggxtyntfa.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/glrpuzagi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gtvdlhaeh.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gobzjcsvo.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gqryqywgm.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gcxrbqplg.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gyyvkahlz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gletqlxdq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gddoelqco.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gmmnjucig.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gciwatyfh.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/ghbikvhac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gylklnnql.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gshcvyyvr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwtfyloeh.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gqikyrvox.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/grgbwyzfv.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/guyqinozy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gnhmfqanx.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gjrjarrdv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gvehxpkzw.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gjebzfnql.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/grgoooyrq.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gjrwaafmu.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gecbwzlbf.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gtzujnuli.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gmzrewpmp.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gflbczsdy.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gnqejmopj.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gcwsobbnx.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gqrsuskzg.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gywtcifxi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gvavpdhrf.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gdulfjsbn.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gzqhumppz.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gjzshpbyv.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gdndgpfob.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjvdhaemq.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gmaruvkmv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/goijackhs.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gtyavvkqm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gvwtkrcma.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/ghvepyitx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gdgowidlu.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gznmwtwly.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gyjxablsu.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gsrqamhow.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gpgfdvrig.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gcdqyalic.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpneumjmy.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gfyprkbei.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gayaitxeq.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gbtmlhzqd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gzvmydqde.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gwzeimnsa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/grtyvplrw.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/golgjlihv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gdsocnomm.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gmqwdknvl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gtfuyeijk.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gctioeyfs.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gawotnzka.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gnxbdbxuk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gcgyhfoor.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gteoyadsg.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gwjcnnzyx.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gsuizasbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/goifhsijo.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gyfpmvqxg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gllmvxbis.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gbsmztofa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/giqqkxdgf.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvkzbgdzd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gnbrgzxyv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/glukgzdms.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ggxasxybn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gwzrujvgj.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gusmhczbi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/guosimusi.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gsuuzztwd.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/grxywqbbi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gxlkmookj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gweqlmmwo.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gvcovkxvc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gzvftbzoy.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gfvoljkna.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gfdikhdul.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gicakaigf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gyvglryxk.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gyzcbyjfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/ggstftefv.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gywzrpfyj.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/grdleeihy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gureyncnh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gcxhaniaa.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gnnkyxrzf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gqwnoptmf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gyfglytzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gjdecdpdv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gywcqqbrb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gvnxzfqxn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwtfkravv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gxalmszer.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gshmlenej.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/grpucsqbe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gseseqpyb.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gigojpmcu.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gaiiwafjy.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/ghnvgcmub.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gqwvocvhv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfybmaetr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gfzuyihnp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gzwwfdrem.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gvmqkluyl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gdhbegkfp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gweotnfso.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gydvxtgrg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gjagkhpmv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gkgmsxatp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gkvnyfopi.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gckyorhil.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/glyoduyzi.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gjydwafkz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gfoeldfzx.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gqsiabwcl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gzixreofu.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gypsntvbo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyyddybfp.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gxhtmnffe.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/ggrizakeu.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gssfccphx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gefrwydww.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/glguqnciq.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ganauhlos.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/glrxoyazl.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gcvnikgfs.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmnlewcgl.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gufocyxfw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/grdhtwyef.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/grixevteo.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/ghvxwttyc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gnixegqkd.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gobqfddqx.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/ghbiwwgwt.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpobgdxay.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gpzpwoqzt.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gfmocjodo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gslryjljp.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gxcfxgguy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gjribdmcp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gvxaonrgr.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gucazibls.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gpazofgzu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gslpoepkq.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gfycbwxbo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gfvwkovib.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gveahdbgc.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gikpefwmy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gfmrmtzrc.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gvrbvogxh.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gpfxjhmkg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gcxpkxaoa.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grrolysxr.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmaviingk.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gkisrrptf.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gblrsggaj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gpxnxjjgk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gloapapsp.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gnftlywwp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gfyhhkozc.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gyvgdirek.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gwukkzjbx.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gufencuku.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gvasudglk.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/giugqtakl.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/grcikfgpp.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gptrijlls.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gcwojrbef.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/givgjdgii.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gwbpuyzpv.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gtmsaonnd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gxpfpsoto.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gnpenilgi.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/glzlndafs.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gcdmibpii.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gjbxbuves.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gvdyeimpu.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gefobnbyv.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gyetrxcmd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gozbjevhq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/glndwqxbk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gecbdmkrw.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gzibrgdij.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gvlkopqgl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gbjmekynt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gyhnzluhg.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gqessczwh.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gddrigyfw.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gplnsczqg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdiqgpiog.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvmckddrp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gsqlygfqr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gsttvagmb.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfuyvcxjv.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gmyptxist.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gxbhyguuh.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gndjqnuyv.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gyzjevngb.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gbpbccbrm.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gssieycnz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gegzhcjii.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/glzcrmjdi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gylslnrcg.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gkbopugdq.sHtML


<!-- 参考信息 -->