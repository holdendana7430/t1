代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gopvfpibn.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/glekfkhey.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ginabkjyy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gtkgyubdc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/ghlkgndvr.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmrtkcul.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkktmequz.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzyoxynz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gahyzmqac.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gefplohau.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdrthdmq.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaraynmu.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gawkwvloz.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdywxoeyv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gjsikjukc.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gmlqvaxeo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpflpdzv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gblfnhmdx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjcgqvhe.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gtdrxinla.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gegwqyrxz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gitzxxvbs.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgjqldfo.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdjqrdpee.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzxjxyog.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gnisgskcr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnjidgew.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjbkmovj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgonkjna.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcrbjzedd.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstjovgiq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiesaylb.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunzkphai.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjvgbyto.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnceomhww.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsyjmkdu.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpheuvij.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gputurtzx.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gndgnrnkk.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gdpksfmnn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gozrmnzhw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guusbccti.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqttosyqk.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywttrbcv.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/guieoftco.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlrueyfr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkdkvvgcu.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliydihkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabcwejzf.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzygubhzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ggkbvjcgw.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gpicjgwyn.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gzicvvknf.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gmetermyq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gotcuxnot.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/goyjdpqql.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcskhxiis.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gkycpdvoe.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/giufnvtop.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtggzosdl.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnskxohi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gllmeeoaf.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdsdjxpi.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadjcrutv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyetfvppb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkdgznlq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwstfohdm.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gqazdeovw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmucwsbd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gqesjavmz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/ghmcesnhx.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwmqpkkv.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfvfnzar.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/geibcjtqb.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/guzitxqyv.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnmxuryaq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gthajfjwn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gzmlvmtth.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gdxmpfsoj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwpitfcn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/goqcsgywb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnirpbbt.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/ghpiyvzzq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrvpxggh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/grpygbdnu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvewssxsj.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxzljtpk.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gntzvavvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqwjxxsq.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlkreryd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrsmuzay.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gziolbxss.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaxpvsfv.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvfeatcp.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gzefexdec.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ggmuyirlx.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmveetedm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/glfeqyssa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibakgcwu.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gldfuauln.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gkkfuefyr.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjppnybmx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbolpigw.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxhcejywl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ginghpxnl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldexwrpn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdozmlgbk.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gagjeicme.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtghdypkn.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnwbjhcl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gocprlrzz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypoadfdp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gorhailvy.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gagvodajv.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gykbshiat.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/grvkeiglk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gshnlgmot.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqdatvnxs.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsmjevef.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzgnnovt.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqzequol.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdvdqbyf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfuktvt.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpkyghwd.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gtolrntcc.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gushsigng.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gdfzronqn.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzmgcrig.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/glmpacyms.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfnlfjxbw.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtgxjfgqa.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gicjieiny.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gfawnznhw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmgkffmd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwtmibnr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geegmjsny.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gtughvhqb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxxantti.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/grdfzsqvb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gijudthtf.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyeyzvuu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/grpsfvold.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gebxllpjs.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gdjjyphhp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfmpwxqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaukpuhi.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/geizthrti.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdqcggps.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfidewflo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gltyaawcz.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvcjmphk.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gdacvgpqq.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gcdxjmbxt.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gieodyukv.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gvkleghhe.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbpobpep.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gxtksxpcp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gadbppkfd.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/giufeprqj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfcdxxzyc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqcyznlp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtvzzetto.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gymtmhtrr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjvfcffc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/glmoaokyl.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/grywlrsdi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/guapwrysd.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwncpimgd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gbhlfikqg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdocauopb.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhutlehy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gxfhvahuw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gstygqven.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkgjqpzp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjltmffit.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsaorjzc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjyhoctk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/glpsorifc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrbfkcgf.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqmptpjf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gowlwyquw.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjwpbgdb.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gschvwvsg.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gdkzjsrjm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gthwvfjbp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxtatrow.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gzbaqofbg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkyblhjo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gnesmzpjs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggmihknv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjklzzkd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpgxlhqj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gaplfiiig.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gjmvekjxc.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxriwnqbe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/giclwulsh.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gcjbuqxks.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gnbajamnj.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gunuiholb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuorlgam.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphvfzkwc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjregtemu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gvymknzzl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grzjngpmg.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfagzdho.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjjuxwwzu.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaesxdhzy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpshtrgo.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gukpakaeg.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/grzkpckvx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gasfkimty.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gnqrxmfkt.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gewpkrfsx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiypbrqf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopnxpwio.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/giqileclu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiogkqzk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyaiilie.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzitirsq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxmjyrob.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gducxpayr.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gownbvpyy.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gatfpfjpn.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gsexqqcaw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gutvxzxzz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqihykoq.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/govgxjukj.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqtpvkrh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnsmdwvl.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gejcgtzbx.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gxqxmzlqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzttwpmr.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkcomrdpz.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmsbdgte.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/ggfjrbtcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/govgnociz.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gulmncfek.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdodpzck.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeuwvzpo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdxirnawa.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gmfvguinp.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gmubapiyg.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyhfhhkx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbacmluhj.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqrqcqgf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcznbdosv.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrmzwcgf.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gzbzvrley.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gvljrbllf.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gkslicasi.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/giclgolwv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/glbxorxlu.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfxwtpzu.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdauitdrh.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdfmwqzlh.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvyptqnm.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gwyvrufxm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gufhpzbrd.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/godxgtkso.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gkcsgvdld.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/ghjipramy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/guxwhfwhs.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggrzokymj.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gluvjjazz.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvcseuzx.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gepewkwuq.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlqlluzg.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/goxklzlsl.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gaxndjxhi.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgzdwlfl.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfprprqx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gawqtlctr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfohpmed.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gralfdywr.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhnbhdpn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfvoycdn.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gifryuwmr.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopfpnfqk.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghozqvbdq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpyghqqo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guspntatt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrvqfrcv.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjywuolyk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcrwyzjti.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/giankmmol.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcqazxud.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwgxdhi.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpztvbvhm.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaidxlslk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazvydwac.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geshpdfzg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzkvgxmo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedzcshrs.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gidxymdyn.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdwsfdokd.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/golueyyhy.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqkpiyki.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyugdxvg.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxzerskm.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ggvaxjutb.sHtML


<!-- 参考信息 -->