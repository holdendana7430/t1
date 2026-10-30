代发 wailian999

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/genhprbhc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyunzkep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/glyntoqgt.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpqxjnzyz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqsebmrf.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gdiqcejyj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdooltjvq.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrmzjqrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblehfgci.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gucckqpvc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbboyykv.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/govrdqzcv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gaowsnefx.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gmtuiuwid.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevkblaxo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gcuvlpnlx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtgwjpab.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvfbxdepd.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblqxfwnl.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnophkws.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknljoiu.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzouejfp.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxylbgmd.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gxkiffprf.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoxoqbgr.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjupigkk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoayultw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbcukauq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/ggmavokfq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjhnzgaz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gkafbroir.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/girvkmvzq.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gkwpcaakd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkqpqild.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gpficbugv.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfyzbefhl.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gazrtvent.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/ghypvhnca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrewdfus.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsolnzzn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/grvczmylo.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gdshbikqh.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/griswtaop.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpbmivia.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/glayvdufv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glepsmzbt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggpfeuldd.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwddngtfn.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gaiuydxut.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gchzqfmkx.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlrjacej.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gmariagoi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gjhjhixai.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyhepsok.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcemzanyl.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqndintr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhkehye.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ghorzmbhf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glpbcgrtw.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gofzmkjjp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/geoglngpr.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqgksnkm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gewshmahm.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gicsdnxho.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gztmefzzo.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gvkhpptbz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqlwfdfg.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbndjaqn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpznbscn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gbntkavug.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaepqrdob.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzttpgryv.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoapujiu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/girpluhnf.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzieekqrh.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gawltlcxn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrnzbncp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gleewxyzl.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/glltcnzsb.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/grwrqnlui.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gethvqtbd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnnrdxam.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqkziiy.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjmhowzwn.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzejehwkt.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gswjfttxu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfjzgvey.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/goinimkuz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphhvraca.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqvxnqyy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusuaoicb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gpmxsnkag.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gqqisuagy.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gwqhfrgvz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndylxfvw.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdussyih.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/glqwccitb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/goulfqtpw.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgbexgdp.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gclgndifb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqthbtrqn.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gmyotztla.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gktbfhhlz.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/grlapynxz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcuxlqmf.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/girbgjcrr.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkverhhew.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgrtcmvj.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtsxgwgei.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gydeptiwn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmcepnk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvdpjqci.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/guorjaydb.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gemuiwblp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmwifblqo.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gscnpqwcq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gfrvzsjag.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxkwyfzv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpcjdhkd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljvxjwmk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfxocavh.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/grozyenhl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ggntnhwqc.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gaeajcqop.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnggibxbx.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gghrwcdcm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyjszcip.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gymcctsut.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxdduwcx.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/getgjglqu.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gjkeuxnka.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcztfvbmb.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gizgwnmuu.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvgerllgb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/guarrnxve.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnuagnbr.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/goydatmwb.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gsshcfsfc.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/glbidcars.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/guydkagec.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gkabhwtjt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gegyuogvj.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunsbphfl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegrqjjxw.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gppiljocl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvnzezmt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/grayfooja.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkcvrvgye.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzudkrjnq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/guzeofqyb.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/glsfbmexl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfrwpwyz.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwmgkwpo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiashftv.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtpvzuzdu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gnqwvslqy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzzjhwnel.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gycpstjkn.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrzifzca.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gptleybwt.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxakxfxkv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gndmaudih.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gatdokvrh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/getcamxni.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gmoelyefc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvuddjsw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/giilqchfb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdjgxrmzr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfahrkqd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/guleosgjy.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjtkqwhr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtzcvuzy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gujykwzck.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdahpeglz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyikanjac.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gheycfipt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gsgrfjfgx.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmasonku.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqagfkuc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyepboaj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gsrhajaet.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggyowqwya.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/grmliousx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gcttyyejz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejadxxlu.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gyyeuaghv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gqqucupnc.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfqbasspj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ggtdgxbxa.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeanmmjy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbrvmhil.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gheoatlve.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkudarlqc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknhfqxeb.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqgawzi.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gablnmrjq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvxgjxcd.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gmovswtia.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gaviqmisz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guwlfbert.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrqsbczm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfivptaf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/grppgojnj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gethszwvu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gonxypicj.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gextjukfj.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guhiorpgr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gufqzqckm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gaxncsuul.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkozixyet.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gzbvakmbf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrqantrb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gulapmegw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gapzdaeta.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmkfnsrx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmsimnxg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtljrbclm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtfytstn.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gsrmjuhau.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxvggikfe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxuwxbtk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gojaltanr.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkfxzoiht.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuzrqlry.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxwqmcic.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrusdzyi.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicxvccob.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdbwvcni.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamxwpbci.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqiiailiz.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjyuzoi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkntmibr.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gbjjixazx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusaxocro.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gafnnjqeh.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrzbyfal.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsotxjlpm.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwxjebqd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/glscthfid.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqurbrgif.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmcxbnyd.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvghfzazk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqnsmlbj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicnbqjly.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gyrlyqilg.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/guupwjwxb.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvpvysbf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvymdatdh.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwfpblcq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpatvklwk.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gmebldrhw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxthaadbp.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhfsjcmb.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/grobpfvht.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gdsltrmty.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwowonzq.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/ghjlkmiaf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhzicdgd.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gklkqbciv.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gobeslchh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/geqlcyhui.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gzzletkue.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gojdyzjvt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfbqidff.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcraihvao.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiqdbgvu.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghxrlgiwr.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdcibymx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmcntyno.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatfdirzl.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gnxkgnwbg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gtqbmwizw.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/geyraoyre.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorezribi.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbogbrgt.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gsnyitcse.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/giapegwnn.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxnlpruo.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrwavtmv.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gcwkjgysk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gktheeysu.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugsyxkzi.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkijpyacr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gtroseamr.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqfhqwtil.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyuahzse.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gncjpkzjn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gmctsqrdv.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/goitzrhnx.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwumqumm.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzbixbra.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goyydnvhl.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdyzskkmh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyrgglsi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxltsfor.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqdolapv.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnfvgjgp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehzrgnqs.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjysimgja.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gjrzpwffm.sHtML


<!-- 参考信息 -->