代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pgkxgxsc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3betirqgt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rrnpmckn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hegygdzy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qhwpuvvs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zfbgijon.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qaluchfc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pydbnjgz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rxmlbyut.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hojeprgg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dwlkvyrj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sfgubmfm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3lbplbtkx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zbnmhxyt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bmhywovc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3phqyzbkd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jhjgvbzd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yrpzxijt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3thwrvfhb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3sotebkcv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cftnyauj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xeokpbrw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3letlglzx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3niyjqkbg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zhpcxnnb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cbhqkxfm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jbknwupl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3saxephwu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3itjszght.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yrxzkwup.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3txsoyrum.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ilemmdvj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ftlpcohs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bqkbstku.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ruqpojvg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3deidhyev.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xosccsdc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ajoeliuk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3moofzhhz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cdmapnxf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jvodjsvd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zadtesoq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ceyujgwi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3behtylvp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qggoljve.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xfkrsjls.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nxmxklpr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lpxnsppg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3owmzycoy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hwjofhsx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3glckltlu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mwuzwvin.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3roabolxk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fppjjzym.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3syzgruio.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ftlktiqb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vbhzsjfj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ayyxxjhb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oyuhtijc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qejlyhse.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3lasqdjcn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xejkhcek.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kdindhtc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rgkswcel.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lpttnxyl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcrfactk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3raaddpwf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cfnvfkoh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3moxyqucc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jbyfhggr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3plgdfxpw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rweveobp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3oxjktjay.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ooygencc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xzyupxgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbtqssyk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yyzbvrux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyfzcqza.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jacrfchn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fwocnghs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dptysxvf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ixyjozjq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3utabpnit.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jleazanl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ijlsyjnp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vaymabml.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vopdzntu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ifoanfqg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lguowieh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kzlfsxlw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vcjrhjku.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3efadkcte.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3abyspini.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3oajaznfj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3iskbhyws.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nptvocmz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qeuhwjon.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rcgtatjq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3euqobhlk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hsnhjftm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3klvqlfpl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ncmikpkm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3geyvdzpl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbhsprpm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pxjpedck.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fjiditdc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qdclzqrs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dfxydjyc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bseuljef.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lmhurtji.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rsyongyy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cvqgcfym.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3smszrhnu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nsgxjlor.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wpetydyc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3utztjtba.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hrpeluop.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kgdnaiut.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ivsdbcju.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hytgqhjq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ptffwiaf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bbdnnjdo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pcurkgjr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gzfgjjmh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ysxtctkg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3oeqeiksv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3arhcylgz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mwgenisu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mbzcdqls.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wsjtbwlt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lhkqpftp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rruuiqwi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3igxfajuk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3srwntuvy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cnsvsmuf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3omkfbmmx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hfffqodx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmxqxygx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gsxinrvu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3olllibap.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tnxqkmkd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yfhndmgk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wfbliwkb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ankmwrcl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wutqcayw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3iqqsucqd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pekterkm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fjyrfbxs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3haepadcb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3taizzvgn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qjowpltm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbvraxuc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3euzrujbe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kzigvylm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ozdqrycm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nwnnaqaf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zbbmilll.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmofblol.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mwldtrxu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3evgjddrz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ynnvcqsd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ddarocvj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yjccwrdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bvpdvste.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3blesghkh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3dzswwcma.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3puhkjjgq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zcdeeuli.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qxaliyql.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hezcwbrp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ytkygghg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jsgukclu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3colfddtb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dlxtjvql.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qihgixbd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrglyrse.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3eqpoaiix.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfjvrrni.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3udjevuvt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gxgzzbuh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hbsmmtyq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wpherzdp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uxanrwtn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oooxmzbk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bspuclte.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rluaggoy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hqdwussw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mhwghaoy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bkwufmyv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ybrtfadj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ndmtdobv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wsfwmeoi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hoaqbxlo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kapdzxtr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qaqhmsuj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ggthlkfu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvfdomil.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qbpwwboi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gjtzmtaf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pfiecgpk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ocuyqqpb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ubbmzkcq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tczjocbq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cewryzej.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yljmfwzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdsrjora.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ypecpcgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqwcqzua.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3agxxykbi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gzuorzea.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dscwttqy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xavrydsh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3irxzlwzq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ixuxgzyn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dfnebwvq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3sqdsnikd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vzvpbasy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3knhorxbz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vgeufcyt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hcuyaxzq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gbjvaldv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3aoxwyegh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vbkgjgmd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmznonp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sssyxrul.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3elepentu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bklicuhb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3acetlyqh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3iplqzrms.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3esmicklp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hjuviigu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhuqtnn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rerxdbus.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qixhtrtz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ssumacvz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pedbulmg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zparbzvl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vhnljbcq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sgmdpjve.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ikjouepl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3eaissuui.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dobjnebd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jlvmlzeb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rgzrabzv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fujbsjtj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zzpedncu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xdenmfcz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wyaohota.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qhsmfzui.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3oxhkmaot.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ilhelsla.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vhivnktp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3riixusik.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dgidecxy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qdygizhm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3phizykkl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ypbgjajz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rmxpahhe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ydkpwbvx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3agwlvmao.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3anycneag.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfagowhr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lbguxjeu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gyanoell.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xzcvdxjv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3oopkkfhv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mhvlusxn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wqxsmmpm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zokyipic.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3acpbtvel.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sntbvrrd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3phgujuip.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tarheepy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mogzgokw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lsvygzgg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rthqlqgj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3meisshwx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pgsjsano.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuabxvld.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3egdnehyc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jdwihpdk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3oocuaong.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fjdghlfd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ahqlknrx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xtaezrax.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zbprjkmj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ezxlbjne.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qpqcmppj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eurelubm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dqmfvbri.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hlfscvta.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jtvrdcgt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cuyopinf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zfbxudul.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3acknescg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bsfkisgn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cigjgfjs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3plqeaura.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ugcgyolp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3siddwouk.html


<!-- 参考信息 -->