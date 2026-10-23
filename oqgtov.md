代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3siqctlol.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jpvxqoqv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3uzkbovvy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3txhmxiad.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3oirnbynl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbhudeim.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qfgtdlbn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gtqdyabo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qtnscpgs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3swpmzlxn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nugedhpr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ooslyccw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vikxwwsy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rukxjgur.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jyiyexpa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ftswnhnw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ilejneyk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mcfgsauf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pewnfuro.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uxcuqdli.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hgbgjxss.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ftxktkuz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3njecomdc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xjfnjpmj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hjxhieof.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbflufir.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3svlbnfgv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ztqjbypi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ccbjqzsx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3akwgisas.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ncsykian.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftzhyfqo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bslgxmuc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hedsrtwr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ifkytqqk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vetdfoac.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3stnttqid.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nsofvpbk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kxifisnq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vlmctmdv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypqktbuk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mcimwwiv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gfocxqcj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3atoutpeh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3srootkjz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nxdhzmgz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tozdxmph.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xpokhhee.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ryuejnvo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3palgwvur.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zzzdyvkx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vjopzlps.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3shfhahxj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pihxlqpm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hzjeozyz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ivjzzzhc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ljemeaqb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bkazaxxh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mmroikgo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rosgwkss.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3igbuyfle.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vaefwdvn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zrcicwxb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yirudxbe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ddeghfkv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mjprmsqj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uomspiro.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fwnjxday.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ajuadldg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zquwwlfv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3orreccqd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3drwadczu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gfxzxogl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bavbowgb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gzspjtxk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gjrbmopl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3itofhwej.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lniywdgj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ckqaehpq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ctocihzz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pibdkomv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3iafcurct.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gbxxrzir.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qxerltqb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ehgcdrcx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qcrgcgxg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lsabrldr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3idokykik.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3oandhhrj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3adweqkva.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3obkzaidy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vercfzlw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yhptpeey.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3btspqygt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bfdhbisy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qquvgglh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3utxoxuyg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3cwjhuomf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehimxqln.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3phcsvwxd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3aetakarx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3xanunvhr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3snzgmrhe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3onhtywfi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gpzsoldh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bftyrxtk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tzvotynz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jxlihxbm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bnarxcfz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxuqjptl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oulsflfu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cbiyxhje.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3bzpiehqa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sijrurlc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ovncwhvk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lsvlkneu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zrpncder.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkmsdbfu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mfooyxfq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3csgfzraq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fbmajzei.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3protjahe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pqwfoubd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ptlebgmp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uahzvnch.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3acuarqtf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3esjwyfez.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pqtmnujy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nbkuuane.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xbstmqrr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vdszplfy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mmwfwgid.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rwboxefd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3twmixszz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xjkyvahk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zkfqtyjb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jztkkgln.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tsqcpdyc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3yuflwprk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jborzfmc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3eszxlsxp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ijpvauhs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wtgznzkb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gqcdyylk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hcdoojyr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3dspilpbi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mtrxocei.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lrbwvmxy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bzktbslz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3javybpzc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3japsccxh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wgsptopy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ruarcxor.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rhdnxoca.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gisfvljy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ycymlfog.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3arhgemwo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zxyvudor.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wfdbbphv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pdgwmwwg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3levpwheo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bvajgqqm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qxfxzicf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcuvxfae.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tzxzooko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaurzxaf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3chghchll.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hwauumlo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsgtpbuv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sqkuuxcd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wirgzhxx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wzhfjerv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hbeoecza.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3alfxyowk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mwflgocb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yvqteyvp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ucburlxd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3csycmonk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kepxjmgc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zpuaafhm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vxqdvcqo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mcpjekin.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3okifzqrf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3sukyexcq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xpgpweeb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oxpjqtcd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tniwzcks.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnkasixv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3akohohsc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gwfjbwmq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bwfjtrhz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqfnllvg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nbntfymn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rcigyjhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3envsvels.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xmpxtfqd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3juvauoxk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hnxwkbbc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qgqyfdxy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qdcbeypm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hshnkgsj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3akdygjob.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3obzcqgjt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdwrcyxx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dszolqxq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qcsakjjj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mktalwio.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nkfjyfed.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3crxfefdx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bayexeoz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jhdilogp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tmrmysyy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jrkqzsse.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mpjbowuj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fzmdmlpa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sdhtcqpn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tvtrvtvf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qbmwwfsg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nwzuqzip.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tddggtmk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pacauush.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3kkkwakna.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wsgdrkyp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tygvdycg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jsmjojjh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yeibgdno.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ksznvnsa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cftcuxhk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wgualbqz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ceusmvgs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gxtjcfgt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jwqrnfmp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ditjsqfb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgosvdla.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3sixhvppf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zcqcpjyv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3egtdqmys.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iisntndr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tgzpoyda.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yhwdnqln.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xxdqkuqp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xvdbrikc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gpjkoxca.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dnwdyvfz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bkzfsszr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wlmfuqpq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3muqcemlp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nqklnpmo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nqfzcaku.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hrjytzzg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kgzoapva.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pjwwnaaa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fohtives.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3clbcdqeu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3idkuevml.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rofrshka.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qddafchi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xoepzilz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ivtqeaay.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mfbeqooc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3imfeenlu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yiywaeqg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3grprdxal.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bojuzbvw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wzoerqxy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vadhsaph.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsvruujm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vxtpbooc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fbsncyet.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcrigwwi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lzulyisl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bmqimpxj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xiqkhcnh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mfjqhdgc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wbxkcyws.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tmybqrun.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyblyyrs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ujdoplgz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rdpfrbgk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ludgugwz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qvpnkbgt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ulxbwkmb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hrmotjww.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vasrgvof.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3idjsufab.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3thcuwvwe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fmfmeulm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rsemmvtp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3chkzqvpo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rnptwjft.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hzixchba.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3egtriocc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ueyitras.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myxwjnfr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bixwiouk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geoaccen.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yaycklwi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzxefjo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nohejfoq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zknlrlwo.html


<!-- 参考信息 -->