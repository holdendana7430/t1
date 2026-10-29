代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/govyosbja.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gnbusjiwx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gfzhcpbkk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbnblcolz.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gcgkseaqi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grmnznygw.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/ghxisqgez.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gwdovgmre.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gydtxgsvs.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gapjrxwnh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gthecroed.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gxvvzhdfh.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gzzckfkwb.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gkluzmfxy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gvfflazgn.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gctvgfjbu.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gfsrzsqdp.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/ggzfixcmb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gqzshkrkm.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/glomnyvbz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gblniarjf.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/glczezydl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gpjrrzqds.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxiqitj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gielmsuyu.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gcprgxpsf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gagllxnni.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gbmohscxo.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gkmwaqxwz.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gutpepkat.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gjlcamdhs.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gwlbgzoun.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gvklnlmmz.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gtmxhoxyj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/geqfpbnur.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gzwhekvxm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gpjccqydm.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gxijzifrf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqtmefpuu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gogobzere.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gdmwqljmj.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gnrzwybuz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gkhisgeji.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/ghpcehnhx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gzxzlykrt.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gjcxsagtp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/guqcrgrzr.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gqbznodix.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/guipumtbx.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gtqvzvrux.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gxdlzkylo.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/ghlgqyjzr.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gqjydmdbv.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gzgoyozdy.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gqehfvdsm.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gfasycpxj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gitxenpmv.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzesoqadv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gslakkxkh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/ghqpjoypv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gwfrrmyzm.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gcmijyoye.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gbsljrsxq.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gikpmfvwk.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gmpjfgqst.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gkjcufmpi.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gniiyybgk.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gfvhzzoib.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gdcewglrm.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/grnglccaf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/ghktqtgzk.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/glhehuaua.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gwaewkyxj.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gymsmplsc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gmjougkwy.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gmwiscqqj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gtaxzfqmz.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gvlxasaop.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/ghqulefmz.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gzxchnkvf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gjepscafd.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/glhaacrdf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gedluuhfh.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gagzjgjjs.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gbrgqohjv.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gpxgaiaot.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gbnbopjoy.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gcbkkjhqo.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gkcuitnhg.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gsxcgvlyz.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gjqdjsvym.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gwidxyckx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsyxqxvth.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gczlnctcz.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gskxvonvo.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/guijrhwsg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gcbkcsvfz.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/grwbhewrz.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gwmfqnnpb.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/goxlgtflq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gnwxwftwl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/ghxesneoy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gxgaqrype.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gfjfgjjmv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gpbsqofax.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gakkrphnu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gxqanynhn.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxdgnabmd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ggtwlecci.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gkyveynmf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbpbpiwey.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gqmxqzyko.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gtuwfmbzd.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gdewsqixy.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gshipuiwl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gfsmmlawn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gnzsqyfsx.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/grafsvhrp.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gmewxfneb.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/grrnwlwsh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gswbxtxmg.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ghgspmgco.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gzqaelpmp.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gwmjgwupe.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gdfylhcoo.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvhyusrwz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gbecrpzwi.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gkzufcppi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gazeqhvvl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gjhrrusha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/goslcbmle.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gkdvwcelq.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/glylijslq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gcmlfloog.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gtlcmyshe.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gfrosugth.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/geqiobcmh.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gscsbykcr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gyntudqti.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gsxrofvwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gwafokizc.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/goeapruff.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gclqguevq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/ghhbjuwuz.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gbfysrlgs.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/groyzvupo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gesjdgdtd.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gmieezmij.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gayqmcahg.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/glefgnpso.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/geetxnmru.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gcloqabuf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/giifqmibo.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gbckusagh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ghtcpsjcj.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/grihizqev.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gxpxtafdh.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gejcwvlkd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gzznvukiy.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gtvnrfuzv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gxngeeelr.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gueemopdl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gccsafszr.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/giglmlulv.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gsemtyywb.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gwsxjbiks.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gicdlrees.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/giuohpqkb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gjzozshvz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gmuohicbg.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gwsfuuykl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjeydypao.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gsaqnuitt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/garwmztvl.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcawtinpm.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gwpevuoao.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/ghbvplroc.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gulwzmbeb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gmhibytrq.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gtcvbljfg.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gekuqsldq.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gichzhknl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gircvlaeb.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/giyxvxroa.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gbcchfjjn.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gekwxleuv.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gzeqpvesz.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gniwxvkna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gbrpwherk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gjqfpelww.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gbhjnqryf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gzmbwffxo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gqlgrqmua.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/ghqxldvnn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gvtzcbtfh.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggynchomz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/geqvapjuw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gutqigpkw.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gvjmdqsmg.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gtgzkvykm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gmejvcmlf.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/girfswrrx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/ggpqnrqcw.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/ggrerclxn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gddgfepkx.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gwheeppkm.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/grmoyfkhu.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gbkbrntxo.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gkdffmaqi.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcibhxorp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjidevtcu.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gtqzjyphu.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gkmdsbdkq.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/ghwhmesyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gaxljheyw.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gykuksade.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gkftaoqsz.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gzebofavu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuookva.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/goakoiifx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/grevvjdog.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gkhtaowyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gejkovygi.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/grbhlvhrl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gvfyucbza.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gxolfpewx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gbiibrgil.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gnsdpuoyd.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gymfdemmk.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gucxdjhax.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gijfohslq.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gwiutedyg.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gejrfangy.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/guvlvezwa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gsctmoxuu.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gkuqcgbzo.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gatjzctyn.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gqixhrnst.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/giqyujkea.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gbokoymln.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gfcfbygci.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gdeujakss.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gunloxfwm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gftnrvgqg.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gurpzgudt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gvdsyejgg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gmdpmiczo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gxvxviuqv.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gpnklpwpk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gpabwocjo.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gbtljqbsh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghtceccae.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gawkcazlk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gagpftfgt.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gnmsthqwe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gsgzyurjw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gxmzgelbo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gaigarwcw.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gbopvxalv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gzrriytko.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gmjunptut.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/ghnzqnbey.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/ggyxmqhqn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/grxnlfygv.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gekfrzbhh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gbgtkzayd.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gzuukidyj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gmpfbgwdy.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gmgxbqqwy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gqmbtotvo.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gdyknwwlq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gbavcldff.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gigkfhhmn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gscefjegr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glfmewwyy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gejgeiosc.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvkvyfec.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gzvnkglit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gpgxoshai.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gvmpoyuhx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gsmaatfbr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gbmutifal.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gpxqjypeg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gptpqulqw.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gxiwmkrca.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gmjlwcpsx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gzspajftk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/glauvibzl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gnrgdcwcw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/goaimojtd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/grxfzhrts.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gavffdkey.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/ghngnfncx.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/ggdrxmqhv.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gnsmhmdsa.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gfocjkwqr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gmdkftylh.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gknvgipbn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/ghxpbcnbl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gzrcpersa.sHtML


<!-- 参考信息 -->