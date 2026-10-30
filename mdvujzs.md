代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwvaudzy.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ghjucwcax.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giahhsdse.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwvqioqd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbunmbhz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqdiungq.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxgvoxrij.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gpomoivow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeuluyym.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhhxxvxr.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/garhlvcvc.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsmtpyxq.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gndlvxuph.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdkjqgeqg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyoqlmqq.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gjltlzjie.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gcvhbugxu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gjykrohjv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gfdhndbwr.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdlmnuhas.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/ghajomaxa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtinkjqw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gawcntqkf.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogiksacr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genovkznh.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdvuakam.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddmcsbnt.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gvfcbeoat.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gpnniymkp.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/getmlnkfa.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/geqjwbonv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gubezifqu.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwqlmhbq.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpujyfxy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gritsehyg.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/grshvemku.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhxrziis.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjpybheg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzqxcefk.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxnibibx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gyornkjbb.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gsblqytnz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzdnkqye.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdjdrcgg.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxeveymg.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gliajifup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkctlpdga.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzjmkfcy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjddjjtiy.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmfsukle.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzsnruqwb.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gcysvazcz.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/guexkirkz.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gisvkdxwa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtcuwuvvb.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/guhtcsmmm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfucrbyj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gffuifnym.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqhbwhgy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwrvtskq.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvcpjxjg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoewwtmc.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdibzelwt.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/glazukcny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiaaevsr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvutpare.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gsqxskxef.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghukdnnva.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gbjuayvvi.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gncejendk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gemsabtwh.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/geufnzfir.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkkjxktue.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gujbbcoru.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ggbgxmawa.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdgnnjog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/getgcajjj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/glzjmujyt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfybgazl.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwhjlzmr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrffuezw.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gbiuhghih.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gkalcfloq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtltvwobf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gjcbpeftc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdbzkfcs.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/grtziyafn.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfoywbupr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsflvnbl.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gebutdtwr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/giodwndss.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjogfgqw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gijtugwqf.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwvlrigf.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbzctfxeg.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gcplymgos.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggjkdmwmm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzrlkvmui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtanqiqjh.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyduelhrv.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzlbbhbz.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwzpltdk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzktzqpgb.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxdgtshk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbixzmxox.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gzkmdjfeg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwvctcsl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicryyngv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gaflpsawr.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfidlqom.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvskxmd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnymmuvpa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gtbwsaktu.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqublyrhc.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gwzdrltml.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookpvxmp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuoobuwz.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnszuqxjj.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwcjsngyp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplctkdlp.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqntgdrfo.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gernyexcw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gdafvbbxk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuhsawzj.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwlxdfwwx.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcclqjtoy.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwbrpyad.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glmdbxjxu.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gizqbpmnr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpocmiwfk.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjfgzvbkt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gydwoqmyp.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gtqoxzsvi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfrqqeak.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gaccuwhvh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngtddkco.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gtogtnehc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjtpojut.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gokubrftm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gthpyvmny.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiussiyk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gkbnalqky.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiqfyfuf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnmiftbp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlzushka.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpvsdvnk.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbdyspdis.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqinsrfmh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gepwdqktm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxncxroqz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/giotqqxis.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gilzyehuh.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddfkyhxq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgdkuzdw.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfugnslfl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/geefrtulc.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjczsjbs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gyvfznhel.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/guosjifis.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbryfaxke.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ghglawhum.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpqtynad.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbftgthy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gmasecdvd.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gciszoloo.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goemhiqet.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gdxtdwukp.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gqntwxvlp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gucgvziys.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmhfmouro.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gafmlkbvv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gsnrwxrwg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/galunlxze.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwlrxnaa.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcaghqnx.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcrbcghv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzgnianl.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gedeurzkw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsmvbsii.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gusjdiswn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbsyulol.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxndpvjqj.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfywmkgp.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzdbcjke.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdnkedmt.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gbpzujwjf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gekwocyaw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqyrhidm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gendfwdom.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gswwoykfn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gihwjoxvy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlhriwqd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjsusvldt.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gimnaybbm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwrbwqmf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugzhmlyo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjtpxpe.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnwqkyibz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjkfqydr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gxijdylsv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/giodmpcou.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gzpimnmpo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gihmwprpw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvpvjcwfh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfngehcae.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfcboevj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfrbvmaz.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/goefmnyhm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gomjfszsj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gryfaywdy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gfhvargbx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoqbbuan.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gflpfsoww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuynifkg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/geiuaxbwa.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqhxlmqas.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/godmxwnxr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkplqwnct.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnypykswr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/geifhpkxd.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/grdexiulp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazteymde.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfnxvnfp.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbqsehue.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghwhvbwfd.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfpqaste.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gpsedyxmp.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gafxwflxe.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmikpbra.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvzkxbqb.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gviybnkae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpawclddh.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyfjxiic.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gswkbxsuv.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnekoendt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghisgacfi.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxrhjnkk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiaqrrjt.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkvmhqsc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqedrqulk.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbqmscxf.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gfzwscaaq.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnuqsgur.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gncgvwaxe.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjppusfyg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiwpgyqv.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwytnbukj.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxqitps.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufhsimcc.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsqsqdcs.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gywfrrczo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gckveolyu.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gsopcmyxu.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grzvfgoit.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfcpksew.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpiahvon.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/grbpfwrid.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkrlfbme.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gwqrqxxao.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoqxbfzx.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqyaivhg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdknkhdtd.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwogpannd.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gvoiwmoot.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gwaurmfij.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknnqgtqw.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghyomamsw.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gvyqsgffj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gkicjlzxz.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gixsgyxbo.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/goxgrnwpa.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdddxwxd.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxpeeqod.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvwcccye.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdehncji.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqfmisolp.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gefvunkqb.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gscmdfrkf.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzzpwpurq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdlfazmr.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ggslnqqxe.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaczuooyo.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gatuyspwc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghkgentoy.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gisdpmxbj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gltsekvtm.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqwpthsfz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/grxnxzayk.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemyavvbs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gffcioxyf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvptislfq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/grsmlonkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqcxbqarl.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrdwjhhb.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/garaefszo.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamwfjjuh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvfvjzhx.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmyzcxnz.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhgzecaj.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gysothxdm.sHtML


<!-- 参考信息 -->