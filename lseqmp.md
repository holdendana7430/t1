代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qczvatyi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ynnfglyb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eergcwev.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rzymkwym.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ocxxbiev.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qkqdijgq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rnkonrma.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fshtqbhq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sxylwjei.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wcyyetts.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yjmjkhoy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rncaafdv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rclqvjkw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddaxxxbu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kdjehbds.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3olgqpiby.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vceseopx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3idfikgxy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mbrvqdvb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3spyulybx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lviastxe.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3pwbxvhqd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wceizwhh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mbjqhjdi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dbbqnday.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gzhrbezw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mznpigst.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bqtwyuvu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3alpvnbpw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dwgonxrn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tchjbwni.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rjcejvik.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3oljsdwyq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fdsduojy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3taukxfsa.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gxsqtckx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dmdwtgqc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nyqibque.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hsifbnxu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3aensmbia.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hkoyzmjt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vafbjrqp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fyitohga.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ocrlcjzg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hfllsjei.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lsabqpwj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3owpqviho.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ffezjbxi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3adwhaugc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mlitleeg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zyssenbh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vstoqbqg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rbzcbdxl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qhrqvriz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pcibnjtg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tkxttwrp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jqtqfhjp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcnlwpcl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pzallffa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mxebluea.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hohegclr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kkjhtmgy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jmlxmnvf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fqippycl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rtbhhnkj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3anxzipzf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hnolhbwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtvosuau.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zurnlwal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjtzmdcl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qaxsozai.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3erfpvokt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dftdkmaa.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3grzrscfl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3csgqfykf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3smlhwnbn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jvgoygis.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3arrgbkyx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vnwdxkng.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3awazhfxf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cqlyqypv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qiabddwq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qafvxutv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ylegljcg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tgfxlbad.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bgtvwtyi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sdtvtsbl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3klmpsiou.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gimlbtpz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cacectjl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sbgvbkwv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3itlshvys.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mgzyffaz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ijwympwa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jxargrww.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbvrzogu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3beuapvje.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ymfsaqqa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rtkcblhm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qbnedzxv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nfjjcpft.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rclfrbrj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qgcwwcqe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hqnrxerc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3sxqzlzzj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nlaxoddl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vnbfthyv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dyqvmfbr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jzfmvnjh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wvljzonv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dhitardu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gnkjmplr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3avvjqlip.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3msdkghci.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fetmbsqg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uwkvkpkv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uoontvrs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ugptamer.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3obkrookh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3miwvbmnc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3lhmqnuad.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nsrlubdp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nfbzxrfi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yibcesqr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ghmhzvtl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gpsldobz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fkwhcagp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xpsxhxkc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3yypfbgzl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qarmeuaj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ievjhlfm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ssmrexof.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3erzumysj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vktojadt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hggfmnmu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vbgsfqop.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dludthgy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbaerbjz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3pqolzeot.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nwlqecgg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qgxggfjw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3crwlwnjw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fuuamxhw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3dziiemfl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ldltxuei.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ejjaemnc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3iancidqg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eyqgbhtf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ahcfengo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wybdodfb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ghbwuixf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tvzsdkep.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dcueyacd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dszxodgs.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zhtqfyob.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fcfyoakt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3oquegmqo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ewbzqipq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ciwzmkji.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3bcxhekei.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cxxkyjjh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jnayczwa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vilerpzj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pngehmgp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ooanusri.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hglrbezp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wjjgqhvi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnggfvwv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3uuehkapi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nfpngswb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iigwebzl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uqvdhehl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3etdapscq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pjcrolzf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vfvivoqz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ffoybefs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tvojdchd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mtbnoorx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kwoachsg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kthpqwho.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrtcszs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yevdvbyv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yrgwyuoe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nizqmfjo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hjinmbvy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xldznrvc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wwatzdpe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3yeapaita.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dmdwzxkj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3otumkqtw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mgbwdyxw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bjmkrznp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3udsqpkim.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bjhkddiu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kwrskkwr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aipfzmxv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bgcrujmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlmabkqw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3levhauju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbneahrq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zvjbtmpd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tqbrprhe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3latslqrs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3silzbjzi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3szbxvpqw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mofijzqc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vsfeqqwk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3glvqwtpi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3enmtmkjz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dswjtdxd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lmnhmdvw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fawlnsnn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ajthcidj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jcqtqved.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ledpzpgg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ulbkdqxj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3crxgscjq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3twgskmpi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bfzfpdky.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xrrogwxi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rcdbcxrh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jxykxjug.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zcdvbsrd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cxpgnweo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gqaqklnh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3udlhebyn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dytpulvk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mcezxnxw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qrvzcvjq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nmnslppg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yuynpfjp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fcvxpemd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3poqdfasi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ofpvylbm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qvhuqsug.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ecpivlws.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jvgfwjcm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fznbefrq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rkiwfdvj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eygxxsyo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oevbudlu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bokjagzr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qkxxvnuw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iaykrnfe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3onzetenj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3aysnyvha.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cthwmwsf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gzldggtd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hsbrbutn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3orkpvfqw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3isshoemy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kxtdermp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3amezxrab.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nduppdvd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aomymbgy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vcoafrhi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3haofjrgf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bpaxqhcg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3aizvyaui.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3izdvvrac.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yiqhorfe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sqwxsuty.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jfjlpagc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dkezbqom.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ouuuedjm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hbjmbcvd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mujbjtqs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xclhoyqj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jnnhnhma.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3knwauqrq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qiwcbubg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ligojjou.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rczwsnwu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwthmu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aiamkkyi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3osttqyfg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3msmkavcg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yafjrgfh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mrdehyys.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cmvfpgua.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mvlacmwd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3plrgcazq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tgifeiwz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cnnapzgb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gtsimsja.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fapaoyai.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3irnnucst.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iibzuvxw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wxvihovx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3plangwyu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jfwqncdd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3odycpfwd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ukxklfwe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jhhtpjcw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3epcsaoeq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dsavidku.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dabjpadv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bnvarffl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxtnodgi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zotyamxj.html


<!-- 参考信息 -->