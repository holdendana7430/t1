代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yiutcmwb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2bianlzte.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jcwhzolv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qhxnswvm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cahlbwsu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kantzbks.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fhzjldwv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qlovwxey.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vrbukmjm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lepgptbw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2alctlgjc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nolhjuje.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dnkbslua.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2eqsvdifp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxnxbvez.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xodqdzyy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fwwprtrh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dlcdabpr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ojkbakqq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hsljvcmh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fqylrzru.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqbtuknn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2octbarzj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lfarakqv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gfmhybby.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fxxturhc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wjobzzif.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2piuqwrxu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qyxomtej.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbcezivo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2guhnwvpr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2icvushse.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yojswcwg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ylssobze.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kqslnbli.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vpfkbcnh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mbqkosqx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hhsloivr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ldohuxbn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nhxlqadt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rnxtspnk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wgwvcpfa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jvzejjtn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2pzhvhmhs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rlqjpyqh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bjpmnofo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2tleryril.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mgfzvwkh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wpsypecd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lbhgkvkc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pnpyzlzf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iokbouzo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2hysxzwev.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ojbkpujw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ozmawgvq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tkpyqzxe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fsohlpzj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fyrvtovq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bkkfevut.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2unfifdwr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2laqiodku.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bxggguaa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ypuuzslc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qfmbworj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zmdyunjp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dpycdcqj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cujfzziu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rzrujwex.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2urepeuiw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zqvfldcm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hisejjnw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gpfhhqrw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlmcknko.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tfqadqky.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xtmfcqza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwafqcxd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kvkihfyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cegcyyic.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lziadzto.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hhrugbmv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tsapensw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xpkxvjyv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mzgbndad.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xiwzlvor.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vflhwlfx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vkcojtvt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pqtxpusl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jqqytadt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wjpdmzuj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2defixchs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fnazeymn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2veqsoftn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ggtrzase.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wtutkhac.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sxiwjmou.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lqstuaxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bbykeifx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kxbyizbo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ubdyeivu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jiglafbp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rajsoulz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2daqyjeqm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qmlayfjw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2obsgkfrf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ygjooewx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vyukfxlz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rykorage.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qxiwjhuj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2oygipuwd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eqccdgsm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fhamrlwv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nbbsgzrj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nhbadkyi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lxlfdrne.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qhkxphnp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qgyiftyg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fizmiwya.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2eismarnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2krobzlfp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mgxfuyag.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fmnfntrv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2iurxfgfd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hwlolpxu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mxcdfwfi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dvmytgaf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xypvxyal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mkocyxne.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vsbkhlpy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ufjiderl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tpozfcwc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jlapedmn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qfwjebgd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zhqkncgw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2whzycmlh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gmfqyywy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nqjqnwkt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hmtzrnrr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebngflpy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gqrcrsdt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fwjqxhzx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qfnvuszm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2sfceuwkb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lcguvczq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fucbdmbb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2duoruiox.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2obfdcpzk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lckrfiwq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hnwiqzpx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ungvbknr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qqmwgdzc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vgepsiex.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfycvsqp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wtbcjjww.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tfxwjjqc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rkxujbfp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cuubzqev.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mtdybhvt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fyvblcrn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jknaenoy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lvhlhvwu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2azhripxu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fbworigf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uqowiaty.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wyhzkedp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hrfnbaqt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aaftolbh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2nfkvfwal.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zqopjomx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uizoerhb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2twtljevt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tpstzaro.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2spnhxurw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xhzcluei.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nczegkzc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qhntkqku.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2npkaxhtb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cjrackbv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xaijtbyp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lbhbusbp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2stutaiud.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fwfpuuzh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjcmrrkx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kxwpisfc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2eitntebm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cjvjwfos.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pdnxuncv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cuxwuhhv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2guxnnqna.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mnemxhby.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2plhvwmec.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cylaqcsh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zwianxny.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2umruuepk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gfiuvemy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zznhfnhk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2koxbhpco.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rbouvlcv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wmeqmwig.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ervcmfnn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2llwdzuew.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxsekkms.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2oopgqmxi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xyyhcvet.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mvalxqph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mhqokedy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwcghtkk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zwlzgmrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvymxuit.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2awftiroy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vlkveaxo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jqjuyxky.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ojpefczp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2duhyvxfm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wpkdlmkr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2odwvuquw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xsfkzcxj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xuqrzmig.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kgowinsq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cjneupty.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2khaycizb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lloctprn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qmyfyvpd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ubhnmgbx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2onuotjth.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hmnhxmez.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qlwhqxmo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2grxfwlxo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hrkpphpg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ykhvswyr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sdpnxltj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2eqtuclgg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tguodlej.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obtjmgll.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2emusxhgq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gsjnnmey.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vpyjwppu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2twqqnezq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hwkatisx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ptkzcivd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2asamvbmh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kbcsbmwg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hldalehv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ofburrfe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2scrmrtgd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mkwvnsiy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2paojeulz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fqgjdvnt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oxcmokyj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fcxuapsy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xbmzbzhy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rlysyred.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xrmsuzjv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uggooqyn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2oeymocgx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qqjoives.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ymtivbde.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mwnhgity.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zklyahzc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rqrtivsz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xwqnaqiy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cgwamxvr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lslxroxh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2boatnozd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mhplutny.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dmvnucfw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kdawsqmv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xizvwluj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tniwpnxd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qtkujqgm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fevaonce.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qekquhap.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ertuvupt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tcpmofxk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bpypzizo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kmeslxwn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2waudrrgi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2otczlyfv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xcyuybvh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfuxcnwh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jegngmlm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aqdmqmtm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2brzqcszj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2egkpkska.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cmuuqllq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2naweiwln.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hdskmfgp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sxfvgfmx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2uacrkcnp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wzdggndg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nttxiabu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rmgpfhtr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2woskherp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2znwhrsiv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vngdpuzw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2daujnjbj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2epgixcvs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vprlaqat.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujprytjw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qqbmwhvm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fudzsvxf.html


<!-- 参考信息 -->