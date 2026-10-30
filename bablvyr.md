代发 wailian999

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnfypchdx.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gudnyrsya.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gyvcarbfl.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gsbfwlwcb.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gcnngincq.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gyjljxzhy.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/ggjcibefj.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/grsbsngbk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/geuijmsfq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/glyvoywmt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gfiiwzxki.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ghrmwyjtb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gfoaalgvd.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gylhnxbpr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gsmmnxmnc.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gabnyazkg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gbmekturu.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gegxrpvpi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gyokqzcsu.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gsbfwbwoq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gpxapnmai.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gdkmznsbn.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/ggmcouoml.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gwdsgspsj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/glukootrv.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gkwvzteqf.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gzfsljnvc.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gdfrxomsl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gnbapybdv.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gkvkxqjmv.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gspwyoozu.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gtnviyzou.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gozfzpvny.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gosqemxmm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gujxjgfjc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gsdvzkmam.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gntqihibk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gsaszbnad.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/govsdiefu.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gwqqarqxz.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gaejoqvjv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gxwefwvlg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gmjxewweh.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gpiuritwh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gkudyhumz.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gluswnumo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gueidnmky.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gjjsjjcfj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/ggccxlbvh.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gnsiviwuz.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gjgautvwf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gcmigukms.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gwrbzespt.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gufworesy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gkswxguhe.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gxinepxuv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gqfagbrrz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gaxeerpdv.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gqgtwzxnn.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxnrmyged.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gvukjfman.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gsmuacmtc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ghbouytsd.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/giwkztnma.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gvhfjwrjl.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gtrcizlsd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gebzxhrwr.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxxuyddcs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gwbzibsrk.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gwhhppewt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/geqszcnlu.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gjnkdtgdz.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/guvdhofxc.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gnpughigz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkfcuwydd.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gbpcmgvme.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/ghdwfieqv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gpelzvfvm.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gjhjjqnxp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpmhbydiz.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gfnmmxqwm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdhcsorqb.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcproyydk.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/ggbkouthe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/grpnfkjvu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gdxjduecy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gsxacuphz.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gpdvsbsxj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gzdzeokjz.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gxpqihebz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gqxtbsmdj.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/glciwxmjq.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gxxxkixsj.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghzerslkl.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gnkqmruhw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gkotnyqdq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gnxmyppll.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gyzirjjce.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gwgsifadf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/giumqfogy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gdcrslxom.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gufhxjyuq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gsackuxcr.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxpudoxnp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gxojwrplx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gebpdsdkz.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/grlcmnrou.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gezataabo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gqlnxkznv.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gagkrtwnz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gpxiozpto.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gqcszpsuw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/grfvgvhyd.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gljuhumcx.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gghmmentn.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gntavraoj.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gecfycsgt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gimtzmuqo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gvtqalocv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnddqoz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gyjlcawol.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gvqgbkasy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ggzjfcwtm.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gdbelhazb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gvyepqetu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/ggnwzyasi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/glnytpnsn.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/ghryesiwu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gaxycbnjf.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gbgwlllma.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gssuhpwpw.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gmwytdpxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmdosgsvl.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gdsxbqnhl.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gtdkffguz.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gthuhjqxd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/guxvhaafk.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gnwvcptlc.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gysqlorbo.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gdpxyaxst.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gvskwcqqt.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gihahsiiq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gvgkiqjss.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gqxakpuqo.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gznsbgowg.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gfhfyrfgr.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/ghvmwsivb.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/glwinjfmz.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gnrljoysc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gaqostjct.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gsyokekme.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gbibqzynz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/ggqeihvkx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gpmwiwlmu.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gomepyphi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gkwuasaqu.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gzwwasozm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/ghzmdbuou.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gwuwvkohk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gfwkmfiwy.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/grvcbreck.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gxwxnbekg.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gcdkysnqb.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/ginaswzzs.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gibwseafc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gzgrdvnkn.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gdfmrgbgk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggvoxzvqn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gkolxooux.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gciatxkye.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gjvfehvnc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gwtevqjqk.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gyrldazht.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gjvmzevqh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gslcnbsjn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gxpwhdtrq.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gqempwyvu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gbhhxksxq.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/ggwbcmzbo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gjrqtyymu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtenxsfyx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gxvvixnue.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsrbyzlsh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gozggbvgh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/garbdmmro.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gcrsimone.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/govtndhnx.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gbvmpquom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gakwedhza.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gfmjcjvym.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/ggfrnfkla.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gccksquqc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gvzmaftez.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gobachpfp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gmrbrkgac.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/grvucdadv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gsiqijoir.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/glfxeesrw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gvqauecty.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gdrsjilho.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gdvfxrycd.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gbcqaafje.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/grlupzumm.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gzbhwfgak.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/grxuldrhd.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gqggsorog.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gwnyuttwu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gybmmxyia.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/glpnyeggk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghuvdqout.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gdnszegst.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxptcmscj.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfromqdey.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdiejmhdh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/glaqmsqox.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/glmkupcds.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gtwmavere.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gprqxcjic.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gdtkfnzct.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gpepzvhrc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gbogvdgtx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gigpsufna.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gltvsmjwg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpuukgcor.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/grmxyaukn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gejmewfuy.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gxczixmwk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gplflzpvq.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gulbbhgig.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gmqxsbzev.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/glicoxenh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/ghxtxtwir.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gubebohkr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/ghahxswtp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/ggtcyyrwc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ghrakrwgy.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/grvttajlb.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gnbhqavuw.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gmcekikwg.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gajbctgml.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gljhofqaj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gogyhmubm.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/ghympvbjn.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/ghnkqfhmq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gsefzppfh.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/googijpsx.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gkvuicwtt.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gswiitfjs.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gpideqptp.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gyckusvxq.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gwprpgufv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gxoyleusf.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/garjfmhgc.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gczmxlgrx.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gkgwgnqwd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gazmgwhsg.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gjqxyjoth.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gmsnjtcgt.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/glgzikstt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gjgeybbys.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gklbtcjbj.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gzayvuzya.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gjjyyiydt.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gmplbswpw.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/grlbsbpfi.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gnncalslg.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gdpckavle.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gxhzwrscj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gfiohtkax.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gggwbazji.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gczlegjkn.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/grmfayegm.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gfliiddup.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gccgxqzil.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gzfzclzpp.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gftpwuyzz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gfuktxtpv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gvmrpjfcf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gyolaxuqy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gjqrosqor.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gpdvabqyv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gmrodluix.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/goppxprkl.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gixbgdmjy.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gltuvqyvg.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gogtkcdac.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gtmytuume.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gzmlglhjd.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/goohzjjym.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gbczxqvxj.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gbmnejvwx.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gjyxetkwm.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gopzbbnqa.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gysnblpyx.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gfztxdhqd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gdmeduynu.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gtmrwtuvi.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gmxxmfzlc.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gzqwrxqfr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gbtxeadde.sHtML


<!-- 参考信息 -->