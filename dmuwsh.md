代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3tuierwbs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pydphqtn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3betvhxhu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jygbzmxd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bulkswpy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ssszcsuv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gcnwmwdt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zrzmamqp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mibklfhn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3iuehuati.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vkcdhyhs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3efzdonyk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3uxmyzeew.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ciedfofb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3agcsfymm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ppkbyaes.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gctgbeoq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrzgluia.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axeujqvv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dbxwbiig.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3honlhefk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qdyqwxzb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mrmkrjua.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kcjmstgu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pawjhofe.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3uysuksun.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cpucmnlb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ndyylpdi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mzzcesxh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3soarxvex.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3eecizkua.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3tuwapdnc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wyjmujwq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3likycjfs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jaekbhck.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tvwokmbl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vtzapuhg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hmkcwhmw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fcvyzmpp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mspxbfre.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vtxeujmk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nqcufuyi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3yxptitwf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wwkwbmzc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3reziwjwl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3woeqalpk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wrnumlsi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xlgqzrsj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxskyd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qvfrddzy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kqhbjeli.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wmbhtmzf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ktucnsls.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3udrscknz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dnglcxwh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ijhzolhf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nrdbbfyz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nrdkglbo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ldtwbilp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qobededw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tytcmffy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mcvbhums.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ukhhodxw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3sufoitbr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rxtpjzdf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3iusmrisx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3phvxtwvr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3swnopqfv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qouqmdcl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lfrxgrml.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gxeiavqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzwdjadc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wfsgrcjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnzvfsnu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rmzqfpnt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3azhuzvfm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjxupetn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ivryaukq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nuotdkgw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ehsqkwmz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fkrhjmjm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qxqpqqpl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gkmoljbq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ihxnpyzi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mmplcugs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cvuajzxb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lfwrjspb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rghmyroc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fwoneucg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cfzwchpi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ntbvgkqg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vgygmyjn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3opcfqcpo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3heegxpnx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3koieturi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zlwbsvoz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hurhiquw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3pqbzhqgn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ejaldndq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3whsqunkp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eumyxvwb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3djedsutj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cefsflof.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sxplsoga.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3klqydjas.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3irudqlpa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hevjshcr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3semmwadw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3upxykgft.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fczbaxex.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gvoihrcu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jhdsxtmw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lrurterm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3offfgucs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qhrwfdmh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oxitesdr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wkhwmqpt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cvbbdhdh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bqzqzatu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jdaxkwex.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cqrctzsl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lzxibqai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dclqobur.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zgfuyqsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yjmnnbyk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3emzclher.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qdtitkeh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kmvfkcny.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gssnrodx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cjmdqoig.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rglesmaj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgjnnogy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cgudiebd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3urixoazc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3viimshis.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xmzhbhif.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3plpjolsp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dfdmtcmq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hzzjunak.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zqxnczie.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ihtorfcn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3etgfevrl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jfnvznsk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bqwbohhl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3psqhpwqw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kchijzkr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kjdywibu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rgkdtxvn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zigcxlqp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqkcrzaj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lionwxdb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sebgnqne.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ouitftgb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hcanhbhk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jzjfbbxm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bfanptpc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xjmgxhvj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bxxvrujr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kagxulsw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cncjldfd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dirsdjcp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3arwvfiqy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxbqltyf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ynavyqdx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cpvjstzu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jgflvdjm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xwxruenj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tyvjbfzj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ihmohlkp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yrdrtzuu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wydluuvh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kcmyywad.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dvllvsjd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wbhrmbnu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3penrbnjp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3szlogtww.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nmwbqbws.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzxqkker.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dychqspk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3trkjzopy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3piqbalxj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wuoqsqnq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3egrjobqo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hxapkrxq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3odlhudee.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ueekhogi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kmvtiuky.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nvbacdbo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rbmqrbgu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tkgpyugu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bilmijtn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3xycftfmv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zcyqgudo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pkkzeasa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gyahzrcc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ogprgvxc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mzodqobs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fsknijta.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zquhoumg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tyxxrxlk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ocxsedev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qneaeekm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uhwxccak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwfbdsho.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3arrcoopr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bdxqwpyf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xdhjxmaq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xyaqewub.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3brrsyuxz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fajlezcg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mzhiytxx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3djkobgwo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3naxrumzk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gpoqqwre.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jxrkhfbu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rxrooxxi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rzknubjt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jwbsgfni.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3urbrrfrm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bdwecyyp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3girbtcnr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ojouiiko.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3acxrqjvr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3njykfgfp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vnzitcin.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nolwljsd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vrlfucux.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxapsjh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3iazdcapp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pargmlef.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hwonejtg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3itpnaglx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zsyoulhb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ldifbmye.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3exmyjmox.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bcdayvuu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tyyvjevi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gpchbizp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sqvhycpp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3twipqvkk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cnhmvuoz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dwqmjtxu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3arkkatyo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vrebgnkj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pboeezip.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rqbsevmb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tazzvgnc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rfdpkane.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vabwuvyg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hcnowgod.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mxygifef.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vesiomks.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3usofjhqx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vpmwimna.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lgylxuvv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rwzblkok.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3abbrgyee.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3stbnrosh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fcagvqoe.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3uiojjxie.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3smmnfyrq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lblikolz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zjpvqxzs.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3acjgzjga.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xaiuiyqh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xknrddwy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vdlkrvhy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3euuzigmf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3expasmtr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pozhuqmr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ynwkemnu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3udtwoaiu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nxlefarq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3unggqymu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kdkjstkv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qmautkwt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hgtuaqrp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jsmyvlqp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oqwqyrrt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gfijmuhg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ymbegcty.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mnuxxnzi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3thgwdtpg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vcpjdhtc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mpsniarm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3glekingm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yuaycyqc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cpjwesti.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mdbolssn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xjuwqjif.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3syrlyumk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljtqegrh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wwaywggq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwuqizb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xgruicgv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxucgjsa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xkexhbue.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsvozzhg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gkkzhhlw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qdiumrpv.html


<!-- 参考信息 -->