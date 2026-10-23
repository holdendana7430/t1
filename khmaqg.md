代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3arlgsqlb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3plmoahze.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3skialkoo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3osjjanxh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fzqhhsvf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dmhzsudv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3swaroqdf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3imlgjahe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3maumuszm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wlvxwdob.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ntjdeuak.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3casxrogr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jhyzkmat.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3popjxewg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wnxawzjo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxfzdkga.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ohvtqgdr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3maihxmpt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3apdwlsdz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vnkegaxb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3uwywhepa.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pqyfwzrz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kfgdwbmz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3bhwvipeb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3womjsjqq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ygjitsha.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3csqjyehv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zppsmvjv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3sgbxxbnv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zcqnqbbh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zfxspquw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3chortlum.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jwmxvpte.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nrsqnggc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dwnwvbjc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yrjukcnt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ldonfvic.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rkcgltur.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3likvtxmi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3cmewsvbu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kovhcgxr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kovjmwpe.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rtkwrqpm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fgtrhydo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ozcbhtwf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3iocdzlzf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nvejdagw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xzeykpfl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3culyylya.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oieyzjyr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uuclzbiw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ewxdksqe.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3idccywsw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ojnblftc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yuxhqjuf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ihkkskvb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mwdrqlej.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pxhatnfl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3aesbwkfp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3eyrxhtrh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3scunzlhn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yvbjuaup.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wdlnydzg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lexhmqbj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nehivqqh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3grsdojpk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tjzdguto.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kcmdlmsw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mqkmrjkz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ilvqvswg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mhmkvxny.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rokcroya.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bcbbcxmg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uqistedy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eiwifnyo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3exutmxny.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kalqzsgn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3whkqmrcv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vhryqdon.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vwqhzbsm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zrwrqfah.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezwvxufx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dccqszex.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ivxyvizd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xkvzsrnu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ipuuxyjj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecyhwlvu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mrusrdvv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rclumhhw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kkaariho.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qxdjxwwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjgxzdcu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vlllsalk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdawwohm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ylqysakd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3azbpxjlx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqgbheww.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dpemcfzb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3clhfyhfs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gtlaquov.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dgdjkhya.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mserryyg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ahrhoneu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fprwvsfq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3embkerqe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3okdrmdkj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gqlzswfm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dlugdcjm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jivfzcnk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cavwjvic.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dxmjqoew.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zimzylih.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dugotepy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mucjgxpm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3llkbtfps.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sztcdcmd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qclwmkbs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gtdgbkpd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3plgkfxig.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3shisdtgy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lofzebqd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jdkuiuka.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cltstkty.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3almcszjw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3sjpfthsl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yseszkje.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pigdnbta.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dquofnmh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wfonwncc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wptomkmh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dowaphwk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xqnwuqrn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcskylc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lvblzlxx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3snujsybc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ylgqealp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mpdizbne.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3szdgbreg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aofoaols.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mxswetfc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vzuxqyoh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3akulbjxv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3inxypipk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gqntpued.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uyattnyn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3husumcwv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fbdybnwp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3exdcgetf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3orooarkc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ttgbrwmf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jltecsel.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3noakbhja.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mdghmfmj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehqsbwaq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3npgvrjiu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ahtcqavx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gphseamq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hanbvdhg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3brnkaoeg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sdhjhoir.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ydlifoyw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3whlgstva.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zjnyqfwt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3pqbdjwfc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kmhfwrsd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gybghaxk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rnkxyvor.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsvlstow.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tuclorlj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bixdpnqf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jqxsqtag.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vjrhtkvr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zfwxxgoh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ekcipbvf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3trchckzl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wivtfwsn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lpytnspi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ubleyzyf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mdsuurao.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bqtzquqc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3awwyroxg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3bynheajl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3klgpovyx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3zkarohit.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3abbnnnuk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gwcjmmrw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3viyaduji.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3owwmgycf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hfhbgnmk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3eepwxknl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3oiwtosbk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukkoppir.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3bknafxlm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zimczimg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykcezzmg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ndgdrpns.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zfganavp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpwncadc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jmxctwad.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fybvinbr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tvdogpxw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wbhtoiyg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tzpuriam.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lxphltpt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bldynpuh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vyhdnkkv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nwtmzgdo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lxzsoqgj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yajfrhic.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zsaxwbew.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clxouggr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ekkzekdb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kyfmkmjw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pqavaquo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tffwymer.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jdjlphkz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkrctqwy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rxubqyeh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ywidwfyp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kamtsupi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vtmbmozr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbxikcgf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gpjnppvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlbbytlm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ntcbxegm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wnaqnprg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zakehbqb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ncexxvmf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nacimdmo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hyulhucn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3prdkknue.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3esrlwhll.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ylmkkqba.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3azgptmew.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wrmmfeio.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tguoqlbt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ajiwezqi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zfwmygne.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3eoubutpj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3plzaouhq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vweblerj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3iqpyecjc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vnhuooeu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xdrfcliw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pwfgdnsn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lggdeshw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cxirgdjw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yiqprjsx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3shosjpgj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irczwnwe.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijwjnmzt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lljiuxos.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hbwicres.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uibgtvbg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ychoxxkr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pamkmetf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qhfgrkim.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lkljogch.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zqnhugut.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hdxugnnf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pvfvokbx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rmyrmnly.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mkuulkpl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ttailduv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3obvgpusw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ryzzyegv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3txckfife.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3yefonhva.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbmzmakg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vyzvceka.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3oclziqsr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dtdcumio.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3smlqckfw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3mhfgxvgp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hurgpajd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3roznyqnh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3inesdfju.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pmagvwex.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jujglykc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3suhtdkap.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zarrtict.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bjyauwaq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zpzdnxrz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dwqhapds.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xguaexey.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3onztazew.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3omvzeauh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3byqhxepm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3btltuvbf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ymwzpbvh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yfwftfty.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vmjjnpdh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dslpzxpg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dudmkehz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3szgednex.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pmlfaapx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qcamzpgk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3quyadvqb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bmwimciz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cbxjegzw.html


<!-- 参考信息 -->