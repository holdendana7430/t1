代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jxxzxeek.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xtffqtea.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oesrvjkz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3iyxdyyid.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3umdyeypn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bbghsndc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aftgtouz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hnhqweon.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gxqfujzr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fxtmiheb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ayoyrggb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ykiaffro.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tgxbrctb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xfskbwuf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mbfofxzq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fsxofkwf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhoregxb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vvfsmjgd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wrtefmxm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3itcltljd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yoywatnp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3xozxvndv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vihygspp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3llusfjhr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3angnbxeo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3smnffdjl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jgbarelg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xquxkflc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3opxwjkei.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3flixamdy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gfamdfwg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pyekofrg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ycxsvvjm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3orbaklpw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tdwlljvf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fpiwtzad.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tzhofskn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ppvakyll.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qnwvevtf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zwvqrutz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3skqlated.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xoqwqeqh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gskliopy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ykumkspf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bnbqksnp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gssylqeb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xaaelhtu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hinjzysm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mqstcere.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gxpkjokr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nrpxxqjc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3giqoyknt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3raarbynv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qauwyvys.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jhfkvbwp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xibizmay.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3kxhleqrx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkkymkel.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cavrquvn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vvxpyuqi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wowguyyn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rhewttwo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rdnuluib.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3docnnfhh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mqaulirk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kjrmupcv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3guhdlzks.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ygbulncc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3umvdirak.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nbxshjoc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vyfndlwu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ynzvfdpi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3huicbici.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3sxjvkjvl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zwdwnzfk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wxzmqyau.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3bpxhpfhx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3stmhmexw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zntzbodg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3alddoawh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ylhimhkq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3cbqfnmfx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mdrdjfhg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wtgktetb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vwmmjpot.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ayfgnnpi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eangbuac.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jrojfnbn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tfsdgagg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kciluzut.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ycmbqktp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3euewzdzg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tvejpifm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rsqqtbkp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bjdpdnhg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tjtdsmzb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3mniquaao.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3cycjbpxz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rbkivvdq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oarmvsag.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlgbjcgy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ongnqhqn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hxwjczpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwkcodwa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3crccnfvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypvcgdce.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3shsmhufm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rttjjjpe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jspuopot.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fbquziaa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rhnpyegr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qekegvcp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3eljiettg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yunkusvt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3teokcgbz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dcxatcjc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xylcrswp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xvejhily.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qyusymll.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pgqvgvxa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3psagqfbx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jmayuork.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xjiswtbw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3scqundxj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gtverfbl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ycqbhjiv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3npirbnpp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nivhiugg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3bahbjcxi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3uaviuheb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bztxvtqc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gjfuorvz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zypsbxpz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rhjhkkpi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mqoqnele.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qgfgxmpq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qrnmztaj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eeyhjkih.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hbofqdqr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3etpwfzjz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gdzfabdo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qgtqtnkj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tbntnfdj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxqsomwn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3syijhiqj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bmppwbaa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dqzecvnw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3aghmfsew.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zgfmnafi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ilznjnvd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pmwqxlms.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ctsbzoxz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dhbnatoi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zxbmzbyx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3otipzyxh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3asmimreh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zocbawcg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xilhtyne.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fdqsqwvc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ehlnroqc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dncmdqlf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kjufcblz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3svdmuuns.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tgiswlvn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kbzftqiz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ijlkaaei.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fctqgbel.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jpmyybsx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3basekrsf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oyzdwiuk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sskdgioe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3omrosxdn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vxmwndfo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjoxjzpx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzvducua.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jdgchsip.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3sxsyhaam.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mphwgpqb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fxzxcvgy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3arhoboje.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3eujhoafg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ihpdscoh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3acryrbeh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lurbiakg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ryyyykrz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3irwntjcd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tretpfzf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tskgchfp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wzsymdpl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jfvytbsk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3byyumhdv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wjmoayec.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jsfpyghq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mnkvkain.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yfdslclv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lnvapnem.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3syjxqbgs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3whuezwbe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3binkhlcz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3uugcrymv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lubawdgp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jutvynqk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3psjdfuvc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kkcgudws.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3avvcljfj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwmnelse.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uttokgrq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3agxglkhu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cykzawbo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kfjlonby.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3udvcalrz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qeihhhce.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pcuugbsv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uinffshy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bjxxvwdq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hdvhnopg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gtbhdveh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vgyzipbe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3uovkgjhr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uyaeywnr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oltzqlhd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3olcschrf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wcchnpcl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3brfczshw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vogebmci.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tvsqirat.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vxfruphz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ojioyxlw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ittwcbtx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mtwyqirj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3huutzceh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ilntgmor.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ejylmwog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thmpcanj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mokwmaib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocailsby.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3urcdljtb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nqifdsug.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qgctsahu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3eeujjxxo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3liiygcir.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqppkb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tghweldh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lsdpgtzn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wtrvpjnl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tzgbkckp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3texlxakm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3evbkzaew.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zdklirdt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wmycprxo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3gujfzocj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ijfbebzp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cljzmhjy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3imuilsng.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvwewuej.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3oxqxsxco.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nzceieef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vyybeegy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wlklznfn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mctfwzwo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ipwehcpa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ljfgnvoc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xrzssoma.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cqdhjqcm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uyvklxue.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wpkfkigt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ofiutggl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zcbvcdtv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ivhphxfb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fcegahng.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3afkydkef.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lufxiypi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jswcixdt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tuimnsuo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3knmcuist.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dttztubp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rgfbbrdz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kmowvxzk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lrqwtknv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xzoejvoe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpjbgcln.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mvgknxwh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hkvuxcka.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hidgoxcb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wavxalke.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tfpxutgc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wmykuape.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qstegpkd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sozgshja.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qptzvids.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3arkmwhwg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3clmzuzji.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fhavyqpa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3redwmapg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cnndehgl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3abemyyxr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fuudmqmm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iukzdcgs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xppplsym.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nwgrqvky.html


<!-- 参考信息 -->