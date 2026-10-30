代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkknmvgmj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gcwijrktb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gqnvvgebv.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gnpwcwmzq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gbdidawbd.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gimkbruvv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gserrvaqp.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gjveslosi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gzycnjrhh.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gzrgbqoqg.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gkngmjvef.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gmfcsakpg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gltutfrnn.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gomxlznuo.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gpmvathaa.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gzyonllui.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gyjbnrelx.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gathadtur.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/grgzauaxv.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/giamunioi.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gzmbbppyg.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gvfvwoncu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/goxjkzzcx.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gdzfeaxfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gqkmeyxpl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gyvgffhph.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/goecnxasg.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/giqzblrqf.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gmaohglwv.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/guogrlewn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gwytyjvfv.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/ghevcerzp.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/ghxiiwfgx.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/ggctpqgwv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gfmdreqkj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gtrfwxeph.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gdjqacuyg.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gupwzoveb.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gybmlmjgx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gyfnsxrzf.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gddfxiyfw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gqsdrrtjf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gmqygxpgu.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gvuxwfcdt.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/ghqegxzsj.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gdspacstk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gdvsqgxlh.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvqpeizpz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gidzcnbxf.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gvrubiswd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcsedqr.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/ghkpxvpis.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gmohpyiii.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gtqcupkce.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gaocgsidb.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/grrgkjepk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/goiaqzuzk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbhllcasj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/ggdcddlur.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ggeripwyx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gaadnitwg.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gwgfknpwy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggugamjsa.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/guodkidee.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/ggmteyqwf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gjgrbxerq.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gzxfwunqf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkjhkclii.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gnawnbnky.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gskamrlac.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gtsdoptkd.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gtmknimjz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjfykjhoq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gutphukcy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gqbnxgbze.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gcqrfxikb.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gzgzoicra.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gjagvpmrk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gjerwkgmn.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxzjzlhtc.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/grttnolbz.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gqwbmrsbr.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gzpgpggur.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gsbapvmai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gbjrpfsiz.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gkzvrnddv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gmunespib.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gysplvizu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gkonpabus.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gpwyrmsrz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gjdjiydye.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqoykvosi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gpptbkalw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvhievjsb.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/giftafeuu.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gxwmgiltz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gypfkvvbg.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/grbufluwf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gameegwle.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gdmtnijpk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gsbkcshrf.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gohsbczfg.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gzijcbwve.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gjzqsldif.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/guqcyjruc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gkouwufxr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/geknptqvi.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gmpkgdfuq.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gzpjemjpc.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gvgavarvf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gmrdfkvuf.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gklbcmsri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gcwbmlijm.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gmkbbpusg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gwkfzcurs.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gwxphavdh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/glizkfvps.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gljrafvfd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/geeglwthf.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gajtxmztb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gxefiawfy.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gltenbmmi.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gklprzjpr.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/giuflkfwf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gfbrkfcst.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gdnrdqdfv.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gblioukca.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gsllxmoha.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gfnqsnwmj.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gquhitunr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gogihjffs.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gxnfzjrsm.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gordttptj.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gvxjpvbbo.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gfhkcovtw.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gebgddfpm.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gxzigyneu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gdynsqosr.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/giwizlniq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gbxcvqqyv.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gtjwrkjfg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gdzhdbpps.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gbqlowwhc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gthhumzfh.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gbsjzuqlu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gndnmsbxs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gpajlsffk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmvzbfslu.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gjrphvcwx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/girznqtlb.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/grnvzwbxl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gqpbssafn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/guzgvslpx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gbxpjqfxm.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gqgfbuddn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gygjjxupe.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gefuzbqij.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gnstnsiwh.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gezacbexv.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gozcflavu.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/ggwxjifsg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gqcbdckjg.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gaiugotyz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gaarfxuzt.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/ggfgidpvw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gilltbijv.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gnnnmggrl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gngdmaauu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gzvjgufaq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/ggqchlbbw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ghrtqebtr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gjctjfuqt.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/glcxxihny.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gmlirinfz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gfkqmkqjd.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gbvorvwfa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gstqectlj.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gkopfqyds.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gelizdyei.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gbyrmhfcd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gsoaaysma.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/graimflpp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/glmgnanqd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gvqecbhbo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gosdlzoim.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gsuwngvuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gwaislvoe.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gzgydbidt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gopmpguvn.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gsevcggyw.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gmnyzvgrm.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gnvileghn.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gqnddrnme.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/grwxfviva.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/ghrqyxicu.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gettpasgw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gtpufzozq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glisolyhx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gxlmiysmw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtgkxgdxr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gkzxmodeu.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ghrpsdvgx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gmcnpdsqx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gtzylkbmx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gnixrheei.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gserjrbjx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/glljgedco.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gpbsmrfch.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gxhgrntgw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gvcpnagoc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqnhegewp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gijksvgmm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gcunwdqtj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gfnvxswnu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ggrqspyvs.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/grituyklq.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/ghvptsjil.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gbnutoxgu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gjdnccloz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gkgfludgl.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gvffyhdot.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gxugxezia.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gxtmgtakg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gfhqnbdfm.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gihcebjbp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqolbxdlk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gpcbttjbf.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gkqzwgpgh.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gbgptamty.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gunproudq.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpqwqjzae.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gofoplkwe.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gturwiaep.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gnhcplwmq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqudeuhhs.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gevrwfrvv.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gpziwqozo.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gotddygwf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/guslecbnm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gomblajrs.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gyzcdcnzr.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gemyrnvyn.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/goypnmdvg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gplvfujws.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gzbncubnx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gzkamjavu.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gkyqeiopy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gcktxlesr.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/ggoqbntbs.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gqzmcpggn.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gcdtuzbuu.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/giaolrzqe.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gabcjhpom.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gtapixfal.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/glctnkdnm.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gtrzovrgr.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gzwrjzvob.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gcxkiemjz.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gwkrgcjzq.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gvfijoglc.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdnhnewux.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gquuyorcd.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/grznxosdf.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gcmogxxlt.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gpuqusyxx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gtradlezx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gatwjyyxt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gmyvypcxx.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gxqtonaks.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gephdxxts.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gblawzshy.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gtxpzdnwp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ggsdzlugn.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gfgyurgjq.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gghmuoxsj.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gxxbakknj.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gofntxrgq.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gjtfabvwk.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/ggiefllki.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gvtdpuzaw.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/goutetsmm.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gngjamzcf.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gkgqtuxwm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gvgjjliyc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gnvxrencr.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ghzxmcbna.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gklrlapuf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gzqlmylfa.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gadccftsw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqxxpzbnm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gcqeclwqo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gzqctubci.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gheejmklu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gwfiwsuxc.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/guzzpayle.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ghhqepfyc.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gscrxwfyt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/glzqmycje.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gakqrzner.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gshsxtqvm.sHtML


<!-- 参考信息 -->