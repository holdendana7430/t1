代发 wailian999

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gzzzntjcp.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gnkkpibgh.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gpldjiocb.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gluboylsf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/grtyxjukb.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/ggcjynzqk.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gamtxvwxu.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gayycnxcq.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gbvprpoxc.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gpfewsysp.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gchfxqphg.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gwjbcxewk.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/ghitbtbtw.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gyeqdxzoe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gbnehyanm.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gkrbymfyq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gqhlmwxbu.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gmathqaof.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gkgjqbhdg.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gxeadxaiw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gdhrvdkqx.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/ghdsyxfsi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gimzmurok.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gefabsnck.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gchtmobkj.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/ggtchwwom.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gsexezwdf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gmnfcxitk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gxqyzrkmd.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gxzorolal.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gjkydrgyg.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gemkdgsyb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gmbfnahbn.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gomsgypqw.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/grchjutof.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gbvxeidgn.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/grlrblrmz.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/ghrqypcvk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gytcqqibp.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/grobecygw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/grxzzraqr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/giemsupnw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gjntsdesv.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gqfregcji.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gfvfsjxgh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/getozryux.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gxtquawug.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gpxlyhbfb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gqwmizlyv.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gvpbjhukq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gqkhivogb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gqzavxhzq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gujtpfcpq.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/goqbzedyj.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gdidrcxqt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gehjckpix.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gitnleqkp.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/galmdsvjq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghrurotlj.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gblbsiytu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gxpdmvpva.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gnyufqkhu.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/grtsbxojr.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gzyaumpem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gvrvjyozm.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gcyxbycje.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gqfooozsc.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gagyaaond.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gfxvgpotf.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gbrhrfaco.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/ghtgadiwi.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gangpwlgu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gkcvdnhab.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gvwnuaieo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gudlsucmm.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gdfkxgeua.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gfkpviley.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gmoiionnc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gutcefrnx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gajzbjpwj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/geuggalfb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/geqnoohfs.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gdqafgwbx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsqrrstln.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gxnfrrkks.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gurwdgssu.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmhblovrx.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gajemedhw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gxfvhweoh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gmgimwyvw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gnxvonojv.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gxcqrfrdw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gxouvjlmv.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gnaemdwgb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gjyvjdcau.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/grojfhfbj.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gtgglqptc.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gaylawqws.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gujxtmzoq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gdjwoeaky.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/glmdypqma.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gthdcgrou.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gqavswlya.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gcceispmh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/glqvvvcau.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gzjonkfjk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gcbzyzxtr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gzjxieyif.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gaaupcney.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gzzlzdxzo.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gmcrgultm.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gvejexumf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gdvehwmdw.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gteuknjwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gceyilfxp.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ghznqwdlc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/ghzotitlu.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gepmiulgq.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gmezwvznk.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/glvyanpgf.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gnxnyodnk.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcihmlogq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/ghygbzxcn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gsyrojbcr.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gullgvial.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjioaffqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gyexktopo.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gwblsuoxy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ggnfrfenn.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/grpxcrvip.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gqlrbjyda.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gymbrcqaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gyyuedslo.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gaezknogo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gtltlwpfe.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gqrzpaifq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gtxsjydnl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gusgdurck.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gkmrmrenh.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/girfwkkdx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gccjdflmg.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqafrbuqb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gducijszo.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gnxntvnfd.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gcepkibue.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/givbolumj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/glmiyaxjp.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gniogftpg.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gqnaferxv.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gvdwsskfs.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gkocxgnhw.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwdtngiau.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gkqsbfbfr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gtjjyizcr.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gwzjxcbfz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gtgrwdivg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gtsfzhvch.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/ghsgfelru.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/goeqpacwd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gghorrfmi.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gsloklhnk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmjucxjix.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gqrychzrq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmaarbllu.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/ghkgysijx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gczypskgg.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gwfclhmur.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gjhgckfiq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/grqhjyxoe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gslrsqrum.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gvrjzelev.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gedhiwsnx.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gmxovauok.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gpjnflbbd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gnqswoshf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gcqlwbdll.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gjzqhgplt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gknsvcanr.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gdgopmkxo.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gdtdnacqc.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gdqnbsinm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gumqbiuhk.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/grgaqtthu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gyzdxloya.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gmccersxe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gnzfbihjx.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsnoejtcf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gscspuzzx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gshbbbrcx.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gjxwliptf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/ggogpgdln.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gzlzltgvc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxzwfhhde.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gbgwodfkj.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gsqmhhkuj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gfwjrjwmp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gbzfcnsdy.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfzlmby.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gueozvghh.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/graqaswzs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gwslxquqm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gswjajnaz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gkfwxuclg.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gwxqhfnoh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gbluzycbv.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gwmwbdfoc.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gaajxfcwo.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gvbpmyzbq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzblfoduw.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gzuglcilc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gotoyverc.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gbtiebsgn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/glotxejqx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guqzaagmb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gjejepsxi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaivlteom.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gfieatuqg.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxjqywixm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gtbzzhuzo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gerscryxg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/golfacive.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gzcxminlq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gvoqpjkqz.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gvbsmkuqm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gvtaabpjw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gpdlgxlca.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gvqqnwqyx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gsqxhphcr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/ghcjtoasz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gapwebuuo.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gfyyfyzkv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gddzsfskt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gyaijjlll.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gdwgkcfue.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gtscaacwc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/grlcozkjc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gxbgvqrrd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/grzhhxnmt.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gohtbpecd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gbkmacbru.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gpqvfkwmg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gsmapdrud.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsmvqgymm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/geetarlon.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gragtzmct.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gdokdoase.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcukbehwe.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/geogrmemo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gnenxerbm.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gsjfoliqh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/grbfhmnkb.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gumgeflfk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gdgobuoju.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/grclnspio.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gbmvukenl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gtfkzjmeg.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gmhqphven.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/ggibbugvd.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gleudjuod.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ggrbfyvxl.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/ghacyyiqr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/geztoitdv.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/glckfrnkb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgntudv.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/ghuenstpj.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gqakzxhyp.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gczhfegdk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gzvnsmxdu.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/grrmxoijz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gczerlrwu.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/ghlobkuig.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gdeomlmbt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gliepjqxi.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/giaendpbw.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/geiphbucw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gcbtuamxl.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gydifyfij.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmtyfhbln.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/grzrcteyw.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gqkvemedh.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gnrhmmcvv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/ggfublmbx.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gqxpwcxsa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gzokprhqv.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gdlvizegn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gyebbkdzb.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdcbhijyl.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gwgygotov.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gpzounjsk.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gbjzgmrfu.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gsjkccezu.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/grshxcqgx.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/garjjoryk.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gwyjkjybc.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gnlshyxkb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gwquhhhop.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghbicjaeq.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/ghoxwfaoi.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/giojociqn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gizazmkde.sHtML


<!-- 参考信息 -->