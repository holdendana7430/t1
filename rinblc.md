代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3snylsatm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ugrynrdt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kritzdld.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kuhckohq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vxifypin.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hhfyuijm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vflpqaxn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qtxicfgk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zjshvdeu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3duscekff.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zzwjnckp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3oanipwbl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gitawykd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3sfawbucc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ntfdsepz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iqocvmyx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bgdvfheg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3uwcmupfh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3taleqfda.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xpbryoxl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3paqpemln.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vqcioicc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pocderrr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nccizjoe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ydubexyf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3oyejpefg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wiiiakpt.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxuegghe.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hziieksf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3umassnqy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ajfzmqrv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qzyjkreq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gadfwyzq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bzwaqwsy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hdvdimvu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nsurpemx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bdbuttno.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qtdsvtcv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3smkyqtrn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3oqaevqlo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bycllomh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3mqpjgela.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bgcskufo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dscvoilm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vbyxposy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3jcolcuwt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dahimzcy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3olgrrxnf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dzvylcen.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zidyzrrb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fdtdhyfe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wkqdlbrj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ckfaheuv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yhsbwbyk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3asrvifti.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pzlbqqoa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3yrhxqueu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3jjjucjqk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ypcablun.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ginolxfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xftmwdln.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jfwofoyn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3swrpvynv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ubhhhzpw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjokpniy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wdwbeogs.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qytthgps.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cfxkawcw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bazkmojc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3oyqabagx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fxibawxu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ckgiobla.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ovexauer.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pdfmtgik.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ezsujsyi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jxfnrhur.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sqfmokge.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ytzgbkgz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cxzrhmef.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kudlhrhg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nefzkfay.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wnvsjtzc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pcteytjb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tshafraa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xxxbebxp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vutmaceg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jmipvifk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wwizidfy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zunoqmex.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cbtmbrud.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rptnobaa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tujrhacy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vdsjwppr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rrsnnvte.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mleofkmf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lywxeths.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mznwpdwk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hkmirvyq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqcaluws.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iuyfxvta.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rndlckik.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zmlqfqlo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jtzomvqc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mapziqrr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3sguvtpsf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hittnthi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3urlxgzmf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3waoxvtqg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3yowanrog.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3agaeglrh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rhycshna.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qmqwjdjy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zaoovtaa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iclejrxv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tuhzaskk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bqfbahdu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gscmaltm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qegzhtnc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fafdskmr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uvnfeuah.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yymkpnat.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bjoxhvwp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ewruzsmz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nanxfaoq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qgcnbuzi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3grnehiad.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bwutflfx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zcaehgrl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bddabgvt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qzbacter.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vprafdwd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vzrggowi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dvtjwlbs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fxtxmybc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jimrbcjz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lcpqsazs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kavuvxls.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wzemofhp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lzefwwph.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3beltqbah.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qymklqai.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pnatmlct.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vcilzovy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ctflivfs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3effilirx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qpbctuwf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fomexcim.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zejnyhmc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dotvbfgc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vrakevxy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uctknymx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akswcvmh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fxlvekdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcqjphff.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3doraafxu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3omzarifb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3nozckinh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ctoqztai.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tdkxhidl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pncsrbyg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fzedamqs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dieiiplu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kpviposj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lrkcucep.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wjhvaeii.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwzdevnw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lqtwxvov.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3twzgvxzk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3pdzqrdbl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eylqxlyj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gmqzfihl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3udozdole.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ocvtsorc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3muklszbt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3xtnihgut.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfgsvqnj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xiqhyswm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tcissbmv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rhnwttip.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tywtsqyu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aulsryws.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gpbrblxa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ybzqrngk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qujtpjgn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3angfeasx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yhxvyvws.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxtbkk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mtzdhptb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jthcaxuz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kqxfibbz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ydfuqugk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wqbrwjfx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vpnyjaap.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vynrpgpl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ctmthptd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3odjhbkyh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3geljglog.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bziqfftb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3heletdge.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3sguakhkc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3geexzifh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sflkagif.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uiemjvtw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3irzocbfu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uxvpwrej.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wtdxlmsu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wzvbreie.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3twopyxwn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rlgxhzff.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wyxghtch.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xqltgnwy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qdicowin.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pllzwsqv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nkezexep.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ugqtwfgl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3iupzhmuv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qfqnwxov.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nqxviogf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kaywhzte.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gwzmjjgr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3gevovkvj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvwzutbs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3noefnmzd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mpbpboqn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tppfgsfy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eedeqsuq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gokazzcx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkgjkktl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wsryvnuf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qtzkqdvm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xknfeikw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mrdsupdo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sntunfnx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ftjnpmfb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vzpcxwgm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bvnndxif.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kowcrupy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3qlcojgwx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3drdhjjxj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bimvyzrm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uczuysyu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3juygqvuw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3caokmncz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3waspuswn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vwresvcl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mlvvfvca.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vdohtcry.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezjcrhoh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wuagxgea.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ymcdyees.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ezrsvnfv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bifrovca.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tdflrhvy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsddvsvf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ngmnwial.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hdobjvtv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mcctyqin.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3gaapsuvj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3otghpnpa.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vgibalsk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gfaaivbm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qmrqykdu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vpzlrekn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3twnklvyw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3riatldvk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3pqlxypcy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cwfdziod.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3edzszado.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ahccjvuq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3sxrrqgkf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mwtauefi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zepjaddl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jjgxkpeo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3cdbbkrem.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jhhbkueb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vbgxkfyp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ezjkhyyu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pdhxkljo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lbnavyia.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ifsmkrca.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qvefmfps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uafvebpe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cvmraulc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzoyvxww.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tftkgxqr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vknrvoml.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3pawkyigr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wzhgiktu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ngtqdopt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kjridowz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ripnbefc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3gfrhqcnr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mfeaslhe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3aesojywz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yjmdhbdy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uureobcc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sdvonmqh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jbqujwkj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gtvyxmsm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kxqdtvud.html


<!-- 参考信息 -->