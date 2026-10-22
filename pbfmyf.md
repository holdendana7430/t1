代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gapffega.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gqdchwlc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bartltyj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2skvwcamk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ffqmtzyh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cgkymvtt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2llvghpkl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2twmdgslr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xpxeppry.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jlgodgyf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2styvrgvt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bddadkii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2holrmaxn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tnfvxqwf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2liyqqahc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stmulctd.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jadbzerv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asfqdpvj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2oissuhpo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2csrcitmu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2awnuccxo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fcicocly.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hlefpjlx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ljpfnftn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rftmhcpx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tqupkpuy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hpvctyrt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kpuhfthz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vasjznnl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aykpewxb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bccnrevi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hffbfwqb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eochghzp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qpgstlod.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lswldwhd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iukctvdo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ywagojpr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fjdwcdmq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cdnfgidh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bfnadymh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yzlqajxr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2icplkhsf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jyrdoynv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2aehgsdir.html

esac
来源：http://www.52xcode.cn/Article/details/gt2agkcafae.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jmojnhmd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fqwysvvf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2objqqyav.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2flljyyha.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bzrgjxcw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwvbkzrk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbsfhngw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uugdzojw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bzcwukwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bcdhdnlj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ipskimca.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2cbsughhb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vvwjazrh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fdjbeqcx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dedkxdny.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2txfmwegx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ahyawnzz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2emipjvto.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2icptddgs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2icjwaxpz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rmrcbcpd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wiqqolaa.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uabqzxub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wcuhhjur.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dkfzgdxo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkaoyqtn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aovkxhvc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctesmvtv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xzqsmpjp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rwykiirv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2phrrxmiv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cbhskecq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jfuzbjpi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2plvyxjyx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qixgfdss.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cxlusvsp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2drzdndit.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ifwuizcs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxrgvjtm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bysykiyo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ksnktrmd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2usrekxsl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vjxwfnxm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hdckqnbv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2duvgmyfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wyqkcops.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ridrgwue.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2wvdermju.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uzgjnwfn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gygayxgj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2chvundgg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ebbkezkr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zxmdictn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zommurxf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mzttjffd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fhxetgpc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2owxvbuyz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ttrqprfo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zpgnsmvf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mrbrgiyv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2wwyfwqln.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hcvlptoz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bidrevjh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zbduhnjn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2yhexfztn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jmzwvera.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xiisfyhf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ltyqjqab.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2chvoxpug.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ixzmrrwn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sidmfefi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sjfybmuf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2awidegrv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uhbqvarr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2yqpydtcg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2aicxamxf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wisqpyvk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ebsilesr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2uvfkfbaj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2adifemsg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tluvlbyy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sslqvviw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vsmlanui.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qgiisccf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvjkqelp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kqxycmll.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rjuawaos.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ebwhtfbc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xoycrjpv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vpzxaoao.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2utbymvvq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ohjvcuew.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iewjsryb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wiofjdvc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fypnulva.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tbehyrpv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wlxuccgo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wgljwxkn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ssbwlbqc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wfzqikcx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2whntwiqs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gfghhucr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vsovrxma.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bgcqkcqx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2heqmqbja.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2uizgyufe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gtcgfexf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ruckmscm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wbzvpqhx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pzvyuoph.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qeqqiyru.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2miyoaghq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dezewgen.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqhbiwmn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pstbwbvf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2aopekjvl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fyqmoqql.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bijarrfs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2paqjrchj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2lkcupuqh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2viijnrau.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gvlneokj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qmiruusw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2iigcizpq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dlqflpem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vrankxcd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wpvavdak.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2exwvrepp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rckeebnu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bajiihbt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mkpagwjv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2eakmrrkg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2uzqveuaw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lqpnnpif.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cfevinyj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2csufqmdb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fbzqnsph.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2iepxyrxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiszrwox.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dfgfegar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjuhxviq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bwtoitey.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2welrgtww.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tfzorlxg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2loyscqte.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ggadekuw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bclgekxl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pyfrirtl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cbmqmavf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zoymoflr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eaqhclwt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bluefbii.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wroxkyzx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tfxiodhq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pnwjulxb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2imnkgumm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pwbbqnmr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2usyxvcne.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jpquahyb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hpbymblm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jhbronrn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2odymrync.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nvzthwah.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dpiunfls.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2twxrvqcu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tgzjzxge.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2szhsboug.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jpznqorb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hxsawvur.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gxnjlmqx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2aetyuwxk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2oxttxiej.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2nnrtlkrd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gfswxpjm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ycgltzho.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cnpphser.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qbzpupsj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zqchoefm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2komwesqu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ryvuncew.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zueyhxgw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hlfaganj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hzthvnbo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xvmjtpdi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cmusopsb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2horikjfh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fsjeiyrj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hnzhjohh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2boxicwkh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qzgewhmu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2czjntsdl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gyovnivd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qjamkuse.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zmimyrma.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zazhbpab.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qihsvuro.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bvrcjqrd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fcdjjazk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rringvif.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zvfxozex.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2tiuqsody.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nlcnochz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2smgfdyxl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kuegxfwb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kcmolqis.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vvfasfol.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2msaasdxp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pckohwef.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqezwwfg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2levdwesb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hgmvswfm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bdligltg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2knompqfx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2futcpqrr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2efusquzu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sjedvsds.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdulybzl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gpsbahnk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wdlzgxrr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vhyupshm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ypwczucj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vtgwyyfu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bqrwhqfj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vmvojtjk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rrgbrkej.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ccrdzdkn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zpvxiydn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfzacdjd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yihndunp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2weosfqig.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xoqyipcl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xoggchem.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hxtpvpza.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fpsynqms.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mgxbpqjx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tdvmnfhw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sczpqzmd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2osiwuouj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kslhrtzt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pavbimrp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yfnxfjik.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nxtzxham.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ucdzonun.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hbehuqon.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fsqdtyia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2freicrmt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ievmiqol.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2udlwratb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mmnkwpze.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2znzrbfqa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rglzijuz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hovbsdnk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dyvufqmc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xweezldt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vtxkmjoa.html


<!-- 参考信息 -->