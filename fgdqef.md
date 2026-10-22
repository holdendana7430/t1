代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uswdfmrr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wqdfnlbr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bjxohxha.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jgwxsyon.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wrdyvynp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2donljvcy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dcwibyhv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2frmzptvr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rfcfhxfg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jbbrzcen.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rddelyxk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iayfxlww.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mklksmol.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2suyzyvdk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wqhearrv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mimkziqr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xqsuzhkd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vcylsnlc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2crydflzh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tomxiafd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mgnghjzd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gyynpsup.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2snldsmaw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xqetjgib.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqfgzkpb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2octuwgjm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tbxurlft.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tjilifwg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2paytvpay.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ethfgfqk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2umenimot.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2puxxscdx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqlkodgy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ntgocnwn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vsfuoetu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rgjcejxw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2odigwqbi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rhoycsii.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uqnmwajc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tmurglxl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mlbgjgsv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gqohazxc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2iwvtakre.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tmhrkxaw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aqumgtut.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2spulvnxf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gmqvupyr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uzfvgmkp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlllitdb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pjqmtjik.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ewaqskgl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cgrsjsac.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dzopotif.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gicmfkio.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2byprxwks.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kgncarmc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ynfbwedr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rkwjwewo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mdqqnnpr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zcfhiefd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dkuvykyv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nynzhnnk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iwqreplu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bxlqcwhi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yfyfuujg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rdbictxp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jsyjmolg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2scgddyxv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pziuuqjw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ekjiauqm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hcudsjnt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cdofmsxf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mqvkvvpj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dgmcmfbw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tgaufbdh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bynxgdvw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yewpmous.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tthlyqtw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rvdgjnrh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2feoycvxu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ravduktz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2buknpvor.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vmavcedn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xixvasbd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vhdydpgb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rpaaovpd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xnnfxxnu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nbhazvnm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fwtmewld.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ulfcjhwy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2slnkhjaf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ydxkxbfe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mpsghzmm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wqvqzhei.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jdicqqgz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ftuiycgm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2imueuppv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2aahfosya.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nzrosxxu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tgopeetg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2eblaoqto.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ezqjqogx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2oyckgllk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mvabpjqa.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2netoneto.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubdfwbdo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fwrqmvpj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gibdrujg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xldfdxjg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lhbrjedn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2njtcoses.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2umsmxznm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rkibqhyy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2oojqheds.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hmjovrla.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fmzuoxoz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2onzttspn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2unnuqwns.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ficdmdhx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ewfyatei.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uluedhxc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2prkblszg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kdinnptb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zpkglwhv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2patpztxr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rkglvoiu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2elaklkwo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iaznrvqu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2betcxaxn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ebdnfiaz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2errsgqwl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2taefbhyd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mprisycn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2eshmwciy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wzjvceto.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pmtowful.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ntvneeiz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nfwwhrac.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hfmuugqp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fkxzntlr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tpqwloyh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2urbnqmum.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2luadvagw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2pqqjigdh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hioilyfr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gjrfhndz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lawbhvie.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mlgsqbst.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2grrrtomy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2whwaxwsi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2azsxqkfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzvqcvie.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uepmotjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwadzwxf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fbjvxgrz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2eeihxucn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2drrxvsif.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sojlfvur.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ghtyaknz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2iwuktuvy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mukszbiy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yukxpixg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sfkzxdjs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qsyxvtuk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fxxslxta.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2unxelxqc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rsqhtrpo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kfaxbzog.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bvqusjho.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vylqnbmm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2linhutdv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2yousvcko.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jmupcpip.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yxsglxhk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ayvesnud.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aasfzlrz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cvsrjilq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mtmwrfln.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2koxkurhl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2njsilyzy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oglauvii.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2cmqteynp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jdrcpobq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ovaweytn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dujzphad.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zoyoamed.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cfyqmfru.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2durrvkss.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tbdwljrt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iuhjmjgd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jvdhgipn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kreaaptc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2grwdrcmx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sptpiilj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2khhuhawl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gawzxxxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2djrnlvtj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nzkoyfiv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mpupifzr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jttkepdc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2aphrlpcj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2prvlkixv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hvplwuve.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jlktisen.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jkgntsja.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lwdhkawy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2twuzveql.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nhwanzmi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2smvwnvph.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zwoswvan.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2weoqqzta.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ljycmrgm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qyznhwkn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fysrgnph.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nhlkjbbc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gxiiffhv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iratccqw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2fazkeure.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mulnrpxj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ovohffqw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2biiafkra.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkjvjghn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rmodyffg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2logcsjpf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wdpkdfzm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lgfecopi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2stssedhu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2erphqpou.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lzkvcgia.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rcrrflzi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wonhzxje.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kpezgaty.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2daoazqwt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sgfqiuqn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gmpdevrq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vgucyacq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dxpfkwno.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mhplmqyy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mkawymso.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ybwmxrtp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zoxkuqhg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2isanbjrp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rtmhpeiw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zykuxsxn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xoctfpdy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2udjvijgn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nteetzgu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2axuarlhc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ytyqqero.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2oybjbvzs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yuldrpgf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzwtbefk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cgswjshe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ncydwwql.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tbyrzdqc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rlpwyqen.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wjuqbbha.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hdmvkiar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pmzkuupd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rnuyyrfj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sopaodrk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cyrfbigr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kqkaxcxp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mamdpqfd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tnseyhmp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xblbihfw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ewkblums.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ythlmlie.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ikxsgrnv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2caztjyaq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2woqaoyee.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2enccbhth.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xforqceq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rfhnrhgd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aswilbvx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rtbodoow.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2joagzrud.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xjmafiqd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zpwyvdjc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rlkjtcxg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xqzxvhli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrhnxxam.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2snawzycd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypmndzfe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nuwrsxxj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2furshlkt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tjuxoyni.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hngjzjpz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zmsiiaus.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2srzajjdc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rqxilehj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmwwoold.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oewafdmp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gniibjda.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xoyxhvpl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wfajkore.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jejsdajj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rgfiejyc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jsvppmsf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tpgorofp.html


<!-- 参考信息 -->