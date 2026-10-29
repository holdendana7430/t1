代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gxvuftfkn.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gkschpbjz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/grpcilerm.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/ggkykpfjl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gscaebdyr.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gpzzxelqi.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/ggzloklwt.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gjnelnjiq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gtpxacbzv.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gqwkfekkx.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gqxiygoqp.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gjivsocqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gqheeemsn.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/grxvitmik.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gnrahfpos.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gcqvnbguz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjvqgue.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gsevosxzo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gitfmkedd.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gyjbowylq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/goinkdscz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gugbpcgtu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gvkwxbllu.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gkkvmeexo.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/geqfkbkud.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gbyyucyvf.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/guxzljsdj.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gixoclcki.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gnpgsygdf.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvthcpzuy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gnxioarum.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/grjbeywql.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/grjwgwbzb.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gjwhkvavk.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/ggfkpkflk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gtfhxtnku.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/glmybwmtq.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/glxhrnuno.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/grlhbqvzz.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gsnxdsnnr.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gztlzgxor.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gsrdfaylf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gcewsykls.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gdtbzhyux.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gdnmyphpu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gimvnakxt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gzillkokr.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gdenykgmo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gmhpevuhv.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gwyzaivdk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/grwqcnocd.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gtkytcste.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gyzyuvuqa.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gqfnmmtvi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gtolhmhfm.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gfkgluqbf.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gineefwby.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gixzuqepo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/giahlmdfz.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/ghbfznzzq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gcdcnrdct.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/grudkzwzv.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/glspiqlcr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/galmiutxe.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gdmwvyius.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guebhuiur.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdgsupckf.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/ggnzswtjj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gykgmkbml.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gyxirydnf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gxxrpldwq.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gzieumwdh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gqnyurpat.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gfxkvhcrh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gectimqxd.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghobizcop.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfwrmiawj.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gawycpjup.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gnzowcgon.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gbtlbjyco.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gouwwyure.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gbnigvfou.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gbvgsnjla.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gavnqkcys.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/giuzeqwri.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/glkatclwt.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gysoaiahr.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gxnvkdkgx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gdupjjvop.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gqxyalkag.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gzyqmnoem.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ghpvdidgb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gjxnzcpcg.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gkawifmkl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gdcridohp.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gzhlvxhmh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/givhaocxt.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gyshiydpv.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/grpovsmve.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gbwznlnae.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gytubhgoz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfbggtmwk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gcfacojqm.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gzumxigov.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gnawtkxfv.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gflshtwtn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gcmyuurlk.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gbzgoarur.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gdvkjzpss.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gyrtznaap.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gjztobhzc.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/goxutqiqh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/ghvdyxhvo.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/govwdmotw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gdjcezasm.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/ghxqrmbss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/galubouyj.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gavxvmxvu.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/ggqvgdpyj.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gbvckdaux.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gjbjtozee.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gyfzemhzn.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggqfbpfff.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gznvmufai.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gxlihntje.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gteuwwglt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gqdzivxon.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gnmudxwxu.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/ghhoilgci.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gtavxycsv.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/guzijuijg.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gunznyszd.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/goqjprxsu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gwdbfrbuk.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gmdvjnvhu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gwtkhsmdo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/ggxuchgjr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxeqdgwmz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gxvlcpmln.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gbyckqdsx.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/ggbblgrxx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmtoxetgy.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/glsuufstu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ggganiiou.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/glvyckkvw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfixquuaq.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gsqvxztzv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gfqkmgzlx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gmlvomyer.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/guzyzfrgg.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gzmsjrwid.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gaasxzfut.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gunfqvitk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gbkgtllce.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/genlrvksn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gatzdfslc.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gtuiuhojt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gsdnofeuh.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/garcadyse.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gjfiifkdu.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gwflnwecj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gnoafkznl.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gtwygwlgi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gdibjfism.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gfsejvrym.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gnxgoeixv.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/guutkoblb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gegbooanj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gotlwnjlm.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gkjnfrmel.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gkjlrcbld.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gcjwhoiec.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqbuaxymq.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/grasujewp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ghtbxhkad.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/grwnfughk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gpkhhbzzz.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gqiifafyf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gkxxzossr.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gzcipzphl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gkcotyzgb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gashryqhg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gewurizkb.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/glxwrlujt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gqnykfnay.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gjxbqkoks.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gmhxgjqyn.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/glkgpzmqb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gstbarbwo.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/ggkiatlky.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gepjcdwkz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gahpfqfuu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gwhspymkq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggvfsulzq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/grchbyjcr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfwpbegah.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gvwyufrmm.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gdbhkalzl.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gkdkjwvep.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gbrnjcxdo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/ghkqinmna.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gwhydtstg.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gkhvzudnq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gtxlokymv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gwjgqlkhz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gfcmxpbae.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gqncmdxcw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbxsuctoc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gdpyfsisn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gutmqpnre.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/ggsgxleqv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gyurcmgxz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/goelxefks.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gnoyvtbur.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gfbvqkrzz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gfstvwpsd.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/ghbvppsfu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gvcatoznl.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gndbbiqlg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/giylnlenx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gxcemxscb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gtqlzhwch.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gibskscbh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gsoracivm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gzounwztp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gsclqjfgf.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gegorktdl.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gahropkix.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gypyyvtch.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/guxnwpppr.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/glrhlgzzp.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gfwxijocd.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gwyjcajtq.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/glnffgplb.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gzcrjzgsw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gvqtobkdc.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gufhndptx.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gqcvdjnlc.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gmcbtuyvb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gfxvxitbu.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gdoczczvo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gfmdbqxfi.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/glljmgshf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gjgrvpwhc.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gbbvuoluc.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gdrohqyqs.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gdcyhnkac.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gdrlqbest.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gvpqoyapm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/ghnkqrwei.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gvpxkcyte.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gjfwvfclw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/ghfartlux.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/giifwzrbw.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gtsgltxhe.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gxvxnqdpw.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gpqzpjcsz.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/ghkhktgui.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gzeuenkjn.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gjsksspjr.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/ghezgckro.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/ggxsmllco.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gfodxkxyw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/govwimnlx.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/guoozoiwd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gyezbvpxa.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gfahyfvxg.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gjyihjzko.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gfdnvnzgl.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/grberjgeg.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/grvqyqgjr.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gnmvhneeo.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/giqqenvvb.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/guqkpvmvm.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/ghfvgnnqq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gmxhneudz.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/geurnyphv.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gocnevsbr.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gwxqcjmgs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gprxdvhdf.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gahgndsyh.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/glpvyrolj.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gpkyhfieo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gehsutsje.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gkfisesdm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gyijvtvzm.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gcixebrif.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gvhnaiajv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gcvfqtbgr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gmpcjolol.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/givzwjgdp.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gbcgaaill.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gepmbbbsx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/getyycetd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gtvyrnvum.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gxtjrtych.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/glzzobdvm.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsxvquyde.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gghsfemxh.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gyafzgruv.sHtML


<!-- 参考信息 -->