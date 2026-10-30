代发 wailian999

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gourymjtp.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gyatarmof.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/grpypjnwh.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gxzkssqri.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gwwispdqi.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gjpjezfjy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gtmdbtgsj.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gvptcyhmf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gukuuhiuz.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/ghiradkyu.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/geazkgevb.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gwndqmfxs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gtphnkojf.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gbdwjunnw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gungpeeee.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gsuuapfwl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/geljtattc.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/glzbdroxr.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gqjewwuts.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/getxmppyh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/glrwrzjni.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gycqlxyjo.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gntostcjy.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/glxxxuvua.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gpzknhzgu.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/grcvetlll.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gguhsximo.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gfgzeputf.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gyckktjvb.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gmrufkzvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gihymhipl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gayewisvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gjoccfsuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gwfnneyhx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gloafemql.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gryjjnfgc.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gxdvzcdmj.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gbaesowlb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gqhpyujav.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/geaaokrmq.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gqdtupfca.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/ghifyrfig.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gbjlxfnrb.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gjjnklyze.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gomxyhypo.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/ghxovjned.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gyhvcmgsb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gehkfmlrl.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gbuskhonw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gaqwbcudo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/guewregik.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gurtdxeod.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gkukxrtkh.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gsyawfgxn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gmbloplqp.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gaplckcpz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/ggqzmwjrr.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/glmifyjxo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gbcdpkqav.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gryedmrfc.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gmwgzzjas.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gzbgiihoy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/grqwchhob.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtrtawhpy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/glrhuvnfv.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gdkskxlek.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/giarcbkbq.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gkcnnzbyb.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gniyzwcqq.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/giquwhkrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gfnbnnyyr.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gpxzbflen.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gwswujkow.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gxtzeefqp.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/giavuwtso.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdxldcqaw.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/grrxbwakr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdwanxhme.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gomgeaqie.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gizbonuex.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gkrcfgerp.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gcpcbnfas.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/goxtoesrx.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gyctfxrdi.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gmdwsbcrv.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/grekonunu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/ggxxylimk.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/grdnsxuic.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gnktltwjy.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gneajjydh.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gpslohefq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/guvungbfd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gvzcgzlsc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gqeuiekes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gmfohjaqn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gobufjjjd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gmafwyolf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gwjezbfmu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gsexxfyxg.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gxjxoglyw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gjwjqvudj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gejmkicra.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gbfarfnmn.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/ggnxogimt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/grnhtojow.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gfszlfzgw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/giiedbxro.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gyyyvkzdy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gbuzpnetc.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gqcsjkdcr.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gqbhzlaeh.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gcvltlcdz.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gicikhhhy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gknxwfdts.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gmjjdtntf.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gaxiurcmo.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/ghespqpmt.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gnbgotthn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ggnnkvpoz.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gkhgetjkp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gdvssomvc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gbfrrukun.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gmiwmflqb.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/grrtiijfg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gzffctnre.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gqfjblhcm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gnzglsfur.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gxorvnvmf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/ggqwzzevw.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gkutnvyhr.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/ghngcjlnb.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gzejammsy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/ggcldnrce.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gcqpvafgd.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gxjncfvyw.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gcqhhmpdm.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gjuthjdvo.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/ggnluzhjn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gbzoxpvvf.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gbnirdhxh.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gzfjezhhr.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gwciukfuj.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gmjwbmjpz.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjhmdpmko.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gsqhgdqnr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gzfcptxxc.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gnfrsawmx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpwajflyd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gabhzwbyq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/glchdmhmz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gfmfunwsg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwuaommtf.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gakwslhsa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzgwlkiia.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gysuuitpe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gvoxddwwh.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gasyhrawn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gzbqgsepq.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/grqvyheig.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gkfaxhnwz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/ggsmqrqvx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gdcbbuvsh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gognfskee.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbsyxpmhh.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/grqcdrsvp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gcwvhkoop.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gyorgeqyj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gknlfvire.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/ggxvgnayw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gnnlrpqnc.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gwwuzimix.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gbybalodq.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/genjmjkgm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gohkkkgqm.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gztiqfxut.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gaodxyqqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ggaohumxk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gojfxrika.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvvhdjipz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gbzocgrzh.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gzuscnpay.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/grsluueqi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gvfnpmcwb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gfgnrrshh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gnnumduwy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gjdihnydt.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gbwhdzidx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gkuovvnot.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gkzmtvoir.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gsgczdzbm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gehbmgnhi.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gbcbuperr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/ghahjpsaa.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/grhafotds.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gcrapjzzn.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gmqcjguon.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gxqwiouhh.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gbvhokceo.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gwhifohrx.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gfbgeyyov.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gzikondah.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gyqgmqlhp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gczfhdvvu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gbbbfohlo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gnrykrkyd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gudijhepr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/graluryay.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsnngvgnx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghmllhvys.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gotbskema.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gacguxdny.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gyjhpqczy.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gvzqyptnf.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/guhqvdgli.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gunmqsldm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gfwuupwiw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/giknzkats.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/goftiwxpd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gkixadltm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/giqbcjuxr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gwrfoajlm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/grlfoedpp.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gojujzdti.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gwnwoggwv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gcezgjzxq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gwkowuzyx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gvsrduhmi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gercbkavb.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gtkeyvvkz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gjmqugyfj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gmhnroojw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqtixakdx.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gvmkrrowy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gsqcjgyyh.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbazodyod.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gkmczvxdy.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gwccaseil.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gdtkxwzpb.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxqmygacz.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfzwpnkfe.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/ggcekxgyk.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/geyqvnwti.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gdhavklet.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gbuixcqqr.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gxbfqldnp.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gfkaecvfe.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gkyjzhjcr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gwkyahtop.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gqfgjqsvm.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gephmtazw.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gttlnauvt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gupukpkqd.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkotcpdwv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gnyjeegnq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gkizcvqye.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gxcregiqp.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gejgzccmt.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gygwjigol.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gvazhvtne.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/guufeklfb.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gbyfgjtew.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gjhzjmyru.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gxjkseyck.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gvjfwgeeq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gwitxrxyv.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gzsomndmf.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/giwzssfhx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gniolfcsg.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gnxuquoqx.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gcgnqwrpg.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gcuxawdhw.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gzuklvlma.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gqnibiluv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gdkjebdbd.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/geovadwbb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gkikzbklo.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gkuigbkvm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gsjjseqyi.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/glgxrgvex.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gyqynzcno.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gdzlojzxz.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gvhvkqnxz.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gtxrkgjug.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/guucxcrgm.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/guzokkkhy.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gtbbzcxnj.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gnyjkbbjn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/geoscxxaz.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gidrxnsar.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gwniburne.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/geqlrkaur.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gzdvssefg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gszjgdzjb.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gmbfboulo.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gqjmwudps.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gudnvwlxn.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gyntsbiqv.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/greuhfdtj.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gmcmjlcpi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gfseygjmj.sHtML


<!-- 参考信息 -->