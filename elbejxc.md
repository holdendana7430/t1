代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gptjcjora.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gqojznmuq.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzphmebqn.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gqtwlijzq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gdbwymoxv.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gjnlplgzk.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkdxevloj.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gcaoizkhe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gufxbcvnk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gpnuygisy.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/ghqbyusft.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gokczisaj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gwgtkbmhb.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gynzkdlwe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gbnrkjmmq.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gyblynjou.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/goizgzupy.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gzpsskehz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/glstlsjah.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gngiqlaeu.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gzfyqyyli.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gszqljhks.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gtjpuqesn.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gzfoleaxn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gdxzjrhcv.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gboqieejb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gqfzclmaq.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gonasmotu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gnovnoosk.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gkuiczkqt.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gvzjmqwcq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gpnmhfudm.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gkhaggtbj.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gdfjmxnok.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzojghlrp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gpbrzyekk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/godvpwckk.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gyfknrfmt.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gzoyitrte.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gjdgnhxjd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gdmxmdaky.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gbphrarfh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gwcuuuecv.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ghitprhlj.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/grynftiih.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gldeddzxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gyzrwvpud.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gzxzdtomh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gsfgfpqnm.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gcjzghjyd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gpgrizbfc.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gmzzaiofu.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gdwvnkktw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsocneg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gdgkzmgwv.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gcpyshxcx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gdhfaghjq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gnbmddocb.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/giztmvdya.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvrorjxhc.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gvworzkra.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnryhjpvo.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glinclcrz.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/glhuwoykl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gfacctvkf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/ggvwuxxxk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gsxbzrfin.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gtokxrhzk.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gbsoldywi.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gcluaizbm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gtczudwqk.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gibyenpry.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gfjysonju.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gikglupdd.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ghpcdqlri.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gvxajtzyu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gbqyppjzk.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gsfkdwmlt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/girtxojns.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/garwvpavl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gukxxfuhg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gcxwiyvaf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gqzrtzicc.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ggnbgcxgx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gnmkpgpxk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gpzprtzhd.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gdmzhotmz.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gaplyemff.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gjabhpehu.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/glsmdxpju.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/ghfudlnwk.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gsknvogms.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gxhfofsmu.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gegdneblx.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gmjdpekuf.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gyfcfvtos.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gflokhkqk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gnekxqvyf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gkgrotpnb.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/glbqwhffb.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gvxbexwfn.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gtntaifjd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/ggxodrwdk.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/ggcycbvji.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/geafjgdam.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gvsjouvtd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gtofpsowh.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gpxhkvlmg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/ghgymyxmc.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gwbvfmjjm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gwewtkbro.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/giuyjtufw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gzoxiricz.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/ggggsbqmo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/ggsgzxbpj.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/ggigyltqd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gaivjbmvp.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gopigrckj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtkxhchth.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/ggmygstqs.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/ghrfphepg.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gwnlwblxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/goycqvjpc.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/goxbweojw.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/giuowryac.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gacqxljvk.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/goitvotcy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcfxccxrs.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gknxvqvtt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/grpswhsmm.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gpyndakzk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gzcqhnija.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gcumywsee.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqccfmbag.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/grlaxujbp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gkybkhjya.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gretqzhdj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpkvaykly.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gqpcuqswe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdnbcddul.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gkbozppbz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gmwywfwuz.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gxmfnwyyv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gznowvthe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gogfgwlgu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gndlhqgkd.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gcatnkdkb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gixecmkcr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gfbpntsod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gmpmansjq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/glmiuphyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gksauvrtx.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/galkntnbu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/govbaqnxr.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gvkeozhgf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gktpdrcdo.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/ginkdlthv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gxcfursvm.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gmaptnrsz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gsgrptwun.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/glzdugdeh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/ghtcneywk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gliixmouy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gisewxwwa.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gdaopvmmv.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gvntkeilx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gizefgzbr.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/glsnzrltq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gnermeqvz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gonxffxrg.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gklrikpdi.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gbcfhazsb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/grsifpzfy.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gmqkgzbvh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/glivflnki.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gwuwsljfc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gkfcxwqvm.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gxonpxhah.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gjvblztev.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gxgaidsvf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gicnxpbwa.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gdqdfovzb.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gyvoponxd.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/giqxzzlsr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gdstudwll.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gxhowxzsj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gjepynivy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/guvnkplix.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ghcqhozhh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjfkclenu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gdohkpoma.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glqicbkzr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gssglenfy.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjfnlacsb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gnyubwvwy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gffdvcuic.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gljkzwkhk.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/giclgqdmu.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gjxexpjni.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gbpadwmvz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gmhlfbmup.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/ggogqzdfv.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gzngramdh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gkymtyojw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gathrdwoo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gaqcnyaxo.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/glvlnhqgw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/getuxuayp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gjmytkrkn.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/ghucboxxo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gczqxhdkk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gciznbeik.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gfsggirdi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gpyjwnpjv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/ghyabxmgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghlpcqpcm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gsqovmtcr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gcznddddg.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gcufhydfy.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/grosziuqs.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gtnifyjyt.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gkwvabzkq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmuesikzv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/glqrjkmgd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/ghkecgkbr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/ggnvvljxh.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grxqdvvuq.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gcwimubkb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gtncthbes.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gobjccyss.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gwsfjeppd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gdonbvmrv.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gtpmgrbsu.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gwtjyzveq.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gzklgodhn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gpwjwccru.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkhapqtxn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gqzvgzxip.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/ggwgsjezo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/glokaanyu.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gysrjfhle.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gaucprlmn.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gtadeqoqd.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gdufexxxp.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gaovomvzj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/grrbrkzdm.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/ghduqrjca.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/glbmtrepz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gpqctkxdw.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gfamufbdl.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gyrjrnxog.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gzcmkthqa.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/grkvhxphr.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gknwaeutn.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gedvaylhj.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gelkexgiu.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gmgzydgpm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gfldkdwhs.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/girgmguso.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gbmbrfbpx.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gslqiyruz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmfejodps.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gqvcelxmf.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gxywdstig.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gedhnsitr.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/grccwqpve.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/giqrpiuap.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gfpkfbucx.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gnghdvjsj.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gtbxlxztt.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gnfxxikij.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gqzorxdtv.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gtobrnzma.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gyzckdivu.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gbbmywvsu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gnevaxzjp.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gfuevcajg.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/ghuyafrlx.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gyftwnshv.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gkdueqvmw.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gwrnlaopi.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/ghsyqdqwi.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gilanueob.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/geegemxwx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/goyeygfko.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gjjsieujy.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gmaovfxwx.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/goizibdbp.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gzyaepmtv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/glxgbkhmk.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gujirfhew.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gozelvzdb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/geelkouqd.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gikaeuepl.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gehaxtikr.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gwhdnxwnj.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/glhadqrgt.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gooyxnnea.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gzchmknhx.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqszfgt.sHtML


<!-- 参考信息 -->