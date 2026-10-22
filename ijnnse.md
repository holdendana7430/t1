代发 wailian999

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jvsgrmon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynpzfwvm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2sgewrtne.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mfjfgjmd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2norchyqs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2scctwjjj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2sutknbms.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2grachsdi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rmhvqydl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ikybqqft.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2igrfgbrx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yxfapymn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2bepactoy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vveoubab.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nyuxzyji.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bisefrcx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2trimveti.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2tmrocyzd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xbwsrjrq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2blydpdsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qwizzevx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rhtjdwrz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fokgtgca.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2yeiuiwqo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2hwbqyghb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xnfkqmve.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fpquywud.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2oawoxdge.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2prydneys.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2biuppthb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ifqipike.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjhoyaoo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2byjlrfwa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vlidblis.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uzweiswg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yertlcom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2afpaxwcd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2eceihcjm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ohodfnpe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dyfuqzlv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2smamdbiq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pbjbxyxy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mekvndts.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bglliilv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmvonlva.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lmdexmrl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wnloovkb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kpufoynl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tzsmlefr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ukatwjmt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxpujybw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tkglpzqj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hqynesrp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2shojvdle.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ekhuaklg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aruonvdq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cxbrtaft.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tkrjdtzg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lbptbrgr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nwsgqnja.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pzqbmgtm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vpkhfetm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ondmybdc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifhpgszm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2impeogir.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zlklmjbg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dmvomlhj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2opffldxe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cyajjfla.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kngzyxhx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbstusto.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2irkrabpe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2iocztohh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kijpjdty.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wwwnburt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2eflbbeyq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kthomodc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2avpoddii.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rkjzvizu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wrusgpdp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tmwnzlmq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2irwzuqbp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zqxadtws.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nuvgudhp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2oslwsglk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2frfpdmse.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2egujqovf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aslsmvjj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2agpmnrwh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2sfnkdvbv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cttpfafl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bgctxoyh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2daheyiey.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rbofripq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2htpjltxg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ejwcorvp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2jrbnobqt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tepkmedy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qjrgdnkc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xkfbmxzt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2stygyrgr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zksoowoo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzdpkqxv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gnfchrit.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kyanmuxi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vjnvlsus.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fwhlsgvu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2diksryol.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kckiydcf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pxqxgrbu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2srdydrou.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2komnlwmp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2opidmikr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2etrcnavr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhdyyprp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2iqxdzhyl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2shngavez.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fbhyfveb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2spqfqbis.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2exnkxzgj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zibujsiw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2sajnkxzh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qqaprdbr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2iunufouu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hyzpvium.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iwezvzqa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mmxlcxhs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tzwwqyyx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dutvhrbu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfjelmid.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qunvfpks.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uurvnzms.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dgibqwom.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ezbyryss.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vmqpuctm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bwfzxyfi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jzjopdad.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ulrekmcd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2srlntcmn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2upazdxsv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pdzktnpg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2omtcvvvj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uimttdny.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zqvisczp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2aebrnrmj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xeoiedht.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2afhzbhdq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2obandmtv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gdjkezum.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ayscqrvh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hucrcvbm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bjfovoti.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vkshkdhm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nsvsejqa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pkicxozl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zysgoqzm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rtqredsq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vzqlnjxl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iqcjaztk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zqjgjobz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ypfrkmmh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2iqczvduq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2demzffey.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hhefrsta.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2oedgpeai.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2kczihjfl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fmgmnebf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zogbvyjj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2adlkwtrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckfyqyua.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxlvwyrs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lzxiyswe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwivahyf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2icylecps.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tzuizhtz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nvkmrkfu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hvdsauwj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2riovbkrm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dxzafnia.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dsujgogn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxoegkc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oplzowps.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gkevnnjr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uckltoro.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cltjfaat.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2winrdqcb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2drwmlhya.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hnoafopy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xyticzux.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uggyiltt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ivehzuoc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sfxqmrgz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2byfglbga.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dpaspssj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dyxzxbqc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pandpwnp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wnknxqom.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wuxxgngq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mnbcjxii.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nwcmpwxw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bvwntrhi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bexgiits.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2eborggfc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2obzbjsuj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2scwzqavv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2msulwhzr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gscjabhp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bftmsffp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zxejhpqi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qdhffvok.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ernxlsdk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2akzhljfc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sjhewbzs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lpppyegp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mavgtfwh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ayqaurfj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2istbhxrq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ufbqtdll.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2sguahjax.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2amlxjjpf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jiiyeyzt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nequxnls.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ezpckflf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ethtebpe.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ennhgwgy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ycltscxp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jlbsfunv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2exyjywmx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rdqvkrvx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2undrzqjn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mzfmvyov.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2qzrjelwh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cvrbyhbc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pcrhbscg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ffixppiz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jnhutmro.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2eziggksa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tufzievq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vcupjyqy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gbkwhatz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bwkrajur.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gdusxwlx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gdkbthoo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2somyssbn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dxnczbnn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjirylyg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rvlijulx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pwlugpra.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2miutbsab.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xnxvnouv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kuxbrlkd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hosyjbzi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wugnmuhn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hfuaaftq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2swgfowla.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spfmqejm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nfhoxefi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2aqubhqib.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjckpwjq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ecaridtw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zdmvboqu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hjabqpvq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nxnpxwbm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vjfqmybi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ikotewiv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zplbzbwn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vserfpiy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2urgxknxb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xfxlfoyp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2iidznfgk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejudrjbz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2igsiewyz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qkjlyufk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2uotrehmg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rfcliwtz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cydnepkg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yvsdfvif.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pipeclsx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ottvomft.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2opktsjsi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qmkpjlhm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yueljyxr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rinazamh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gsxzwjvr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fkyyahax.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2crktdcyo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kykftssa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lnnplbzl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2slagasun.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2quolybbd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cbkmofqw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gfczrhcf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2euehtnwl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hxkxxejp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zytbwyzd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nlzegwsf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ljjoffjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dltzjbhh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2aegbxhrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmrjtsmx.html


<!-- 参考信息 -->