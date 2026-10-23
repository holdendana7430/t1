代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qzqhibzp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zdfctogt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nzwzrola.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3buvmbafl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nqnspidi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uihlqaeu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dfjeziuu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kwoslfty.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3uffydpjo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wikcbflr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lpoobjgt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3uwurykmh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rlzkqfbo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjigpfdg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xasuhilq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ovsjjuyy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vvsulsmy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jngebjbx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3akgyekoo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3toiqoebg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bbdkihpz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uksnhvjy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nxxsseho.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dbgxwzrs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3furaqmox.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mwjnxzrh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pqlblpbe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zjyepivx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xcaxixzz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mcbqqnzl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nebdulgk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nlbsjjpt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lfywbtus.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bmdcuuaj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lygrgzkk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gqgnamys.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3akimkwiw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ksnayrwf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hwrxzaxx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hmjxuplz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3uxawahnk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iufbvnvh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ccssrbtp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rdrgthzs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3txavuojc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dfddxikn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mwkxsiep.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkioqmio.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3yedcurdd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3usvddqkv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jidfiqty.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3sgljyefw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3iwraxegv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3helcpcur.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ujcjzwbr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3flqlmhvj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sxqeysos.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3woliorwo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3duddtusm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apgbwaaw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ddepesav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fupjtpir.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ucnfvawg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3omhzqjca.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3quweqggd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3maggeytk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3juojayrn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3asfwvwip.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tnprfttt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zkrcpbya.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3oxmwbafo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xchgxhmw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tfiyddwk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3coirkspb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3sckuhado.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ndpscpug.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wcrhzaca.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3yfsadcnm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wevytdpl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3anwikmfx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3havdhtmm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pnxkpdkt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wubbxwfm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwfsfaxl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hsujmxms.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3twgxxmdr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3atggpwze.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wxdvkyim.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3phwoqocb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mmpgkohm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3johkjwdx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zdgaydch.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qsrstpgg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qxaseuyt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nohtrmsf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jtnzaotd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vnplpblc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mvqnkveh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ybwkwvmj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hhemirgi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rympsbxz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dqtqykga.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fghaxyum.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mcjrrljg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rtyacaho.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rcohxqkj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dwncmolp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qxerjotp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qefdhuje.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ncgyhytz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3alnabbrv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dmnrgudw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tveyscwb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zczswqam.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bykddswk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tgcitsgn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xxtjlyzw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gcpbqtfx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bcwszodj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3sglcnruw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ekuvxbpk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ygyscclx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gwymrlyj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ybipexyj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tbreqjww.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3llzgmyep.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jxbpjewc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rxmwrboi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wmlcxghh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3biycbokg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3okbqfupw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mvluglpg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wznzhujl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xlrdaanc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pyhjwszg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3owlmisjk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qyktdvnx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gizivxwy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uvdwjnqz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3quuraqtg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3klunqnae.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wnabqfwj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uroorjos.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hxdwvsrm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yzqhvndq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mtgutehu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dbklsysg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3dydqanzq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qciuexzq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rfktvxwv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vknlhfww.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mkzqmnij.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cofcjwfq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jlklqsok.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vzzjfvst.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rmsbjbyw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mxzddnha.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nwseeqvy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3iblsrxgk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cnjlxgza.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hpxiigql.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3omgytgxg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozqcilnn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nqdqyddd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jotxrrra.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghvvlzkd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rhhtyhok.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gqgvmezo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cpnvstaf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugxaadsv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rkrqhrzu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wogkvblb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekghoxnh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hwdqsztq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gpsinwsy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3oixtvnhw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tbfvcqmh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3krxyzkae.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjiucfqx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wbmnulyp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3eacptjhi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3juqobogs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3egwrrfkm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pxmvewcp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvurtzvr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3xrkhmtmg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3urdndjlx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lngeuqpn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vtbukqyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihpjyhbx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3stokbbvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkcxmmln.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yjoztfca.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgdnpuy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3snzbzxdr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vngrluft.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jtsstuoh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vowrmdto.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nbfuskyr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xcjiwrxd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aqvzffpa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mhygowwb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3joqvkvvb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztchwskw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wctbyohs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xghgghfw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ajvuyvxm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aylqapxu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ooowvymp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3madobcmi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtjctgxc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ezanzzgf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qxgrmqzl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kmdmzpuj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rbrrypph.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pcrmwnat.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xdhmpdlq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqqbzozq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3tccmwjqm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3epwxyvuh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kpggtttq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bxwiswfc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nygoxtva.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bhfczxxm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lyztanpm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3juojeufg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hwcltglw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zwbwxtgz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vpoblknc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vdmwrjat.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ayjbnzwo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vsonlxnz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bhgmfpsm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zhpskahy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xecfteqy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pgvneykf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtfbxnhy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3drphdyvg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3nagqbfro.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lhjafkxo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3icgtygrr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yufpabgr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mmiqdwpy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xydqhttd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3miruoatu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zfkmbfxo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zgpkdbas.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hwabinob.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rmwdsmcq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rpqvgsoj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tmquslrr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3asefzuiv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vtsnrfqe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dncvshoe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dhobktvx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3chlunbdm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gvhlwpjj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cummrvev.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hmjgdwvd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bcfxyygk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nrhggavs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3osrrqfyf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3okjeffdc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bsjnuhml.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ifmhnjdi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zcpdwfgm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lrvszyss.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3bgdmtuvc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3miejrnbi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ogkwzsrg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hytzbwxj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bobgfvvx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jecnlqbu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gwrdzsth.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kgeysldo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hmphkoob.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fssbyphe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3exaxltvj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3yvzzqsgc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ipchvadi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qiewyeiw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3htfubbds.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ctpiuovb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nzqppuzs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lupvobaq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3btuqnilw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hyzacxgw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rtzckzjm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gwgqfeff.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghmkuhrm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3grlflazj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vpxizlnr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3paaldgmd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3inrwkhyq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wxfjwqiv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zuqadewe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxzfcbwr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wltaawzx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bnzcopxb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pirkmdoy.html


<!-- 参考信息 -->