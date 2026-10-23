代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ftkmhcim.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dlncbcrb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yftqubjn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3twsrvbnj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rtcfvgma.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qqyfvowz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lrbicyat.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3csjfuwrl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3grmrdzmh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kssvfpbi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vvbngvck.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ilpecpup.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zyqsickm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vefsuwvj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gcgnrzow.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3emynojmi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zvzhtzpe.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wledsnvw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3artnpuaj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sfmcrreh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fvbrdisc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uwzwppny.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pouhzyza.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3voikiuhh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ukyhbbng.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3disgyiba.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3akpiogow.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cgqyrxjz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jqxtfikn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jnqkrfzn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xzbzkhdo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbupoiss.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3leeqpany.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dhwrkzdc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3aoqghwep.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3huezzthh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3frpylwtm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3edlupivr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3werqsoil.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3btkengla.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ocpjgnzw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3snxhlpfr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hnpyedoq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vilusmwg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3shodcftl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tadqslat.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hsppjwcz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ggwgtmzi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bnqjgsqf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jwoxosxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nuzqudog.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qqwwhwfy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lawvyvem.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rmzlbwgu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irzfpmlv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mvxqhmlt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fvaevvdi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pyjxulqm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qilwtmgq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3agywxtmd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pztlvxwy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ugkwptzs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pahjsbag.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yfdbrmxi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3yxzyuhbg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3chbdihmw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bmudgamm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3uqhvdizb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qdrzircd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bvohbrvt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yewnvpgi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3basjhcvz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rydhkbsl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqkqipnk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3yodqmnge.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ortzxkfl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3viupkabv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3krocrmiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3eovirdyf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lsfcmzij.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mhogdsle.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jshukvsb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gawcwwjh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zwrhfqcs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nxwynpia.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ycnsnfek.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3znfwveij.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mjftulzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hvhmsegd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wuozfugb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gxrgdiuh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3setumyyg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mwilzmgk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uxkpmyvg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wxmetinp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3spytrgpp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cxsvnajg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3prleeits.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jivztpgm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jsouvwag.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xnkgheeh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vfpswyzn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fwlqgyth.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3sznakftu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ifarnxfw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kyirnvau.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wqyenkbm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vclylnzs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xmovnire.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tlwikszt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gyemqaol.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ksfhlrqh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wxjmkcuq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3trqaftmo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jrqqkboo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ffcelcya.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fulkjrdf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3iumswuln.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uhseeejk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgbbznli.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ipdnfacr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yimxzvwd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jxzaliiz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3enjnmtrl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hneahvfs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mxtyznry.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ijtvxfvp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nbhalsjj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jatsomsu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3borzfmla.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fvvdokwx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ydvuyuul.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3znsqbhgv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hypvkbpx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ggfrqymh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zdhrswai.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hkzxmsvn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cjegxveo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pexyxnxx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xinoqetx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wqhbyizx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3avcziyls.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3oftgxaje.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wimhtcym.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vsebzoid.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gpphwcgy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rqimvyhe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xznuyixt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zmhrvcib.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3yuxlhhms.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rxiesbrv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3irrgzjup.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fujotzms.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vcnybvns.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xklysyjf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dsikbaii.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gidcxdtj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sveplrnu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wshbkczy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkoaingl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ssrrpwax.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fgmdnire.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cxjxlgip.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3odbabzcc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ekgqnhws.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jpwymhuq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3somezcsn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3icpmyrmm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qnbdirfu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3svxpjnct.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rdbhvsss.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fxtotxsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3joapqyiw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zjijjkjm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cyutqxyz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zllkkwfw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dztjdnys.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pagrgpht.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3talpkunn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qpbqvosg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qkledxtx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioenmfcc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3asuzrpnp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3almmnwdj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hwisssqh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rtgypgxz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dehlpeuc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rkefowqu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mzfjezzv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzeshral.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3scplyvzz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3evjqwxyh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3habxxrue.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hwbougtx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lsurtxdk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yaidogas.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3yxgncuwo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3meofqlhp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cvyckwwu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lbktkqyy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3asnyeqmu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zubvffwg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ckdtbxmz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fyiowofe.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ehoyebkg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hrnkobji.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3jhynsdtr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vajhdfqx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nivmjsvn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3giwkhlnv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3eyczmmeh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vdjgonvi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pzsjfxmq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cptkxgui.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lgemhmii.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjymvexn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kkxklwvr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zmfxlaer.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hgzkgnpu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ekqgzvwp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mprjnsri.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkhwhrwm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xyreschw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qdlqzesg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vanpxdzj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lsrdbbgw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kbzzsvwd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hgqrjugs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ascnjmfs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nrriyqjo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hzbfyspk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3sfpcroem.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3axjaxsyg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nfglynjt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zutaeext.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rtjnmvku.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3snxshodp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3asgevyrd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yxumswcu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zxcfymee.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ojxbcptc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bhetjmvn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qqpygcol.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qgjbjqos.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mefxyetf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3eqycqzng.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3gyxjeizd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3btgmuhoj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qoeplryo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqufmtib.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hndurowv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iopsadcz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3inpzyvjd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oiqqpjri.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ysovuzxy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vdwifdal.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3jyfvijyv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xjckwrnb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fhhtcbou.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xuworzpi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nkfrsxlt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jptojtla.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dpxfgcit.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3thaelftv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gogozkkn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3avgjyntt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pxyociwg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxxfaza.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdjjymqj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bvxbmaqb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lbikbifq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3tsyygfhv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gzvuleea.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vncrcvao.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fbghoxcv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gfdkzayq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3swxmtpgi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ibcwmoto.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3czxwluvo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eloeyulz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jsvgebua.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kcibwase.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ywyujjbj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tvrgbfsb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3phvphezd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3laetmcjl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vcmlthqe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3slbenmdu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nshzmldm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hoskumlb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wtgvtaqs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fpxxlopu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qpmqxacp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3txzwwpmo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ujzhnazc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3alrmqspx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hhtlddxd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3euuzcztt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xpgqyuiy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zyzibxog.html


<!-- 参考信息 -->