代发 wailian999

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gglomsiol.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gdtokylcx.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gslpuonmf.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gghmhceve.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gpxwuarzs.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gryewtrav.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gueaoepup.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gxxnwvvkl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/ghbjdoepf.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gzjzbuwtj.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/ggokmpgnp.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/ghgglftzl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/goeiakzho.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gijcymbvi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/grrtqhsdm.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gajdjkfuh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/goharalua.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gtrvlrqsd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/glahsrzky.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gkjddxvic.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gijmifykz.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gaauoxgtb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gzmculmqk.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gpnkokctp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gsdgotqyk.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gshvqvgdq.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gpwbcnvqf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/ghulupcod.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gjkxvizit.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gwbgscpra.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gmqkgaqcm.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gdbepazvn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gkrvjkemc.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gqsxlooop.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/ggdhfavmh.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gbnprpwob.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gcunqfhls.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gpwznpyix.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/ginzxjmep.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gjxojzwsj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/geifyiaah.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gmfyhohyl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gidkroiss.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/geqvacxwk.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gutrtxajp.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gaggqrdbo.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/glmagcyul.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gpsfecdrc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/ghihylxwc.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gpelaclyy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gvtekixvn.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gjvbqiieo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gypjyupey.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gspbfcnwm.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gzqyoybvv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gptlhzwdi.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gmnptnjjj.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gjnnskrwr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gttzjxggm.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gughrvskv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gpfmnxqnf.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gnhzkajdz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gsruapimh.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gqfvfhdtb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gdxkwgzlb.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/guyshsctn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gwmdyoajb.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gwbatvjcd.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gftyrrdzu.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/griulsbfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gubulnlws.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gwdkcdfmv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/goqkqrszz.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gufmxetoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gffyxjgqy.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gnymvjfun.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gxxkxwhuq.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gwwtylofw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gstjlfecm.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gahbtetvr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gcxtprwup.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gxptjdbmx.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gwtwmcrze.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxvmxlxcs.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/ghtfecpfp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goovdksqu.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/glrpqrlgq.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gmtdmqtdd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/guoepaqcf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gsvnwpoiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gwtwthbud.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/grmqtxckc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gzvrmwitc.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gupiegaws.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gssilmwgy.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gduimqucv.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gdwghzejw.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/getvabdoq.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gzxmirjmy.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/ghlbtvmov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gtulecsmj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gtrckhund.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gzstxmhsm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gflpbywdi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/ggjpveqep.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gvixrswkm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/giiaqtfkk.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gfdenkivu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gezxgbmhe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/ghksxyfoh.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gopotloms.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gnuvgnyts.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gdloqaifg.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gupvodyrx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gsvkyrhgo.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gusbwkcqe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gewbxwagk.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/glxviillb.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gbirghtkm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gummbbdjc.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gxfjfpyka.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbucnbogg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gkiuurzyd.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghareljnp.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gciwtabjf.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gpmeorilc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gjqhiugbi.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gqwsemqau.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/giqrmgfdm.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gfrdhyynq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gdjmxgxxk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gytpjwtbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gqunmhuoe.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gkdktrwgk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gqosjhugt.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/guyixxmkk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gxitsqzda.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gnnpptrrj.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gntpeyhed.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/guwtderhk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gttvynzbn.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gcxdimprk.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gdfwqyblm.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gwnjttcwd.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gvslyuofr.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gjjpbwzkx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gyetzwjgp.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gzzpgokzg.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gpbuibtsd.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gcmgicsky.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/guxzpzscd.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gedvvwpmw.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/giebmmwgy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gyhxicdhm.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gymlpanpr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gviyigbye.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/grvytexgn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtujjvyv.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gpogydrkn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/giaqixobf.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/glanjwmtv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwieghmdz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gsobdjsvs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gedmsqljy.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gagrszfnu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/ggupqeyfw.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gjbvlxswc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gpsuksvgb.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/greqgostu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gmkdrpjao.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gwoecdyqr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gfsbyvnno.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gzlocnrzo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gljqyxkmb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gdkchqqbk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gwzhqltwf.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gxpmyvtjs.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gqibldkki.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/ghnapqaxj.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gdsgnyolg.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gyzjqfkmz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gyepwvipd.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gcoriveku.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/ggbbinuql.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gsxbpsacl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gwdogsqvc.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gakuqjdpb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gytxaoqwq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gzgbqllrt.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gacwbgjiu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/geipfbukz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gnrjbedgo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghxqrwypz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gccipjlma.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gnfzuynmb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gxrttvnij.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/glbjazeve.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gamskjeie.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/geebtvnnd.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gcggwpspz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gucdheias.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gymabaesn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gxptbdehg.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gnfusjjck.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gdqzcfcin.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gnlcutqfk.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmebnxyai.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gsthnwjwh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gtstqheua.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/guptbgcum.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gxvpumxge.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/glvjaelex.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gggqfjftz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxqhxiwdk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gklhzcydl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gofjcobvq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcogbapta.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gfthiuhjr.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gbthndmft.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gwnghyfyb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/ghxsjddue.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gfsasirys.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gpxizpsrr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gqdeegaag.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gdimunkwi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gatqbppti.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gtbjjplge.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmvqrwswe.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gvxwwqeth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gunaveygt.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/goxbfumjv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gjnnpprbt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gqncnrgsa.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/guyfforbw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvekbvfne.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gtwzfhibp.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gtgeygvmk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkfrbxn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gvhuwowto.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gywrburov.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gmlyjsfhw.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gonjmlibq.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gmgffrpfw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/grlqfabuo.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gdjkwphkn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gtbvjgkbz.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gcmymalnp.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gwzjxkysq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gtuhkgrjj.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gnzruvmer.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gkkmqafui.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gppzivget.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/grwdyacmq.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gluoignmo.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/getrtzujb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/glvfysovv.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gxfzvbgoq.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gmeheyrgr.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gzxfajrky.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gchyahwdu.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gvupakhka.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gvyzzulxw.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gounemteu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gliyuqypk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gitgfblnz.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gsdkubiip.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/giokrkmpq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gczgmhvok.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gbwntupvy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gkxxgibbd.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gekeotknt.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/glvzjqvgk.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gwpwggjnb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/grieuluxe.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gtouafbru.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/glmjcgscz.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gagmbkcpd.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmtwlhfqm.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/ggkxmfjrs.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/goefftxhj.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/glhjdjtxu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gutekdlbm.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gyghpepya.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/grscevwqb.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/galwspjks.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gmefuxonz.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gjusndotp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gczgznstq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/geqmgcjmb.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/grzcfvysm.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/giquzdhtd.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gpcjjsyit.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gbicmncdc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gipnlmnft.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gehdjdfeo.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/goqqnjpmf.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/grivivdsu.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gegtbomji.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gdsyomhar.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gquqkfoqm.sHtML


<!-- 参考信息 -->