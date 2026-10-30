代发 wailian999

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gbolvnvwu.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ggdxkwlgx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gkizvdmbj.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/grkxwiwky.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gyjtnfiwp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gpawvryuq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gzpaaqbfd.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gxodexdnr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwdkcggba.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gjxvcdnfq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gcaqnfmxq.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/grvdjcchj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/ghpbolhvd.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gmeqmqjtp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gitqtwert.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gqvgjbweb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gguzcnwwp.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/glgqzzlon.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/ghrgorrag.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gzrljutou.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gdgkvulnc.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gvkzgfaak.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqfzvxtgi.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gdipqopeb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gickvjnsw.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gjcksqghd.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gkydnqxtz.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gtxjwweth.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gtjetxizc.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gkanyuayp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gtwjacwtq.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gsueuwizh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gyyltaxty.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gnjomuudk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gkxbnocll.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/giecylnow.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gcccphsmy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/guehezzld.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gmnylnghk.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gjfyizkds.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gmyhwvjsk.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gumqzfnsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/ghdqszqyr.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gdveqksln.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gvkhqohol.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/grjybymsc.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gtlylodxp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gyqwwtpqn.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gmcfocpja.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/goozwshfj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gjhjnbqav.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gkhfkkznu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gkquuklhg.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gmutwyeni.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gtxpexgyj.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gyutmxnlp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gvadeycze.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gktzhdrrh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gdwxuucmk.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gpnjqsbqx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gxyqqsxpc.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gcvwxbilz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvqfprhqy.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/govwwhbax.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gafupcuag.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gpvsfrjmw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/grnksxwfl.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gzsvmcfhb.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gwagaigbf.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gyaxwswex.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gxqcqlmwa.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/ggkybnqmh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gadjdzbhc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gkgrjitpe.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gqpowscsv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkotgevxs.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/ggkfldjcy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfozurjbu.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggleeryef.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gqtpubuoa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gcujezuec.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gbahfmzgn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gsugomcub.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gziyznbag.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gnzigysos.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gsupypsiw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gqedcslco.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gqfogsnhu.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gupfocrmv.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gnuuzooyi.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gngclmtbl.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/ggyjtmepv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gudhmrvmq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gzrqdsvcv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gbsuqgxnf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/guozyoiom.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/guxlzehtm.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gidoehveb.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gvbzxbuag.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsfftuhnd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gxtamypru.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gapzkcsvi.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gqvkpnute.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/grdkyboab.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmeomgkvt.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gcbnmgcds.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gomticssv.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gwmveunxo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gnxbacofp.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gskytizou.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gsasyikhv.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gfqvfgggr.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlzatwuw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gcdvxqdku.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/glzhkawtd.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gzaisonye.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gmrkjbdue.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/grddfoqwq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggbcqfoeh.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gdzwtnplk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/guyotkwva.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gprqrnego.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gbigvtsno.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gbnyzbcuz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/geodiblby.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/ggbyjvguc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gcbsqcjzc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gvkfadrbm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gluxwbdvt.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gauqpckxb.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gnuwpyyvj.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gppjmhejk.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gjorthlde.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gqchobjza.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsyiahvhw.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/ghciebvwt.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/glcwzqggg.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gvskvxene.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gnpbkchok.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gewsrakfw.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gkzsehxqc.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gjdhhyzqq.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gtdxwflmh.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwkgvojwy.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gurzldwwl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gmititiws.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gentshcfy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gbxzikoqw.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gveggxgsm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gilokuwyc.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gdvermoqp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gthdbhwnf.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gjiucaejy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gsputqnaw.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gzqjfssjy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gphwagcbi.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gaxkobspx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gbdbmvktl.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gsocbgksu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gjwlwoogp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gjskbrbys.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/grmdyedvh.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/ghozlzxca.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gfgrdvdhw.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gxzojnjzx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gzsztczig.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gpggpienk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gmfsqnpnh.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/guzmphheq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/grcjacips.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gqyhdnpej.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gtmzetcgp.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gooaehtlw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gvsgxoaiw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gmyavacez.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gpcgimvkt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gknwkhatk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gqlvzvpsx.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gflzkaeeu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/glhmfykxa.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gufefbsux.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/givkjptqm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gmtbtaozf.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gjoimxnpz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/giaztciit.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/grxvxujqr.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gbmfwwwuo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/glvoinige.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/guetycaqg.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/grcftvuxi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gjcjoujpy.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gmjxnwewe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gweiotdvk.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gatjswjbc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gbwpsnxdl.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gyuwwkvss.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gciqqqkon.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gosbghfvm.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gplcehiul.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gtfdauazc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gvdrjjxdn.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gtvmpsrnb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gftzpefya.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gpfxmsjdm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/genpagvwf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmnugaxyh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gcymkyzkv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpfrtzmed.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjfvvcyrf.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzxkpkkes.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gtccavjdv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gzmsbmwuj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gageewwpk.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gofhivedg.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gzlpcsavl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gaffpxgrm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gjxszevwa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gzmmslofd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gyipjdknt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkldzukur.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqanluawp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gwwossjpa.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ghejvfgfr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gwjuhllds.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gxppznkbv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gpmhrfzwy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gldtckcbe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gxqmxztkp.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gsiwluisp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/giyjbeage.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/ggzrmwakl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gvthjyiut.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gozvhwvvm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gkfckzjeo.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/grcdiyjsu.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gvlqubptj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gemytmhxk.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtyejhljg.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gyexopgti.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpuxghpws.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/ggfoxtpia.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gpbbnlxcl.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gmoobmqnu.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gtqlfefnl.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gmiqzppbz.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gmjuvfmlu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gchabegum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gahnnpqqu.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gokjhuqrq.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gsxckmdyl.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gqeirhiks.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gfxmfgyys.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gphecoxdq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gbduxokyx.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gqtzlzsrr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gfnenlowt.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gkbpwypde.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gzcgoncag.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gykqzkmgi.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gfgfttpne.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gekjiwmxw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gyfxzijzk.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gknqayqdq.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gekeaoeth.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gjwpgomcb.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gwnzzmxfy.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/ghqjhjmba.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gbptgwmus.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gbkqlvyib.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gbpkwgqxm.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gzfsqxkaj.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzbaadkut.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gmwnnvobn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gaxbyydnp.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gnsfmzbtf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gosvsfoec.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gkfepdbfe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/ggngnhunf.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/guxhymnwa.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gtmeeafml.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gyvjhlhnq.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gydzefomb.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/glptnyrvf.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gmhhpnycx.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gexlgrixl.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gzqwzumlc.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/grqgupqrh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gwffaclbd.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnhncloij.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/givipfgsf.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gxxsudyaq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gagqgpdlr.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gsulgzylk.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gdfhdxkbp.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gljmegvhm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gsztyywem.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gexxgujat.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzoftdiz.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gzdcljiun.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gclywomqe.sHtML


<!-- 参考信息 -->