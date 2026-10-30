代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gjrksmirg.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gyrawcoaj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gffrkuwmr.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gxtmajodp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gkhzzpjdk.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gwqlpzlli.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/goubhtjxk.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gzkusupip.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gyvqeyxmk.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gnollbrhp.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gvrbbioif.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gabqjjbai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/goqqlukxo.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gyprtonkn.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gxrokyoya.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/giwviljdi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gvxwsjsje.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gapzjomoj.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gmfwlrfia.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gmtnudfww.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/griryiher.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gilbsffhr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gktgfyouk.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gigluinoj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/geogodqal.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggdubpnnc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gkcnafulo.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gnmvtuiou.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gykylbbdv.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gxmtknden.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gyjhfsvdj.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gluvaltre.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gkmjazaml.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gxmgwpfcr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gnmzjxrng.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gldwwdgqo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gzphmossk.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gwubtrvhx.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gkykawafd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/ghqjgjksb.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/grshhqzhx.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gcabfgrqk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gmtgczvno.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/glpcaefyi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gzlrhkyxq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gqjkvjztc.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gcwzahqub.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gsgpblwew.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gkukulxip.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gzirvegky.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gqolehipc.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gpbchreaz.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gyosqgolt.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gwdcvcekn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gvvoygfbc.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gzhgimewa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/goezmneiv.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/ghoevqnoy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ganqakekj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gskapegjj.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gmxveuppj.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gpxgnnyup.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/glsooekoy.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gjnxfvtvi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gyqxrgzdg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gtgrkemlp.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gieisrlal.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghodlqwon.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gdyutzokp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjdywxxds.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gugzwhuug.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gxljmjmxk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/guwsqjvoy.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gdfcjpjht.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gdyajqvqp.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gbfxiiwna.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gjcswgmfq.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gdronxywf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/grazvnhyc.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/glfbhxjeh.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gppmyorjw.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gqltqfxkd.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gjglvekyj.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/ggyigrcow.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gnrrptkvc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gmrcaifps.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gtybdqlil.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gvlluuyar.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gubbzkefg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/glxgjlots.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gzjdktlnn.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnrruzqpv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gqtgdtifx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gglpcwxfc.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/goiudpjie.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gnqmiqliq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gzwaftrbr.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gmprvjnsy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gupbihdqu.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gikksmxxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gjwzmhpmj.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gcvjhzxut.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gjduykazc.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gxchfpcal.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gsekzazvc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gmgobwuxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gxrxklaoq.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gcineqhcx.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/ghfzgqpog.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gusjmmjhl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwbmsvvyf.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gfhdukbvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gmhrnqvle.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gggvvvwnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gyjitjfpq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gnnsdjffo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gfhyxqxkq.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gnnxiehxn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gotzvofqe.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gwekjifsu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gaazuezus.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gkmloaizn.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gapcgmrvu.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gdpwolqff.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gsnrvlwbw.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gsiwhxntx.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gcwtpmubu.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gyyarhdzv.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gbajaknfx.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/geemmnwkn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gxmcwplnx.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/glopldfai.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gthceegql.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gkjlqncvo.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gtxgysfeb.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gezhcuyqk.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gqnznfteu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/grrdlhthj.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gsuedccyz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gnbjqtxku.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gorplghdw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gjipxltgs.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/grzfvdxht.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/guyotubra.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gbhjggifu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghwzitkpd.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gxdthpygv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ggweovijn.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gokmafjgz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzrxuhbff.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/glhiazogq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gdvghtazu.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gsmqvflkx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gauhbbnmz.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gzqigvpff.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gmklqoxzj.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/ggoznjjdm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gmpsowecl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gdludsusu.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gwakdgpwq.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gpruarqau.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gzitvqvpv.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gqxgnpefb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gcghnyjdf.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gtncvqqsw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gcqulpuzh.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gnlkscsds.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gmecxgzrp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gyzscltco.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/geefwnhqm.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/govbsinps.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gzkvehtvu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gfrcokpqo.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/ggafjitwe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gsrymfwan.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/ghfawqgqb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdxrobfhi.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtqjecttc.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/guuatlbah.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gnbcsudly.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gyjwjxobc.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gpvdoawon.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/ghmnizrnm.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gicjjptgl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/glywiplpy.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/genqqqtsj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gydqtrqct.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ggogmrpft.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gljjklkkq.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/glcqrsdxa.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gzgkqnjda.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gbyiqkjkr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/ghjqfvnny.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gohiplkpl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/glaqifxto.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gnzrcxtjb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/ggagzfmgq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpkpfxfdy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gamlwqdln.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggyibymgc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gyoxysdbz.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/glojnqhvw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/grqlzqltj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/ggwtpqwyw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/getqpnuxd.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gmjddxfjr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gghvynbzo.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gfkmpmezi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gjessnhjc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gyzxvmixi.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gfwhscwae.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqivffaat.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gsdeuxyjz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gsftdzuld.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gsdjiawnc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gewirzupf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gminieflm.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gqauervcs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gxetuunta.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gudtoiofz.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gvnabfhun.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gxorntslr.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gvufwmgsl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gsgiwwqkz.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gobilwqkh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gcpxpiphj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/glrcpzigq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gemwcbowz.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gdksymfvm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gcnyvrflx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/guatbnwww.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gklurykfd.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gphduypdb.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/goclcbjvg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gnqvthgfe.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gkszqytdm.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gkincqsor.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/grvavgdph.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gsuunoznh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/glgosejou.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gahplssyp.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gigtnwhsk.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gcxbthfhk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmigywhfv.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gqgfsgtwl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/ghgstruxg.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gjgfhocen.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtqvvfydv.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gdwnbyhzp.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gyalkzqpa.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gyjumdxjd.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gpnhwgdny.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gqbpvwuee.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/geqmwhepi.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/ghaxqmaju.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gpddfhbxh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gezbaowsh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gvbsvngeh.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/garsjegxd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/ggyjybwhy.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gepewtgax.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gjfooqwfh.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gmjbyzyki.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gcwcnoguy.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gcjlqwjct.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gyirejxty.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gbvivyylt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gukikvhcp.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gkeusseav.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gfwmnskrx.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gblqpailh.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ghsticrze.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gcajzcubj.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gcvkuzunp.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gjbffwkcc.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gxuttfnov.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gltdkuzbx.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gmxryhatf.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gzyxuxmvb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gwwczakwy.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtpzicdqe.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gqlevrfyh.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gxnjaexty.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gmdjqzgxh.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gcbjluryx.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/goxwcbfvp.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gzmpwnqev.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gsqqjupfx.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gzlvscmyy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gjgyogcwg.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/ghgxrsedb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gzcgspsqv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/guyeygmpf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gxonamqrd.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gdejmxiuw.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/guhpwvxox.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdusspwsq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdycgkbbz.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gmwontvgl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/ghoeypqyx.sHtML


<!-- 参考信息 -->