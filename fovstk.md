代发 wailian999

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3whznjiwi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rbajouni.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uxgfrhkt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rhhuzggu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qzcsbpat.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dhtsactf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kmzgjojz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbmcpnml.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dprfmauh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ffqekhlt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vlzzlhkd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3aetwfdvs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bcyxnpzd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xwsrjulm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3larrnqai.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tnihrqba.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3raqeprnk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3itehnrpe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gyknklse.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wwannywk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3aajbwozl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3dvqjsvqc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vqvlgpiv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sexmaqlr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3risgmkhf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pjcgqfma.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qusinkln.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3czvuyibt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xebgavdp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3elfzjyex.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rmszbwcj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qyuhbprd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3bnvjlyzv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3tffovxdx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3eexslhfn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gtdntwkk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vqvoweoi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rherpumx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pzrqvzjn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3agaqrkio.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mgaewksj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3eovboqez.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3agnumrhy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3uuvquqyt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mvoiwerh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3arcqcnaf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gbdnvaec.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3kzkqimqe.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3clgihcwe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gwlhpmmp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xvajmnhd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ndimubhr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lovobetj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ytuxgank.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gzrtmqbj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3irfiwkzu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yatyzqln.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3uloixgql.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zhoaqomx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3njofbcxn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3dzaudcoa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gnxmwhgh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ndrgnand.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3seeyismi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rothrylo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gcehkvqm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oukvqumt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rlcqomwh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ctwrysjk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tfqancwc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3adwxnjww.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxrkrggx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3felvybtc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkskuntc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ahhuxdin.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pdqitvlq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ouowbgba.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zujjigzb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wdrqalzp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oeqpicoa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bjfcjvag.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xrybdpbg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yacxtdzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xaenlybp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3czxgnutl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxoyyfqc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zhtcdzaf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nzaliini.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hmpzepri.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zlrbqbfi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xoewmebf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jixxpncc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ueheabmm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tebqjwvd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zdlymnbw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3swyubllu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vbnaggut.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3podyezbt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vwlqpkrc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3scssuxpb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gdxclbjk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tdlmanvl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zilvapve.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yfaqbiyt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3plkscmsx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3nzlzrnve.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bxxgymsh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3upgjmzng.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hnamvnyp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cxzffviq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yofrtqsw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kpihdumj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xmejjruc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3carlftdk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wrycemon.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lnbpyppd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ufmgxzhs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3wdkfsnpk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bkxvckqu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3uaicxvun.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3symcigkt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjlisfht.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tjojngni.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3aoqktkua.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkortvi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hatetkve.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ccfeujay.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zimifuwm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3inhioldh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jniwcroy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qyhmyeup.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ezsjudli.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fxbtnpgg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jgadkzhl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rqqqhkkh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vzqvporn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ibjdcoen.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bodfsvwt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3olkqzlxx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jriugoik.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lysmaift.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vbhzvlcx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3komhxixy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mzkjbrtq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3aqbcwqll.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmkcovwt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ilgobpmv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pgpnlqvn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rlpogztf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vaxpupmu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kchzfmrf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lwkxexzc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lqoibjwo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rovhecxu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mzoovxmd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kvnrlvlc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ezlutfwr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xcmjumpi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kfsesqdc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3aldbljsh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3yaaqmgoe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fiwxsood.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3idaxrxyi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kvfxvfgb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3euapsicv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3lalunhuh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qutclevh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gurqvvly.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xicnxeeg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lleidxtn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3agecumxr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fzgamyzk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctehfqqe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mdpvhzfn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ubqzqrsi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gixvwkyb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3imirmuqc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xfyovwoe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3eltonstk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qpbmssjs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qxntefrw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vdiuuwfl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jgezhsim.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjpesmek.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qsuwtmxb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pbtuvnve.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vlzfdhhc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3imujbkog.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tooxjmvx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iaicvmpn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3chzejmai.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ewjscjkf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ixigqijs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bzqokwba.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pdlhqqxj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3xohmuvoa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mamifpcw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zelrlymb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ddaqztai.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kjzquwqi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qzclldul.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zncvydxe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zcbqlwlr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3axjavsmc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfurpsyt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dviiypqa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wwbidnya.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3aegmidsm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ofgwhlqe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kjochxwb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3raqriaab.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gunuoqdw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pocakeir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prerwddt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qcgnmkbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bahjrzgz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pzumbcgq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vxcseolc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3pyjdtwnq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bpefwulv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dwzgzdyb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qkttidmt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hegogsso.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bxyksuih.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rmcdrfri.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3veliwfec.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qaimmmag.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eeazmuwj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3culmkxya.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ooscexqf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uyndqqxm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dagrlygh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3miemjfxm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rtcmnryb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ukkykbov.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ibaucbzv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pbbjipfi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nqdmgtml.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rxezglbu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nkfncuvo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yaazezlc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdfaijzu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3haiwqeht.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qxotsjia.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kjfzcqrr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ksevlxeg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jnvrjbhn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xgdfjwnx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pqkppeqk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wsysohtp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wedfbcyp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3uthtwhoj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iysuxdoc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ufsimlwy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ocfdusjj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ictxacea.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vhviefuw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kilqoncl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xhovvoep.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rvswndbm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lgnwxcce.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3detaurlh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xtepefuf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ecjejjcu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fmmzoapa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3skinqtot.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3pkvpvnrg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dhdtcclg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kogrodhq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ooeyehzr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3filcvyme.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgcebc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nviagloh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cduayqwu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zbalhnhd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gyugytzr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iinanfpi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fuvwlzta.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ymcqnnpv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3giuawwud.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qwniwdok.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ecsikpsr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hpxhltvw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yxnciqtm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ffusmkll.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xfqnctmu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcitvzci.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3oewzxrxl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uloohosc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fahbwcan.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zypakkdn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mvmwgplf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ljtlgqfo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bzfvbqgq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lhuutubp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nkmzleto.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vrhveqin.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zmtnjuvt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ebmgrmsp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aaoomlus.html


<!-- 参考信息 -->