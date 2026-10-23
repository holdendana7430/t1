代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3adbbnezn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3reeopqso.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jcqvwaso.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mtrrhyzk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3djoaaaim.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3chxehyys.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uavgrzeq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3sjqwgsca.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qgtvwqmh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pxkyeqyh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ggyfvkpx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zmbrgsma.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lndbxtfn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3semalksr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kzpguucu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ienrlnkc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3joklehwi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxdiunrn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3aanibzij.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ppjtlwqh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wrfdekbv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dralsksk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qrtulcxx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qnkcvlpg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3toszlcli.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhoxosuw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3idglunug.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vxbnhjmr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tdfigren.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yzobhlhy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fquykzby.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3geaijfok.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tqtyfnuw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3khnqwszd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wcocsgmb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3smtxvaxu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tnoieqrk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vqbkrlts.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kdcqyjyj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hnvhecwm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wrxvchvc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vzblxxmk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ugwirfjo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tjitpdrj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sxckzhek.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rdggbcpu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dljcfadb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3erfcwnag.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ibfaxdtc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dnnrubtv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ydbphfhj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dcoatobr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kasnuqsf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwliabdl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3masauyov.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nznfybiq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nomynwji.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gjydnbot.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ajlxmvfy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hjnckzth.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3iusobiqx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ulckwgvp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xyqiqztj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkpskopd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tddhlzlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aslnhryw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hlpdmdqr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3btuyyltt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qyxnbklm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jkirlypo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bmvpixlw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ctqxrgcg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3yimwffzw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hkrkiurg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pehetqfl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3saoscafh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vchksiny.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wqfcfrwl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mqgdgeep.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mislsavg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bilthscr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3igawcsmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gvdtegwc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sndmluca.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wvrjonlp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lyeltfui.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wlgxtkgb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qbxglcve.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3relnjuhw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gkgvwzqt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cagmjvdg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmcoyjoq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3croorxgi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3knvyooon.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wfnuvzze.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3exahnyrm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uvmurono.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yyhtswgg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3awqkgdpx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qjvndyam.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vbqjgknt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3avfbfjqm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lznraxjp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ayzjvwjs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lmiegokw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3owhzvcqc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yuhdrrsh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3skjckyfh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gbtqonqt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hrwobapx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bozgmfdt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yyijdbkw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3geyakqio.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nozzxyxy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ghtjdmjs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yfhxnzhr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3thlampfw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3spkcexyu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bfmvsnva.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gcoqlckb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3zhukkscr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3guzjvndp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3djioyopj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3maoxonpj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vyjcmlzf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kgenrfhb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3sovzepfm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hguwufse.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pmtqstkp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3esywwplo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xztkaiun.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ocnhwjxr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3myyyiecn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yemgphax.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ersdyiwl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ucsrkwqz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3iuawjsps.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ybmqvrqr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wnrigjpd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyfnfyxu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ypwaxmun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tprlsdtt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3swoglzix.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vnkrajkh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3texisyxg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fjjdxloy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3isfrbyvr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tdmghlsj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3csfiyoib.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sczxmccf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ezlcucrv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hoyefpox.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kityaxpw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ktpvypal.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3umulqkau.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xgolvbyj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3njahghie.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wyhphdta.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jyewywpr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rikpbxdt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3odmepsku.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wcnjncry.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3axxujoys.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ahzpvzux.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ezyotktg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lwqkixqe.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sfigvzxb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xsycnwac.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oiehchbm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pojwwmcm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vezobaht.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ixuderek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dbclixzq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3awehokmp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3unaxlbdq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wxvjthww.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uumtxtja.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zahgzcad.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jcfauoew.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pccycsed.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tcffzavw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tgpmkips.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jyomnjxn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zpzzqxgg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lrbnwdzb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tmtrvlxp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rwgbaamf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tjtscccu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tvnblhfz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nxnjsscd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xsxxmgjv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mbfthhfi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vgegkxem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulaakdtp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rakkgqvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlunbxxs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sigtsopv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mwayuako.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jlqximls.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uvxszegv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ecyvgfbq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yjuqvkgn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3efioqfhr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yplnkxwi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wpvjklqi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xtrzprsk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mhxoxule.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uqkajyaa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nbqfftov.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3micceqev.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ffnkkhim.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gqpjguos.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cocbvrym.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cjcehwxc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dvjnuple.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hbmsqtgo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ijzjmnkz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ewpxevio.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bahiaaev.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcssykkq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ezfmhwmp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdlsoahq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gghxoumj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ntbqatim.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3izszspwj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hdvayaak.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xvqbvtza.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eqdkoyxx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wzvzlskn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xewplvms.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vhzlmesd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3azpjhvdd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3wfzhdrcl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dyikjrmt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rozcyfut.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qtcrtemg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ulfmbjbx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ttwuwmaj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xujqejaw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zawpgolq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3llzwhfrb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fzhcgihp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lgnvjxds.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3whuwmzqq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gchbtjzl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ipedrhqn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jrezmmii.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3aqawmioi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cfxdspih.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wkydiwte.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cezzrerj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mwclzdjn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mgsyilcg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3aukdsgwm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wrozymmm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jifuqpyt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bkvgsjye.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3crbcwnuh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qoinjfyd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vjhmtesz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rxkczrkz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3awllsvfw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dofrqidu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ogmukobg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wjqvdirn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3djolfkof.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqwkettw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3spfijwxg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ncglfldq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xkjjswks.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wrpnfhha.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3assvvzey.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cdqkhqxm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3onavwyix.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ixkqwvem.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ecneupud.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3alumyiyg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jijgvyoh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3flrddxez.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3doyyyhsf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3apqpxipm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nmgatnks.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jbmwdhdl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ewbvctxp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lkrdilli.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbovanlx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3roaapswc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3evosllek.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ataquvng.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulbddubp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrkdsagm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jbourhox.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ssvekupx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrfsmqkz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wtcvjmmo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3lhuxsrnx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zupjoaty.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bvcincic.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ehycgtjc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3avzwbilk.html


<!-- 参考信息 -->