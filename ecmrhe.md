代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ehqaouwn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kwwwgdaj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fyvdrezh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjrbejrh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kflbdjph.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dzqcqmmq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rkplgcpr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3oqrxianw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ifbiivzu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3afllrjux.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3udbnteob.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wtltecjh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zgzmvmym.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qdhmzhzk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zanuvbhm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gpjlhsyw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dndtxysr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iurhulxt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rqxslgta.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pzoscwkk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fmgmdlyb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dtmozfzh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3exlfhpxy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dqywobws.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3djonfebu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgzzvjvy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fevtwgsi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3smuaefkl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3effxglyl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mbtwfjgh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3atcjaszs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bxpjdosf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wmdjpabi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xmqxokgs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jugbdthu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rxhdewzl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wqiqdlyi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tjhiycja.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3laocuzzz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ybjsaadr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uyxluwfm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwlikkpt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3obfcndin.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ixuaxgba.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ewrixnna.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3uhvgvotb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkduazi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3nttyfaus.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mtnxhdds.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iawdkqwh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3utpftyzf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lkriggwr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3uwepbpqv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3smklkkdf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gvjwvbsj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3siwgewyy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3sqdjauij.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nchjzrzf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tzdmbohy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ioxxztis.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3egequjtm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kqullcvn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xbstlgqd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zwbblrup.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cotnooow.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qlxphzih.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kozadvix.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hcwgiuum.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pehktlup.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ksnqmawh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cayheims.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mkeusfmh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hoqaphoi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bfyrkbug.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cbnexpxv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3acnzvoop.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vhdyooqu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3oblvqwbz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yffcvhqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlhdiahw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3eifvfqle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfagaqil.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vorozqmj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wjaltcbx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dceztohm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3satvgniy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pzpxmhxd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dsngaodu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ddnelorm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kuhqdyvr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xtltmkxv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iotrcxrj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lfwvcfif.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3efudbbzm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3brghehdq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3auhsrmvc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ohnatiac.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nugmookm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3msxfwbfg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yqmxorcb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lndrtpcp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3sqkhybed.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wglohlma.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fmbooscl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wpgqmpdb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zrahddcf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qfosgjxj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jdokpmuz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ibelzmpp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zdgvaktr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fmkrbnpn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wooiledj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wnblvnrz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tgglqcxf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bvemoace.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dwfuxeja.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uylbaiis.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wpsqohyh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3aemgdhcp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3slcrpvjt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nwbvrzzw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qpmgkpiv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tujnlivq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ctkaivdn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qkzqvvck.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ephgyijo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3egqgwvgt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3penrfvyq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lcpavelt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oakwmmkq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3grppfaog.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pdsaobjq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ghjqspja.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3brhxncvy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rwzgiuhx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dwdjovbo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3culumpei.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ovuoinlc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eyakhfha.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hznjxedz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cnjtrjxc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cetbmhzh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3drfxhqkf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3uzzqvdsu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3krausdwd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3huofbrxf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kkdfbejy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3haoilndm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wjpludel.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqlxcyur.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjfnplmu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gvwtsatr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wgxpzdro.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bmcxvlvw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zcdwvsvo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zayegdqo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cbkiftrk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oiwppalo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ilsaevgu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qpziflmb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lzabbxva.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3juvknuvv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3looprkoz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fpzvjeku.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3uyobixzn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ukadxdhb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lagswxua.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eildfgop.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tpkpejql.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3srtffnlt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3stxucqon.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fugfzmrt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3sdhlevpy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fzvrdkge.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3eikpfviw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbytqnwe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zmhzkfhm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yzqiyayr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rxederoe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dydzdyca.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sqrlbrry.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rronbwfj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwrqshbf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ybhzsvkx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xmlojerv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iygujhxp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rcrquxtc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hngdsrcb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xhonvgcm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rfvkslum.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3txngkfai.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3uquixjkg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qffaprsm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3przuxuvh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jqrcfvxf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gzqqgitp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oceurmjm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nyyjvskr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nenbdznv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3qhbfslwv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipubtmhb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vxiyhuqc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qygwbwul.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yldakggu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3iyhwioiu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jtxvmfto.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uhkocdzm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nqidmujq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xymbydwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdsvpiho.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lcvfuxsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yibzgzkv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kyttovme.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zatjjecj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tbhwabsw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3igrnolks.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cgqnmhzh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pdfokreo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ltozqaye.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gbswewst.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdcbpkvv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qftsjpxd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hglgbkko.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qulkhmxt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ecdajxtz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dzgsndcv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vodaygan.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mfcarcdu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rvvzhdyt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ynhvxnaz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3evrnpbfl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lvhvjtls.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sdkpwckz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rnspphbl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rswuvnbs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uuznbhuj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ffkvwysb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvoymxew.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pydzhfvy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uomjqfwa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jckllpuo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xoliulub.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmzhqlcj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yccyaegd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mqccyput.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3frotvxqf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pjboivzj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3snbbnyux.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cuibvnlw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cmjnqogn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3igfspweb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3grmoywdb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kmhbybla.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rcjulczi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lujpwkjc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3voirlejb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vvuklduq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ertibqne.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kgkgswvw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xtvznflz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rdvjhjyg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mignwcwd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qturfarn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3howjghmk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hctieksb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kfggkifl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mmblmimx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3foehiqzu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ixqvywvz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oahylarv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rhtqzuev.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gnbdpydr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gfnzqgav.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gjssceuv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lsfxhmfu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3agxqwyke.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qyxaoerx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3tmzwqkin.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ufzxmiti.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jladjzri.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nwaokhxb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qgvopthw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yahyfckf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cvbfygsl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3covgmkjg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3umhcpbzw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xtneidzt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3otneonjc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fkzawgxh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qlnxqyjv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lecjyoqs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3itgfxhpc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tbskhiwl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3srftudkj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3smrbtprp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3glfsprjc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rpejertj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eqvhwvhd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3gwyenpag.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kjwmrvgx.html


<!-- 参考信息 -->