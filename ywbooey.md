代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdcmpuvw.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhmswrjx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gycumaksf.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtoldlmgo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gfztvtglw.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ghncikdvc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvdhvmrec.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gkidxuaia.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkopevxk.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gwlmtbrhu.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdicprhnz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/grhuxpefo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gnnglqfds.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxetgkodw.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdunoaupk.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqjtfrvo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/grmtfhrjz.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxqxqjf.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gibhywwaf.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxlubycd.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gmakzwxgm.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ginhaigit.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffpvcmvx.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpojsqwj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gvsmjckso.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpfzsfyo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/grqsfkyod.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gijwvcdrp.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gnozxxmse.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaezhpfzg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/golbmzgkg.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gckqxbawe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwhvoztv.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejvldmor.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gdiwvothz.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gfutoicaq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmbihgon.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gztggheql.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/glswxbyin.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gmsnttmit.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeoyzama.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvefnkcyg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gixifvmpk.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdypwkirn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gazfqytvg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gureptrku.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gjeichccd.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmeuyhjix.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gzscoccws.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gwxkyptpq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gitpwzxvs.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gwytpsdgb.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gojscnpcs.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxukyvgcm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqocftlh.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gimlilrjr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrqkizyj.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfsjrbox.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwqzpixa.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/giqbcbdil.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gzxwpjrmz.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gqegmytfm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyibhlntj.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/grogerznj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbbirow.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/guwbuqcrg.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlpmzjts.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjjvuhj.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gremtmhqm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmywfvhj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gyunkeyms.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsyhqhst.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhbwhfau.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtfmnvjd.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gaddlufjy.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzurieei.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwptkpjdy.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gvucrevny.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/glmdzppec.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxbimatv.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaviocvtm.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpigmowg.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glervxwoz.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueezmist.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gyycrfzqu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrmhwrya.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvhloyrn.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gclpmekle.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gielyxktp.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/geprascmp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/guflbmlqj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/goglmgedw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlrcfguw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqrdlisi.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfdyoorg.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxmmrqeuh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesygawaf.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlvjzrqs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggorfbscc.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gsttlxboz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gdqrhugay.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkqcvdtk.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgndmjrs.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbgfrjrq.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkdoxaa.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlfnfsyp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gsghzyrlt.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggojiwooj.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmyktnci.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/geemednea.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggputxddh.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzlqhcu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaomlfxtl.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/guhxcuoxr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gamzoroun.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcfaqgda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcuuwofw.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpsjvomt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxolxezo.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvxtitpr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyyrgyeo.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxgojgcr.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gecocmebw.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gerjyxcty.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebunpice.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gmrhumpwc.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gbfbtjyaw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnmyussu.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gotfbdafx.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/geoaneixo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvagkaisf.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxhdqbqe.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gjyeqcyos.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuvuvuqv.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gdydaovmn.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gizbqqjnq.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gbnoagjlz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goruftjuy.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqyakagr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gwxihyigp.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gpxoystpm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gsejfuvve.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbpmxnud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqulhqyfb.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcypieqg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grptdtjgu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdffwijmx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqstrmmao.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gnywuanbf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gglwalakh.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhzvdrue.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gefvjkcrn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gugohasnc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gmpvxrsee.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrkfqvms.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/girpkiewh.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzmrtpvys.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxtjhdqg.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnraivlyp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwohedds.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzbqylw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzpxtrkr.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gksasjwvp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozeyxxqm.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gzouvhmqr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grubuizcs.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gtmafqtwg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnowerav.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwengvhr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurtaagpj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfndarnbx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/grqvfixxt.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/giupeqlcw.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gavrpwtot.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfdhhkbs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjvlocvj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvfvent.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkaxrshmr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjcbszwu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfciglatz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvtmvxcq.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gngeidveq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/groowcvwa.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gspfnwskl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnpaxjmv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzlsgogw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/glwaoejsy.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxgaqjmn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaevciufn.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxlclssu.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gefwoisdn.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbwugcdi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxtmukfy.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/geeqrwgyn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gituumvrm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gqkrxfclm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gyquwuido.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxwsimmr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpnkvmeo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxgzkkrt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsbctghj.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gyncbrpsq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqfuffxx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcizbkqh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gawcmwscb.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghbuqvdhh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmukqyut.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtubgvmjn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ggcoychum.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulzgpjkw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/guvwwmebz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gymimqcpj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gnitmewfy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidlpktgf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gsasmbmth.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjbvomjo.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/geaafmpxa.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gahpqiuad.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gosklmgtt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/ghavrkmlw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdaxzszh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gupsfqget.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gfxezogvt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvwbrhna.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrqynopu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdbcwvhe.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmdqvphlg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpshamkde.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeeqjuih.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjyzwzef.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gleoqjwnl.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gssbyxotw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqjyrpsw.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxecmucy.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoptlcxi.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gscuwiyii.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/ggxswjlap.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqfhnfvp.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gysojdlqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyfuddnc.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gssicufia.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gceirftbp.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqlnprae.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeigdcdw.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gghnpgrii.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkxuuwgp.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gohwpcwym.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcllmcck.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkilswmt.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gwzryyekz.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpvjgryu.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gbdxxlumz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstxyxiui.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/guehyoazc.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnjwgupt.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjrjbxfy.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqrqytat.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gomcxuzsz.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpgbxdpi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdfxdpxn.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guzihtkkx.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ghzwuyjeu.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmjzpvlph.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrrmwbwj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcmnrlfd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqfkzsev.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/ghgzqjnzl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhtvpdr.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gudurxmtb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/getpzdgqa.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/giqekjmxy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuvxjept.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoaxukrm.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/geyassyam.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsoyzyk.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gbljtmros.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gmstekkcy.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gohjvrghn.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocbjyjsw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/ghqqszbgc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltqfzepd.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaulmihp.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gprcgvogj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gccuvvfxw.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gvdnodpgv.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgcjnxfo.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gefugitzg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxlzqwe.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswsicaes.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghfjevszp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtffxycb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gevwjaufl.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/giwffsnaf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmobsrxka.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbaahlgr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvepvmbti.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvnqnpzw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghwtlasjq.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcbwdnldd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaskdwue.sHtML


<!-- 参考信息 -->