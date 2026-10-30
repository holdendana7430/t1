代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxworpah.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouevaodd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyjicuet.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghcjbwrut.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjmqvvut.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuvbjnzq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxczumhlm.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsdhvjox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/grmzosgwf.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/geudyidhj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glpsiojff.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gklocqmpn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwepvcku.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzalllff.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfcriznz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/ggcywmyle.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfvixdru.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuzkhtof.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gelppyglp.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmpbzviy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gfpyaixbv.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gemlskopi.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfxevkas.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/ggchtxnsy.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gcphbuaub.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gocufrhti.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gokdwfjwe.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gzpmiiupo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gdolnnrep.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gijsvxdnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwnjlnpf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzpcwemjb.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gczgrlyev.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttrpfvyt.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/guewgryjq.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdcapdnvu.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/guffxbfje.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gahytwpsf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdiizdhk.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvkiutw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcbigizf.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gvoarqhqf.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gsnjdkxwj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviaiiznc.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbzqrzan.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyapaatqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyyjywqvx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvhmtxgc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gpgokggwp.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gxopihpxd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphlcyrgg.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gtodcgiix.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrhcjdar.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjylpcdoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjbzjoeel.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gylizjmul.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzzjzfvz.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gkdakzpzt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxnlgbke.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxkaahztr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozmhdzv.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwqjddhxt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gokfsrlvc.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/grlfuezpx.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gosszwhic.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/ggzscuuib.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwarsqlj.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gqwwvpyrb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrynxdyd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/grtotqplk.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gejhmrpzk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnxbxorif.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gelnnuono.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gareplcdp.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gehnvxcxi.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbawduvg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaikvcgyt.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiqeyxbr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbobbhvi.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgjmvdiv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzrpgrnr.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/glkrrevdd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyfwraad.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdwkaighz.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmwtxzvn.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grgczftwf.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvaintab.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/geycbgsli.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gmdazupur.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gxygesxsf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gqyqileob.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdksnhfg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gbtbwdsst.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgmkcwgx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gjoisvvcl.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsipbeic.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccivltps.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvtvogem.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciuxhvuk.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/glfesdvod.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjudnemt.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjfykyjb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/giixlmsvd.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvyuxyyv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guafwqlob.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzigyqjpi.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gvejtyxnu.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gxykzyxgo.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqfjuwpm.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvjpuyys.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqfwomtx.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzmwyanh.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gyuvvrwmh.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblknwrnb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmkzsfrd.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gopsoabnp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghubnfyri.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpyuxrzh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gymqygcua.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gltryjbmy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gksefqgbc.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gonnrbism.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytiywmsx.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeptvvlg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gnvqafxoy.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmcbbyeit.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuohttdz.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gpukfcrgh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gesmjqwoc.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gpnfirvcs.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagfxjthn.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gswvbzvrc.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gidrkllbp.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqghxxdig.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/giemykcxb.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydxqaly.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmbvifjf.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gaphloacx.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gdvuoobqq.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glcrntagw.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gyahfgqth.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkzwmxdf.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvofjpaod.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubiwbimj.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaxtmser.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnlndare.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gbqwtbvjf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmejiiaiy.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gfagycqsm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsgcjaam.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gktuzczed.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gylkdftcc.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gejqhupfx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/glmbxjhuh.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjihzjie.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gonfrdrsu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlufkluv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxornhof.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrhintry.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gmuysejgr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkgtxyvp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/glunpqwng.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxujsogda.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyggoisax.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gjibxmztp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpvbihff.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxmuktdu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfesaitu.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwhtzhmb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gskakhrlq.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhcqdqiu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbtblvtx.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gcsmglqvq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwuruejb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlzwbnrr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggixhjqta.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaaezyfu.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjfworck.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbthsooc.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghorxenhs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnipxdbp.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gponswkkc.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggvelizsq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gycdxlhce.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkpwersu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmuqzbtk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrtmyejs.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpefzvwh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gubjpirnx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvzjqkmn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggaiaocdy.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gmzanzead.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzopoutzt.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gtcvafvyk.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gydlmpdsk.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gqlkrdmkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gcpmryqsh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gferuorts.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmawhrbao.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesbynndd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsayppsx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gibxdggct.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/grvxwmkfj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqltuhynu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwncqhoc.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gtfrwvvov.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcbxetkwg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/glcdknkzi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsorxvrg.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gygazpfzp.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gtehmakpk.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gjneckqvw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/grlnzlsnn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gfyvoogef.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbspatskv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/geonthipr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtpwbbpt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfgjftdz.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gupajrmsw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmwkfzrn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghucpoiji.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjexnnwsp.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqyyehcrb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvitpgnz.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmtcybeq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gngcbbagh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gqjpbilfe.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwimurrhi.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gneosnzdl.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyhuwkqm.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfhbiiikx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayfaixtv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwbdtycn.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gummmkgde.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdkziabas.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdwekvyn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvprwgnc.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkapaxyn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfrxopax.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqdzzvsr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gpapiwami.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjlpamxs.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gexukrvyk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gzjfukwdy.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuswkrly.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/giadltzfo.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkgsxhop.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvyksqbti.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/giggoemdr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gokayjtbp.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvbnacnp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmhyraig.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsvkkhle.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrgfbqsm.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gllkyodbt.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gywudmztc.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/grvjvxmob.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gozjgjqbc.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvjqdcui.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gtwbdblvy.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gfraaukgk.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gmojkxijw.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gseafndoa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcwkgsny.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfdgkviyt.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/glkuqtosn.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpemdqls.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwzowvjqf.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/ggbwydemr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfeykvtq.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/goksidqmn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/grsqnucbl.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gbdxfaxej.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gettdqqio.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsctxtbjh.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gkugepuvp.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gctahddmk.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/godmnvtvo.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqkkjaae.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/glxfpdudz.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ggszmcxyt.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/golgwawdr.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbjbnhjj.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gjakgtzjx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxavlgvyd.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfasmizou.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/getozyuxz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobqaxlk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcerpsyf.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/glspnyxrk.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggargvkje.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwwwfdzlk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpsxqcvb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcajqgcsd.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfghlyvy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/guapzdwmi.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/ghgikuhrt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsnschszw.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gngkkurvk.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggztazabs.sHtML


<!-- 参考信息 -->