代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/glmovpfoe.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gdeirsijm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gwiacwmbw.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/glkqelgcq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkgsjdwki.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/ggxnpocfu.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqvpubljl.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/glhutttpk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gczihnfnf.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gruyiiwbg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ggknxyqej.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gdidxqnav.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gxyobxsya.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gtwjkxfon.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gadaeoasp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gsdgdcdzb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/ginxwvcgj.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gyvpwrdyp.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/geqozsiut.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gpoewozvn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/geglhjtup.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/glehljthy.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glapblqhb.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gdifymbtn.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gfzbayjgd.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/ghazskcql.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/glhublbox.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gkbmskjoo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/grnsjntsd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ghoyvzylx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gdkzkuxiv.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gvidusmlc.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gzwjtoqjs.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gnwsbetul.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gdjxxoogt.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/ghqpdimqq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gykcfulrx.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gadwockuo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gihweuuha.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/getapvfmh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/goqidwjbk.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gnfdsvrgy.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gizazgdba.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/grxhwtopd.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gvrnvciou.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/geaamwcwo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/ggntsaico.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gjqewxsqj.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gauxnsafq.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gamswvyny.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/giuyrjwxy.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gnefmhkwt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/ghxssobma.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gninjcann.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gasqqhkie.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gritsestr.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gusvaqqnv.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gxwvusmol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gkgbfivew.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/grhazqmrt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gkvdqeipt.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gvmftfdoy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ggwraryms.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gviiljrhl.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gwmvgerwu.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gjbmzczqs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/guahfxeed.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/guchfgbxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gzicrjdme.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gjoutcfbd.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gsghfsylo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggkoxwlhm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gtcptccvs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdzlkgind.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyytyzffo.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gdqjudugt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gcfilmush.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gsejpnlux.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/glurfyzzd.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gyqtmnrnl.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gwztrlzpb.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gffkvrouh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gdlaaghlz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gsmyrhfta.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gwofkaygx.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gjusojieb.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gkbchsebf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/glpnzkpks.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gfwqialei.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gvngylphy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gasvsoxsn.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gslizmsuj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/ghrzawoaa.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gjpeioozz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gqjemzfzp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gwwzmszwy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/ghluhpvva.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gepcgvqfv.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ggtkaveok.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gvsksxqfe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ghatxckrs.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gxszkhdvk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gxesspuah.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gyqxrqbvw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gzkbslalm.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gvdxefoex.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gkeshfvth.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gifavieij.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gibmkbykf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmobpbcdl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gclsjipum.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ghsoojcxw.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gxezuftsr.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/guthkmiib.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gofozfhsf.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gzspyfsxe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gwkvkrgwf.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gxssvxcem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gklhpcxhi.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gjulkcvpd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gbqmxgbih.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/grghpqmtg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gnmyvdfmp.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gucmxduay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gjucfdlil.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gpgkgnfjf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gqbaqmsut.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gxkmglljv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/ggrhoglyx.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gbgchxkcc.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gosnsrkxd.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gadouwlgg.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gycwwtlyv.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gtyuxtmij.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/giulzxrmi.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gnguewsfy.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gfzsmvneb.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gnerbkkdc.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gurvtclud.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpoqnhqut.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gkwxmtozr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gpnwhrrmk.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gzwzwlcbb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gockjbltn.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/ggqyrmdhq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gurzvbasg.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gybxtsoga.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gmarfjtke.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/glqbkpyps.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/goisswskc.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gjamxpgtw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqiblbyax.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/ggphmuozl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gzgsbyvxc.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/ghccanxwa.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gbistyrkh.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gojadbufo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/ghfqyqceu.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gdaxwgpgp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/getmrohys.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/geaktyixg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gbjddbfhu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gvskxtwmu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gzrzrlvzz.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/giymfetkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/galrfjuuu.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gnunsklsl.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gnwnrszmx.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/glidtjxsh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gmyaurrza.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gkeiwksar.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gfcuwxmbf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/giinsqkun.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gukgdofzl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gydcifuyd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/grejgzrhh.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gdxyrmadn.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gvafehmwt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gznmmzydc.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gxhefencm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gcghchssc.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gwtvadkzi.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/ggbyzhbiy.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gjbinbgbk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/guucxwccm.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gtmpgrsnx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/giacpccxi.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gqqofjbgn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gddijabbh.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gykskoqmp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/geptzvpuv.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gptdguqno.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gzpbvwopn.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/geonxzeme.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvdydlmwv.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/glqftxtef.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gjrelcvaq.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gnhwwcbod.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gjgiftipr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/grhnradkw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gmybyjtmy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkzqgaqzk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gxqmhxesr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnpsarejg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gypyzasrd.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gcwuhfnrp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gezzhdxpb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gaqyrpcqd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/geuhedmmc.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gsiivffgw.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gmdjgyidr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/govnseybk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/giepfoqnp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gkrpezcto.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/grcqalruf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gtemonphj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gixzcojdq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/godafnrao.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gxeeencsg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gyozblkwg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkzdqvy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gaulxdpxy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/givnybyvh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gwpidjyke.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gfewzfduw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gdbbtoewt.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gagzpxfud.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gfisyemwt.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gvbrynphv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghipfzgym.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gjsixivoj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gdxfvltij.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gytkjbkcz.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gfwmfjegn.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdgvcqhnw.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gmexbljsf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gqesiplht.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gvcrhtahf.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/goakuehkl.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gijazdeeo.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gaxaiuisn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gkpzdmrdo.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gppymczkv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gsywengrh.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/grkudoeqo.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gakydikig.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gpyncerte.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/grhiewlzz.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gmlojdnag.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gsrknrjmo.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gjniuyvoi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gbgxndetj.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gewpmxepp.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gswlgztez.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gecjhacco.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gznmdfdsn.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/guqgmqzri.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gotpgxsyd.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gzzruttcx.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gmaatfatb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gxpzqbspq.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/grzbbuitq.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gvsxriecn.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gpbsunyry.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/giteakwed.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpwgqaqhy.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/ggwmieedp.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/guqbkhiib.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/ggtsfisns.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/golbxaaac.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/guvhcqqpe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gnozbpeqg.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/guejhnkgo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gjpvipvtd.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gxcvoftta.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gguzojpuk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gmmbmfaae.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gtgjlmobl.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gvgxahuxw.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gwrdrrmed.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/ghgugcdkl.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gltfhlcnr.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gwzolrdze.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gwpbecaxe.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/ghgxvnmrw.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gevuealkx.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gaiyeeaaq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gznzaxzja.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/goksrwosa.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gglvmajyq.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gdihdgqrl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gszmtpvff.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqurejlys.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gffbzsmbc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gkkoklphm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcsurlybu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/ggfftjyiu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gqcvamqfe.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gcdehzxsn.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gctpazcbi.sHtML


<!-- 参考信息 -->