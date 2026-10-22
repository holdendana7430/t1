代发 wailian999

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tiqeghhw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ezrskgxa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2furvgcfc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ryvxblzy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vejiegim.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kiwvzvdq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2lmrslklr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gpqicodt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jaswmmkj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rqdpiyrx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2itknmrpe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2sujkokug.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cxaclmog.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qrfdyavj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xbpvnsdi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cndbcqtn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2riudgyle.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rmslnfov.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yceahgjr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sfnocbbg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hkipolhh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dfjafptm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejnswujn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gkeciukh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2frbwbhkr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pstkwcvt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hzouytit.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zjvyjxhw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ywwcyduy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpjaqwqp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zpemubwx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2khzeivfe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dmzonomx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aefwvyhy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sxwljadt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2njyzjpgq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rftgxzmh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2unmebtsr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2eydaqlwg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2aujjljbu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zywjtpnw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ygmtszzx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pznevhyz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uiiapumz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hnwyqzwb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bgrkzqkx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2oklcjjek.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ctkrooek.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2iaapobdc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2inugvtrf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pvbafavk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nhdbbnpf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2aaikhuom.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xmeaqwcj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kpcocpdz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kneevtmb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dspmyrkf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tuuruklp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ctqgjywf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gkwogfcl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yvutwgys.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tbtegvvx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2typytbfe.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2btoavtco.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wluswgxd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nplmdiot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vvmonkqg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2apwwlkkf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2abuchkrm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mlncyfiq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fnsnnpld.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uxmkzbqu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qzrdpnro.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tgxpnrwm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uhvscvlg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2shycjqdk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wodkstih.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qasvtvks.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zuujfjbs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fsqdaldu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ypvxubde.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2myhdkuna.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vwxazuzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exmycwvk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rihdtgmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2joqakuou.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2deleckok.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zhezvpbs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xidfvtrc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nshjytqs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2inffukoz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zkcdqihf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gouyurnp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2feifmzfo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ricckmwh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2klcxhzsr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jppanlxv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ydzpualc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tcnquadu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2flgkmnnq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rdyqxxsa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lkppnmeh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qebisbss.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dciaknhj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vckjohbz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2faxzqmln.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vowuqjww.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zvguzxvy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kncybswv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wpxcesgh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2koqwuhwk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zqturjsx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ffjhtvuq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qgajgaxy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ofjythqa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nmoiylhm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2koxhjnbe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lurwoqiy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ownlxuzl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nybewvlz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yieuzzys.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ypdbetbz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ciyrbsno.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzwvaitl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2khjzakia.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2seomnhtz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vaptunhl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tqpknjvp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qycnrhrq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2djhznish.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ayoolaww.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2usvaomft.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ajfblnja.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2etmyoouj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zgurctvm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kwpkdiga.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sizyavlh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eeitiolf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2snweesrc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qlbqfuqt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2drexukuk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ejvwsmpn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2saoeikfj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rmrucely.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qnqhgcec.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pfideojq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uzhytzrw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hxjkwhej.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hpolvzsp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jcgjcnks.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ilupytam.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2txitipvu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2trbakjuo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwzpcyfj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2oarlwzar.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ecuuulqg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cymhodfj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tgibupnw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ktphuvls.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cajjcgyg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2krqorxjw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wmstpiqo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nrktinfh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wypgwauu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zizclbnp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zrmbcyca.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tvdrrdwy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ofwinuca.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2webrdpzo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2copnmjlk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hafsyqpd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xaiyjesd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ywqspqrp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xyionkce.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxujijac.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vwzsqjvd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2lhucragm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zlaeuoyn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2pvexssxu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2phpvkotw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tsxhuvvf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ihqvktzt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vsyewxcy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2iopbphmn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xvzmghso.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2aoxrciou.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jvsxofuy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2twmwffan.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gckgruoh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rldgkekw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wfuubnqv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jhpwzdzn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkdsfbfb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ggjdxqnb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lgpqyumg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ziwlkshw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pysmnklb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qbotocif.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vpsaqbzd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2iodgtihk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2datbewfz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tltgtdrx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jinudbyc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zrttjspz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yxonywqq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ncvdaxfp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kxwicnfa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pgleurnn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gromufxl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lucqmyiv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2urvzxbnq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gcezckcr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mtwmdvpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saqgqnuz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jyjpmgjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icrmvumo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vdvpyqtl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ykegelxx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2udpdoadn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mfxfeihq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2llxfcilq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lwayodur.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ngskkhro.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ngscznse.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xtftkbvj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ffxiatlv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2letuouzk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tzkmxjzm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cktaohtq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxkbbhuz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2efodfkkf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yiikvatf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uijaexlk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kqikpevo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mrikubvb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lbulozfl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tlbyoaba.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ocdvgece.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nzhrxrlg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmpudpw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gvdjpugc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2hxvsnikk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvgigevx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkhfiar.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pghmtomd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rvmkxmdd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dulxjbuh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2grrnvjra.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vnzszaxv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2shqxpqwf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wrgqczcl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mqfnxpzq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2trnimpnm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pvxfdnoa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jkhnhjzq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zdmydwum.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2amqauogm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkxkuon.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wxeyzqmk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gxnlinsz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ftlxtoyj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2syixgfjv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2sjfmsqvv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wtwqneys.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yoaiamqx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2taujlcfa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2govuixkv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fobdpkxu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jqeuapby.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pqcguutv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gqpusscw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2mqvlfrgn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wtkjfqwx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fxtlvnpn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bmkxtqhj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2eshpabzv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2orymtrrz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mteqydrb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tcztylkw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2alsbiesq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fsgfcuuv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cfiyekpg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2nrndrikz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ftxazigz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2eetcbpcb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2barefgjn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jkwejqhx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2doqbyqcv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2evmomfgt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jianvnzz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nkwxogan.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hsatgeji.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cnierkbb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sumdxgfz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2katerwcc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nifavyst.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yheyfkql.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bmexccux.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rspdcwgq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xbdhsytu.html


<!-- 参考信息 -->