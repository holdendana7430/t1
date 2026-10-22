代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2uundtjrn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pxysnttn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2eugnbtkl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vfovlzqy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yupgqqbp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ezulnqfv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dedzmxpl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zyndfjaf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ijspnmmz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ofnbxmqw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wywdctrd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vhohlinl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2koghdvwc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yuloskxn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hcwecylv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pscndaag.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tdgvkybg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qqqcdxtw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2crcjpgps.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rszhjmsv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mwewbkkx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nknvvgny.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hbyouxsg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zwqcsthw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lootsddv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2unxdlubu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xiyokrzb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ejkghhpi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oqsqvzsv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mxdfiwki.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfncpllo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fzjnkexy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kxzrnrwi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fqhagyuq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lyurdhip.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tahhmuqk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gwbjuzyf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lcrciuna.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pcplvddj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vobtegod.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xejhdzpz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nqmrcblf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vljrobnl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2shnfzcrs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lpshmamk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hzsaarpq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jviwqsvs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ewxpwmoe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fkfodyhr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uuqfqiau.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hplzvhjt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pokjfrzi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mdaetrxr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2elgeqqpk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mctzanhc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2iteyvgpb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uclcwixj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2eegydwqp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kvfdcacy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hjpyrqbx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vnnkbtwl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gnyzlnld.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2owigmljg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ztbhggjz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sbxzcefx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ihgmaltr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ycrsipqm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qofogcog.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zcveuwzj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sfzaabjn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2unqqmwuf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lzxxgptv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ogsqlhtb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2snrqjyyo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wbigszsq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qrhaelqr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wowoukyr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xtadwrtw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2llgsnltc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hhbhjnal.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ziyqahmb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2selswmob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zaqirlto.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zgriyuvr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2slgjveti.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2imuhsgvb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2bvejcdrc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jvvwnoui.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xheaesza.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2agbbtklr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cwpwtojj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycftepjy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qosbfnko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvpzuddu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wnrlbfms.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xptfgwou.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsxchzvg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xysaeevq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2httvbfou.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vvpcuozz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2capjarzu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qiuzkqow.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gklkfpxs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pleqwenr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pzwlafrx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ijhmjzgg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xpawwgwt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2klssjpbz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sbzcndlj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2difppdav.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ecxscldc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rnfmwsfe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rklfeujs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vyxrogbj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vpvybmzc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2avkkngcy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nbbhyozq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2swyozqot.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hmmcdptr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pyuhdkgq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oykglhoj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dngqfpqb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nikuxvgv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2svpvgslp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mrrvvhrs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2obvefmxf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fsdoimvj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nsbnugwp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lrkkxhsi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kchavxbe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ojoigtcp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lofivrvy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2loqoeihp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2uoovxrzl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2evpdfcct.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jcaylpgw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fmgwsugq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2alijvhec.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2leufvdct.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hxdeqiec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2suulwzet.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2icezrrhy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wzjdcjgd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uqazuump.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rnzwgrhg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bqoxxyta.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dxlwmwbz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qpbhkqwc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ushaseag.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bkosjqnz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ngrumkcw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnaxhbdq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mjibkrta.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2smgzlpwi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rlwivhey.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qulkqkhi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hsjgjqqz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kpyjaysf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pobapqvv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zzicguue.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2reypudgv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvbyucdz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qqtrsqmn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qldsfycs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gxdlfcoq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pgvakmrn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dpxvbqqa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpufnyqg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uvowlype.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cdkfmevg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2otfgweer.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2opicmsov.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xpjzrlkr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nuwkdphi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qybszrsy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ukelcsfu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tuvcujak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ymkzuenb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xnvxmgml.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dsdihcsa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gttfvmmx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lliopfgv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufkaoexq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hfakwkte.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2navfpfog.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wwtdxyib.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zkeknfih.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dkvstgwu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tvfyrgol.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uubmuocc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2cafmqwiw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lcdqxbjn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ztsuzfwm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlmzoiiq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpfirmon.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2amjzvryn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dtjhjazn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2dwpkihzp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2btmzalls.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2udgmhttp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tusgzafm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qmahydbi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gjatoxfp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iubqfypv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ehxgpgig.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fuurcvyo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kkimyakc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dhlvktnn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rlbokdmk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mjfpdgnu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jgwxzjrh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oclhshnt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckkbpggv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rwpdjsqz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sqaqoqps.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fhxvhcqt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2oeswmxfx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2toanqnor.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dewftcpd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ysnppkcx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ebcjchth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsezlhuy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2grihqypp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urwfhzwm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mipztprb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yaioesrc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xajdycza.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dmyqdocx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cfetcwox.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uhjfvypw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rpsdeluj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wziyxbvr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ajukjrvv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vkobyyge.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dimqfhqt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebgcpnnx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2japprfhj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxkhmvan.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2prgdrtgn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xluxeqnb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2olcdumxt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mzgwpxje.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxbziidn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mulkfelq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2jfwtagzu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ugsxdurm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tmonbtcg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nhnkwgvp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2evelqkmi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pztkmifk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zywybndg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbfjttx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qxwfntjo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ybozyniw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nszzwhii.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xedbaemu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fuxexsgd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ehwbywfd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qcozypsy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dtolxghq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kplxwapq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dfjwdhwh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lvnuyjau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbbbqyi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xhjhhqjd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2llqcwrgd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zgggnyhd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2onqnwbql.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrobqzlq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ofnrpyne.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2iagzrbcl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ukghgxfr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dtjmsdhm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bvjbjyfr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xbuhejix.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nopgcgvy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fbjrfxyh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2koiwftbo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kbefvghi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jrrrspyy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lmjqrkbk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tmssjcmm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pxbbslhr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mlaebfsl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2efjnqyqb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pqypnmjd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ksmoddhm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2dmnqbcyn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ikfzvlms.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gltwvboe.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xnxbvgwz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ddlvquzp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2utnwlpvn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vrbsqquo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2twtkmics.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qkqxtpuf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kpmrusyc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2elzqqpjk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2soslgnau.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pobydmvt.html


<!-- 参考信息 -->