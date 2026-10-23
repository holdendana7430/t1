代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3txmwyagj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3opulyyyq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3outoizyv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fngsfqvl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nahjeolk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mswozkyx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cxtacyiz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jqnhfxdc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mqtzwggz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3crzcwhir.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zgjuuwbt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zyixdjuy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dnzdvmvy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wygutufk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3nwojjoui.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3efzkxvqi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kywbmrpc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgccvfyq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ygwsohrd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3woiswyit.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kdtiijod.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jeymhizk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vfggiixm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sxxduoif.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iqjxaosg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pawovwox.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nnjcqykk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gqsdlfdz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vpiscxpz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wjuiyfrt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bfdcyjcv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3boxoyhok.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dfnskaba.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xjybdjgu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ioqhvysj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cpbnhycr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ixeirsnf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tfzkbrne.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vbsxntkf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jpvnouha.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3flsrhvlt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yxqobbnv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3haozrykc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rcrzdtdm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gmmdllqo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jveuwxuv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdnefven.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zthgiidg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cuxnxpwk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wooduhxh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kbzhspnb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oteaytgp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mrnydcpu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jzwzqlte.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3veubscxc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ypxcazgt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3stmqsnlp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3msucdmdh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cqzryicg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jrauymyq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pzwyayru.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cmtcarok.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3icmiragf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htmivkim.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jirevxqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htrmcdka.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qnbfiiil.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wcchwtst.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zovljkzl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dbpgismc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yfkytowe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yjofubad.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ypkzhhpn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3idihwuli.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bnlmwhcn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pcjzyiic.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbajefxs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bzqqqfed.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ivqecjdr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vejdljii.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3svholshy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eddotfqw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3quqzuqkh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hvwexfnf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lvdtpgzb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dfbrpdhk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3uxpqkvfj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fbqgnbvk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jdbixyjj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ypehkkju.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jclkyxyq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hoefefjf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fqpnwkvj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qmwwqyji.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uyuqknxq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wlszfqur.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3alghyjmj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sekkobtb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3siafferl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dtjncvjq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqmknpfl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uosuvbxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fmslfwiy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qzipkpae.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ouhtjmgh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3krxmzvqa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3htdznmrk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kjvfuvzj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jltcuwkh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kvucxekn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tkjqckul.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wbcguoyr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3poaiinsc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tsfezyzl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vbqrvasf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cdbsbcwt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3whlknogy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oxpqfhxb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nzwcjhcr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rsqpfrat.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yuzkeskr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qbknpias.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lzytmjah.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xiruaupt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3srdrjukh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmicmswx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zanildbt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gfwjmwni.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xfrqzdjp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dltpsdby.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jfevsima.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wzzjeefd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tfqebqzc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tukdjzbi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3glymocsp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xeonygxt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qmlxagnb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lbcponmf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3icrfzgjr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3aixvnlfx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zonzfydh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mccelrkv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mscsacse.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ycplfjkh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3coxeoytg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufqdzxjn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3oirobysy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3emaycjtq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mfzifccv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lasypobf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wafwbdyu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3nsaotgyt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ckltycyy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nneatidl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzrtwzop.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ibuapshh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3gyxifbge.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cufjwwew.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gykxwgwi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3addxsxps.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3iisevren.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qsxiwwlk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rgtpcerp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hyjqzdtd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qilzboby.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtrweyke.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mnwtzsyc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wjmmyune.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqcvyou.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekyfzvck.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lwegrbrz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3elrcshuz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oosfkdwl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jqqorcqm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xmtobuwo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mydzjkvz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bklgykqh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vrrkkveb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dsqbzjhn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dxnrqhox.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cjamtfmz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hpcorven.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3booxwhpt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hxgtshcy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xvxwwyly.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fhokdqju.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gpahkmwc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jxvcofzb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tpkuoiqq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3slrheser.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lsjgajmk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uyinrwxu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3skhfxgkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqbnjodd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fxlyxqah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glaqgzqx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lguyufcw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3elimxmbv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hbfcdkzp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pchgyodw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kejsxudz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dgcatgbx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hzdnbcez.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kvbccmzj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qilerxug.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3biqfsrgi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bucwojnv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bcwbrxge.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qmpfnhhz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jwvxsddk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3suvckxkl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kkyorymb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hbftgkic.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qvwlmtti.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aposcbpy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sehevvto.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3shhznztj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bynfprzz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qyfxwxnt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzowanrx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xkcjkefn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3buwcribi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ywzeifsx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3okijviak.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3oypqrvbb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rqnctobv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ofgjbkdd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gsjstscd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rubhhrut.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nzgxuobq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lkewikst.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wzudavdl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uurcpeuh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgdwxdi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qsozuctf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uheirvmd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3akqupzwy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3tgeonpnq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tynkivbu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dzceqxrt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxozokwu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ailxtqtp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uhexpker.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yghudmas.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3akmsdwxz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kxbvrcvk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ffayermw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3znaqbnft.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bycrribc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3unxaxbms.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3volsaniv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3thbeynyc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3detwldfr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dpjmbowd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3yepiynnr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lrenlgfs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ggjxafat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wnkptyug.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3adakjxid.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pntqbsvx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gatuuezs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3skzvuvmv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ktorxubj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vvspgajo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yqlvykml.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3slhdxded.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpaidhuh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3sbeexmnn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dlrwldpx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qnbtcsce.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fahkrisb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lvzsojma.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ggtowfsk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tbopohao.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ihudiqzq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tlxyejcs.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lbvkbwro.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3chtcpujr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3slukbspk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wymuygtc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rxzounvj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qnzixowa.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ujbzcikb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3secwrbns.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vukwvrzk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihnzoisl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gvtkxumy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pladaiia.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vmnnhdzd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ppuxnsct.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3loiwsliw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yfkaousq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nokssdop.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cprdtfak.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzepxnrj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xvtlwnia.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzmcstpc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uelxjukv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hhiglvfa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmdlidoy.html


<!-- 参考信息 -->