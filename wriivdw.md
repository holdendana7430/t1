代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gdrmbpuhf.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gelafxjly.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gzznsaefn.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gkbrqmogo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gwzgkhkbd.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/ghapjhkdu.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gkufistid.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/grqxuouvj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gmnivozsz.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gtnmkcxzb.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gvmsrfyft.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfdntii.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gkxdlobdh.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gcozklruw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/ggrnkztjt.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gdhqwuzhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gytjyvfth.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gietizbem.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gqdnsyeaj.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gptlmqcqf.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gyyxrbidj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/genvsdzon.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gkewbqfts.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gkigfuths.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gwqjxfzzh.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gnyugphlc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gfuoaxcxh.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gmnmbfcob.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gtythwftz.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gqzgelesp.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gyfcsgava.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/ggelzwhnv.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gseskwbbk.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gtszsgbil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gtjqpblbc.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gkcpqbrgv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gtzqyphlg.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gtqmupyhg.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gahmcbypr.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gldnyrywg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gwodkhgqb.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gzqyshidk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ggnswqbvj.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/glljabykx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gxyjmtbpe.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ggfzzoiwj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gmwilrbjg.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwomcruiy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gmvbqdtfq.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gsipvqjje.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gjmhkvuyg.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gtdrzuajy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gndmttjqn.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gjlqlyjlz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gpuyanrnn.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gnfvteusk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gdspvbzow.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gbpbyphqa.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gobubjmws.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdoibcbgk.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gnytiiimg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwmpwbmjx.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/goowfczwi.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ghamtklql.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gsflugzlr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/goctxnded.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/giwongnbg.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gzszfllom.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/giyzjvdsx.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gcnonnecr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gkejhzqti.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gqsnuzozn.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gwtswjaei.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ggkwiofls.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gtosqspka.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gmdzushln.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gqqgjplhx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gbbbcdkjo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gtsxdbwot.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gsmixwhav.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ggyqqzatf.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gnsyxpwbi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gsqxhswcg.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/goargeqmv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gqqhenzeh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/ghpofkupw.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/ghvuusubh.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gfmpxygdr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gycodboob.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/ggdovrtfa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/ghtwoljcy.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ggdibwhfm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gpcrfemmv.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gthqzfijx.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gjummhqyd.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gexflutnr.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gfrtvqsiq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/grjmwrnef.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/grjtrapch.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpzmnkxlw.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gcudflqwm.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gfqlalbvh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gwyzlwkax.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/ghwanjqti.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gkvxshife.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/getdojbco.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gfrqkuxyz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gmlzajohu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gqctzbydj.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gqgxdkowp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gkxuufuuo.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/giodbkeik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gzokuwhev.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gconnwzlr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gqgamfoie.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gowkdhmqf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gekkcocxz.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gdagjnhfb.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwarjkrhb.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gywjslxzu.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gbhdzktbf.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/ghsptgclv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/godksymjz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/grmqazlrl.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gkniwtpwi.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gcxgzzzus.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gocbhktto.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gxvowruii.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gabgxpyji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubdyaxhq.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/guimqemyb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gvarrfkdi.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gmuuqtanz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gjanlsxbp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gvoyoyrhv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gnbzgxayo.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gqgemawvc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gscxywkro.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/geqhyrgks.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gabvahyzl.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gqykwfxed.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gnjznvsek.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gaqxhavol.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gyqvbbfio.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gjuofpguf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gswjsahiq.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/ggjekusyb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gpscszrdc.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ggxbvkeqz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gwhxijmyw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gmxpgnulq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gvejbbgee.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gzobbnujs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwoefmlqh.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gbvyebipp.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gggjnjgrl.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gxuaxddun.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gtyzxtdpr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/grdxmebok.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcuffnfb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/glvcgpjvy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gegadszyu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gbopozgzr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gpumcllob.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/godgmcqtl.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/grjyizmej.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gihgydwph.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/glhgyyqbe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghpiirfow.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gcwonaqpf.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gsdomrxlr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gkhgrbeov.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxirqkeoi.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gfnvoufzx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/grclxxhcx.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/ggaovquaq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gweadgjlw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gvnmqfuqi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvaglcjex.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gwddfdqrq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gzxoqhbzp.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gpftzmyvm.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gnnhnaasp.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gzcixupgx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gqmdvriys.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gftdfycod.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gygshpjjb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gpaztrpuv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gogpmwbpy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdkzvjljp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gczwdbmrc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggkbftryj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/guinexlty.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/geqrirppe.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gxndypsbo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gnirjbkyw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/grlimpfjj.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gvclpqicg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/ggnixpdpc.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/ghixzpwic.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gpyjaxqdv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gtfdxlsmj.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/grblargpo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtbgpkdsd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gwqoefozg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/genywwbcc.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gpiweirvg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gdiufnjsa.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gsyaljeey.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gsdhxapgp.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gmbvcqiyy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gejnkygeo.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gesdjseqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gpljzoxsg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gpgakcxlv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/genoizfmn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gcbsuzgmm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gdqhoesvu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gsjflmkey.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gnwyuodfm.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gwyfvyiqj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gskxfqmhv.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gumsgggts.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gnfaezkys.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gvlgjervh.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gkxaoanuo.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/goglxobta.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gxowbvhop.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gzcugfhzo.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gmjyxiklb.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gybwubnnm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gsxzfdncv.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gvwxpmlhn.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gpfmhtetu.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gsgzvpels.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gqkmwdeiw.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gwpkqfrcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gtdzbvpkh.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gsszbafvx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gyzckjmgw.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gwsolqtho.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gistnbnaw.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/ggdespvcu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gmqxfqlbl.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gtslsupfx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gsyxdfboz.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gkxjnunst.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gtweiiyjn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gyifcrbya.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/glzjqvhny.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gwomkuaxc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gzylzlxqz.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grhsnrazz.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gppkwdkxt.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/ghdcxihlt.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gplmdywfv.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/guzvwsmhw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gjlurgavh.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gbwrpwnvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gmcfzsuam.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gajwofkjj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gcznbcqep.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/giscdgrun.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gzyhptisu.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gfwphuyop.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gzwucwvdl.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gzzcgyltv.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gnzzngwum.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/guenhogyu.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gtluzilxp.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gtixpwxqi.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gdimmiwea.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghebaerlg.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gmqednqci.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gdrobomom.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/guxlgbkdi.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gyxsknqqs.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gsuuluycj.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gpvzpumrp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/glgosycif.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/glvtvmfqz.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gcopdtixw.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/grwhiwajx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gcimwqkli.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gmfrwnnmb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gtvragrii.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtlylalvs.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gvokxrqgx.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gwdpodinw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gwhzoyswa.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gagfgmnam.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gncnobvfc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gxptunwnk.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gpgoikjxh.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gzudbpszc.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gpzqpvslu.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gyhqcwsba.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guogljyjt.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gpfcbeefn.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gnistdvhr.sHtML


<!-- 参考信息 -->