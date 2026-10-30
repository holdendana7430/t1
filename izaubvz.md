代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvwyzosp.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gmjqyqjnu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdovqcfox.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/glekxplhq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gvbsnbpiu.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcztphsft.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gamziwckq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/grqnnhqxv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxmsookpc.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafbejhhx.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxodueclw.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkugrsem.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuydrzbg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gvsgwpahb.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwbnkbmn.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/goxychjbh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbmnxksl.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnrjyqkgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/galkagsad.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/goqnkszhg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgkzmezw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyccmzxz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtuqdcjx.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtlgfxcea.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gfsnpgjts.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbioazdni.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gtljyzhlz.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ghkkaoayn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/goheumkbi.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gljygqeej.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyisuuuka.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqjwzdka.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdmecsqm.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gsbfieksx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezqguuwe.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gezuimdkn.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxmqkovy.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzlxnkv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtjjtfwxq.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/goipfcard.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeozeikp.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqbnyvrh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/ggawnvwpl.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gujzawwed.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxbffdyh.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gffxsjnks.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkubtxiy.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbvvxinx.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ggtkudijz.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gifaicbym.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzmyqpyf.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdpiufdvr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gvunihwsp.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpemfvti.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzzcmhmjx.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/glefwdyrw.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ghlwbrfxp.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/garvyqlgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuizzuou.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gnrlsdccy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvkaszxb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gztqgvyqg.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvtvhjax.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gloiqpmsu.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqswteplt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxovavcm.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gudenxebv.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwzwlaeu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gempycvpy.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gynobqoim.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkarnxudr.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbekovdp.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gvqqmhdrn.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxruoox.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdealjjo.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/grirvfmsp.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gioqtzqbm.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwhzntil.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawlykvik.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/geqacvpyw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiylxoch.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gquaitren.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/guukawicu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoxejpcm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdlgmdm.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/geddpzmwh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvzovkwa.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaxsngljf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ggfcoihsm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gzbuggcyv.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/geucalbtg.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcelbcywr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqkzpnx.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtpartrxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gjyolzvwj.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggilvfmsw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gtdoyshjd.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/geqmasimk.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzwfures.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gedhykphv.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxczluym.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsvgtzjb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqhnmokf.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbknxlcrz.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/ggofvlgfl.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxbccjdyh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkccjkbkf.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkhwcddbe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ggqhdxxoz.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gzpxehsfa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gauvsblvt.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gzamwggae.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gupxxzxcq.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gnribbwwp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdpgkrsi.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/guizctnoh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnerzozfm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/goellbjrf.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gjnbgjhgn.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/ghvdordpj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoillmfa.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsofechpm.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrkemjeo.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gznzzfvbl.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurvhdgxb.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggdfsklll.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpcplrly.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgfziqxa.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtxitzufp.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxntklzja.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gstcznlgl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gounzmytr.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwsdnivrm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmwexmwa.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvgdbhzvg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtqhuwrm.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymtabuve.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcllskyfx.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gganprfug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsdxamof.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxmakwmd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtfxpnhuz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkcckosz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geotzgmxw.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gxkdhlyox.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gezinjhjs.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guspnhpwo.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gfnpngnyf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpwrcbqrd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxbplqua.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjlyykxm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gylzwdszv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpeeaqnz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gzrydpofw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guqlxegxd.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkreswuul.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gfaixdlvv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gejolagtj.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/grcxklvef.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gseehdfcp.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsofznkp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gucpfrazn.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gcqqozcig.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvlhftpz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcthlzmn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gepvposnf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjthaxteu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grltsymkc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhpcjhez.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gffasivma.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gujkitfcw.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gmvsnictw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnivdywjt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjmjypaj.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/garjrcywu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/glwkhmhjy.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkwyqgcb.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/glvspzzcp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfkwwqdr.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/ghdtpfdku.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gahezfsps.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gveefovdk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gprsqtbvu.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gerrwwzfn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gapicsbav.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajdaizfy.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdndjpcz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjooukfko.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnwetwew.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gzekxkxgn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsovdlgsk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghsiplelr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/giuubppkw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlmycvbj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gformthmf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcumugfaq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gayyynsur.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geclelphh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuluknvh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/guogukuay.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtxununl.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqixkmnn.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/glurwhpce.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjvzogda.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gkpnniyrq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gcljrwguv.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gslwknpyv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gmlmnayhe.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxetvpfkk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvxpgnibq.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/grkaycjot.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcvvgjnh.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjhqlizok.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gomccpreu.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmjdlhgz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gghtfxbvg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzaiesdm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrvllouh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrpbqwjm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsslxyekb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiyvardj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkmlbbob.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gaejyhrqw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsawbolgn.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gkmswfpwp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gwpoybilq.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmxvtyhte.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmewtsyxm.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gpukmraws.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gstcfkwnj.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunpztyr.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giunlmucv.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gyngtbkbn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpixxsph.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkfkdqkp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gozocjfrs.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdidsjmyp.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmhexojg.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwsziryc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyqzirbf.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcppuwioc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwwqgzoj.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/glyhdwbqb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefssrhko.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfffdctf.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gnumipdix.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyjwhagq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlvdmwrm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqpzctvh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbourozwc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjznabgn.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gdyzyqvvf.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnrsqdvp.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gukxzwsam.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gakhpqzgd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gcxnnyzuz.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdrrhnwf.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrglhqsl.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjmsusywm.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqalyslur.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogelrps.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gcipvwdio.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gocsbbnqi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxuqygjq.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqimsmhcq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gubqwbipa.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gabcqplvs.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gmnhgazop.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gryovxtfa.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdapqtfoh.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlhebruf.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/glmafsbop.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfvqjrdy.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmnyggye.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/ghirnjzhl.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gaqrobzub.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdowekgjc.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gnxlbueiz.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glygiyezr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxajidsj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcwcstoq.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpfrfwzf.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspjtlqct.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqiqiutdq.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjfxlyzzz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjvymxzs.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gjkpsbjqc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/geescthlz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gezgwfhxx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluqwuqrt.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpraowypr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtspczjza.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhgpxsgu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwkdplqa.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gndwyrsma.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gngtiwfif.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/geawnhzaf.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gipqlbyeo.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmikwzuzv.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfahxsyi.sHtML


<!-- 参考信息 -->