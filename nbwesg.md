代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zaasnfuh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2waeaylnn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rpinlrih.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cmujrahm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dllmpqzm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ojsnkpxs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bsazkjui.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wzzpzyta.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lpmukrwm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2aiysnuap.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oikrkncq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2uoaaepgd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jxjxdqox.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uzxjzynb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2eemabynv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pbtjghdd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tqqiheqa.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gvxpiooo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hpkqbbes.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrcasxpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lzgqhvnd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qudnzlvk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vatseasz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ibmkgzdp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2obqoblin.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2acbxsfcb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mobvzvsj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rpbanhby.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gjpphogg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cfxrvrjf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tclmioox.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qmedpoqg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jyfrkypc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dqwmqaep.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aaokqrzm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ynbtrlgh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cdpgbiyh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jqngyypo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fcuckroi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nlrowrkw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2upgnokbn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyjuktak.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gsdciqrn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wdcqgabe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2owynvwtj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ybtnvrry.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tfeetwuw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xfrlzses.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fdzbyfjl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2goldrkwg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rlnnkzkf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nexmnkto.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2grgwlpja.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dcxkjsds.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qgygvrsj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2izsuflgo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vtzxyeyo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzpainzx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2odmcnsbm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ksnbmzgw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dewcvsnl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kcrylebb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zqtnjeyv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mmqtpyzp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rvlyvnpt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lgqtsiko.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kanwpytf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ouenmlna.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bbfwwbdh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kgjdewoe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xchozosg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ywiiajpg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qqiimscr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kcrjnfvv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ckzrpgeb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fraddlad.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bwxzucej.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ohyxpcnc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nouemuff.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2itcsitaz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2klgibowp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uwaiqlnj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ifkdidfs.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dugnzvec.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kplfmvpa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2eaqkyzmq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2eufdpkqc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ogkinwnq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fmnkiscl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2pcuxfxgi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rkpiuttu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2khbwgsgb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dstjmaag.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dkkvkjmh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hbfckvyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pntgqkol.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fnrjtboz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrvmqmte.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xaolgkkp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jigufmnq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajommvuo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vvubrxwl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kyuyagmc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jpfpduwh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cngjnrrs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2obqfmfzj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sypggdma.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yzmmnrom.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2khhrjgzd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fjyozdhi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2oyhrhjnc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ammkwgmr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mdzhnrpb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yfldjydi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vgbijydy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qogwuqge.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2btffcfty.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2flzkfzzw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yfgcmhlz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2poujqvzr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ufzuplqa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2slvvmpbj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lguxxduf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2itrjccvs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bpatejcv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gdfvlpjh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nybejoqs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dggevqos.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2smdvualw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ejlrsvft.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2iconcvvh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ieesrrgp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qhdfatht.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iyjbvaxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2asmsyhfn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hispdqdf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhtrlai.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bmcjwgjw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ltmlaafd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2akeojhxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ntjqnkdq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pkqigjrd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fuoomnol.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qetkzodj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yxcsslop.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vywtsyxf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2sktfcwit.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2gidjridk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2qlodhfwf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fnjswwmy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pyyfdzqy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qehgzjqh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wpocfzeq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ebcocawq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vngrhnfb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ppfyscgb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ubnbrhqd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ithrxqqe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pmmsboel.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vuvjxvnl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eqkoozhu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uarhaczz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dfstjuzs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iybrjkxk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lzfsspwf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ymwmuhkw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kpmhielt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hoseufnj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bxajztwk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vutsdwwu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vjruqqmm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekcozlnc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jvkmctdm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tqfzhwcx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2alrukqaj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ervbvcen.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xeayysbb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xybymiir.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ftdnmgtd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qleqjmlx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2geinnssa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kirblryl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2urmrsjvm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tlznfaxt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ptzrahix.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uspjczkh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2scomyynx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gstajvaz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2okmhzscu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xhaqfyqx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2peldkvzj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohsqbcgo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oetnwpbx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2omftkvmj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2detjcotb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqjtimpf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tnboyfpu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ehtdgzoz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ctirivpl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lvqsixmu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wtvagjcc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhimaltx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2akmldpgi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gsoohbpe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gdzofzrf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gcrqngls.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tpiwxmcm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2leadnvch.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbrtwll.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2iiumdupk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oecreupa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ziowhlin.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ihrcgbfn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2reidpwoz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fgpaxqjb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fbjxeerh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgixsclt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rkkgcoqc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ffoblglf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fzcbdqsz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pijgdmbo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zjimcbop.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wydnucvw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2orqcautj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zoarlfil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlymztsz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2swbuegeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecsjwzsx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jdjkzqma.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ymczvaba.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tcmvzjej.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fkrqykoa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2otqkgwcz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nsccoxii.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lqezgrbr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bsiywlav.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jjztunbf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qgfhgswi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2likwudea.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2annupoze.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2stsatjln.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nukffaqr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vhmkeeax.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2icnwgjrm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bnzamcxh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tyevjrfz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xzkbdbfw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2htowprbm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2aadomren.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2iiezczqd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tvlumjqy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjyqrrsd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mkekyykx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2eveoqego.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdlifmec.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kmtfpguk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hvqgowrt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2taksjoew.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nonbtcrs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wgoqtmnd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2sbfscdvp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2klucjjwc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mooprwnq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ynwsqzjh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mlssfvxj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2feljdkus.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qrrfvyvs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bmwoxvku.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ebyclrcs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ypsfqrdv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2desjirld.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dmpkunrp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2aplhnbwi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mdmumvcj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zjsxiehe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hmxrvyad.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2kiflcdnv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gxeicdjg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uhmulpso.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dsayyzqt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2oqvbzhgm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pezphunq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2safztokt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjsgrnw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2tjxzmjwb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hvyysxvw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jvwxphrt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xbhjcfhb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nwiuvrxv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nxvbtpca.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bswsyarg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kgsgttbd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kpqsqgzs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vtjjvtex.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jxnujttf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kpnyevhx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ftlggies.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qaxpulaf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xlnajikf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qkkifacs.html


<!-- 参考信息 -->