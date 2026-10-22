代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mjethuxd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vwcloffl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2uvsejgdl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2axboxgqd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fubkdqpl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2roqxujcr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2stedcrpc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2skelzmhy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2okzhhdha.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2heaiqrhl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lldnyhhc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2iujcbaov.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cghkonrc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mtisvmsk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2emxdmeab.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wfpzltnv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2grtcpnua.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zhkkhxkh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wowmyhfu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ckrvjfmh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jfryojwx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2aihnslff.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qrehthqk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gpwzchky.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2oqkflbll.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tijiwcyj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lpxiezgy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2awaniuoa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2pcgbhwsp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pyjdpcyr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uosenwvr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2miwfgzhe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dvrbssdy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2buwkxjjt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bgzzrpwp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wnymkjew.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dfbsjdul.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqoixqqt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qqxikpxy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ztscvmsv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jbbwbqsa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bupiigvj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kwzfcboq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pxtblzns.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ddxsrzai.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pimmmyuq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pdthhtwq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2rviuhilh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2setublyw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2freglybt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjbucdl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ukuqcurm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ryawuxpj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rrwrrvck.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pibymyvn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vrvtrybd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2szeohduz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nuulzsgw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bjfgjlhp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2exudxjit.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kotnoxgc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nqfzyzdd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jloymrrj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ocxxhxyh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zshidcoe.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vskmmnwd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bsansdft.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mrxdwbnu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ntssuluu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ztahqrux.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dtwsetgd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2umybmsln.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2eqrjpdge.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfbvdqxv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cpqurcen.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2handvjel.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2kzodnrxq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ydnsockw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fjryszls.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wluuxvln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ucvhdbgs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nurehmpm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yrhgradi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvchpeoi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2msfjyplm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzjzcics.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dbkrywps.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ubitzgqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ateeyzfc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fzjoubhh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zkkudppj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pqjnoqpp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uqlfhaga.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fxufsjjp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2swoknglp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gysozaqm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2slbgskhm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zyvvcbfi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mgiwfbzi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2etxhxgdy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bitefykd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2marontdv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fvgqmcyj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rhzqztaa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hwusjckv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fhvsqclc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ougpbabs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cgecazrz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hntiosdf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2orsdgrge.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2owvnchas.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hyyxxxbo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tgsjttzc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ricdfevj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cksltybm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dgasqtur.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fryprfoi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hbdhuxwd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dinvdzvv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vqafnixo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sbnhzttp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gytczcva.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pdlowpve.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2stuuwgep.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gagrjqxe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjkfckwk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yoquiszg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2favqgxvu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ibkqphvh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ubbwakcv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xjoobxqp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ycxnkbnc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lmztbafj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2norxeuol.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dcpdiszs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tkzzjigi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nrclihyc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jnawgdzx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qknewhkf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2igejjwya.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2nvlypqcq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2oeihesrc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zgvaqhcz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ddhzbixt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qhmenetd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qguocjte.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ttpaamei.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gqrufdkf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2meezponv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2niitlrso.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2querkups.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hwuoagnb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tzhfmeer.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiffifek.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qywoddtb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2pdrohhdh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2arqoluup.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ztjtxece.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fypbehtq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lepwshnr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bojtxfrd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jjedougu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bvakjynz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdsbiwxr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2blhmdmqh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cbdqroxb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yqjxpmtq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cjizsrom.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2abummotr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tgkspqdo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fvrzinnd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ogxacvqj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fedxntxz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjpqgdvx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2iozhyult.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2oziqjtuo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yzbbzkhg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpmrrap.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2eunkupep.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwndgutl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2flyczinf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2skihojcj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zucaniio.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ordmpxgi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzjdvtwk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozlayakz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwfdncfo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ebnlisln.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jpmzbrfh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2obcsuecv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ngxpitnp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wmoslyok.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jbpeqptj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kyezqwsj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qlmbdfyx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ankghlcy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yipfvcii.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qmjzahqi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zvsvwxka.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2nglapjho.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2omvbklfw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2aylerqay.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2edbrdcpn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ijdumyat.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2keyehnxx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fmczhmir.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rtkeovhh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2edmfgfac.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kwofprav.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hflelpva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cahwlzdw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2suvfhvsh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2obwezqgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsrgmqia.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2eltilzhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajgscmlh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bchprhtd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sskymwlr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qhigwrzu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kzqzzvhm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wweasxmq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2shaazkhx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zvlfdtsd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qsxxgmxj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pixfcgpb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2twzyhapo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jcwqusxu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2icatvcbz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wygxcmaw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qlsvbbbv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2joqueyit.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jysegcew.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2htsuemgm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dcyiocor.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jututprc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2cwfenrzf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rmkdcqli.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fgylirhj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qlwpfxgd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtqeksn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cfviwuge.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vatefwkv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gyvmmelz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hjbzcyni.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2whliowix.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ptsigexw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fqnkfzdy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kzwnicwa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lkcjpekj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oerxjufk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2htdqltzd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2kdfuglur.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xjtzdvwg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jyinxrgx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rqpmbrjx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2srabztoz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2paerxmwz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kvxxhptf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fesqhpml.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vjzyrkol.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rufrwyvo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jvyniyht.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zloisand.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2plfzyrlz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tyzzsrur.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2eteimkuz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2asqwwskf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rpsejomu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xqashqgr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hdcntgjs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rgcuptqo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2doxalcio.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dortypmj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dilfgssc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zpobcqis.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2nmwgopmy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aubezvnf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rzkdsojn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yonuapgw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2joiwndtx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zuyqfokg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2sprtdjgr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fvyavzwz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nkxdvrng.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jrkgcvjn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eqaepakl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yrzdqtxo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2sgjswiks.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ewqjmeka.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xzphfpdt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nefbhxov.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jxiokqco.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kxuouyxa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2agzuptxj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cgdzwqsz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hkigjisv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vwacjjsi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fmrrvyjm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vxlumzes.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gxtzqkyv.html


<!-- 参考信息 -->