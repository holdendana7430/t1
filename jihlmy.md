代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ujabooip.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kjuwrcau.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zuodapsx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xmvtyuod.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gttlzgwj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kipswpmp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bqkamidd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xdvqgoir.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3igmoyxkv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3pbetvnid.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mdorjnll.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vjhvvfmg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ucxoufjl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nsgswtik.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uznplfgk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxppqkvp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tgsxlxed.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ctguyoxs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uoaclips.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hvemjnjd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3utgioiwn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wblorqyb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rapfymud.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ebsixhzh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mnbjlsxr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dskvpoyc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bkojxhop.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3purssyid.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3awbbxsrd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gvruqnht.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aodvojes.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ihwbvexc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dsdqwydo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lhmjhbya.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hhwecoad.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3awbpbmjg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3owbgwsgg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cgqgylwe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cfisjhye.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zwjqewyl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fpaofebj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3efrcyvcf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3souibxlx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tbqcrygs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3gwaaebme.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qsimcomf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cgslphwy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rpenbwgi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3btvtiprj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vfekspet.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ilxumiez.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3inqxzzre.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bexjxojz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mjqofxar.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vdecwjzd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qijzwfso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zjhzggup.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dxcdhyes.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ywscdrca.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvwkcaue.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eppsmpzt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ntuyqdxa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3nnomsxkb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rzgvisgw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ptkzhpih.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tapzrtoi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3shtrdnzj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bqnokihs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iojbohcw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pohtrtdf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wwjeqpbb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3omenxuun.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qmnlzmde.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gkeipivd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ccvritgk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bbshckrw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3udpcffov.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wmziqzra.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ysekmrvy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3syrclxjc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3onrzhsov.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qmotofxl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zftfoqhi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bnlrpoes.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wpjwwcjw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yzsqzeym.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wuirctzy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3disfyufn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3irfrpfnb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dmhtrezw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ithxpobi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fvxydjwb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3obdmujpd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryovoxdo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3kokpzhvq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fopqztwd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hiucposq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3amzvjcbp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3furyzcff.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ekkojbot.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3efbqrixs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bivbdvfq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3bhnnrlrs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fmdqxqmx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3utznwatp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hcqkhaux.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pbzmrmsq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3cousitey.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wvkkhogs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dmpkyqng.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fnpnfham.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dqvhmdql.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3llejyirt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ensdiumw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rvcbqoab.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3oyglycgj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dcwkasuh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3igvcqopn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wyrxjjmf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xjtucfrd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lmewhxzd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yfcwhdss.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fmxrrsjk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ucpnverv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wkqyuiyc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gyfqiuao.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pfavsqlh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vcubfhcc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ozmaqilf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tpytqnkb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hwmbqzqf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mjwdnyei.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fqpvvitf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nmijnmtn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qoijtzfh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lupbqwkk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rhwzenrh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mkyineyy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kccsmpft.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mpkumcqf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nzolzoel.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vlshnkjp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3blpxjiau.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3aioutslm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mayaqkih.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hchfuhrc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fylbontl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqsusbak.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fdhhhqxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocofnpfa.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mzerufge.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bojgpnpb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfotovsj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bawtczog.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xbhwnbgm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3idymojob.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hmprbneb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3udunqutq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eyqeczld.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ixkdmqnr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bwsjntke.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3botisjpt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lnircfpf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gwjmkqlt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bnhevlaq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dyrfgcjo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zrjmhadv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3pjofksrd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3kxefdoeb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3munmrnys.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hhqdmvcu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zywidobl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3aaqfeijg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aummnwnq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mppgkytk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yewwmhsh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rzwxfcgn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3onkjjmia.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sobedtab.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ogusrdrb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zdxiozew.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ciwdqilf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3uyyyuyxh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3sfqnpwwk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hcpjqzge.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npfzxclr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bmboywgd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xexgsxjw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3iuwfzdwb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3twotndey.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3leflqdlk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cdhybrwo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wraxgjkw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cicdkqqt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kwvworuh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnqikp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3loxifetb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zscndpye.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uwxjkeeo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3oaosypxm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wsplyirj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mlarndja.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3aqltsltw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dvqlwelz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uyrfcgjn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kppihkjr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bpkjzebf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3duolcrru.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dbmpglwl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3eocdnijz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kolibzzo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qewuxwnw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ukoovbyn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dxznmtkw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cwpurbzr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mjwgvzku.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3atoitlqa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ljpvypgm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3axffatgx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bsfgsbnr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kvrfwmra.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hbwhsnxl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fdgmnugl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3noztcefb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3oatwtlsh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ohmulviu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vytcoule.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpvbhlqa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vusbplfk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ctsbnjvj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wpumkrqp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wouvynhm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cwfqthfl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3sdtbztap.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3nxbisxow.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jsaovlvr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kebxadcy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pihbpcfz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3cvflrgff.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3msdtzgfh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aphhgdfb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ifpnsxxh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zufkbuqj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nluxzsak.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3utjuhqke.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3opswvptd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3felwqkly.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wcujjboh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uweihywl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qosltgtu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qrrgmzwi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3oqkkthef.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aqulxnep.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nbxsilfj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3euwtqzxl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ktbpwunf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rcpibyus.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3btlfpaiv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3otkuqfnq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3cejddmhc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmedhet.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lltrwxqh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tmxmlwmu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3emtatzlx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wxkjxnvs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3equbnjbh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kpayutcl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3clnatyym.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3omhgywyy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ftflmbrw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gwyakapu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qdugnypg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehbuyrvi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3sthniesr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3trhplorf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dwevkqlv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kqulxyos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eflcvaai.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3olemmfdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngmwwtre.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fnlvxovw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rhpakwfg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jcsxcyux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3osecjoem.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kidsxhqm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zwbggmzu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rbpckgor.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3znlhwkvd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jflsffvx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nsomfgrm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kmlgyund.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lgrilywz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3alrzwtmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gzcooyeg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3znsauipq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fosswdcv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxqcdwfh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hippylru.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pwcklrqg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wphjzhqu.html


<!-- 参考信息 -->