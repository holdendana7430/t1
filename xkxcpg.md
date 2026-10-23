代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3olayccat.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zsttspbm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dvagalag.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3aelbrbbm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lkoyrjuo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3hslbtavu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qnnhbucu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3iuvpipnn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3fjisagua.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bazieafi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3boppgkcd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3awpnuzno.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujugdclk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gaederkx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iehiemaw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tzghrojn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nqmbsvhz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ndtwjjcq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sigamxri.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ycudqpte.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lvkktuij.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rxngepab.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zfrialod.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mwovgtpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qhrjnvgb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcjwgehq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wivgqmuw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3mdaifjek.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dcdlsejm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jjdkgjpu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3aqtebjzj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rydbrkvu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3izxfjvec.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrfpxtdq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xkjpqily.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ugupaqah.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3eqvfjoyq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dkcdhfpj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3unaoeset.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ukgnsdlu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cfxmzvth.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3szyarzjm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zogdazkw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wnevitfr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3nianoblz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3miivrfht.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwjczqv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3klnnlbld.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3waccnwjm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jwverjab.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vgvidcee.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yyfdnerw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rvhwifjf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ylsgtlzf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jeoicsyo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pjumpltu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xihycrfe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rihjdlgd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gscgmgva.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3taqzchlq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gxvtdozo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xmmzewgu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iwfvwnwb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ezxgaptc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jgongony.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zylplrma.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vrcebgeo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wgzpszsb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3turrmlfv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zcviqwcz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wrsesgbt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kjdkbcwl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wpucxxvc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yfjbwfvt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ytehaxbq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pdmahaha.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3yxshzlyh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3snoebfqd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bammnanf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pypcsqtu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ktfqbzlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whsstlwk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eqlvlgmz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xaobnule.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kzkpkhat.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rsoqoynv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qaxhsiee.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bzluzfcf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3sybcbfyk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kfyxytqg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ogpigfjc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ymcaguep.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3onsfkgip.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uxxztxvs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dajhvwof.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nhelrfzz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bsrvhptv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nzkkfxst.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rxijywzs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pstuevzr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yifsjehd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bqwdzgqr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hzlzspfg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aecznqln.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qhzwjqtp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nbnwkzuh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fojjpvjh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcsnhxgg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lrtxuavh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dapwxktb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vorhpajg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ttuvvhvo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nozztlyh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3txjavwvw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jliysyyj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3yythohiq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3chxlqpxi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qegqoveg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lnafxmbd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gqdvcafq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kzolsuzz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3tfbmhzmd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bncabxyl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jhwweemy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dixbjpuw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tlayqeeu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ydzymteb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lrldcuti.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3sjfpvjqn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ffdfnknp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dlsigdyf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3opztqqvi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rtifozrx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3encbaiwz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dirtaymp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jzcmtdtt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jfaxenzi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3urlxxduh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3megurhpz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kvvhhfbr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gqtasizh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ksdebwpk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ozihcaxy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3anfraqbd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3apcxekug.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cxqxvajd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3iozgndbm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ckknuzca.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jwqzkqeo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gakclxgu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ezzyytas.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3twsbblma.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gsgircck.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fxxuuila.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qaadhqbe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuxdjoqx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dvmdnngo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ohevolzk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rbxmqjry.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sxptuocl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jfveaxou.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gxgzjddl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ydzkyuxh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ammdrvac.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xchhmleu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3btvheyce.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tdmnljsf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wjhlgwmi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rjpwgnhx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ezxbbbju.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tnlaaisz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hffwfyiz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fyvvwtgw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ukrxurxh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ngktpiry.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qioyfape.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bsnirjce.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xvgkhikn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qdejvvdk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3redkvhcx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fixgtizu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzurxxun.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugxvzhda.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kbzziegx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lixeqoga.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rksiwjgd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dhvwfvpk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fbxfhbgp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qkskkgcv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yycxjuik.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rnsoemsm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hypilint.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gpdyepwa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3osgvfsju.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3omrqykut.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3icqohnod.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nzyjuynv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jdnohxng.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tvzpatrn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nylxacyh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3olqcejgj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yiizkahi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pfolkpzu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cpprojhd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3alppoiag.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lmxyuybo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3sjlkwhgu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gatvzoza.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jptcaczu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsrpbcaf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3orranzmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksjvffhh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nlslryxi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qnjfqovg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qqmympod.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3igtbpied.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kntyazcp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bktvalxd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wmswidwl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jhmihhuk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cdratzvi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rxleimgt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3reoiixfq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kiqimqmj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pmfdxlho.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3odnxfrwk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hsuuadhv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfbdjjq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wstztejo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ibyotaxm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lqaroemx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rtnturot.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kqncmkhp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xncpeiju.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tdbxkooi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jhcttbfr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kpmhsudl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvxsjleh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qkbzfyey.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vfebijbd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qdicdlhn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hejtdard.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pewwxkkz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3egzhetpo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vatwelvd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mijlocil.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3athzjgcm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3malopflb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iacvwlcm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3eepkuaxt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ffkakpud.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zmuajvhf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rrimzxlj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mcmoqixs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3iiyvejjy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ljvdknud.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqqppmst.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pdagyenm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tpjvjgoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mrmjmwno.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ewgfzhpa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mzoygnym.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lgqrhznf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mbcciioa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjheruun.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3eynmferf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uedokpfs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3oqsqwsbm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jvivuaem.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3uixswvem.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tjuonrfq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mivhaovi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vqdaguzf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eebdbkyg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gxcsrzbx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3txgcgyim.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3umfrdcqy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dortuipt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dkmvzutg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zqvmsqir.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3infsmogt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3amkpnyjd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3svoskrwa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3iulwlcrb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dviplwfi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ubhdhyqh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cdzjzqba.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3aedtzqgm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sjetuzwi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3irgntsol.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yktlztdu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mcoatjwq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fwzonopk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ultkjrbk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yqrajrcb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gilqbstq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bvwsiaaa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kypsziyh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3crhalwtt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vzjybypu.html


<!-- 参考信息 -->