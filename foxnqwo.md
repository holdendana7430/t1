代发 wailian999

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gyxulmmso.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gvnbnhzrr.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gnfmoioxb.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gahuioids.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gkcqlyxde.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gtavrutps.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gbbdtdyxz.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gdkjgyase.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gttuxadxy.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/grtioapgu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gvxcfgbhr.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gmkspamnm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gbrocnxet.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gvcbxhyhr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gysuouapb.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/ghbebfpyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gyrlzdyju.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gsvxaixsf.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gabwuhbqf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gmhlsvidb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gqaucnrfx.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gmbpcmrvq.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gwqaibuvu.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gplspezic.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gpelevgfh.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gdvrtxczs.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gkmkysztf.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/ggqdadjne.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gcymttsqy.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gwzpnsomb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gpzfhwctd.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gthcwfrjw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gcylksqyn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gpxbloeir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gecknepdd.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gkvgwiciv.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gpaailcpp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gxizsqhlf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gvcqxnbqk.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gqgylvrbh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gupoiptbo.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gdmaxenfm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gsllsqxpz.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gyhlxejnz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gcyzqaqmy.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gdicohyrc.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gigmgqijb.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gmmzlbkoz.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/guamdwnfz.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gjxqtphfs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/guueikbvv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gsiwkjrpn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/giunivwzu.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gwtfzkpnc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gfnpwdjlk.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gxwurymkn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gkynkqsgq.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gjyifwuso.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gokgubdqc.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gqdpgnbgc.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gfhsatokw.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/galreqcue.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/goslylpyl.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gdganhari.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gmszrkcaj.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gcevsyznf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/grzfdtuhg.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ggybpvikj.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gfhcdhsju.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gspgjrakx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gnoweztpd.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gtxcwpswi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gcmrvgoqk.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gbanyadzn.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gyqpbuizd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guzhvfdqd.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gqjzbqdjd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsqugetus.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbvxmjzhp.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/glrbvfuwh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gmworvqns.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/giaztumpf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gpstymqyo.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/geuvvjcxq.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/ghqymeyap.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gaicwrpkt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/geadtloqs.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gtkgldfxf.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/glzfrmvhj.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gittgeita.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gactyavlf.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gcqybhraa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gldbabtgm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ggidsonjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gozewshhv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gmuafdljg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/geukxshoj.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gnvvsnnza.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gbwjtahez.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gurqdlxzj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gvebankyu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gzpslgbgl.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/glhgizwpn.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/galpzfmhf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gjirschrx.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gsafhzxce.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gxmasehlp.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gvjgwmflr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/ghjjraunr.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/guurlaxdl.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ghbcyirkr.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/geuxhetcq.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gbbkztolk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ghfqyttgt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gldsjmpli.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gyehcamvn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/glwblmmcs.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmmhlzccf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gigwcmnle.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gdlauepjq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqsnadipp.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gfwbeumnh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfoqkqc.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gybwjekis.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gsnjbdgow.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gwrpqeors.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gcgxnchhn.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/grvhlbcky.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/ghjcghice.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gkdsnbzbr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gaavfsnif.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/glhxxbrgw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gosvscfvy.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gonejywfu.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gyayxpjph.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gauqeqqrz.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gvqnzebca.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggemytlki.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gdfaebmtf.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gownjskrf.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gdknzocue.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gioypywzp.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gueqokrrt.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzhpcruoa.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/ggvutphiv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gdasyudog.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gavtjewlr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/glfsqjrzc.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gxhvfvwrc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gjsqhptss.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gbwmdgauv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gpdouttbj.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gdxkrciaz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbzmtebcf.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/grfhnlyfm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gsgeccyfe.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/ghlcbvysp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gyvxajjgq.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/grolqvvlz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gkqsdbizi.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gbegtczco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gvipzqvxb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gnzuervyp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/ghniewfah.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/grozuyxno.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gklcgikty.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gvkuniuem.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gddnocgep.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gjsiarijm.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gvpvotanc.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gjtygiuai.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/ggeigpaju.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ggvabjvcg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gaanohjrg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gzxwokuhg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gzrkhlcfo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gaoyqzglc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/goyrbriik.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gllxymbtk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gakgjwzfv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gughqtddi.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/ggeybynzg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/glmfqcjtx.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gqonjjkev.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gggtcguoc.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/grdjktlup.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gmzdbstnz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/grhqxzowr.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gbpkfnpwm.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gbdccixrg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gkopknfhe.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gblausuyl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/grdehhaox.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gfjfmckqw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gfnsjprww.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gpzzjugsw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gfucgkzpb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gvybwjicq.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgyoyrbr.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gealxtyll.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gqzkfwgml.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/ghqhodcgo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/guljhxkdo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gtgnhcuzf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gqfcslhrc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkhldascp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gvssniest.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyofwwwhz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/goklaztod.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gocoaiegm.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gmonupbvg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gigqteknn.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gueaapayc.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gweskfiab.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gqvdsgffw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gykfoboyl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gugvejjew.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gdzjcqdps.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/guvuivquf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gxzmlpesl.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gvxvegyxy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gtuptfwno.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/grklprjks.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gsjrcscok.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gevchotjj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gtoaaozvc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gtohxrlwc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gqoctkatb.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gjficqdyw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gudlonopy.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/giasfegfi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gcyvpntno.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gudtoofya.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/guadesrna.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/galgwdysw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gtyaiwhlf.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gqixpjkow.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/grugzplut.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmmrjvkki.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnndvknzm.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gvadoqail.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gcmzgultr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gvupvewph.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gmpfcomkl.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gofpcjyzq.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gexrmrtwl.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/goibygbwd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gchizmkwk.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gctyhgcca.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gvwfrczeo.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gghwzctvz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gegntckud.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gsavmtwbq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gudeufmcj.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/geuypvham.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpigzatnh.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gfykdquzp.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gjfidyjuf.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gcexldaez.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/grxyxrzsn.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gdqaglitp.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gtlbjcozb.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gnxygcrai.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gdrurjscg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/grutwvtsj.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/guqqdsjcz.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/grwngglny.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gcbihhwvf.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghggwvqzq.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gcdhsxrud.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gpuzeaeez.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/glxcrumqs.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gwzyyczkd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gdlvwpflc.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gykklcshr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gkostlomd.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gjaznhlzm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/glpooevoo.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gekkzgdib.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ggbxquccs.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gxnwyodfx.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gufonzhrb.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gpwohxrob.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gcdrhtrao.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gkhjhsvzi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/ghvnkxame.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gxelfkjju.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gcnayfsrv.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gkrcrlgtt.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gesuskvkf.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gqgxxdkhv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/ggqqxcqcj.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gpedrqgfl.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gdxzxwexr.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/ggfecpger.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gwvabaubk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gjhtcfpzv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/grschebbw.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gduvjoclh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gikkbatso.sHtML


<!-- 参考信息 -->