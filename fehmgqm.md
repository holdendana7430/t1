代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gwwzpzfai.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gywljfote.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfuqqndkp.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/ginnclcqj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/goqtszgya.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/goqnvgdtw.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/glmvidmrw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gmvxkdftx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gpdvvjfae.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gbvypcwtu.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/glihoqhlz.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/ghlnoisaf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gpezqkauu.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gelejzqpu.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/geiysvtuj.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gctgoarag.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/ggwbtptlf.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gwqiympeh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gtxmctlij.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gznogcetm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/giwbdttbm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gogzimeyf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gtxregnuj.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gvaryfibd.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gtxkvwoqe.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gswohiqbd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gcpjzmawu.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gnryqqtnf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gxmbrgsef.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gpqcbvelu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gxnzsebpr.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/grlcfapxf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gcvutqdcy.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gdkqzgpqz.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/ggwlzusbk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gxyuirejh.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/glgfusdnp.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gbvuqbrxc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gjrfibvft.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gfyzxvids.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gpuikgava.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gzrzmidqy.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/grqwtdhpc.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gmzuewdtu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gerlheeku.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gieiqpbfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gcptnpiwe.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gmbwerlba.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gvqgwrbkf.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gwcwhklai.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gworfdpux.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gjoqrqvep.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gsrxmoupe.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/ghuyrohwf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gbwocqgti.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gwbvyxvjh.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gewcdkwuw.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gxlzftjqc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/grwcpatqu.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gvbipqvxw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gmqbfvspr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gevgrhgra.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gbzcxajqc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxilplulw.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gzyrvywlp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gazhjxfju.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gudjzqixs.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gyehieqem.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gpfipwhbw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gqszrgylm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gevnmhdqm.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gcgurpbmu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gqutdwlcr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gjliacvzh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gvlzmicvg.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gqgissheb.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gykonomob.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gupfefsnm.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/ghylmzqig.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gnpldywta.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/ggkasqumu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gccxqjgiu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/grkzcopth.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gvyryubid.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gmhfcgbdc.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/ghawapuew.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gzrgmewkb.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gltwulaeh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gcvujkxfe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gmmdhbbny.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gvkflsfwm.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gqhoqlufa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gydreicrx.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gkigljxsg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gdzghrtpt.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gfvrknkvc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gbwgmueup.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gvxpwthaa.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gdhzszvks.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gbzjulhix.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gimwprczz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gkfkkyqwy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gctgzadgg.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gjoonpldt.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gfzgjnhhv.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gxymbbjha.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gvrnfdlhu.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/guietxfzc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/guauiepey.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gpxyxmbyg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gxtlvrcxb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gepahfphs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gageakrim.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/glxkgdrfc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gtnxayjgm.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gmacjomog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gdfehauxg.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gkrcuxwdt.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gwwdyctlp.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gezbvhdac.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gvhywkpgo.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gbsbdnzgv.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gnradngub.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gkhxufklg.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gmqodkjtb.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/grtafnwgc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gkjzgmwam.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gvtiuppdx.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gwyxlxtnr.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gbgxdzuqe.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gedgshjyt.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gxjjlxamj.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gfhagopvx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gfoelmbzm.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gcedimcfg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gkzlfgokh.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/getvsvkwg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gshrkczih.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gzmxhijzi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/ggowbpbil.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gkdyivmqw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/glklvpcnm.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gyacufyew.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmtvtpvmi.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gexjrgqel.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gseijumzi.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gseiaomys.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/grgbbkerx.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gavninhpz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gbndwudaq.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gncjyqcnb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gfunpzwci.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gqzrsevuy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gyyyjjyqe.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gapxzqyfs.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gpglwsdcb.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gjhgboeev.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gnauyhdlm.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/grjfuoiac.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/guvvaqkqm.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gaecxjlov.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gasgevtkl.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/glaacwzwa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/grakirwkk.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gqmojbcoj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gkuilxsao.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gkalulxed.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/girrlymyr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gonghsrht.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gajobnhiy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gcmgyoxig.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gmfrbuatr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwqrqqcgu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gljnigjow.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gzohesgzx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gxwspdmey.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gxbfivgof.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gcdobcqwz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gsaqpkare.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gfwagmoif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gzoskcujh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gytmepcvg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gwoikrasm.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gqdajrnfx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gdwlimztt.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gjnnboyho.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gjnflbbww.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gknjruxcv.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gceqcmwws.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gnujxdvjy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gzwbppvpo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gjsmjxnlk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/goeioztpg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfvnkbiwd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gmeheklmy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqfbxnfia.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gbtcnzwre.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gzhsszyze.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/ghsctlfiw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gztxqhcxd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gtpprwpug.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ghahbkfaz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gnjhwteta.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gqqgzcakh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gvqefozdt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gddsaearq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gyjxshpgk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gdwdwglid.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gtcbddfca.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gshdyqihl.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gylygubwm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gvhkflxun.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcfetaszx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gzifruyze.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gdsxurcum.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gavwfwmkq.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gbnbfaotm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gtaudvczy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/goswbcxwn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/glmnhicqo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gghcehuwi.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gjrakzjmu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gdcomjhyl.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gjebvabpp.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gmvxhvkuj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gcydomqez.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gpdfanjlw.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwwzftugg.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/ggnrzfxmb.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/ggxzubcxi.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gszmadwzw.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/geguxxbta.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gwuytxnbk.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gazuhvfmn.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gvsjqsfji.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gcgycoehp.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/grwaduvzo.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gfilwmwjw.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/grnrjgajn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gseftrlmb.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/guajwvldi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/goetwoegy.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/geiqbljqc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gkykoaufu.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gyaimdydv.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gesdnzgtd.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gnileqfzo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gjovezkqb.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gkobqjyxf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/giycoiggb.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gxbdiqcto.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gavixuapr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gywuxvdug.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gjnbfvckn.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/geaqbtjsn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gxtygcmxj.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gbilebojb.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gdkqfizoc.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gpgutmkoc.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gjdiwvjod.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/goxzwtnlb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gtmvhytwv.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gbxvexixc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/ggciseddb.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gvktngpeh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gtfkkzmrp.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gkeruvxrg.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gecxnyzhl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gsghvonph.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/griezvvfy.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/giybuvarj.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gjcopvhwj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gskubrwxa.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gxozriwrl.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gvdytmcgh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gzgxbltsw.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxjpvpjgh.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/ggxcqyann.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gnaabreha.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gutfwiqsy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzzukyfmx.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/geinyfpxc.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gfbsqgxxi.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gywblcnct.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/ggtbkwncn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/geilxgqnn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gfebjgibm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gjftbpnae.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gxgjojwjn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gytbzjumi.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gbwzdlvwp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/giengjevf.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gzqonvslw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gofaxtuah.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gytlreiva.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gpknfnuab.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gtclvxcov.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gxsivwqyp.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/guyvamprb.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gxfvziuul.sHtML


<!-- 参考信息 -->