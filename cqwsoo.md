代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydafkkma.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kytxvnyk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tllvhdmm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3smgfzmms.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xwxzfhss.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xubfhwur.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cnonxjkw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bcfzigqj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdpsyqww.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hbdmukfd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3etbotkbk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jdbqapbx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jjllotnt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ppawavds.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3iqpjgkqt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3aedftasz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3snqchkrc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jmdcivvd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lphkimoe.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jemkypjb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dusupdsr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rtyicxef.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gjbhrrnc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3srnflabu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3umoqfibn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3auqjrqoe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3blyyppzp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nubqqcit.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czemywkt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3anoitevk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pexkznys.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3lyvlfwfq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ndghkbjy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uciugdrn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xmduidal.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3muxpqrxl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vwribnox.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nmbxqyby.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gcomvjqb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cibompfg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwkaagk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zckmtnju.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hlkkhhfm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3khsahwtu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jxuqbjxj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pqwjlrql.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ccecnsgp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ycpmhmsv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lyhrppoo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zfdbmibj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hyanytuv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddvduuvz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jheejxpf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3auxjzxsd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rdyyyyao.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uyaohbxc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mtvfbqug.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zumwwvia.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cyqwsmwm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xvlqkfkt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3umsuwexl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3evwpjcpe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3axtceqyj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hddlscsl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3htrqruyn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kooletsu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vryjbjoc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ulfuwafg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tkiyhmwq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yayzbsgp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fzgbvtxs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vkpexjsa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nfjcnccz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wvzimhte.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mpwctqfu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pbfvgaxx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rvcpiqgd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3csmgengo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vzsfeewm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bddrtoqy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3cfampicm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qgwqolkb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pmdnqxfv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bldcqjxs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xwflvumr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ybakawdz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dqlvwkme.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xlbujjvs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xlbferzp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3glqcjrdk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nmrvwmfy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ewojindt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dpmoesza.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yqotzdvh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3upuuxgzn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3jancuzte.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ohpaxrpg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xnjkiltp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zdjpndkn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nduxcdvn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wuvuuieg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uihrxawl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3koaskeoc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3roqlzobn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3emffnfvt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3eylnzhgv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ecyfbyhb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nnmqfdhk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cbznaysx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3eerwdugf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ztmwndnu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dxooalzp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rbutikdn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gbrgbmpb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gzxaxaem.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ktcyfenj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3iiwngaps.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bslcdpnn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3luknehwc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3eubtdsfp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vxcomkpw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gdinsqdf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3tqekzyoh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3uheiagch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fujjkylb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uvfzrzls.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kgfkxcts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwaczbrx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tqeobtag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsbbouyn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sinpqluo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3djkurcat.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3asckzdrr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jbqqgkgq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3asvgvufs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mxfsewqm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dxpnhvtp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mfgkzwek.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tuzjrwyi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3porerkoa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qlklsdzb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zpdwryly.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jidzzekm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tkctuaag.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3aavlwdbq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cqauyupq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qrsfkrru.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hxtpunsx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vgrfsada.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dynqzube.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ifrwqfry.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oceinfqb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zohenvpa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fplrsjrk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nyipywfg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aibdflln.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qazcikzj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ntamzkmh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jsxkwldv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3owujhgfv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tpjajvce.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jjfodjqy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kgohddfk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wgmdhdee.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vtwxmfqk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wvmmmwqk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mzsqgmvl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3agdvdebk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lhwbhoof.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cwtgehzk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kyyryxpt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tlkfqzit.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qflwscjc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gsdcjuua.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xeqoyhvp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kgjnrmeo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3khbudatb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hxugvcbf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gpmbtgxe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zfszglwk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ibtgfqdk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bivmoxww.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yjhvxglr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xdpenvyb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ewsjbpra.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ubjnbizv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xdyaivnk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ttvrdlwj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3whledyhf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqyzdffc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gsczouop.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3smexplea.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oetqloqd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lurmyinx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kgacvflg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pptdrqhi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3poejnmws.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqpkthpt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvpgiwna.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3amqccgaq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hhhbbdow.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uzvtwray.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yvpwdqci.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqleptad.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mkqcehhp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kkrsmlrb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lpdgoxmc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qzcebbph.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3atwulzhb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wildkzwh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xymidblk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zkticnim.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zqqevaog.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nvchsdag.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ijyauvhr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxqhpzpp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3feuqxpsg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jocrsnpt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ioxjazdk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jyftabfx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hlltcxnr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3syxbunfu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gkpcxlgv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdeilxop.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lbepypaa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bhxeofnc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mvjuejjs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhpnbhkg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yeksuisp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wddspvxa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjbtzhqe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ctenbbdk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3puyutcrm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhnbmjex.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kftmsbqi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wrmofdbc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kgegxqvk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3acjmvtly.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hwfvlebb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tetczjyv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xedvxabd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bqwrylof.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sfuttemc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tidsmzmq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kolyzshy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3scecmajh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mvlbvzom.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vnragsuy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3qpiueqvg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qnnaaled.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kezorvqx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ecmwmcrz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xwggnaec.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3joctwhla.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bdfqkccy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lyhjnnpq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cdgwspbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjivlkql.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3duhxsoiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyxbwivo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wmokdlth.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ouiifbgj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wnercndo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3acisxpjn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bmfsknja.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lmgwxmuz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rsujznyg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3eidrmvon.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qmxwjwta.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uwvbjsxs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yxgoxtxb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fmufpnak.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kudfegth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vqxyucai.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pmvmuctd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xcqmkacg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbgawe.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qjxyqiiu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyxxqgtd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nmklxegr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pksmgcjz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ucizgfht.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bharjuwg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pweopisw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cmnqwgli.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3svmmtree.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bvqxbsxz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rirvzxdp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fksuepls.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ftztbdts.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3agvaygrb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jzozuizt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xoptckdj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jteohtxk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mqtlloym.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nzynsmdz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ncdmzwjl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3szhzbuqa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kszskyny.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mngmxxug.html


<!-- 参考信息 -->