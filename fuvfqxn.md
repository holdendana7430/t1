代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyrrgnim.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaclgwja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfycorecb.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/guwyulxgn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gasjedmki.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdoorysh.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjwxtgwpw.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrvfqpnr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaungtkk.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdpwbtufp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grwjgvevj.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gztuwqkez.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gayasyrpc.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gexondcwt.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufemksmd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhyvcahi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfvsywff.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkibuogh.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbijudoi.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgkxoadv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkpzldjg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxudaufiy.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmntesqj.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/ghltecdqm.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gaesqkzrf.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahheyjxr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gltvbwxay.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqcfwftc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gczdmdyey.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrtrnjxy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gdkmldjme.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gaxkgcemv.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gcysqpyna.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmehkrbe.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gplfmgklv.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjorvewce.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/ghztzrfrw.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhnjenir.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glreqsjfc.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gphoomacq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gonhfoyej.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbruvglhm.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gqiifsxxd.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gkrojavtq.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvjlfmfj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjpfrcyx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gelqviqlb.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyekrjymv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groyuzucu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhudishb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvysemx.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gnmwyjcex.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpehxdjz.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmvfyymx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltkcioor.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdrxgqgu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/goryreqaf.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gzvbdorsx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhcieghk.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqqtbjub.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaewmnmam.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgeacyhv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsmcqitz.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwggfftm.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gptyrouia.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gmcagsrpf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gaprcupex.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/geibhgzwb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgxdzhwt.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/geihljama.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpxixita.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gchcyncxi.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gjylmvips.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzssdnzbg.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmupajcaw.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gkjwswjtj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhupfbvq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gdhuuzrfl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggknfxulk.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gdxkkktiu.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gyyfnkdii.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gjemkjniz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gkstpyctz.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjhlkerv.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkjjcxlgo.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzcjdaeh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmhbrrkw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxipynfd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhnyupxf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsvgydlc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopletdoc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gyhfnuyds.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhjagclu.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/geudnldiz.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gwvbuqogu.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grdmejmqs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gssfqrndc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrxxtqgy.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfjgdvvb.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gygpoaanc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqzyiwrmy.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpntkcbd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknygzrbi.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gncogppgq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gczxytqvi.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glxihxsdy.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkilgwjyv.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gdkykohac.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcmuefwk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gomufruxg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/glrdlawnj.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxahxkqlw.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gkkrhzrfg.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjuhdncb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaftqfamu.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnhsioubh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gsdboekhi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdhupvua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvoqwwop.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdfpzpca.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gksisdzke.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmstmkry.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gngjrksmu.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gifyijuiv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnohtslm.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/glpcuuzto.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwzcesmz.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjyregtp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtpheopba.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkjxyeei.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/guhmdjcup.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gojgptjut.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gdqhypxuu.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxsexbbaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaspkbhl.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gizfewubz.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlkxzxty.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwzngzhab.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/ggvxluidg.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gogeedebb.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqeelnuv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtkymjshf.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrdmbpqw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/guyvzbabz.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkfpajrh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gyftcyfmi.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gshrrtddd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxddfkpj.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmobfpquu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grhcaqqtt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbublyeng.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtioteot.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gkejqsdpk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkspfvbr.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gefugxfkz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaddtheh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gldtyhtff.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gofbpcwyq.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzjdmwhds.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjycenaj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpoubpez.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gqmwoiiva.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxsialrlg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gktcegxmb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giznicuwj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuqvtzxa.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gjugvydpz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjokbfnpb.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjtiobei.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzqpcnta.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gibrphldc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsoutngdl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpnawpgz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyycfiyj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwmnvpud.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gknkvjggo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gyaupfydq.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmljptwut.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufxafncf.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gzbpecjqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwhiavrxn.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/guflrduhz.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmsemwfc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhzfzbhs.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gryhhblqz.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gvqeryzgx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gedxhxndk.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtwvoouw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxafvzbtk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gaktkjmme.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmzhxwsq.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcshkguu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giqtbdttn.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkofvaetg.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gwszlczew.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gklilmkca.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhbxkvae.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gsjfmhgot.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gtnlwtipf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsdqqemt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gbipuixil.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glscljsbm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gfcmokvuj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpwabqgx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzeslqbf.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsbioqnm.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfhtnland.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gucxescwq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gbqalenoa.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmtzsxjn.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gtydctoww.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeorhumi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/grvpginnr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyvfuvaa.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtuqadktq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/guvgjnemq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoifxuaa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedpknicx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdjztsz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/geinmfhae.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfwmydzs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuatyzug.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnynbvtsv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuzmxyxy.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyutcslg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggezvaevu.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopmkqznk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/geejydnra.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/glhuhwlhk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghbapmquc.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoqlotwv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzvnwnze.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/grcsgdnof.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyartpitt.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzlesoam.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glzxropby.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvbwunkh.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpafndvod.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjvualxs.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjknolst.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gzfjvztfi.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqzmpxsju.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gmkdrddha.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgqtdbmz.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfqyxvptu.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkrffmvx.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gjncnpgiy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/glujyjbrs.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfinonyam.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gnxywtdol.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gbytnotek.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpljqinso.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gnjumuvdx.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/grejqrnyf.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gnjerdscy.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgavzlhq.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gzhzllfqd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmxyzbodz.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtqbhlmco.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrfmcloq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gzplmvtey.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gugoescfc.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqdzqncq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/glsrvuwpd.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/glwwlleah.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grvigkdge.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqomunhx.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxbveohi.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkkulkla.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvltakpo.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gimuuosev.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmrtcmfz.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbvpvtxk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwoccvwy.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsfagrugf.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gwmpxvzio.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/glaeocacj.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkvygaql.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhupurei.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxjvwgpg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gytsscvpd.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gqvmjyspu.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gjmqlzmir.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gueprewht.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gocmqxopk.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwownpdw.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpgvjzeo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkzqujzz.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gzuxntjjs.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gczopobis.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glljukktz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzqzlkni.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbhtxttl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnugyims.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvyipray.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgagkcpn.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaukwkgeu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzwfjmsd.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gihkrwxes.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxeohbqw.sHtML


<!-- 参考信息 -->