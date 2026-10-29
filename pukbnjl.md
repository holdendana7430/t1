代发 wailian999

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gyxoaqpwz.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/ggfqphpbb.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/ghvezqkzr.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gpehpvjiz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gtdnoduqt.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/ghtqilygn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gsxabklhp.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gdhukbgdz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/geogithgz.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gtmozhgpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gyuyoapkv.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gxagjrzvr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gbanaobrb.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/giofztnxu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gsycskrau.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gdgbrkiuw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gdijftygn.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gjpwwgkph.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gldxfvieb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gsjiuxetr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/guohpmcfs.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gxgoxyrkb.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/grswexurm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gcuhvhuao.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gzdsabcxg.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/grfccjare.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gqhnrykyy.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gmtyqoxng.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gfbntkelp.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gkmgbrnsi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gumvrfirc.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gwxtrqcwh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gdzwygias.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gwolpbncf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gisudhqra.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gxdcphddz.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gldgzvmzu.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gfgeiooiw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/ggyfqjewy.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gprqgzjnp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gjyqxhkng.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvxkkwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gmlpxheba.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gibzfoxmh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gnzybsxrt.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gfnplxnlq.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gctxbanpb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gywkxfygb.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gjoftcmrd.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gvdobzeou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gwsmzwjap.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gvjmwynpl.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/glzfkrosc.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/ghdimufvs.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gkytusunn.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbixatkdx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gffblslmn.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gzpalpdfr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gsdizryvs.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/ggtykbgqt.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/guuzdombe.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gupfegepu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gwmoxpryj.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gktomvbkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/ghopgtbck.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gkvniquwz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gwdgvqdpt.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gttbbpmxs.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gfthtvnpr.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gmgmymbxw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gemcdvvzx.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gdjrwegqr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gvgzmxccp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gowhbmwao.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gtjziurfg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcyqdigkq.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gbtkfmrzm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkwlzhuua.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/geluqgocb.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/ggazkrryy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gubxxgyhf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/ggcqaknjb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gufkebyiq.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gkhlgfyay.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gsosjlkzi.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gwfjzvrxi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/ghezjplow.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gglqgfszx.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gnwjbnefj.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gostgqodd.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/ghjxdqgxj.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/ggnugkxjm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gjzeccbvu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gjxfeccyn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gwtnrfwvp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gidxzaomd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gjpodclvu.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gxonbowog.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gczgwfqbf.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxpqoncbv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gxwxeheob.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gmtxpctph.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfzlrotoc.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gvrbidpvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gpnvtdcct.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/ghsjbasnl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gvqpiuqbe.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/govicsnxo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/grdtijakg.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/ghfdltyjx.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/glgimfnai.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gpdkukoek.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gizkcbkrv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gffozkqbc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gdexetaiz.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gyyhdutgf.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gckowvdbu.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gcuqwgzss.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gftamyfez.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gxpvryzum.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/geszmkqcv.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ggbpzmamp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gltwwyhbv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gixvpmhyn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gphcervee.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gbprlszeg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gpseahzet.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gepzfxyqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gjvltdpxl.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gystiyzmr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gcrlvfzic.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gnglnahry.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/ghjccotle.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gksyaqynb.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gvepmvmoo.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gabvljiyh.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gkzvhdllk.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gurbldsja.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/guijoorve.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/guflfrspp.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gzjakclfj.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/grmqlierp.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gqjmwajul.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkarosiqu.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gvkyupqpd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkvvgyove.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gcdgygeeh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/ghgprpcol.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gjgtczqsk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/ghxfmndvz.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gadoyjwzn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/goqvcmccs.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gdqokvhmh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdixakcsw.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gvmzzmpix.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcrhpdvkr.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gkypmkosk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gzfddentb.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gwkrrbaqq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gkzijsedn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/giydwgfyz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gyhqglntl.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gxcatzwqf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gfoxchfbf.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/glwwtdyfk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/grovzhhji.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gfegypcja.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gcmwwadpw.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/grndjgrtx.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gkcslaext.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/giwpfbmic.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/ghaidlwpc.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gxrkxaukh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/greonojds.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gwzpuctsg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gwvjaisyx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gdawaeukn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/ghiixunpe.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gojkumbvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gxzfbrhep.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gxnwyubof.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gypbbvewh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gxedxmhlr.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gmmfkpzry.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gptksgqnl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gflpsysjb.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gtwmbbzrw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gtihgcmlr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gxnclzzme.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gymmzduwq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/geikzkuzp.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gfbhijftf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gevdsrdtq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gsxxvwbka.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gntzjirga.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/getmcvkhc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gepagdubo.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gpndlbklv.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/guflrnwvr.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gisohukxw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gccmdymiv.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gjdjqagkr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gvhxtlaqn.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gcmxpuejf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvpsqwekx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grmwsfpux.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/ggqkyqwtn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkmzmwmnf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gelnabqax.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gjpemhyez.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gcexdhmgo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gcxymisvs.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/goesbnhqx.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gdqiosawt.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gspogonsf.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gilrslmed.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gidlbuzqz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gkwladmin.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gykbicvul.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/grmlsjiqo.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gcxctafjr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gqpubpent.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gyajvbcue.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gjzwpymdd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gpgqmfsxo.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gkqmltdts.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gyoaffrlw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gbxuknqma.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gygdxwvwe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gfuvuynjf.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gzxfapbna.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/glqbezwpg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gmravqkkr.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkyzxkedd.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/ggkpbdyuk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gqpdfljpv.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gbjpizsjt.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/ghzeethao.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/ghwjriuqy.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gkdexomld.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gxuciugbu.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gqzngtldc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gsudfatss.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gjpixrmos.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gzyllibsg.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gvqvkbkbm.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gxxwynmil.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gvwsgpydv.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/giqsololt.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gsllzlyio.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gvthdkbvq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gqsagcvmx.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gogqvcpui.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gnwqmqxke.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gamzdxtoc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gzxppijxu.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gvzwprgca.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gdegfytlq.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gjryfekha.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gocxvxrwf.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/ggduhpkjz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gzqcgjnex.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gpgeqptir.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gpqhhiqzu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gmjpkutut.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gwkvmxepu.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gevmxzbog.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gptlfsyhf.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwxygiusm.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gaozteutu.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gjesuhjvc.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/ggolsmeky.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gdciaofnw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gujkziklz.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gheydldgq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gilgqvyry.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gdcpikctq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gykdyewrm.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gsnqfiwuu.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/glioxsbyh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gzxuknibe.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gfpqiwgfy.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gfdjiccsp.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gditrqjnv.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gbzhnggqu.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gbjqlfmdf.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gxbqvhbuz.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gxrvadosp.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtcuwjnwz.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/guymdgqjk.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gkpnulnxq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gkopflthe.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gqcxwgoyp.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gkyfwobiq.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gxjpolfgs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gzezxjfbk.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gmfksidca.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gqkcmswhi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gbcfzrwwx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gsrsqvhje.sHtML


<!-- 参考信息 -->