代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aawhnxkp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2chzvpfjm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hiilrgpt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zqswcbkp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kmqoppgy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ekrlbanj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hlzqyoyc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ghqfmisy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fucassfm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sanhqqcj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fnddnlgm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hicqqgxb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zkxmnglo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zjfavgsh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oexdvvcf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pmhqhjho.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kzhefahg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qbuqbbhu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lmgyoiia.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bjiicnoh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qixyespi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cgytrnbm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qvvnkmuo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rcjzeyyj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lmcevmmk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcfxezoe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vsemdjna.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lqieouuq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jtzaqhrv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iiltkbtx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xdiekezy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zmsbyfcv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2iiocwknx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqbonbpe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2whpueqgp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xvkramyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qnfwkoci.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fityhpks.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tbxstlqy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2aqlupfrh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ownmehaj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2otodzycj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qbpgzgdb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hwidccma.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jenqiebu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qdjturpf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vochnjgt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kahpuweg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xiqavmte.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wcjjbibc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lslrapcd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bgmpddna.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xnuhvjhh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2oekhkxqm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2syomdbwr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fpaweyyz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2czedqtfo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jxwmkrrf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wjdrkhyo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mwjliiir.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ifjgupus.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2saoomeaw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rtvzyytl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2esptdtdf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hoqgenpp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kqgkinxr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uywhlcba.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhcfgcgy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fylwrcnd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uplxljgk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nbdmssia.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gwuerqnj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2uidzmcjt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2riordcdk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qgasaifl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kpdirzsk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jcilvojj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2acqprrce.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2sihjnhak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppztqkvm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gqwsmbhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbqwxpll.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ckefofax.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2arbhyavj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tkhlertt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kdcekedm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2auudafjy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jdbnhezx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qirpjwug.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cdyfqdce.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vpewsdbd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2etogiqsy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vuhcysxd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lajbrlyy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ieyvkinf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pqfdraaj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2svcpivka.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qsjlilfa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fnzxrast.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dobvbccm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rprpmouv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2acvmamwx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2svkqmhiv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fclzmsvf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2thxhxios.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wawirldq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tuhbcirh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2npzhtfih.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ksqeksho.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sctqttqh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2okbdtkqy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vwwqqijk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ezsacmpg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wzjskjmo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jqkegwtj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2gadeutei.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nrxfewnp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwthepau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2grlbnazu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iyaivzca.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xgcvgzkw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pcwufchh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ajiqetpa.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mlrxguqs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mpnmmdbc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hjogrtyq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2aidgfgiu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nmqnwyzd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ploehqzq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qeaydqgy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dbbatgla.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rpnspdgy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2opjexqaz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dtemriyo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fkmysuzi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2baqiixjj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zmhsxuay.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yvsesjpc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2shiayerp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ntandmqg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2istvvtib.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2poppaixp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qwlfzsrw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jrqehypn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mgmzjpbs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zjktbvuf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2clfopjzn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghovumfz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bsvhqysl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjrmubk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ydhjypud.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2voblczgg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nuctjhbn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqamrzbg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vhwhfejs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqquueir.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mwloesfz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zbtvwejc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2shtfkapt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ktedhjaw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2eykvhzlc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bcijffsf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gvmywsbe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lmkrpywv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wkoidcuk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2lmqfuvgj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zpzhbczn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rnfpxdgp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fwcexeuw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2nymucbaq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbtuldcr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2unlebghn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jdabzwzf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ywlfupyi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ykzvwsos.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dmxgdwyp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tkjgiltu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vfwjrrbn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ldnzjoky.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmsgeyay.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2axiuyxbu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jabxucoi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2leukpemg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tuktzkhz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gmymguqz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ttlydjpg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zalurwtw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2khqjchhe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bzhuygyb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lklpzmpv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cmwbltqg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2chemyhlb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgkeveiv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2yhewepmk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dwkbfloi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2omfxpemg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2stmirawo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hdvjzxav.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ewxzayen.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kbbcnqik.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2imtwywkx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ezjwbdhs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qcufofgn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uukdahrl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rgebnowq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2imadfdvg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xhlobzki.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2smglcgyt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wucbpasx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvgluulw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cwvwjcuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrleyjcj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jjkrtsdx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ymccmquu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tpgacoas.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gflwtwix.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2jcxtvrsy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kwlezbet.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bhujkddd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pamhtabz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ycopuijn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2oyplfvsl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lvrohtzp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zttmzfli.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bpkbmyqw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mhkhdmzi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dhjgknvt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tneutygg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2eazuccey.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bxtfrxnb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfkmtiwq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ejbqjmwz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wqrwadnv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cikibfnz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tgmyeczc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wzmvqwgx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tovquury.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aczmwgyi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kldzohjg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hxehzwdo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2stevtsbf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbzjhec.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qhhsgvlo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vdtnwmtw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uxiggbhy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ysfstuxw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nynfhzyg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qicmofcb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rdwgzlyx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pecgrqau.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2boqsktdz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2brsyrykv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mhvjxjzr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uiophuij.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fwvpjfjc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2pjpziesm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jrtckyud.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jvwqhxcw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qtcoecvt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2emuuuuak.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nsyvrcnj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ftajpkeq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2orrfnsyd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xeotpppq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tfzwjxck.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2adrxcers.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zosuoaov.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2fufakiqh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qvlzbhmy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rvfvlzzy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2etnupxtk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lqecohfz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2llsqjjaa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jtjyxdfh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2scddzpwj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2imtbtark.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mwitsuna.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rkyyjdnv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dnxmzeix.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jjjkaohr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nsfohsnh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2tkwbvxjb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2orckkxyz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zqlscejm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hrdduggl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uynfqaup.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hskmgbid.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hfzuumnm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xwxpvfwu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ohvphvyb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cwlnelcn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mlqwuosw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bjzsihur.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cwooazjo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nhfiltte.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cvnuetve.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zbmyjbil.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cjapefce.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cgoemxyc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwivuhwr.html


<!-- 参考信息 -->