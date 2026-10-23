代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mjnsqwtr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3grcjnnct.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pimwjalr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dzdintis.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pzmgickg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljkynsni.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dbsfuemy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jikzxzhn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vuwtuqlr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kffzghmu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pgvzkkhv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffwzbypq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dynvudeu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lyvfvyeu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yhxtzqni.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fnaalves.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qewdoros.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3uqdlcaxl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ewzfxpio.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rdyzbgpe.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gbmwtwjk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mdhibvna.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfzicqgl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3guequffr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dyciwqyd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eonlvqgl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wuhukaeh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jitrefml.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3omjlmpcn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fiqgorag.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jdgzewfc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rdfpkzix.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ogmilwmz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jhzmryur.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xuehxckh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rkqswede.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sfrpibeu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3txdsodvf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pxstexqm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhuoftgg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3axdjklbm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qvfeekkh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lydonpnb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3adefbesh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqlvvrbk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wizqjzqe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3taadackj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3izsznagv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zwqffmiq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qdzsptrr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ocoueehp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gsoomwtt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3haqvowrw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cjvmigym.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yhnfgtow.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vturrtkc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmqnsysj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zcvgfzse.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rxzumoch.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ezhoofzs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rwrcrmmb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3akmawycx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3njmyunzh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3njocimqi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dxsiwxzk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dpeyebuj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zvnienmn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ebwnjsht.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jejxtykn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3eteudxhm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fsrsvilc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yztiuuuj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xrkflwsc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3efvesfkt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3namlkhqn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jcionppv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ypusrzuf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oelyvrid.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vybpcpyu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3avxitbif.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dbkxdqub.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wmrrxzhk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wvyctncm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mddqqmeb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hmunfmkg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yajpicqa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ojeiidqq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3iaarloss.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3kxvpcvjm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3irdmebty.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pseejygs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yluwmxqd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jbpndmig.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hmrojryw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pswzwekk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3cgfeqrmw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kmxjytbs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3smfystik.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gkqpgagk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ityculhg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iggigtue.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hilavlmo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ysnfndjv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wgmlxnra.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zrljuchc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qanupbru.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3twslpkmb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tkbvjlaf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oippljcg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rqdaqqes.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tahvkpqn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qqmaagxg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lvcpoyft.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zbcdvbkt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3udquudyf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3navmpcff.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3edutytve.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zrunicun.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ugmcfdgm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bsnvtlyy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3npbjegyn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ltznxhkz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3yeieujpp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ylrzcgcs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wkezbbdz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3gazcbeut.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hiuwsscp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ddskoscj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jubslsqp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rrhyovag.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dmofacwx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3frkugcnn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ihhukxzm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxbjocye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hwonohbq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3icrbmxda.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tucqtdks.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3onmjvtyh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xvvdjzpx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gxpskpid.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dlljkwix.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dkcyitrc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3omwwyqrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwfecmex.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3plphpvak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgtaqctj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nvasvwmv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fyjbnykj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pbsloodz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gwpgbtqa.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3egznhrgk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3teixdkol.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3balnkgxh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3htlfnysz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zgbuhwts.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ksejqkxo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3riqwrmfm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3samdgusn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3begstpnt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hhqfbjgz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yavvtmhn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qafrqzdo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3txgfsktm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yevmgddn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vilvjovd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ldpgtdfj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rzctulxa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ydluizpv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xutuihho.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ckzstldr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3odxeenkr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhdmzayp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nedlsash.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bokqrvvx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nkbtapyi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xgvwnmbb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lpioxvjh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rdejjicy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rjyssmty.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wcpokzup.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lkhcxgnb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ycefalcn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qcyfbzdf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dsqcdram.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tlmwtafo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jpgdqpzo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bemnruru.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zaeeseiq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gzogfhgk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3iqsraepu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vssnaetj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vrsrnxwn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uampoixh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3llvznoih.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hdlnjzsx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gasfhwsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3glotuwgn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mpylezro.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hvaytqlh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vqzklcff.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3trwwvgnd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zxwombeb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ushjqiml.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3aickwdpm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ygqfpnui.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxvkjyfk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vldsjbbx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3imykjnhf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gqemzvio.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ulzbvsxq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3egxhjgxo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fhisjtmm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rxkwomwf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsdopayu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cczdfuxl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rauoalof.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fyrdibgk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dwjdiyuq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tnnhmrtp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeqwengt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3purekhnp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cpfesnkb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mrgzswuh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fqluccrj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fdaurqsc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yzhimium.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rlduwbie.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xnkngmkt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bxljfuii.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vhkorkzq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tdecvxuh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3etvnepfa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ohlbjbka.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rkrisusr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ihrjoobo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tispkidm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qidktkpw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jsnoxsne.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3witazett.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbdzxz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ddfezdvc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3duvurbxa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zwnlanli.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cmaydubv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tbvofoay.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jygfpisp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3veprslpl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jdfnulrr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lcbrzmyd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftdalsxw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mulqjyfu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vcbdedbx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kandexjb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ffwgxiqh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zdtuzkbj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gewsdbsb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxzarngl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3witeiiyh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yicdywtt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ftmbcazi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gdnrhonl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cmcicrnf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zflapcyn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hvlidwrk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oseqzkfi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3uqfpbcfd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xfvcitvf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tfgypuii.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bokfotez.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bmssriei.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rxpiwhjh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cgeawngp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sspjivis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3essysmrl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3opekgdvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slvbmlgy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3brjyhwmt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ggjuxacn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3uvsbygzy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vbctbqzl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nyvceyij.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uupqkpih.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gulirysr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dfuoxjlr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oiothlty.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3uupgvmcc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xyautokm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oiqaztfg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fusnwoqm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqpzyipq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qpphqspw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nzklsnba.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxijyxyt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bwspfqko.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3btvhksdz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fastglyp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3poujcwsc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3azhimsfq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wlwtyiew.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oqewpvrw.html


<!-- 参考信息 -->