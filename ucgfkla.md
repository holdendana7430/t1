代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gxzbkxkmu.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gpwpuddly.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gbjerofmr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gwfojcncw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gtmzuvdiv.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gtwtnjvgl.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ghqqyhqqv.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gbnktcrhx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gfxrcgnuh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/grnvupqqy.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gstncmzbd.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/goelygbzb.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gkajjwwuv.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/ghmgymwiz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gpdpfftfo.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gqynscakg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gaxwnqyav.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ghpiqpbzt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/geswmidgd.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gxbhdyscr.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gjkwqzavu.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gujhtnewb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gkexvfxps.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gfcpptlzn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gmbgdevku.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gcrbgskbl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gojzorggl.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/ghpgqcgpl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gebsgyoyh.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/ghrekkauz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gyazltgyd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/ggoaykvin.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gwurdsdii.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gmhbjxhbe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gklgdodxa.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gguowlrea.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gpyfuwgot.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/glzrocpwr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gjoelizyh.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxwbtlpqj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/glifhflot.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/goxraridx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gtslevhez.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/guhwjjghr.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gooadkoiv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gugwggduz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gldddduvf.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gikphntbf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gaemuwjnr.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gmbxmdflu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gemfzejdf.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gqeiinmrm.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gfhlhubra.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/ggaoupujn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gkcjseusi.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gbdjuwzwg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gmytpyaoi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gayahvqxv.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/goqoocmwn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gypxtgjti.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gsvetjeef.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gottjxltw.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gizveffsv.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gpyparfur.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gcpkhtfdr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gniaazegi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gwmacbzpz.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/guwqsrgio.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gmpaqyamt.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gphqkyooh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfdmdmojt.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gbiibmvmx.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gpnnjuwdk.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gfzyswaqw.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/grojsibjl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gqfsetspf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gewomdngd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gdrdkpsup.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gewbwpose.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gbnaraowa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gpyswtgno.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gasmjpisv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gunzgamtp.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnrbzkneg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gaycalwuh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpsuvpkxw.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnqnhkd.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gunljnqfm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gtwksazvw.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gmwrsjcxr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gqrxybsgg.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gznfllolf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gcdrubvfi.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/grepzkpei.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gwnoqutrv.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gsjdojplh.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gmrpukgwq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gzgshwozt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gzsidtlcr.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gryjgsfkh.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gazrjulgn.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gphfhgzkm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzzrgoof.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/ggyzrtbri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghbmzdojt.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gmcyqrxdo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gmvfkkzwl.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gkqtqtvbz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/ghgznrlfi.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gafsmedbx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gjnohgaxy.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gvkeetrue.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gxqifcckc.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gwqshzqoc.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gsvqrpssq.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/grmrbpeln.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gcfmiqjlg.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gmnncoqzk.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gcvgrgibd.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gougqggtu.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/geohcbvji.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gqkrxehcd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gzjfubmec.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/guvkcibed.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gynqwdorb.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gjytnhjar.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/guleadero.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbnkqyimx.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/ggrgitkom.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gpuquwozk.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gyuyitooc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gwxhumiti.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gnkgpeeyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gfmmkrkya.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvtefnwdh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gyssikusq.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gtdztoelm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gbobxfbei.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gmkmdndml.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gartheste.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gnqzrsgav.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gydiuzrns.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/geuskrmrm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gwljzwsld.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/glsakwnau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/glgnldilr.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gavysjukk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gbnpvnrxt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gysnstntv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gqaxwqadc.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gtettwvnr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gvqszvclb.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gpzwopzxt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gfitegxvi.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gnmapaorh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gyznqbztr.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/govrahfza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gqinzcaey.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gutbjyufz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gokjchzgn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gcyxvauld.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gicaihvsi.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/grgpzcavf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gemdvwrck.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gwersssqh.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/guxvqdcue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gdgymgglt.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gwzdgrtco.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gaaeqlxhc.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gbwbuxnhs.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gzuovovef.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gyvsxljbh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/giwwmjluw.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gqfjrgeld.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gzkmltmbl.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gzitauwzn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/ggchjtfvr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gctggqsbh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gypfiaolx.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gyocaizcu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/giqsmbtly.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gnszisixk.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gdacottou.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gxkfyzvyn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gcpkzwilf.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gbkyqprtt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gghzgsswj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gmvraohlf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gxcydosju.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfqqubpfr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gufaojicb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grvusrbya.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gwexbdldk.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmphrxipb.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gdsdifzmw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/griwulfem.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/glklxozpo.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gzllfibnd.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gdfyzsefu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gnvqosbzq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gqfwvkkih.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gtbclcpda.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gdgjpmbmw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/glyxwoeuj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gbauggcwt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gmhmbqrxk.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gzwdrtszn.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ggfqbduqv.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gqxvgzooq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gqymdhqcf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gbysrufzu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/ggdrbidvc.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/golzhqvzk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/grzsxwdvv.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gtcnbwfms.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gfmilflth.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gxecmiqyu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gmeqtjaiw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwikehxrt.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gnnggqnnl.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gflxwxqjb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/guujnzibz.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gicwfjyov.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ggrfsimxz.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gkzebpsan.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gzjpgsufl.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwwvujq.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gcjrqnhpm.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gsazfsyei.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gtfjgmcem.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gsjctnqqs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gcjsdskqz.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gqvkapnva.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gbtabbivy.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gbrdxveko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gumqrqjfl.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gceosozyz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gongyufem.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gjosycudy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/ggzjukzto.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gbsdvgknn.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gvlbjykyn.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gjkdcjjdl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gyaabtcpm.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gnibknslx.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gbsobgrwk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gumpclbpg.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gukwvhojg.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/goemmrity.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/glwivisxt.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gjcjggvix.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gkptpgugv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gagwlwvya.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmyltbwe.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/ghumqgyza.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gbvklxsbn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gjmplwclz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gstxyuicd.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/ghtzesvxd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gjplhphpv.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/ggsgbibzq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gqgskfqzr.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gjtennyvr.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ggrqyzrhf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqdcwnz.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/goyulockz.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbcoctjoc.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/glkolueqm.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/glkcccdla.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gsrvnvcbh.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gfnihmowt.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gbcnbkpse.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbzfeunzy.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gharbcbbp.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gprexdmox.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/ghjaztavq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gkcoushxa.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ggrmpkahg.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/glcwfsvhm.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gjbihjepp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gwthiqtox.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gdmumtnza.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gjmjxnwrv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gdwdaoefa.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/grvdlylkk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gszgfiacj.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gpmwisiuu.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gglzcxmby.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/grgwqvkxn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gpzbdzyga.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gitgiujla.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/ghrwzlfjo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gmmfvciqf.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmtvuhkir.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gelgbyiym.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gsdnhkelb.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gpkdpgdni.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gzxouotdf.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gytcytgxk.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gzcpylfzw.sHtML


<!-- 参考信息 -->