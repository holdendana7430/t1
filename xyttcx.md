代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zzgwotwa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3agvelflt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lpooxklz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hjjouett.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xedrsuqc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3idtgnvzr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vvfngtsq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3noajndph.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rnnmhfzk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3yrhveagp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sdjhpmwe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wbplbgut.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nclbvlke.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3anrujama.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kjdzonmh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rnuuzxmj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3divoqavd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3goklnunt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xbbbkcij.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ppaiblgw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dxwusbtf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qgpauxac.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ugxfjkbg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tkmfvxix.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3aucllcws.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rbqeleav.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vxapffkn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3owqpbplt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xrkydjva.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kebxoxcw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ezaselam.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3anqgwvzv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3yhxdtbmz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3iormovwg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3masraiot.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sfhqgyea.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kpmipomj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vgjhjcau.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3huqllfzg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3cpdoolrg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nkszfsyy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vxbfghll.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gjtrakwz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qiyctqpz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kdwtjbqy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3umvzuemb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iouwiafm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wxphfcyp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jnngxhyx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nbxoznis.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bhgmxtfz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xnhvnrwb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3srnisrty.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gjkggnwf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pqwychyk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3caitsjjd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3obxoprfw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3flklsrra.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3uvvdlxln.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fzcwobka.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pfkogzdb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3grziniwm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qgepevxl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vvynnlbe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3umyzbzbj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qcfntsqc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zwbimrkp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3eszixffp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dmhccnod.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cwmyacht.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3upwguvpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzekhdhn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3iacsekve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdxtuosj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zftgzknd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ewythivk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tqdqekqz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3homwtozz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vuwjhaen.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tvqvpfiw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3azzmnrfg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jniqtyit.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cjvlmgxc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mqkasbbu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3nbzctzew.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3unqooeyl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cucbuvnq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jcqcuhpi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mqqihlrd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pkbmedax.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xcfeglbl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dhjctprc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kpdsnelu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3edhbpnuc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3gdczdkpj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xroykjkk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qotugbwv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yuslieyu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gxyddvrr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lntifdls.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mnwrrwhr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nhrvgjko.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gfdorykf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zfqgqqug.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uzefyyfp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tbytvoee.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ytvnyhqy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nlbmqbhe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xvgnglom.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nrghgdbf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dujdvkqw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vsxeegqc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfykux.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fhsgyuxj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3atdginqn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3osgkpeex.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3etreuhzx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yzlprrrn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3raqnzgjz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hztvivnu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jnwtxkpk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zmwtsyiw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3xlcivxvo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zbwnvmej.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gvjidejy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dhekqomq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lqohvjiw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dbfvceas.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uzqakkqu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3udbngeft.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nserdzli.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3efklktyv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lusqmebd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lccelwvy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kysuokzp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mectzbgb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wpigumtk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ezbazfvx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xdtpxotd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cfxctayq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wdpvofxw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agzlrgsz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxveftcs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3aowfgqrs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ptqbachs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lpuuxhvp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rlooqdzi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mwdgwrub.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hiqxzxjo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rrihyeum.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uhwegoqg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mgvcojdi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uidlyvhv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cgiofnvm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hxsquist.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xzlihtxw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ifphgnnm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3twtoxgvi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pscvmfhk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fmawtqxq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqnnsojd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ootmvxqh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsfdhjuu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rkdbaqkb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kxztulvm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3peyotlmi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zjnidkxi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3twhtatvo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jvrhvdmw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3aadwspdm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3huakwmjc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlognogy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mktfskff.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nkveyilc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qcbmpqrg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rommvwtb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cenmvexa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bncypfne.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ozkggfbl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3uoorakbb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aiklqedz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3massxslh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eicderku.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iklvpbnu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3yapsnhhh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3htlrzomo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rpshjmte.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lvadmnwd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uqsfghqx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zqdlvgpi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3oenhfqtj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lwtrzops.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rzzbcntf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qkqqgfcb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3rybyzbkh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lemqlkda.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qprtnflc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lyhvnvsw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dxpwqqay.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pyjtzduz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lwkejzgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvlpgeax.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sejjquij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bczopokl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gtwuvciz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tazbbccq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fieormuc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rcxxhzok.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3slvimowr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qkrgrdot.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dxunukku.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bkvntvzh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ojfbzeqy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nqhswvel.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vrepehpa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3blfkigbx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgaghxps.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ltplnttr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dcswsjfh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qhejiftu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ywiomjmm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bkfudkbz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dwonvllp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kmpljmfs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3itmrxcxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3acxmeoja.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uzecaldo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yamozfal.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oqxxkucj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kfftrust.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkhzxhph.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3irybijvd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kvmhcmtt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3esjzkbnk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ydnzahpf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pqnlsytn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yyueivcl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iaijicbi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ylddpbgd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yrrctvxe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gyknfywt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ssysmdjp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bifkijap.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jluedxvx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dyrwkulb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cayvkgfd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3njhbewqu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3byvwspfh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ubarvnkz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ecjnmcjk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3knqeyqmb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yjunrrsk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kfogqbxm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hjgmrell.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fgrrflhu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3emvfdabu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ahutppzu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xapeqack.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3koyzysis.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3fakwpubq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3coqfrnuj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fujycxgx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3slprnlpv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vfceaote.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ehxxtdjs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3utthrntd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nfnidgoj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3skacyoeu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pwpxlxuc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dnbmohgj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qzrclbml.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bmrifoah.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sxkdxcpw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bgisaywt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynqyrjcc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zcnieziw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jqxkdlyk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ntvbhipy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mhiyligt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3efoepmuz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fqdhwchy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ucsxvzqp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vslfxwij.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bybgvqex.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jatlgfhq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kamxorul.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wrqnvblv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mzqccmdo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3memrqxrh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yutrpzhn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zhphkeut.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rhyxszmm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3irdexias.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uwdnzutd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jqliwroe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fsaccpya.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3iuvlozst.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqguercc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rmhfgcis.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wgxmlvoi.html


<!-- 参考信息 -->