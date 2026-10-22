代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dznzdrcq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bqnlfpbh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sgsuoawr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uxxlbjjz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xmjswqiu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rmcqdqvn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jcejgcqh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2heunvpvz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2iuxpqltf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lndihnpr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cwlvyjru.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2eiydwnxp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rzbszwyl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqdpqumk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xpwlfbnt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kmecqyxu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vlrkfqjm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2juufvuob.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lvzwldpy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qupdbtpu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2utrjvifo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2olhsxnes.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cptcfief.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xvnemodc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zeyyplag.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fvbfhpby.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2sqgfkciq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uqzfigwg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nhdcerlq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhbvlfgg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ujiqujer.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ossyairc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2odgukldg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lkhhapiu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2egxrzvde.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2pubnvldu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2iohrsoap.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fvjiprav.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kkuhtcxm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ejmjjomd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xcgyzaqb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dkesddxi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgjfudbk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ypknclie.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2iuexzzck.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ylmegepd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2leaphxwr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2djjmuywh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dakojapf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nftgeeho.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mujxhtlp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wqtwosdq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cjhphktu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mtwofehn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eklelhdv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kfkrgxyf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2htboubcf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2slyhpqwv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aarodlkx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2skpcmooo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lerlpasi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fvyejmpg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qqulxtdn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2iceujgky.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dlczwamg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ifdeadds.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hmouxaja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czvqkseo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2avzmohhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymjubxlq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nmhrzgrz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2emfbxoxb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljlvxycp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fckqkpft.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bzdigrtz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2llujrxnn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ltmfazba.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kuyfpihd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ymlxwyjj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2razqvgnu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gvbasrjg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tasoymkp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lcqjhorn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lmrlpaxe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fffmxvcq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2oymtzqiy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2mkpcvwoj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qhpspgzq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ktkirnqp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2prpbmvme.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dejdogxh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jzjnsmvz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kmmwxvqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2thcvljdk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rwvvmlyc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtzhuwey.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mbqirmfa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2svkyhkus.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rtlmdlto.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ttgxrrfu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2durvfdkw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pvvzcxac.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xzjhstqq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qvdhazuw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dxdukfmo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kzynzlpy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2nnkgptxy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fjsyobob.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bpxdxjed.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2iibjxgnp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fzgvdnpf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gbtsiibn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bjmqnopo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pywkivtz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dmgwabcg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2iugctlzy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ceayohkk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2shtxvmlu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mufkkfbd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ibzvdkwn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tcmupbnv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fxjuodri.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bpvfzudm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ffrpzgza.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vquvnonn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gfoeeepy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2diglflmk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnbwbqsd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ireelodx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wrtxfgqj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wtpbaivm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2chskgtrk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qrjadlgz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zicslyuq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kycrxznt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xdppkvlr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uqfefibu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojfqammz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vecydkkg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2touwvznn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ynzlytnx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hjazsvgz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rbqkhtss.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pkswzouk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wivvflaj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cyqavbbd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wusxtjce.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfkxfjrl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2keafejoi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mavrvqwt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zstzpwto.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2shiafjdd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2plhialpg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2volpqksr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2akrrokar.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mfulpvuw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2aweqcava.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zuyfiqzk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuhclwwb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2njbhnqap.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2guwnucqv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ipumbamv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tjimauzr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vkxiuodg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2shmewajv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2krmmplxn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lrukyhdy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjhuvhsk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tcmkpvck.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2roilbnhs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cacmbazk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hiuziuhn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hucrzpyu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jeeljpwj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rpabrwba.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bxbmawhs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zyyqkznq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2abxwdfgj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qbgpgxfa.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xjtrajof.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2utsuirkw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pwqpulgh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2zlzzukwf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2bafwwmcy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hrbnvbib.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vnvezryi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zyevkaoc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ndxesbks.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2joabvblo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2thuvlraw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dolvgift.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jxlggmix.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gezzcopx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rfibzlkd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yozkvoqd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2smbibsbx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gyirtqys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfdvvobh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hmvqkale.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcgvgzum.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vqrlaldz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hgcwfoxd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fdgndwet.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jitfoazc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jlbktllm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2udarhnyl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zhsrctts.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xjnlumrg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kjwtbxzj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2meqetnsv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gmhmmyzn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2skzxgzcc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bifvwdgh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iegtqygm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hbtbxcxc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lcijerro.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rdbtpmpf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2romgeqly.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gfnsruav.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2azhcefco.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2higwbibr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jirgoong.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hhclemyx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2svpiwugy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sdswezrd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvokvtfa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bzyauvqm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oocqgdcq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hrhqxzyy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhxiunj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2junbfahe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lsgrkfoi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ytlnfiuj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gpvjvzsu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gehupsjy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ubkelwtn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2utpajdzs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2koaxhzqe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nstjmqfq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mdabiehz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hhyecbrg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rquvgzuc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hupclmqu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2muitcmzv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vimjbglr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2gyifpcnt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ndkhvffk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zymttsmf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pyzpsxad.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fvqimcus.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wqdypyep.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bwsoipii.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gewenkun.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vqemqdry.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2udqghajy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ezzlsiio.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rmtevhvf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2simtvucy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2atphqmes.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qivfobbx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nvcxjcfp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wnrmycqd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dbzjmmzm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kltrjkgs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lrrnurno.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2prbbysep.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nbhnulxd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2stwsollw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pkwveyby.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqupoawi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqcwainj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2latusyjp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2scnolfmi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2bpzqvuzh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xeeitjft.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sevezktt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2abrhmbeg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dxhdinwv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2luufrllu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dqsinxvv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pfxeadxx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2omszrrjf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fhtmgdsn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2abdhvyzn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xwilljmu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vcudoumg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bzjknejs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hjzunfby.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2asueveki.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkrdvqzg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ymkblhak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgqwooaq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2lajwrvwd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2emlsnrpm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2muuvdfeh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lxxygflj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rgmnvxzh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2akxurivf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2atorerzg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2roumettm.html


<!-- 参考信息 -->