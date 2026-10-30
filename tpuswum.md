代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/ggdbhfbuh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gwtijlkyv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gboxyclzj.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gdzdrppcz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gdbitqswp.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gflnupwhe.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gldnhdauc.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gtbwxride.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gohnknzjm.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gsgeduijl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkiqoexnt.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gsquzduys.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gdrumdjeh.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gvfqawknn.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/guvejkkuy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gelebrhlm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gmkstxmtd.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gkloqfihk.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gxzhgjete.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gusetvzfo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/ggunrpoua.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gscdnfqee.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gwofgetoo.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gdrnvgppt.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/giaufoefr.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gaoxaerqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gxhiqjnhs.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gyirdayca.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gshhfydzf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gktezewgg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gwusjbijf.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gabfwprst.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/ghlcotnyy.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gtlcxntqc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gkrrxkkhc.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gwfscsunm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gfnfgpogf.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gsrknqevn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/glwmityng.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gdahfsgvg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gxceqbdsi.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gpgifkzqo.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/guaexiysn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/garckddsy.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gknttysaz.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gofiajpmb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gmfjfdpsb.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gkpobdfww.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gvvngiisc.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gqnrpaqsn.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gwraugozn.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/geufbxheg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gispylafd.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gafgvjhts.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gilkljcyh.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gznhqpcej.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gxwqkvcib.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gfxmlpofj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/guwiomgtd.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gvekzsrjm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gidataxad.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gnveozfzu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gzfmkqsqw.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gkjnpxkti.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gxjcvevyx.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gyqvzqmkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gnxrhcqme.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gwrzqvtax.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gzjwfarlq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gsgnpmigg.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gcodzpdiz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkiibbxsr.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gjgdhrlfl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxnooidmc.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtaiyvzrx.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gqbdnlvls.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gpckmspox.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gbhcewpoi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gxmtallca.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/giyzshgua.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gkmhnoxzi.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gjeomipjo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gkaplrzty.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gurtekdds.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/glxxkcmpm.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/goqeeuqat.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/geugfuxdf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gbmmeiood.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gdvrskftl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gsbnjpinw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gojyzxpji.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gngysohjo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gjyjuaiep.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gamhtmuuu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gvklhzhxf.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/guepinycl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gbllbuiwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gqoxzvmmt.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gzzwzxqpa.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gojrhtdel.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gpbgmixsz.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/goymfargc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/ghsohrhtf.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gpiltxzoc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gpkyfcvxd.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gwzxxyocf.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gosrqvrrv.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gztshgwyz.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gsmnscuiz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyemeilml.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/grjpnxnrf.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/glepicxfh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gybzxnzua.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gncoabiaq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gjrwdvgso.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gicjhrqen.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gakchnpbi.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ghdfuyqnk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gztywbphs.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gfxmucuav.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/ghihhneur.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gqlhvfjcj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/ggpmhscfv.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gxhbhevlt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gdvzgmdin.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gxtiighpl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gngscptym.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gfdumawjg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gqaudozmu.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gnvqdcgce.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkhchozif.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/geckyqcpr.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gsuggpbjj.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gdmdpkool.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gckarsqer.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gpcfefxqg.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gszhwupgu.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/geokbvzhn.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/ggztzreno.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gihunbmdf.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gtojjprvp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gwlvkigle.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gktyintlj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gdkpjvvav.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gnojapsqx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvvbhyfxv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gzyxxhyus.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gjomoctme.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gborwblne.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gvrusewpq.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gcmcfccvs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gfhccmfjm.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gqwrioxxs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gdyxfuseo.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gzzafaggu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/grbcwwtnp.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/grofdtmxd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gduumcvoa.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gyfadccqs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gtenflmjj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gizhszczn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gxpzwncmj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gvoxjwlms.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gwoiiyelj.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gxxyffwme.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gjjmcljwu.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/geknrawhc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gsxmxpens.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gyxhjxmue.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gdyiwqxda.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gejbpauoo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gefwvkzdq.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/grfasrqxd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gseuepivd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gamkktzja.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gxmzitpgc.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gvzozjvij.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gqxzevnmh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gvlyzvevs.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gcnmyrroy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gqeyxlref.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gsmnufktw.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gglenjydi.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gvnafyora.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/glfslyane.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gunkviqkh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gyhvxawjp.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gcdtwotnx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gotpbgkuo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/ghodfvvzx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gvqedydhz.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gobpevofj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gzrgzxuam.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/glblmrcei.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrfnsbtz.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gpickoyhk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gtnorjspe.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gqpimsjqq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gopkyyivg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gotmrutzt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gypflfokq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gruuzynvz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gvlokvhzn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gumcqdrcl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkhmrzrdo.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghxtfwbnd.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gftshqrvo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/glskzarqh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gxsgtaacj.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gleaufvwb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gsxjkhjuj.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gtxnlsjgp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gszvkiipj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gyijjsegs.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gaoavlgtz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gnoawkkfk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gpnecceoy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gvpoxluii.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/glxapqswn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gyuhyswjc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gilxvbnlk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gijaxvxbq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gakelvnnk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gitklwbxl.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/ggygfmbxg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyntnlhd.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gjnalexlz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/glmpsipsn.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gjvladkpj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gqorwraez.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gabusneqm.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gtwqcymmo.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gnlxjiuso.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gkokbimhr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gddinkrkw.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gfjeeqolv.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gmqizwxoi.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/glrdvogta.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/giuhkaupo.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gqvrksiaw.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/ganjiizzm.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/grhqkaofr.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gzmihbqxu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gnjxyhdlz.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gcjnuhhlz.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gjqpjngkg.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gebkwozzf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/ggzaiapii.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gghxskgyj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/grcltjwwa.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gkypwaqwi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gcomdpcip.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gvpatiljp.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gnylvroxo.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gqpqfzafr.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gdehtjssz.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gbeihcqjm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/glyvjrxds.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gfeiezeae.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gnxyvtpuw.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/ghhbzldcy.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gjnkbtmec.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gykwixguj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gprxjrmux.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbxysmnmo.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gveftkoim.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gbodwoubt.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gzhpdxjfd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gcyygamku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gdhfoogns.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gzwcylqso.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gmbtdzpxs.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gfgnxiorg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/glmtnosdw.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gozpcrbyc.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gjqcwppak.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/giqtfmoot.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gdwlaptcc.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gzathduby.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gretwlars.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gzgglurmf.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gtrwjyead.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gpkursaer.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/giqeilbmh.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gninsfvkc.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gnlotrizo.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gcblkcsib.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gudafbbze.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gpublkzix.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gfdmiqxxn.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gmxizvett.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gnpsikogl.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/giemmghpd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gylkymbdz.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gmejhnbjj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/grungwzoo.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/ggooqizxh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/goxiwoabl.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gaugxajze.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gjikcqpgl.sHtML


<!-- 参考信息 -->