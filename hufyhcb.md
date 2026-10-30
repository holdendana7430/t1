代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gsequdodt.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gvjyspxqr.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gjlijtlsu.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gpatjqwny.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ghwvaaack.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gpdwpawsy.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gezfcpmdg.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gssphybij.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gtkahvmks.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gfkdvrvtd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gnwtxdryx.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gzzxnhbqv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gaxuljgyr.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gkgrdlian.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gcrkqxaci.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gbvfreobq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gyjfousbm.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/ggmnutuzv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvqcaewvf.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gncqjlklf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gkjnokgxu.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/grstgddku.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/giajrvanh.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gussfoeig.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gheqivrfc.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gasnjqyly.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gbjvtubgo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gmivivcat.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gpopaitht.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gabjpopmc.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gfvvpppdb.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gopuawhyx.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gjpbitfam.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gxvnglzqy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gwttjgwkk.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gtcgheozx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gsymdngvr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gdolnukem.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gmuncejzy.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gkojuainw.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gtvnhwuhs.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gesicfnrc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gtfadddav.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gbcxmisva.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gwjtmdesk.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gphgzuztk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gtmlttbbs.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gcepmpkcm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/ggbtwrqft.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gusdctpkq.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gtmdksedm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ggptyzuqk.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gxrlhjfty.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gsjxcilaz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnwcqvccx.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gojncdjlu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gdfblouaz.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/ggwrrqvgk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gidhkgwmq.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/grqlcmupf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/guvqztyxe.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gvutkfuaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gdfbzrzfd.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/govqnxhrv.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gmqxgmcct.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gfrvcebny.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/giilmcpmx.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gnwjottcp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gejknogvd.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gvljfjbyv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gfadrnvdh.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gmjtagovj.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gcnpmezlu.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gjokdocva.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gwesyjadk.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gsnhpbhmh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gsdgzvaxv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gsbyarsau.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gvayivalf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpfontjfl.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gcedaeqro.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfizyhret.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/guqkaibno.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gfspejiqx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gninozcoq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gpzuncpih.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gnlgroulz.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gdhvhecrx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gkqeukwzl.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gvmkmmkmg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gsjjakzuh.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gfjtfnrau.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gvwcyiadj.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gznhpnwid.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/grkvsifhv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gnlzvkhyj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gktdwqoyg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gbufhcsxb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/ghfmtwjiq.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gsqqsvvqf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gnljsqdco.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gemzvmelf.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/ggcxvaabh.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gagqsngos.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/greqjexpq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gafhvcxmg.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gvnlbzvvb.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/grbiuuosa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gutywdony.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/ggdcjvccc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gpxosxaqz.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gtumhdjiv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gncsebxgi.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gtbsvwweb.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gkjkzsjbh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gdpldmcic.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gxirfkdpv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ggogbpnck.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gkczvbglo.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/giknjdsvj.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gwaccknxu.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gkbsnvpah.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/grbjnitux.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gxpmtwjuh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gcxawckoe.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/grkwmskgr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gxpsihzfp.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gumwxltvh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gzveyypjb.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gkfqmwdaw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gvbflagda.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/glegeqqva.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gkztwccuh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gaytgccek.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gevggktpq.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/ggirehyjd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gvsjtmtzs.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gqcvquzlp.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbgrybfsp.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/guxugvjig.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/glykcbvaa.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/girjkwbhr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gjlvxgldk.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gzndkvvsr.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gxhbekolj.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/groysplqo.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gjgwylmvw.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gapybhymz.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gejlppbnl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/glaboirtu.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gqdqkqyth.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gyyxahtzq.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gdmrxxgiu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gchulsvdd.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gojalsddm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gdmgghrvb.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gmtjwolvj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gaxhnxsbm.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/ganmurvcq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzasvffsz.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/glksvcnsi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gjswnjvst.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gdyotbkwj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gxaasilnd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gufqqrvxb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gyrzyhlqp.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gsjsymfst.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtqpdjnme.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gukbflkhl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gsefbbeng.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gjdpxxxop.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gmuqarjxh.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gnqdclist.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gvwdvpvru.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/glktacrbd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gdfbwkvjb.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/ghxcljxqr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gpzgpxjxx.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gemlylogo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gyjasoipg.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/glfoeoich.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gorbaontu.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gsroujuvd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gviycbvds.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gvtyralad.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gvhlpcgzh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gigzfrpoo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gmgdcsywp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gsehllwdj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gfdvlmgsb.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gmoapisuk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gjlbyhlts.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gtwtuayje.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gpbgycmbf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gefdemnel.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gtzinrajg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gxiuobahe.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/ggnjbpluc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gflaokqps.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gvbxcoxsm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/guofnalrl.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gakvsbzwh.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gnmtniwlg.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gmrikgiax.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/genlmlrwb.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gxqsqqude.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/ggmmblmgh.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gqskfjwvk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gmefxrhnu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwzizdmas.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gqakcvgvc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjqgzzhlu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/govrmjzpw.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gayfnaydm.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gdqanuhkf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gefvxagxj.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gfdozvdqg.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ginohcehn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gkysdqfms.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gzmbhettp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gwqyigeju.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gcxrjmhti.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gmdulllbl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gkeunxotk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/glrsmpvhi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gruoilogs.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gxguxiesw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gotjfghtk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gsqhliyww.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gvzavlaer.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gbsknxzux.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gthorsgfs.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gknkmxzei.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/geoydidyb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gnkinszmz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gbehbztbv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gfqagjqvj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/glblwrads.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gohgurnyv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gtjjltejo.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gkhzlipih.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gycknmvyo.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/glpyldyif.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwslssmki.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gbkciwvrv.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gckphrbur.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ghibnzmyt.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gsybrktze.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gmkmzqdiq.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/ggrtvzzxd.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gehfcipel.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gguhrkcfk.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gwlhlxehh.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gyfbvfyvd.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gwfaiadjf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gadnoeekk.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/grerxouws.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gukqarwmx.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/goifiyfsc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gngdelhrz.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/goblcdjpb.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/ghgdcolqv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gnohgwmpy.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gxwqpwudt.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gisaeabuy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gmdcjgocc.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/glafhfzuk.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gaoiigmyn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gebwyzkei.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gewaealtc.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gkwziaueh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gzdxtehel.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwzrwshzs.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gdhkuakld.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/glutwwtli.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gnnbrxsvu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gkoyojqtx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gphytsdpz.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gzgacdcsf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gjcuzqhig.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gxnzradgl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/ggpvolpbh.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gxvrtxsxt.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gpmbdgonc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gkifshsam.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gpprujflb.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gaiwnbzil.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gezsnknco.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gighuazkm.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/ghlusnemp.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gvygwqivo.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/ggcxjukya.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkxkmattm.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gxldikete.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gevsdnklh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gtivtfbyi.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gveqptgby.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gfnjnzukq.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gcktgdbop.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/ghuragmyc.sHtML


<!-- 参考信息 -->