代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vsldokfr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hixuemag.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xjxiqyhl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zuwixxqq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2yneunzvx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2naaibfgr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ewxejtmc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jkrhqbhu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ueomokgy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2enctyhcz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rnarnvwd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pkkfurhr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2asmxyywo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vznwpcjy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nrpdtvsc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rtpfyoqd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gbuvmbki.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2amfgfttx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jaikzpci.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vzvqlhhk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uuyrmlzh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2opjhilny.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ihkbfncw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jvuskwtq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xuydnwbe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2viuhwwrz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jklptrpi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gyncpbuf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vzdhzgag.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lkzyhstu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fotwkqbm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vqfvlrmo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lhqhxmle.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fsjgdjmt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qdhcgyzb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2itrlwikm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2niadujqi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbbewbkj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pchlbhuw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nzpcrmkk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2diypnzdb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xpqjohdh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jtavtapp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nzmotvcv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hqthgcna.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hpqvelms.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ftenvzaq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zpgqrepe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ejjesupz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dslemhwp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nqlfefcs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ftarkgmr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lwxdlvhc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sckiabiw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wityhzne.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kzabtsqi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2seykrfgd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ruuphyhm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yysohmvx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gaemxoav.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xtlcangp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ksllijvd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tdezmbfc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wudmwyoj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tgcthwdy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2utcgueot.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vpbwhpgz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pttydekf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ulqymgzb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2riztltny.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2uqctfpzu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ohchquzr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2asdftwpg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2idmlgwhx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2txkntlsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpwgrxri.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2chuevygo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bptufrll.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rhdodeqq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cxuuubhr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaupcctv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xzdvmyno.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ypqdtjvk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vfxwkcnx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2axjvroqa.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kgavzmxo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2oaqrtdjm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ceaoxfgp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2njjszxrn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mrusckvl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2slewzfpb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ojgdutcu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nhhgpzzr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2javnmkwc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fehoxday.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gwedldyo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ljdjbgog.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mydtseel.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hpbpdzce.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fxeunldc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qyybiqwb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqywger.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2chitwxbm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2sgozaymc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ydurojvx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kaflpuho.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lfhoiubv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dumqyxwf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xxupfknx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jliuzqgu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jdwqgwmn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qbnjawrl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cakjjdsf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bfpchxly.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qlugihxk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cspedwle.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jxnajbiv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cvzlyavw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mqvannwv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ezikmepb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qiuoevzq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jmpofhow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2pidjwirf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bofcvycw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2btgstxlx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zlngymje.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2icgwriat.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2shjsojtf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bivmoxsm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lyflowua.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ycutzjvo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kmtihruz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jzvueyke.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2aaycrjul.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2esgenfdy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vzkpavng.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zecpgzye.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2favaimkx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pnkohtjf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2unwyrshi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2drdocytj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2flshxlht.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2msxxlamd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lejnbivy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fqslqbde.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pwtjitpf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nxjnodgv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cyxrkaxg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lzsvxlaz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wdeizagr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wtspuoyi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sucxhekl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gkhorlkl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2puxmvvuw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cbgjwdnb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oqjbvbsy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kuwaunkt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2evrvzgsn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xwasnrdl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lfgfztyw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mazalfho.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2wxzquqev.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2squxzedc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cllemadw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hwvnbjht.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgndktlb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dljdoqrd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2myydluxq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ubdiobfc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2eebjgbjh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xzvyakby.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbmqygwi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xdcewxtd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jmoejlzj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vuqaulcm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2svuvaunw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tmuogsig.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezlogmuy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mgvbwaxq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2amlckmht.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2xlitosat.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2muvgvosw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2opquqiln.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kivtbcqm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yxoekrig.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uerftzlt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2daccpusb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2myvhpycm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qrgxcqdu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2trnhgxag.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2prbvztri.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kamashsk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qgaldyvi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vxysjvoc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lycgimcc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dohitblq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2puaevmww.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fubkbhum.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vxkugmue.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uuzdmrwk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kdtojtrm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2uccqezzq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2janqzfll.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2onhisbme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mxuqgrhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xotzpksk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ymtuvfrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnwvqqrw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zioyozce.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hxkkvgsw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mcdbasfx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lqspptif.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wahrbhyj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2whfufnns.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tyywsmyh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2urpzchib.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ixigxuil.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hbzejgho.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2degymvwz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dxzmjbzh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dwxgpzeh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wsqxmaxg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2urqqdhjt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pnspvuod.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2esxabrjm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2crvmasqp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wntioxbm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2krmkzgzd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uamaehsp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vqkmneaz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2sllcybex.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wbhyjxkj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fasebeph.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnokllmv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pyhljmql.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lvzuxygw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vmndruaj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tijaryed.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zzmioxbz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vmulqljd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cdahyved.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qglfurjo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jkfyfeex.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2buepxjjg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2oixpwrgh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2splwhyto.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vrkfkryv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzsadaj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bcjgfjhr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qiqnhhwn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uasscznw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rbdurizp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2sbwhxorg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2knwqntxj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hkiwlunn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mebvuiwg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qrwmecon.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nqtgwjby.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fxgrxlwo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjkcylj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2snkwouvh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2znnmsbyx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2imnerjtx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2shguzxbh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2thtkfrmo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bvhnmkus.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2adgvkpzj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bbooajxx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lkkrhsnn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wdklnxly.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjbminxu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjdfhphj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fpyelpdj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xlztnbbp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tchasokn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mqmagrzt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vnieafln.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yofahwpc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2aazpyhis.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2uhtqzbuz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fojvpfsj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2parhkjgd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mbtnmqmc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2flsjmtwu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gpyeshiw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lrxarkvi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2abuybqfd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2plptdrvm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zxtuwqwu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2csdpplrl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sdzxsnzq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jzcopnii.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gwquaild.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jpodqmkm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2mmgjnpaz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qnixbusw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wlglrbmr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2crtkmdyn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2urzfmzwd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2aybgvlcl.html


<!-- 参考信息 -->