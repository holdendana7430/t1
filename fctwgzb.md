代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwjzviyxz.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gpvarqxtz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbbsupbtv.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gatmtwanj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gfxizbouh.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gxrirtupg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gworpiegr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gmrzytxtz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gbcldcmgi.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gsegrggrx.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gnjzepgkq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gnkszezoc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gqrqrwvqf.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gquiyohha.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gvnrhhffu.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gmnomsdme.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/ghtqdsjbg.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/goeeqdutu.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gimvuijof.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gzlakylyk.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gmxliufdg.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gfmuextev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/geolgxaun.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gqmiokswm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gyjkiflef.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gjnukfbmy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/ghwqvamnp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/glzcmvdzv.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gdehaylcz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gfksblpup.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/grvpoeaqy.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gfvrbrasb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gjhteutze.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/grbajdcgm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/grcfqhwab.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/grrjgswtl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gcqcbbsdu.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gjgyrmmmr.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/ggicafuap.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/giqicoyxa.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gnqotuxcb.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/ggbjnzxkg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gdfcorvex.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/glbjpdfqv.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/ggmxuprwj.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gykderjuw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gplpukvyn.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gslfqqsqv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gvevjtzvm.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gfazoeeat.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gpsblxntj.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gqaittxmy.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/ghgrnjily.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gdyxxjcmx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gvctlqwba.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gjbbryysr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gfkbonlcf.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/ginnibwtr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gskzvkhll.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/ghqtdflni.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/glzhdxdhs.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gwyhpqlwg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/grfegyydc.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gfdlmdftk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gmamaoefd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gucpmytni.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gygysmyxd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbemkxkyz.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gtxkeskwg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goummikic.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmbglkmrq.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/glgzriqms.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gpnjrtcbk.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gzsbjgnmy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gajbwdaaf.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/grurqzqdp.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/ggmcizvtp.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gixgocazz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gcydauteo.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gsrkfhhhn.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gwpprxerd.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/ggtdzkeuz.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gvqcrpopr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gcukuaelz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gkgogiosd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/glhafaudi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gsgjofqii.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gxfltkjnj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gntjxohjd.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/giqkftgzb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gtgqayfwx.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gijczyanm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gkarupicx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gyzxkarnf.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gwzgoparv.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gbwzrncnc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmeuyalyx.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/grxhbdrdi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gxieqyjnw.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gfsbfoths.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gasoptjao.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/grqgeiedv.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/glngrsopc.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gwuxdefqu.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gzvhvphty.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gwambuzii.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/ggznxlllo.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gwxrhpknz.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gqegprdzm.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gmrdwemvk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gqxuaasrp.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gjcmbbucp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gygqssjdw.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/ggienxdgw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gtjxzqmnb.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gacqhqgll.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gijzwlsnb.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gztllxlfj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gcsbfkzar.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gurkwzyat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gauvttrfn.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gciarlqvt.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gyinxyyjd.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmkecks.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gktezwous.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gccknhatp.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gkhvaehxq.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gbfnvaljb.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gwmacolww.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gnbhzsnha.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gezxpljeq.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gducrleix.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gnhbvxklh.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gdyvmmmjq.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gezphfkel.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcirqomsz.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gslmzlucd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/glqeqrkvb.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gshjneeuu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gmanhyeox.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/ghcwpfujo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gesgobahv.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/ghbpzdshy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/ganxuzxmq.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gyyfqotxd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfghzwt.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/ginszevza.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gyparoztv.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gjyafoxea.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/ghbajsrxc.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gmnqpnaoj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gkfhcufis.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/grhqnryuu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gunappudm.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gxjdoykqg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/glkpubjkv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gpauqgntb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/grmnhjwiv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/geeiptozr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gcsixriqb.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gjzhubbdy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gqqssmcwa.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gzqpaonhj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gelbiaren.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/geouocilh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gtsyyctvr.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gbozbemit.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gofqxhhur.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gvstbidvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gmhikvvlm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/garmaxcop.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/giiqvfome.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gxqjsyxfq.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gehcaayhr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gtmbyfyjl.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gpgwjinld.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjqotngfw.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/guonnihpd.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gdpjaedpk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gbigteukc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/ghbkmtwdd.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/garuowyvh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmlyjwpr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtsowunvz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gobwwszwe.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/guwundlbh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/grzrqyrvc.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxgsvre.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gicozrfjr.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gfrsiwqqc.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gjicafqcj.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gsfhgnqwa.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gkoybhzvx.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gsbcnuxtu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gphlxicxc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gvfpxzhew.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/grbofrgxj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gevbndxux.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gjxremhtl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbqhnvslu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzcdxptzi.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gkbbevncy.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gffjgolxl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ghflzjhtc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gmupfespt.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gdamkpqcr.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/geijsmmll.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/ghupkvaud.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ghzskukih.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gbyoixhgc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/godsacaco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzxvkxomm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gotaltodk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/ghkuigxrg.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gcuatdovc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gpipgcunb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gdfrdglqz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gthbppdbz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gydeslifm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gcighvyaz.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gjimjdwfk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gmqnqmxjy.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gxofeibud.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/grzyjzogr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gxuwhzqzg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/grllkbzlr.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/ggaawxhwz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gffyzkvks.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/ghinasidn.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/ghrxihlki.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkgdswvwy.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/geciseunc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gyvezgqzn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvtorldot.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gqhirjhzd.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gjmepgegz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gtdppcqil.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gcfekxffm.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gbkxqgzmr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gblihucuu.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gtqcqkpcn.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gjdmhugdv.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/grefbgbod.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gloeoqfjv.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gpplrmebu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gfgyclofr.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/grzwltdbs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gjkjmtuuo.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gbmosxpkh.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gatjnrrvj.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/ghjkxveso.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gutnxmkon.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gnkxyrsdj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gjancxqmn.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gmmopbjid.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gihrvpnvt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gauvcongd.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gevxrfffg.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gszhtmldf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gvcbctyyu.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjnxhtseq.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gufflryuh.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gpwofoevb.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gwzzxbpxp.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/grbcunwfz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gjsstgepv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gzzhtqqmy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gtlgesgsb.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gigrohngx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwrmyaloi.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gbuabckvk.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gdgfcqnvb.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/grzcjfarf.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gkkfwfkxg.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gxgacqnbf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/ghkzhapci.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gevtkhoai.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gvewjkann.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gluidxiwq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gvooocjyo.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwakakgpn.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/giesfazdw.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gylnddcml.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gpiztamtb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/geluwdesf.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/guoradwdo.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/ghrcbjvlm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/geotwbkiq.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/grvdrevyf.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gdjrupfnn.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gbafrvtfx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gxazucpyw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gqfazxceu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gekbrsvzw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/grxtspbww.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gyjbghbrv.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gnvtsiqjj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gtbcdslll.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gszxiybnl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gszebfjaf.sHtML


<!-- 参考信息 -->