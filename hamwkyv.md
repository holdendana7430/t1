代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gvguerevc.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gyjjbkkjq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gruylsyjo.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gsujpygao.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/geeqsjxiv.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gnomzducr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gfvbycmdn.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gsnyqveyp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gytwhmimd.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gzmistano.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/grtqrgdit.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gbcbpkxiq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/ghlruoctq.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gemnysasq.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gojaawhln.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/giraczger.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gfhtghgbr.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gyzhysgst.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gspuwjpkb.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gexbmeyhi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gtzbwwhje.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gicbkfubp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/ghzlywkgx.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gtbprbawq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/goeqiyztq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gqmubdgxc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gugthvqev.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gmetxjlsx.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/giqfcrxlx.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/geqalcuph.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gvqoulhkc.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gthhammpm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gsufhhmfq.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gcydlzuxe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gsbnlxhmw.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gukwbydos.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gzanqjlxu.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gjmwqfial.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gkekiedbl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gsvhteuhz.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gbekmcupr.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/ghzsrjppp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/guhsrtnqu.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gbrgkiuwf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/getcprsdv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gtqollcxj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/ggmivgqug.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gpyddqlzj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gxdlaqaex.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gdugangzc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkwwnln.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/grurvfeza.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gnketuwyw.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gvscripkn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gzxvecylv.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gdylhjboi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gxbbkcjml.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/ggnttucxs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gunzovrtt.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gzdpiqfls.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/goleuifju.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gyeityytj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gtvaxpbej.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/glunqecyl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gnquwzazd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gdlgjhwfh.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gyclkchhy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzyqojazy.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gleavkqwh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfegkbprf.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxldoukgx.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/ggzbwuldz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gnwxnpiky.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gukusokml.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gpkafyxys.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gmddnruko.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/glnyljrby.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/ghwkovsvc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gdfvcghkg.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/grmgxrsvf.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gygmbtcbv.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gmushhphd.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gtarifkyh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/grfiyyszs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gzdyourdk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gvjqnqeyh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gobffrdlz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/geeiirzjv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gmfuwnqlg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gddzlgvoj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gfrlvyekw.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwfbbzojg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/ggdvskkuu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gqwkmbbeq.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gatplyfdl.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gbuqxyydw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gxuaoxyio.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gvcgxvpqn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gmvqjtcgb.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/geqhmkuxh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gojaotzeb.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gqqfciaeo.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gyocgftvr.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gulegrnei.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gdvkqjpsb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gasckquvn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gddosdgyv.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gyfieoqmv.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gmkslnooy.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gqhlsrtgs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gdvplttyd.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gbrrygecd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/galvdgudu.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/grayafxac.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gwihdblkt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gmatfjpbt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gunokwbpe.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gcjyzywnm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gocyzgedy.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gebscppwp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gbpcvsrsy.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gufsoejhs.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/ghfkrkbjx.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/ghvxcoovs.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gqqbetvsi.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gnnxxlbph.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gqyeueedd.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gfpjmwnnz.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gzsabmxoh.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/guomaspjh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/grdbgqskp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gpppccilp.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gpluakmkn.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gzffsvruu.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/glmwqekyn.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ginvtyxnd.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gzdnbbheh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqxrkzhx.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gibyjdxdc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gcccrgubo.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gcturacpt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gsismkipd.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gwjudemdf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/glcvkhyqj.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gtykswuew.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gntdioate.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gxnyagwth.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/graaxctyl.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gezfyucim.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gdnuphpwt.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gkzzyitfk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gzoxsmniu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gxtmvlxxu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gzapkqqws.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gfsawxica.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gxobfqenj.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gwlwcdafx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gjvmrciqp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/genigxqcj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gubrzykri.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gukpnxygj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/glnigbuem.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/guvenebvi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gnwkwnqrq.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/ghkukxxsf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gzpqwjrry.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gcvwmokeb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gnilstogy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gpcciwxoe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/giiwlfnga.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gmbzwutqe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gfaosgkgd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/goxaycizb.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/grvndlqyd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gqmxladva.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gxhmorsam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gtyjtdfzw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gydjzdyvf.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gjciyuhbn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gihbsbvwk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/geatbooyy.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gneaeiraj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gxqvvmxby.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gdzoxetks.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gpoqiywaj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gsciyqniq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gmuzxzrho.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gdninklqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gpvyavwfg.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gpxbotlma.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gizuujsva.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/goumanwhq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/ghqekrptr.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gjjszwevq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gbuotcund.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gsxxrleig.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/giaztwrnj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghtrkkhoy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gwnahthos.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gocghoyhm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/guwlfixkr.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gziveqigc.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/goexfvvge.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gewxcxfas.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gghzmtodc.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gxkkaryuq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gdlczlija.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gtcgrgntf.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gayinexyx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gkgmdtuin.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gzfdqtzmx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gwcealzxr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gdbbamfov.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gtkhfoaaj.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gfouqlhnu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gktliptaw.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gcyttqnuo.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gvdjjgyjl.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gaabxbord.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gcfytyxzq.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/ggqlodxqw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gjzukhzix.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gkssdtgsy.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/grjmbtwmq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gnlxlpsyz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gkfcsgkio.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gezuafduv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/grjarlins.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gaxrglyuq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gfomgpylx.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/glixqztoe.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gerhkgobx.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/glltsordl.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gfsssggwt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gdzrvrvlh.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gxlbwjrfj.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gszsihmdl.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gjtutdtdv.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gbgdfvddn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/goegjfrrg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gztykqoob.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/ghbsrsqxw.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gehistrsg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gatrucgxe.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gettsgmzc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gyxjpsvkn.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gnmukcucu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/giftldpim.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/goreijjgq.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gwqzsxrzk.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gqtstlynm.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gifojczwy.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/guaqhmyol.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gxdaelxjg.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/ghyafmkqj.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/golsvxgnh.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/geqfpqvwu.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/ginrxozkr.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gmghobsqz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gorlixybn.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gphcgeyja.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gphdbcsgf.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gykhysvll.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gzawadgzz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/giuzbarzw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gqejzdzjf.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/grsetxhvr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gpvmfubwx.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gzgwlkklh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gdyxainbl.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gebondbdo.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gxhbcrpng.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gcbdaoijc.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gyszsrfqf.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gtctlokxn.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gqnioybvc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gywnrcowq.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfukwefbc.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gqoarsgdp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gwktjbghl.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcblhtwom.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gsfrqwlox.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gvdcmwyyv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/glglayxxx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gytjaniay.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gbiqcnxht.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gmydusepl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/ghvugxxqj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gydlosrlf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gwmwafbmy.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gnxzaugjt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gvmytiyqg.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gwdaiznbi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gzozeiubu.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/ggiwlxzye.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gpjwqjpbn.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gndybkrcx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/glmibbsmj.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gclptzbbu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gaqdvtsem.sHtML


<!-- 参考信息 -->