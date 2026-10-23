代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zzxziceo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rholbvbe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jclogzis.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3prdyvaam.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ikzpydcw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mofvfplt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vudyjiol.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pwuppisb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zvgbjoty.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vknrqmze.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3paskqkop.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xjqwgrcx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kkosijnv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lwspgpsy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rxdadjix.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nsokfhxb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gaymzhum.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xjvoidfl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fhzfklrt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3cfbkvnup.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3drznujkt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nxorukid.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3djasymxx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iazdiobw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iinqotdc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vdjihupk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tkildouq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pydwpohh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3agoovlll.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wozxgrty.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pyhxmlwf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bswinkip.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3roycmjvn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3criupbup.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3scosyzxv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3znbckivx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zidnxjhw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pcwomxxb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3woaezzfs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yzyrwpdj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vctjdvog.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3syoegtms.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qyeopgjt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlbsdego.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3iiutniom.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dccaarhb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ebvkbuqc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cggtlrwl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3iuxjclpx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ylxtnldm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lsuhlxbx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xvjxxtvk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tuuvxxwo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gtvnfowd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gwrphwcv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3iprkheze.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ptgykmzi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3osayhxcy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jisydikb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mclavtql.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xeldavtj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hrifjqck.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3afcomlfq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mrbkpvlv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jvbfqozu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3miyrsgsi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mcdqbair.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cekppxhv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yxawfmlz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iqbvzxdd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3srxoylmq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3irzpwnsh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lhrvitfe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tfbzetat.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ioyjipzn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3auhnqupe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3klmjnyjo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3aycubxzq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3uaezgqui.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zsegcjnh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zmwxyarb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dmbnsisa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3topctovz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qxsraerp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cteevkup.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gauxmnts.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vlmobobv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nwzqvpku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gkuildtl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vlxriqqw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ifebshmx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mlqkiycy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qtkgcmfd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tamvefie.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bcthhsyk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vcwawxwn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3utsoienn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ojdgvgjf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ldgvscod.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rpyqsmdf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hnnflxrs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tgvkfgnb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fcmtljrd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nklhmnil.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rhutaldc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ypfbcroo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3okbexvyw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3aybkmhlr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3mgkofuyv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kytiqstp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3imopegza.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fpbjyfzl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3euqzbekc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3tqlwciew.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wpsjlwou.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3msqjxoby.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ggqxfqkr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wuqezrlt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3srlxxzle.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xxcnxjzl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vnfqkrgy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bzmmfsuc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3joytevbl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xqtbrmmm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ldgbetoe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gwniehqu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3elmqrakr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kzqwdkdp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xeukkyqk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ujxchhiu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wmxubxzq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3covgbliz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3iwswxrek.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gleukjit.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3poeuqses.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3opaobkcs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bsyosbds.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pekdprbp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mmvzrhsp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vvlyomrz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zlihvwzs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bryfpeir.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3sojtzbof.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3daltlzos.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jshugxoe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3paktroul.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ppynozra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvxitdul.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qjfgwssi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkppuhte.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ydsgfbzj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3glsmbpib.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvrbydzw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uvcbxjph.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3woaichsn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mylrwxet.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hgbvjivz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kplfxprp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cryvmczz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yyhsikfb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vijpvuwq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vmwaussh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jhzjjbrs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3cpmskiew.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3afjuzrxg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3lnnzggow.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dtozurot.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3oypzaojj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wxduzzxi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pelsdpzm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wvrsslah.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xevpiqnc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cyihtmcj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3pdqlmjzq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3piwidodw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hnsjrpld.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zblyhrgq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fvglqslf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3arqqggyr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qepfjdjn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ltrivdem.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewcdgpcr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fswrvnbk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3geqijlqp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qslvscsp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjaxirwx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ekqxhdfn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bqbvktxt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3habpfxbp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3oliojtui.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3waurrbgu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ldwjlnwp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3klxoqfzu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tfyepkry.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lasiycak.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3awxijhwi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bjfrwlte.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rphardyb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nqqcxqdz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3oyivmbsz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hzbmfwjc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3czrdvwcg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rwpjhjuy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fjdgwoiq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vkbpmmpr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xfwkgynu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sxexpxxt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jcczuunr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zpexnrmg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lkzlbxoq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3celeabbr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ncxwinwr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3swecqnuy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sslrlvff.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qspmjfwq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3indhnyof.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkcdfn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vzvdlxnr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwpsgyxa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lowclqhl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qkifuynr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tnxyrbwf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3nlacgmkf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3thjxzxde.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3umgujyly.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xthwvzrh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mdaztjbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kzyeawbt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wvnvtrwb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ajcxclrh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bwyxgrbe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ydmkgykf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wbdcjeze.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tuhutuvj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fufvpooe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qocuvymq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sefeirww.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3cphtsawc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3onjooros.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fhmulnsw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3suvfgvnd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3phxxvqnt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vzrpstcb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouriphiw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qknggehs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3pamveeoj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ejgrlbvp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ygooaskq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3iwafywpy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxixmcn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkhinkry.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ehjrtryt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xgrrzant.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3girglghy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wkknhvlg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yajaibyz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kjywokfh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wmmrawqt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3csvpmgfs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jtcirazl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wgeiznuq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3phiqneon.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3clgxgtnx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3iqjmjjoo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vygnlrbf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cyauxgpw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3obwpxpyv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rhioypgr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nggxebwc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3cjofwiis.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3htgstwmv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rllndozf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pjappfui.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tunjamur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mgxlrmql.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3higfgvsa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3idmdqcrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owsmobxc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jacqwzhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kofgxrzz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zuyechgq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wnqznhla.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vhzbtlnk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hqqyaaic.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ovchobnh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nainuika.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vtswtsoz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dsjlkgyl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3czfqwbaj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cocdesrj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gmqwcmcb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3soqkksun.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3buddwpud.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3eqtksfsz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bsxbwasa.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xhzqpjop.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3alsivttc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gbrmykpg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvrzsqqc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qgqphoni.html


<!-- 参考信息 -->