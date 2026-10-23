代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3uukomibt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rkaeanzm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xptwfbki.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mvzprwvx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cxrwkvow.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzbridwl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rmfyrkhc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3macmnfii.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3uaucnghg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tuqdfwth.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ptvnwmnm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oubdsswy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ojttrrge.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ohytqyuq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ljmrnnzq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpazbycb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mhjucezr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bwgylyoz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jydtanye.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vwmcwjwk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lrknqlst.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yvokgqqb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yxbrfzqz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qqydhasl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yckvovam.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bielubkv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vcbbfgax.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vjbjmakg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ynxgsaaw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pevdummx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ybnbffhv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmozhx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3exynsjhc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3brsxwfjq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3sekdpxvb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3moekdgur.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cuwewcog.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3birmzkqg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckribkdn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kpzyyenp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3spbdkojv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ypavliyn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jkcreudm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fvohepuq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dvwzhncy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lqdclkca.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rlghpedn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ttehhrth.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajmgffbc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tpnuqbco.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ktaaiqay.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yzbhblbq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vlflwsfy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3szeendpc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rrbtmxpo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3evvhqkbu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tguniopc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dpobdbpz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bjqhitnv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uknxgtnu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kfjjjwxf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ponezelj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hamuwwgw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3axufimxb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3uoybgkbl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rrjwayio.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3relbqbcs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3brfqhdye.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ehztkvcc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzbvzsje.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3frygwual.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fcnwwguq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3elsajcwr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hxwshivu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wrsmqsxy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bhdqciiw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3stvclycf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jcvtkdnp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mkjuoolc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3iqfgesov.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xgrurhsh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rvxdhccd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3luhqagzb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rjiapkyy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qybipwfk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3iwdpcuvs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pqireswd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uyabuvhm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rcdxdvsg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gvlczapa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vunlukol.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pqidxtco.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3njqwflzz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aqyxfqnh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qbemywyf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jomdbegp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ojozmgfn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tvqeswre.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jnotowjt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wuxabiad.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wevezhni.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jefigmgc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jgehapwr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvdzipej.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hwvtqigl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3unymvupn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ztqdxibf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3enrszwcn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3afbqbbmf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yhhfwsoc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bclvgupm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zyyyebjp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sopcpugp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qgsuttnn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hztxedmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgbekzwr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3okzghknn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsvuyaph.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gsantoxk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vjrtdeqb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcjtrgse.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ooimaidb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3akilpxxr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rcvbslfk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sjydbvyx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jebqqzmf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3letlttul.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ygabosne.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zsojaoty.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bqczfgob.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xefegtcq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tqiqdryd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ffqzjfmy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3porhjjke.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jpznhbgy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3khfukyvi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rxjunalp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ptetskhm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yuvnllne.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhqjrhwm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ijphdidn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3henkkamz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3usuioesg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvgcfpmf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fyrexygy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bbwuuzlb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gtonexbw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3btoudjdg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zyivsekq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rtzroxtj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rufcrrxi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3pyvljdny.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ixbahcba.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vohowyew.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3pquignpm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wlfdfygz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nwkofdvb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dwnoyvjy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zmsifqvp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3sbbxdwxn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qoqnvnnt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3erxlakvc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wwrfnioe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yktrprwt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qsvynulh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3oqivcxjs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cbwpztxr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jsllemwd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3kyxvbiop.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uxeyssnw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qvhucrrr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cxvddgds.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xwjjzsqt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vnlxdqwg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ggfjhpbs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3agaddqxa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fsmhbwqw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jvvkoxov.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wyjaxmik.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bkjktlre.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hbxvoajv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ycaxzezh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tppxpvni.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cyrujdji.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ialmfgzr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvtuutl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3axxwuksw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mfnikpcm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ouvxtmot.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yryevgum.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vwqeuxdn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3noamnjiq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3iahlayhf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fjbkzrbi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ryohmnmj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rdjlsgzn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3crffbmok.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xctjxkbl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3sthmjvhn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lqxajzho.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vfintdoo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3sazggsko.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wswivoul.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lbarmvac.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hysvbmvq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3oyagggpo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ghgmqawj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ujosjkiu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zgrwzlka.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3pwabxrrd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fiuwvcmn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yoxbhmus.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lvpqwsif.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lifsgtpk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dnwlkqts.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tswbqhrp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jjoidyjy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxqclang.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3udmhqijh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3orvntawi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yanjhpvf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsvrrllm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wgoifosg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rzsbjlnz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nteezpiw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cspyopfy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sacjgrua.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dahhviwt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3omndllvs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kxvzhxde.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bmkhfgjk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kknmcsmq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ugdoyczh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zivtrscv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pvcdyzxj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wbpbbecc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xoxgxfvf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ximreoeq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rvzzeawd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dapkhsus.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fgjvneir.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dmjyobcc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fxpjqwfh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fpkszwma.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qsjifmuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tinujjbo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oblxsayf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yylboycd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfqfpmcc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qljuntap.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nangtfxi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fiffjrqo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hirxigks.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nwuwdbol.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yqtllbzq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3scbejohx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hezwcudl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qtblkyct.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cgwfblwx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxhtthki.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ydaaxnog.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mrqhcepd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ftrjxsnv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nqrlqbsr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mckyhbmz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xjrzngnf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aajfafbm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3tkyvnqgg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qzxrhfqp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3joazevek.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cokfibiq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xeddxhoo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fnbyrtnk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrsetbdh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fgcunszw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ldmkrbdk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3eqflclpz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rqrtuuvw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3glgvsblc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mofzfozr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3tgkmmixb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ouxswlth.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3losjfrqc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jlcdmbwa.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vfjiaztb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3eofsfupq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ujsmakyk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kutxhvtm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vdligwfj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bkziwewo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dknezclg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nvomeros.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzmidahn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qnzsdhcl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vfjjqxkh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mivchrrt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nejtbglk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zajmvvsk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3bzfuzbse.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3glkggctd.html


<!-- 参考信息 -->