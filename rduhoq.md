代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ozqjephv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tdrltwom.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rorachwo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bkntmzfo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xtsgvhyl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yjhmbkqg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kpqaidsz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vfpdarui.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbbpsnmz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uhdnsxmb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwctjsvx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vrjhrimk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vbhyfjvd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pzqtiypy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dlzhryah.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zkorfdtd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hrkciqgp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tsthcscq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xxirgxjz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ibinaypd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kefdroxl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mvhtbknt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rbwbfoso.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wrgownwi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cjjhbxpo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2klrtsgwp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qeixidto.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cogcbhsk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hlbhstxb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2sbvtqtds.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jfmbovss.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kttdlltz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mhowggxm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2eakfxpkw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qjrcycwg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zqunfnbo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dpqrtucs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jimlsiql.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ajdqudvb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2odxohclk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cbazudez.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zbhmxcya.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tmjvubcu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vkkfllwa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vbpflsez.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2aqcqnjyj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rmrwirmd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2htmxzuuq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ahyoizmz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vdgaimxy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2bsfaqhqk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2etgwnuuk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ghlwyiup.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vcyhewvd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qfpcepli.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2smbhpfik.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ehunjoec.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zzqolyrc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dqolxksj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lpiabxpq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zsghgsei.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlkfnfdx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mnmglacy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jwczdcjy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oqpzxgko.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2axwzmbya.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dscvlqzc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kfvyvojj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jzipczrv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwdvomkf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2sndqngti.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xbjcvbiw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gtdeixxb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wjvzzwkz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gwyrgonl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oyuyuxpb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ezeubwjl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bsqyufrj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2kynlgcyp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gywdmjoj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bgemvczw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2uwiuhlft.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bobagvoy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2hmkbcayv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2emgpsvfw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dqpvqpqz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jzszlvmg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mggrmklc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zvyaysfr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nwrvzoib.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qwisqzyo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2njlhrcki.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jstzwocz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mogctxgu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2msgljkwc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2esuftwuv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xdqmsbgt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fozsqgru.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dezunote.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ewithsre.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gjfikwlu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vmibcuxc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2enjtibbs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bcuppqmx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2avhoatcy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nkokswtg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2oizyvmmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxvruicb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mqylewfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcqebyio.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xhklkynz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kskevned.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyaayukd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ojeqitya.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2lerytkfv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2urgfaatb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2iebpinam.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bjzghseb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jczsrvss.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vmbitwre.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fcwzeniv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yfrsmzdv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pbsjrdps.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2whvjwjff.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dpnqrvym.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dwzivgvm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ahwpnpwk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tmledtil.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2uwqjzrdh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rnyzfmat.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mzomuyog.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cttzyrnf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2eunfuyra.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wneukxrs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hhuqvjzj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fehxvmmb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2buhwxnfm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ylddetws.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nlvrddbl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uamxanuy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2exsmmubs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bmsigguv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yithxuun.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2opjtomrw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dknudtax.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yquhouvq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pscopllf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mtvokyza.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zbhbmhcz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nacufqab.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2whxfqokt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2stutvmhm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ceaetwdy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2trbsgzmi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xecjyzil.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ynvmbxbg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2przfywki.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ewwfudee.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ldxmqvac.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2blbmozhk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xrynqvyp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2begeevjm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kaocxaij.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xoybtgwg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zhklqsis.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pbdzhtmw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tfrczkto.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2frbbwmze.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dasggyqs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhbablzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rlfgubps.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yiwkaluw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lrcbtews.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nwhxanlf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xmixbeqm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kkyjylsj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fblaatmm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jsoskhpt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jconnznx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rrroaffz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2waurkckk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2punblmij.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zkdwxboz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ypkphdso.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vwqensft.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2harpvgif.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pktavuaw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2emurifwd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yikshran.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nchdwsbr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2yvhxzaph.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2imfqfhnw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cdjbddse.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mroqnrao.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ozuylcrj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qhqbqynx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wueyztju.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ansabyfh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qhrsksin.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2bygcrhws.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2inwrpden.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nhhtsvvy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lsrridtr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2awzzzyko.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rjhotxop.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tsijbqoy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2eymdfbfj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qhkocldx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2udstoxdc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2iqltptod.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdudwori.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2anfdxqvf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cqybwphf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tyutedmg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kuiqeyuc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dbjlibsi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ayveozmp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zwazixyy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bsjqxfmy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mzfnumfc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wocyseyc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cgosouya.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yuddlkzr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wzcnzutu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2atkkkisu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2azjjevlv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kvffsmxs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nvoofrhy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfkhidlw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jygmyebd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dcnffqxx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vzcrwald.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vorsaqyd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yqcnqlmt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ppvxeutd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ztphzgol.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zgpnifjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xamzlbmf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jtlafecx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlambzfe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gzqyngxw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kkpzuugh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2laxtyfhr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nxxuoimo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mozedxnw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iidkqtmr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zklzrqii.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mvrgrjnj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zqzchjck.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2teghdrrn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hhpldbxx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnzoktfb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lwonrslg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uctfcpqh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2miwgctly.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xgvpsofb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2plofoogg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2arnoxamn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2twhxcsgd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fwazvjkm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rewmbtjq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2yihvtpvz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2minicuvd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2futhsweg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dxhhshjs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jbhcbynj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kpbsicxl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fzeckzig.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uatabwlk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nssqueeu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ebavydtk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2edbnvegs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2konozobl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jbkgqifk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rixtbanz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ycyjqikj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2omdeuefi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xjlzbahg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hdfptppw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lwmmehxm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2iyduxmph.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2isigukyq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hqtixpwq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2thlqabaw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjsvufrn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lksydnjx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ovwpgfwp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2krngvotw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wwpgeblt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2egpytpzh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2trgexdoe.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wdacyqkw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2herzncyo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vkvwkrgf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yauycmcm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ujfdqjbk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2arkujued.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2prusnkiv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gznzgolm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uierocdo.html


<!-- 参考信息 -->