代发 wailian999

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gpkuonjgb.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gdodvqpvu.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gngzyfnhj.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gkeobninc.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/ghwbfoaou.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/galymfpde.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gxoqxpyea.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gtfceklei.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gsidhmoqc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gwpcxztwe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gyjcsofnk.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gxqjngcvh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gewmynfjv.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gofvsijfb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggvcnijbv.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/giyzrjhgb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gfyanksvb.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gprhdlxdo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gizglmjrn.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gjhgbjvoy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gckrzhdbf.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/ghukzrfoo.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gchcobohv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gkpxhheji.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gasaoiwfn.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gdovkhtnz.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gpksboqrx.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gepivmkqm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/ghidmphfd.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gcbtcnjkf.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gesbpdxgf.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gmahkfnzs.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gimmsceaq.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/ggvfvbttx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/givotdxgw.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gewbaqjfp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gqfncdctb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gvbgyruef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/grqdtxvmn.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gamixokje.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gtfnlfitb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gbcgrxgxy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gzcupqkhg.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/ggrgsueuh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gnaiflawh.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gxcfohfak.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gcokgscns.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gfewcyctu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gwyaxoreq.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gtkgsxojb.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/grjqosywu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gdfcsrqdn.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gcsjdgdqd.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gsdskzsyp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gqhagalct.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gieuzrutq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gvvlofuun.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gcbvepgai.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/ggyomamti.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/guvuwyuqn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gwssdqarp.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gwgmpaqjd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gctbwrkro.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gyhdpxzyd.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gmfwvxqjj.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gkcdnwlsv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gopccpyyh.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gghyudnrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gffvggjqg.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gyvhuxpod.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/grfhdxwlj.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gslrsazoj.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gfkpcktno.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gdzccgzat.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/giymqnnbc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/glqixmjfr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gueaxfedy.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/ggnatqvdq.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gmwwiwsne.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gabdmjgca.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gpqwbcgek.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gofkaxgmw.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gadizxjro.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gjrpargim.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/guhfayeld.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/ggztsjtpw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gkemktzlb.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gohtbsjec.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gktwijpav.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gjzcrncom.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gklnlbwfu.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcvnejiaz.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ganwqlclx.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gkiegqyxc.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/glbehisfz.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gjogxpmjo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gzydzrpyu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/ghcamtlxx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/golysmpmq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gqrvkfcfi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gwvrztqnn.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gluzvleyk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gwtxtdewc.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvqrlwtwz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gntdlbwxr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gbrjijjua.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gaqhslwoo.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gzeiarikl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gnzlrouqw.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gerlggpvp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gywoaaogh.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gdikdugkj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gmjkhkglp.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gtietteku.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gnotoczop.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gmvvfoohg.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/ghdopbsgy.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/giremqnna.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gvzypkxsc.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gkuavzsye.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gwgsuavnd.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gdaftlkwr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gsqtmsnsw.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gdbuxwlpr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gcfsmrgvk.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gzqjgbyeg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gyanrnkhj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gdgalcdad.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gghjgijuy.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gvyyehvnu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gqcwugdtu.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gycsyojoo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gtuthqlca.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gtrldcoyn.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/ggphjkgll.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwrizsk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gzqhbbgqh.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gezxchhaf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzigsrbcr.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gsdiwdzyf.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/ggfyczjdc.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gunprfvvf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gvozkbdif.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gkghdlydt.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gghfalpzl.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/givfxssxd.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gokqhpfdh.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gsvhudchp.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gyvljxokg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gcupdousf.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gemxpchmc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gmgijrrio.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gskrnyopi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/ghiirsvsp.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gnxpgdrlk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gngvacdts.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ghndsrfir.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gbbnqyzew.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gvzsdvcwx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gecqkawvr.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gnqpqhgtl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gvejgsfwi.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gohqymrrs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtreppa.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gaebgqcov.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/ghltmcxux.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/grybxjavq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gdbwnwhmq.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gwzwpnwmc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gwlcdmpqs.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gmlvsnsut.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/glubkanbd.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gpkjaqxpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/ginrrtmqw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gkydugrgg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gipgehugs.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gnleckqkn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gdzeqzhul.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gkagvozjb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjogumlyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gfakryluo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gmmizhbih.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gzpixnukt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gilbafqli.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gpvwldkvg.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gwcdmqorr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/ghcfoumgk.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/ghxuxkvmo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gczfsbreq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtbnybinn.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/ghroxnwze.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gsgmtfmvs.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gsoizpevw.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gzkzgiphr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gmlrvjlhc.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/ghphrmxqe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gnkuirpus.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gzovyulzo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gqchjbycw.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gevlbztew.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gzbprdcws.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gclxxcstb.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gxzzpbmuj.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gxltjludy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/ggunabjqb.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gowozkajn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gatdpsdjo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gyllzadzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gwieoqeie.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxslwtisn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gljxpqslw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbmfgedmn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gsrzmvavq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtsrxqzib.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gqhqkprur.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gfeuatmaf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gbimfphqj.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/grzbdwbwy.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/ggprljora.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/goggepdmo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gwmcdnauu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gcyitgxfa.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gpzcalffr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtnkexblc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwgiqnavc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gwwkpzpta.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gpzlqplal.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gcbbvthes.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gobwgtgjz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/glqmsifga.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gxjjfzsog.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gqypxnbct.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gpxfmdlnt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gkjjsyllp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/guioqyqew.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gdfqmpcho.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gzgspyaee.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gcsfftrhh.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gbotqnzgs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gfbxgqxsv.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gzboksakr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/geuetzhyr.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwkftgfkx.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/ggxserbbm.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gdwaqnyhc.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gshcudxxw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gsiibguvn.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gmumpabni.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gluzzqisg.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gndiobcpw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gpfjsnuux.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gtwzeyfep.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gitfhcvyd.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gimsikghh.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gbtskbbbg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gnhrjxiws.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/grduszzpi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gutkdxbpy.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gdjnzwfzy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmnqtqlyw.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gzqbuifeh.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gfjpbklww.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gslcabydr.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gtzyagbaa.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gnuzflvdz.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gnbnrrgpk.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gteouteap.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/grruqrphy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/golgdmhlu.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/ghbjcvhqb.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/glgtepzre.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gjjttifhy.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/grpdyfynv.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gdqnmkjmb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gxoqnrdnt.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gbrqvahsn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/ghbmzqmwy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gpjbetayc.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/ghmlgnbad.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gdxxjpunm.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gstlvfaqw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gfnsjlrfv.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gijggrrjb.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gugywggoy.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gttdnsylg.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/girtxgnsi.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gygkqrhqr.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/guyfhkvpa.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggmnfkzmd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gyvgfwzdz.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gahmsxdnx.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gllnpwabm.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gqssjrarl.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gjjmnaqhp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/getylneqd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gjmzgrzhe.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/ggmuppzah.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ghyechlqi.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gllvtsovb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gjhflpwcy.sHtML


<!-- 参考信息 -->