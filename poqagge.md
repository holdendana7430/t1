代发 wailian999

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gavszlcja.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gvejlkkok.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/grjfkwpfb.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgexudss.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gkquindry.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnsvbotn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gkqlscljk.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuccaoqi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gslfmribr.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbclvote.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhaxzua.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/girqxkrwd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gksafmnne.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gkzusmevp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjetmkiet.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbmoceon.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfuhuzrt.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/goqqgcrdz.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyfvrfvdr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjvrnzuw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxyetvbhj.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqaafitrj.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbftqpjjy.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnupsbzk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdlnaycm.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpjegewql.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/grdbyqusn.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/glzdpfjfq.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/goprcvwof.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsvdmprcn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gukupyewu.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gcojoqprp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/goiijpdor.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gtgiusvfr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gljwamikl.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/glzqfivdo.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/geeqdmecx.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gevbejyri.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gmafxhyoy.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwfbljbqn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbkkqjmr.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gsgokxjzr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/galikfhev.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gflnybwdb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gmydyttwq.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwuletven.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxlgiuyqr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwtfxdba.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjvxfxuj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfwejpyk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyeyuzzl.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/geehoehte.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgwclfvg.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gbsqkptlo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gdrrdtnxx.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqcstrmpx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gabnvghrv.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gdicygldm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknzktvf.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmqdegav.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhawwbgd.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkbgqgk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwqpoizvg.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gubwhngha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhoyrlwz.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjsceakax.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gsoeqjtgf.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gmzrlpmrg.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gvajfqbna.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gkpatxcqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gczlmjcii.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbnwkluf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkqnlld.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gklvhaylk.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfjnfnwq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdieqzke.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/glaxjyrcl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsgkfttdx.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqgedwrbp.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gypyzkkmk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpcvacgj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuahrbpr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gbvnldukl.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkpjcsch.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaalihsks.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghekahidb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnytcwlrx.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzyrtzcq.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrmptpco.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkeomskda.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gadegtycd.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlnhsdwc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsordcew.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gscpwqvaj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gtvlzqofr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/girtuhdds.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gjlwbkmwa.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdzmykmn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/geyayannf.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjrkiptfz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gmupjuxbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkklmsdhg.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjtlzykf.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnnzwybb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifjhugdx.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gjplwjnix.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/ggotvmfmo.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxrydyxd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsfkrezp.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawrvjqcq.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbqcwntg.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gfverzzzh.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gznmdyzjj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqghgvoz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gyljxhwej.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtamvtrf.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyvguevl.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavgfepiu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoexcdby.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwxjbldi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabcqnfvl.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gkbziaqni.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexcgkdng.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqhdlsma.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrcpxess.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gtuwdvfxf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/golwvfyvr.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjtqavxmm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwimlsqgh.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjnoivaa.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/giwwisykp.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/grnwjtibg.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztomcdkv.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqnxbgxfp.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbgamxso.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwtmxkyyu.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gszothxuw.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjsnrspfz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdjohwxh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqrhwefr.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/glxnybnyh.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gqshwtiqq.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/glszmgkcb.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmdzjhlg.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyardlmzq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjzdndpd.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gspirqsiu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwsllvvb.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gvxtwpgep.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gispyvzbs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleofuwcf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gluunjmgo.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gosfulinf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpuromuoz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtrcwfmf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnukerspy.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gsirfbsna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmjjzyxb.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gquonklwa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbijoozp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdqkywdfr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gnvfsintt.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grehpvugn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtysvtzpb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/guqwisqmq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcbxnwmki.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gphksodvq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gachpfpua.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/godpglqov.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmweevtpa.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpabybvu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkudvekry.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gjazbdqxv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyhyopfz.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjwocpkp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gicykijgh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gstyigjuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gohreqigw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyhcldqw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbesfmzi.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gnjrkguno.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gctfqqeus.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/glepwetam.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrjxjtrh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngtctnsp.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/govavpnps.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsrpjtcc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gitjbnkan.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmswcnmyr.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gqtqaenxq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpwgxsds.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gsbutcrnr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gleanlikn.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwhbzcjz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgyzfazx.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbypiqfuq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfcwisvmr.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gakjdgszt.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsprdzci.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbajdzat.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gkrodttuq.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gsevpzgty.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/grygimilw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzznekoac.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxrojkmyr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfronaolq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/ggqbmdxyn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghslseubj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gyxyomfos.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpilabywg.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/geldcctvj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuntncfk.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gutjlnqxd.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoonehjf.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gfqprivub.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/guxymxutm.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ggtqjjskl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/girazseah.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfauvkoyz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gencvlzkx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gixzidqos.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcikeypgc.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gfuxwuzlu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuphpwsd.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkolaonfz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtrmwwhz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeaejwle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzylayjhu.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/grthyfncs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/guhcsvpsv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkrxzesc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gibobhqql.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gckdfbqhw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gekyuixye.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggthuhgas.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfikoswrq.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gviqrszgl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmagqlwl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddyruazu.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrxoywzs.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbbpeorlb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgjmnnmt.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzcvlrhcy.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gfvyqqykf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gexvxsowe.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnvkkgwj.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjppohddx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gzlwmdlwp.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoaocklt.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhsdakav.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gbitdjscc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnkcovgj.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwejoryjn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gricxzxyr.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnmforro.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmaabohk.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gdtxxdibx.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfinxjepe.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhsrvnmp.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gdfwdkpcq.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gsvezkfvc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/giqwbuoop.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevrggezp.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxoaflmq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gqnljrejb.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gldsefnaq.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gfvomoyxj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/geetbqpja.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gojzawgpy.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotqbvtea.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuyqgxfk.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxlhpboo.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeoiwski.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gphgnfvjv.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzvzxokm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gethbasav.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gctfnelkc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gaqhlnunv.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gavykmldc.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gakkkxape.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/grfjimhps.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gddtbsvna.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gypncmlgo.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrhlawea.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwzhyeglx.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gbngrpwsp.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/glqjtbfdk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gkjvoospl.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsuslcuqq.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzngocdg.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxotpnylr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/geokejplx.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glggsevwu.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gfvaceiyz.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxtzjgrl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwatfbexz.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grnoatofx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkonrkdb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwxhxneu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gstisguat.sHtML


<!-- 参考信息 -->