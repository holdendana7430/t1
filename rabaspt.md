代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrxgdnmk.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gwffdnakk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpmztsazh.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gfmuavwas.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/geuarvnwq.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwfgwwqe.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgyfvofq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcmcojaw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gnkbjhzgc.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrqypwun.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdcabkjm.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gfhpqesxm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ggcamuthz.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbjcbihh.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gunjoyuvv.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gflkeiozb.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbpedezc.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gddduvwwi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/geqpfzshb.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/galvqqbyh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmctgfddg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gibemnduf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbzyisif.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/goaciuoyx.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gnknwwhkx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuiiznuy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfcjwsqj.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gftazvbcs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxaozoid.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/grvgznwxr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhlpuxdz.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/goziankfz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkhbewes.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvjmhwvr.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gsulhumof.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gdgxmnuya.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/ggyumxhzd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvsduydo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gezwacowc.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrvargrp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/guyhsgxvy.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpawqatg.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbteeoxx.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjvdggbm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gfaiyytdy.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvessukqq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxrivjyvh.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gahzdfoll.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzcqzriyo.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdlrloka.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyneknml.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grjpthzur.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkcsiqcc.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkcvptmo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gcrdhttvc.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gqnbpdsui.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/goeinojba.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gcswenkfp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gurycmdum.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/ganynxdhc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gakmizhqy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlszqqdo.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdjaoono.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gawjwexdk.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/giemecwxe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gipfluhnn.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzjelxat.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gfygekfhu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuephtae.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gwlxwzsxc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/grivkriln.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gemoiinzr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjvcyibn.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gyyyrsabr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxytqddcc.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpmisngf.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcijtkby.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdcadyoop.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiuucosi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxayfwic.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimhytjnb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoczsmhm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gerqixhlm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gggvzcqeg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gxifvnbdo.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gobknpiep.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gdhqguafi.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goppizhbz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtuohkac.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/goyzxliza.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpiisgrs.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvsgqunjo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeeoafip.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gkvmbvtkk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/goqsayfdk.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtvithlj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsilvuchz.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/grbpbbzoz.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpziynhr.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxdqhxui.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsgihaqk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksfzwytv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/grfkqvnbn.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcneefbcs.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvpwuhct.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gareffvrs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ganlyucup.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdymyoix.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gpsqvekxq.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gghgxiwsj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/glrgqkrya.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlcslwyv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscnakknc.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdsclpkv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvbedmcb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfsnrzxi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghafpcahi.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gymnpselb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geinjeyry.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhzimjkg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxcknlley.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzcnhzbh.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfisjvuvm.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsnqcvxaj.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtmncdrv.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbxrygjmj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gdyraiaih.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gvuikksmh.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbejndap.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamewltsr.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqcspowl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqbedrwp.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqfhega.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtsimrnar.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdsouunh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggndlglvu.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjyputun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwotzfabj.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngqlxwpc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsejllykw.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ggaissyth.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gqcwmoilp.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gflwldmhx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnlrvfezd.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/ganowwpyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gfupiuetx.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grxhvbmfe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/genytaibd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyphsutlt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/ghjrmshbn.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvgycqzm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ghrhlqolm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcjgwtnh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gkmichzgu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grblmktqm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gofhjpbqf.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhrycqv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqygzvrvn.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gicpwefwn.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gogcdxntc.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gdxetjkbj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gspafgynx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijvefiei.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkipaeqfe.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gurivermt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkdiylpo.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gigynbtsi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/grelxopzf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gocjjzlba.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsztmzsn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyadmyyz.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbovtnsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrwgtnsq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxgiblgb.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnncamql.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gkflrzcbu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goaddexpt.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gkszzabxs.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaaboojt.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdqboudas.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/geawimzag.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/glwvgdlne.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzblvratd.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gxxigwsut.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjcnmzbh.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnytjypv.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggetnjipw.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbotsyibx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkcxdzhi.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdhevhed.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpntfgulk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjccojgxq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmsjkxux.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpfzdvgha.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/goufcrhkc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvwrhinra.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpclynklv.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqrpaifem.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gixztmdzp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gcriejwgi.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gijkwwhzd.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxddsbini.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gvqbcgzdt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatkhspcd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gyhvwjdyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtyzqnxk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gglrbzlou.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmflmrlez.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/glzzxfphq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/giyvyioie.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gdjqhduwy.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gglbtsawg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxlspzps.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gdawiswau.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjmnnsxku.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gfuhgzxps.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/getljnuge.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklkoiqnx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gqcohtbtw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glcexqegm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gimeitlng.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmnpbbqj.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwcenynyv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuhfgfpz.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gwlnqhtyl.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrvqcjvt.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guqsbzzky.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gpqhyuwzy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmwmjtem.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvhjebihl.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumvdjsct.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gezrplnij.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gtweeawho.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyhydoeua.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/giainchtb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdvrijnt.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkccsrsdq.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gorguxkpy.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexdtqwru.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgqnelak.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gygmmohuv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvsupdzs.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gwppokazd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbonlwlsw.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gciimrfby.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gwfkdkriq.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/glotijrdp.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoxkggmv.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gysivfdrq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvqgqccu.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gjllhefdc.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnuekxsy.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gdexbldrk.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnllgjkgy.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcqhfzdx.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvadljmsq.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfvwjhtho.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gabpipmdm.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsbrhplm.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/guavbkcut.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfifaktod.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gmyeetezg.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gphfevkrv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsrqhvii.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gyusqgyvc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwblazcca.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzifqipwr.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/glrtiolns.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/glohumswk.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gukevqqri.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpbefwsf.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqpqcmtg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmazkrcis.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsfjvazb.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gipqbrlts.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gplnrguur.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgttylxk.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghutvlvhz.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkfkxawti.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gamvkdzlc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/grcidnabf.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdtgibnj.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtwzxgyxz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqiesbrt.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhlfchnx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjtdcjym.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gdkrlqyja.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkbyvtvdb.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkciitrt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfyvgjfay.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/giyjdiznu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/glthptnoy.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjlkfnvp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/garfxzwkf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjliyhssn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvtaukgr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxohyzwwc.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhtdgbps.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gpffckhnq.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdarzyrnl.sHtML


<!-- 参考信息 -->