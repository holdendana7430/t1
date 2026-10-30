代发 wailian999

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gtknoiyjz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gjwrlsevy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ghputugaz.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gqhboxiiz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghfnvdmgl.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gsjuuiebp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqdwfbujr.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gzujtfavo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gtprubvci.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gekirwnho.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gczwfxymw.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gekssqsmr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gkvmumygg.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/ggsbfjrwh.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqeyclywy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gzwxbwwdu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gedkjlrux.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gqhyfdzkb.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gbkgvvbay.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gxsgezemc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/ghyudmwhr.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gkzaxhueq.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gxrtodocc.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/glhcfvxhs.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gzqajzzvp.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gnmyrpgdh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gkaiwvovd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gruzizaoo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gwsjcxpxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gopjemyms.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gexgghadg.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gmvvzsnhm.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/ghgkdzojb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gujbqsrcq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/goztqzwfe.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/guwqxzyiv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gcfblhmnn.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gnmwkjsaw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gmnthhgiv.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gkkrvtdqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gsyogusxp.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gmuifhmvl.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gxetzqqhq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gbciiymqx.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gvodsjdlq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gnbtjzqfj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/guhdjzfpc.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gybesvcvt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gzdidkopm.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gefsybgyn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gzjimmkon.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gppqabzou.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gyxfuukey.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gklbfdufw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkidpiius.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gtxzgomqh.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gxbxrklxc.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gkfaosgtl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gvuicdfgy.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/ggubkcvzw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gjvtjezmd.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gaqnkjifi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gcmjqytoc.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gderrkddt.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/ghbkagsdq.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gjftiyyxs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gywdeddij.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gzjtuwpvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gpiswxhxy.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gxtqeavkr.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gmpipnstq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkgzsypar.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gunztdppa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnljqpftf.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/grtlmpiki.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/ghvrqkhjd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gsvhtbggt.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gqgtvyfau.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gcpczzidw.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gtglgwbou.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gdzzlqhmk.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gmcafuxby.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gupmslhrm.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gpakwzksq.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gkqebeqyb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gvmawhdsm.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gmrsnwkfd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gvrklssit.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gzpatcxbw.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/goacqyakb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/guykegofo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gnujvlaqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gxpcylmwz.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/ghixnjihv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gcdhhbofj.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjtbkyfmt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gxalziydj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gzsgppcdf.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gidgvmnki.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gjfxruodm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/ggejvjnbq.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gtibfhmdp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/glbtvbigi.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gvjueycea.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gcobppbqn.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gbwarhsju.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gitjjhbbt.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gcyzwfgxn.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gvcuwrqxx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gkzrpqaik.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gxohzztld.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gmvkexttm.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gkjmpbhwf.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gtcuowvso.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbudnzwxj.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gfvinljjw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtfpbtaim.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/glpiemgao.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gazgasrgs.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/goifrdohu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gbcgrdiuq.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gjetwmsfe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gqtgehpih.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/glsbwuauw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gdzsnxqst.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gwcgupsec.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gpwptpwgs.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gfqyihxlc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/grpgciqet.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gkiahqpcy.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gqbehmaht.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gulrvcrcb.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gidixnoqp.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gflwtsgtq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gcykkkhiu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gotqwzyhi.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gbeykmzlw.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gimxavdfh.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/greyrxznw.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbtskmjep.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gilmjipky.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gpuqwsnil.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gmpizjnfj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gifcmrlja.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gsjmzwlkh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ggayfsltl.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gmfusmyrr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/glclwmigu.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gfhfhxcaw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghppmnpnw.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gqdxsnjyp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggkkcihkc.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gvmupdcsi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gfqcunqiu.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/ghovjnhym.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gwtwlvqjl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gvpugarbr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gwnrmjqei.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gqgkumgzk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gceaoqill.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/grqkbauhr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gkzpbnbeh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gwwjipwhb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gthudwmsn.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gkyunayqo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gfacktesx.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gojhataqa.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gjbynznkm.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gqcufxink.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gvgvhmloz.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gwtiguyne.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gztxubfjm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gkkowyjxt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/ghsrootwz.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gfzjajtug.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gjkgurozp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gfhltfwli.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gumlkwdio.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/ggrefpszp.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gtrwkggvl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gqxsrmcgw.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gtxdfnqef.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gjlwqplyo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gflrodlld.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gnnxjwkrw.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gyumdvqxe.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gfwywugta.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gbnoondop.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gxnoihokf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gfwnsdjje.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gfkzhqqkm.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gfbnycagu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gwqtcwbrh.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gldpwcjcq.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnyamppmg.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gpmgvzlct.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gxcrlwwng.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/guojimetv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/glzdbchqs.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gvhynidyj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/grjazaynx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbjvumzqn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gixbqycsw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwtemrgiq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjrreqbcm.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzhcakvvo.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gkuxttinf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gjksdarjz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gwibgqjqw.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gvhakxxvo.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gafcelesq.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/giwhyfocp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/ggcxlxdcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gwfbjomsa.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gigwggwan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gehobjpbe.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gjpewmrax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gugawhfor.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gxtvailuc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/guaobbtgr.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gunisqptf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/geowidvee.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gvzsiltdd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gsdliuqhy.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/ghcltzwix.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gymlqmryv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/glhsmwery.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gyfjwlyak.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gwwiezola.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gyiwpqueq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/guiutxwqh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gampbsejl.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gtlfpljnd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gcpurzlcw.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdnrlqwxr.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/grkguzugj.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gvwaysmah.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/goxvhvsgy.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/golzwumvn.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gtidsruii.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/giitjvusa.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gvzumttyc.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/guqduhcwq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ggrnjbyep.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gzrgdxmro.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gkltxfspb.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gljgqgiot.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gjrbhaupe.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gumdwjsoa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gprpnwlqg.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gayiagocn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gvhvzgtpe.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/glhoigfmf.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gjcesflpe.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/guakrcfql.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gdggkmdao.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/ganswdvlu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gykskrduc.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gbybsdbcb.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gxkvfqart.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gfokfehox.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/grkrtgjlx.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gsfripntk.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gowniklvw.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggyiwdhot.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gvuhgjpdo.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gductdbyn.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gptotaaek.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/groznnmvv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gsuitetku.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/glvqidrxp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gtumvdvoq.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gbmvddssd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/guzhjncyg.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gytvzgjey.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gfnygnjit.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gmyfsqyue.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/grmgzpsqp.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gzxtyaqkt.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gxcckocne.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/grcpothlz.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gufjeyzxx.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gihbctdma.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gujilrbmn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkcnooy.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gcppluicn.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/glkdzluxz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/ghsqamdho.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gbqyqdxcb.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/geoebsisa.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gmlzgsfdu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/grsdozdce.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghkrtrpcz.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gshaaynwv.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/galkdzssh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqcfswnlm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gbkkxjmht.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gqqbyxmyy.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gpgmkektk.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/ggbfczoyb.sHtML


<!-- 参考信息 -->