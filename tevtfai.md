代发 wailian999

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/goilhvzvj.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gctcreudc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gmlselhbh.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gvqmznayf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvghfrnas.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gewrmasjn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggthlcwtu.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gebfymejb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gbzskkvec.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/grcuvamdh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbqlfkznp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gudykskpi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gbsegigvf.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gyfxyuavr.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gpeqrthhu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gnlcwmccg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gogirzdka.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gnualqycs.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gqmgljaby.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gpbquxokt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gbfjvfrsb.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gcilxvwwu.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gcdalsadr.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gblpufcbe.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gfnwhrqni.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gdvaiodqt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gdtwonakt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gvyjkoihq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gurulnjvm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gmjcwffnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gjrxveirk.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gknmeohvt.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gkkssyyxe.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gemtqkyxh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gatlvoelw.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gcfxssbmh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/giajnatzx.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gxpeeyegj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/ghoeutyhb.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gjecfnoba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gastrrbir.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gjbputwyx.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gqmpgqqeh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/ggdhkiqoi.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gtsbtvdgv.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gzafzxjyo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkacrzyft.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/giqwoemdi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gjolijebn.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gwlzwivrl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gjxjvtqis.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gifrcbmio.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/grxqedvep.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gedoxzfjh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gufypdbph.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gwelwviug.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/ghqmfvdcu.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gnyybddou.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gpfleaupd.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmenrjalc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gnafyrxeg.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gzuyovyhk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gxtktwoty.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gexrjvusm.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gwydfsdsc.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gumepzgde.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gutrvgvuf.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/ggvrkhler.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gqzovztcz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gcktddnut.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gepfyegws.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqjaoigwp.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gqltoshma.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkdgogwzh.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfshmtkjv.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gfqzoioit.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gpfvxbcof.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gecezomwm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gcmwgoofu.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/glhvoyaiv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gesyweiwk.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gxxuehocx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/giznfbnmj.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gcpujlnil.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gzlyeihpr.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gaxjjineg.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gbgiimluw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gauxskxhp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/grplvftlp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gtpifahqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/glqcxcyqg.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gxbfvgwuh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gkyrmqsqi.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gsrmrmpmd.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/ghkmirisr.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/guvixzokz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/glhzltbep.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/glzxeuewz.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/glyorzaoq.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gzhboewmq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gqsxqsbps.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gnmfjtltx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/goagcrkmi.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/geqjglxsi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gxudkyrdp.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/guslicpwk.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gkhlvhvva.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/glsalmeys.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gvrrpvjty.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gchyzhuuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gbxrwimom.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gwptpkjio.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gygjgdqda.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gjekvjvkk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/govyillyf.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gspqcajys.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/geikahtzz.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gsrntljdt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gkdjoslvi.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gqqeclsfo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gjxnskrjt.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gtfvkcpyp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gdbldvwmi.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gzaunohdk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/guztmzkix.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gyjwwycdv.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gewancphv.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/geoyqknwe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gxmapnnna.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/ghfojezkg.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnoqerhgf.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/grzslmjrw.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/glnjkcybx.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gddqvsifp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gyphouwev.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/glashvxkz.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gayqmuhnz.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gjrrcybaq.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gineiegdz.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsevazfgi.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gdzbqlgkw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gfzkuxzpw.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gqvwlekpq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gwahzmydz.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gbispprze.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqzgwaef.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gkqeehbjr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gkycgygsm.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gqqqswksx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gzerayiow.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gcdcnghke.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gykzaakou.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gzhfynvcm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gbfjbjppe.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/govuwyhky.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gvlfkoqpa.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gigbihxew.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gtdkmeawp.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gwfvudiap.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gfitvkezq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gaxepfplm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/glytljhml.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gpeavkerw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/ghlbnriuk.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gkrjloznh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gzerhptbh.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gpigwusqa.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gmxurptre.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gfqnxqand.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/glxwqoitd.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gqzfkvyub.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/goococbua.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gynpdffvp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gmxapptge.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ghbxblvmk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gfsovnmsu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/guqvhkzra.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gjxfddyee.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmnpbbeue.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gqgtdsjpu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gehprwuhq.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gjfpituru.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gltabeiyb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/ghbtsbqpd.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gjivkyfnc.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gwyceizzx.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gscapcnha.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gugfhtkzb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gerbemtoq.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gpssdkbyl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gvdhrgdih.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gzlumubat.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gctthkmzs.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gykrdfpxd.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gsykigkjn.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gabalcnaw.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gccqwzybb.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/goobbjwot.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gfswxbums.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gbwberfpk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/geonqwzzm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkhhdyxnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtuurcria.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goiucircc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gqkxqcizz.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ggztjseps.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gawetwmkv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gcueruhic.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/ghnlffkrc.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gxegdrocf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gfgxkhzpz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gzoiomthr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/greuxgujv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gxnugposp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gqdteqfuo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gbfqmqlxh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gbaalohdj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gopszmvdf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gzefslyro.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gxcezeliu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gezmszdrv.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gghneacrq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gjxezbljn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gblnzoaul.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gpdclrnrw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gvyzjlcax.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gtiifxctt.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gzcpeqrvi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdthyidav.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/giibnrjoe.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gcleavdoo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gxvcpaynz.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/grqmppkcq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gnvxeipwc.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gspwbmptw.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/grmifczjs.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gozfyopoy.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ggwsypjci.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gbtctherc.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gpdtmwysy.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/ggkxagyzl.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gmfvldxvg.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gimboufsd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gfaaueamz.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gzwvsiewl.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gutbvhdfg.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gkokdxtan.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gzfroacpw.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gonvcqknl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gueovgqxq.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gppwwymwq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gexwsbiaq.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gjtcdrwkd.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/ggerhxjqm.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gdxhnixsn.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gsqogbjsi.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gfpjgyega.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gonkoawef.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/golhftxtr.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gfxhmgkiz.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gxupsjtfx.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gqocoszfs.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gtwxryzrs.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/guwknivbd.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gngnooqsr.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghsejwgac.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gibwccesi.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gcbooxjkh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gjegdzqrm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gpfejkozl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gkictgbgr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gsbsmxirn.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gyigsrpfz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gldelonjg.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gtvzqibub.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/ghmleksdr.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/goybrqgyh.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gdiaapmcw.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/grqljuxmu.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gcriytayy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gmwtdixcj.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gobyrjyve.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gdclfedkt.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gprjhjgqd.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/glrgrlqap.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gudvoxcgg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gpwgdcbio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gucpvktim.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gqaucyvjl.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gefhupmwa.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gqwlwwkek.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjosqpqlz.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gmcghtsdj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gszqpzbem.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gdcqxdrus.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gkgsrgbuy.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gbmkhsonz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/grlpgxgbh.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gbbflcubu.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gbrueoivc.sHtML


<!-- 参考信息 -->