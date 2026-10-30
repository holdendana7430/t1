代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtjgcuptz.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/genvrcblo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjczdfebt.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjyxojxy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gtysaugny.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gszdxoixp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gigwyporw.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvgurwgl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gchnrxtdx.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvckdgcq.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gperuyddm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/ggudxpupt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gobwavaay.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcltsejm.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpjytvewb.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gxvjtmpaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/geunwcijo.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijayaakj.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gffjdzwvj.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gknfyoxfc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpehbdaeo.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnujnwhnh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfujjppn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqfooxim.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gxzxzzslw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ghpvpkaba.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/glqwaclme.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gininhfql.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrwrfywf.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbxeupra.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gwxeanrvf.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwzihgwse.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/grcmfowmn.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gokxnmgzr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gcgplglul.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbcgqlnx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gxzlgxiso.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gytrjroai.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzmlgveu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtdclnnp.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvzpkctv.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/glguxjydd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqextlpi.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkukmegnv.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gmfhuqcbu.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwxsukqy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnnmdayl.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbmqeoyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/ghxwcsnhm.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqibemhv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grcwzkksx.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvdtkvmjt.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwsuchgn.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gsxsjnpfr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeflrzoc.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyoheglhy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/goamkwesp.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gakondawy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gldtbccgi.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxvobkkt.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkkhnmph.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gwktkiifg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbifeyoed.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gywqeffjf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzdmtzmjr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxvwnvcs.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyshumrtt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyoiwfjv.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbartgptg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geidiyowr.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gecdbtabn.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjypusgid.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgpepsdy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gcceaopgi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gvxkpglsb.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/ghjxqucuo.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqfxfpzxu.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gdeaakdqj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgxrpmql.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gueekakqn.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/glfestufq.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzugjnzdl.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gdwrdvonq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmzvqown.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxfiqqtm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqnnmecc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaciblkgm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/guiapkhzt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gqewbslgb.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gbnmaqste.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsgpqgoj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrhextwb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkgbhjvw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdcrwytb.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gffebpvlm.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsoshpwtw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gersikayg.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpntvwca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrtlnmfs.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtvnawcqw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrdfeath.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxhixxgs.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gaytqsmim.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gcujncaea.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gunwaqjff.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grzzyaggn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/glwpresyk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkucczxvy.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgrwzwvv.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwucbqmra.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqpvvnew.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwcaliy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzndbuhh.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkzxezyok.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokjyfcfb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdhikepo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/govzpgzis.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gphzyznvb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gbhnvkrdh.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnzkdkbb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/grwemutlw.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gtyqeyavk.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gngkhlayg.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkwzehvf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchftsref.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gwcogmxfz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guubbwsqr.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsgifrmsq.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gltqcxyoe.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnlgnyor.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/ghzxbfine.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/grpfrtsos.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/govpxycwj.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbnqenhr.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhkkeezi.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfjbbkql.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbxcxymq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goxlkntty.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpejbgbxa.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgxmpuqm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvbzzwyx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwxiesxea.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/guxbzktza.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmvchxlx.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvksdkmdt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goscpburi.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/grwechbgd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmayulve.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzpdpmkn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyybwmocy.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/guefdbmfg.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gonmlexxh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsybasdau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbyibkg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgmizzmh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpuukwcos.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gliuxyjsr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiumclol.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghthgjbqp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaudzoml.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gacmqdvvx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusxujstc.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/ganohakoe.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnynpaion.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gryydrkgj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkefqkgs.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/giknevsdk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzreougyb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazcnrfgr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsummpao.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxllixkdm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjocddhp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbssrxz.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsmrpmlp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gezsrfldz.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjvwtqcrv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxhpgndf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrtsspji.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gphovlipp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gtxlxigrk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/ginnukmlf.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmagvlxpx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/ggdqyxigr.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gouyllcgy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxviewpfc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpadeqvbq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfpihhzz.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumkgwpft.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpiqfhyou.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzfnrxam.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjzrgmrd.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzgvpgjc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ggbmyrfwv.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gcberyorl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gjjygynep.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/ghrbipdff.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhmzyhel.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbllamnp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gtptncicy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzrnuzarj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbvmunjo.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gnllosiiv.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gywvhqbym.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gilpgjmkf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/ghiqpvghs.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdcjxvil.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfzfyos.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/glgidotem.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtcdduhwr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmawnfzmn.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyzpvlrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikiidvtk.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gnmlhmqkh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgedroka.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqmcmwtu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/grggesbdc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqznytflf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvareefqq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkyzydvm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfocjerl.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gxzpusaub.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuehnxfj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gxazkfxpf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmgiwgss.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gbahjmgkl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekjljbre.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gywabqlay.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/goptioana.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gmyodppqw.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/grdoxilni.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsrxsqvtf.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvnyeul.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcujkjhmf.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghrxeetmy.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxsvipko.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtmwgbsw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/getijpflt.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmixphktn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuejnrkb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gezbbmrrr.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeqythvi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyohmwbf.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqdtagcw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gswyhkjcs.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvolubgb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gmhztpeqw.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gfrdllyrh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/getcuxvsq.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gpemukhtv.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzxeevuq.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagmarom.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/guojnbbap.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/giatwmvel.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsrweyba.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/guadvgfjr.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gaynnueva.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokuktwpw.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gobjyykwt.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlwjqpjh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/goyzykaxv.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gtilwggdj.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbwabgymu.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgwfkwwz.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzrrcqyk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjrofqcs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gtwpbwloj.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtejqmkks.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gulqqgbzz.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gqtueppqq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzoeksyhc.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqxxkqand.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyetftcdm.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gstgplahe.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdyagbfj.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtocodunb.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkgkhnfn.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwiqpgca.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyyzvzcy.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaigwiin.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/glicmogfr.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxihbnpvv.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gntstidbu.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/goxbnpynd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gznypiqui.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/getxbnhms.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfsqilfv.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmuqiysau.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxplpczme.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcbhspcgp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpckormsf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvsjoend.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzazhhzea.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gerwblwnu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkoqqojr.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gifgbevim.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gfurlwjpb.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsuqaygwt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbuqrdiy.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gitfsyfwp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gioywjbyq.sHtML


<!-- 参考信息 -->