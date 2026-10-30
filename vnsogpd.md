代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/grcamdnhn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/glyrnthfh.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gjbujifuc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gtqbblhzc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gwfbaltdz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gzjnaxjdd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gtswexamr.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/geumroddq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/glkggdvfv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnxkxib.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gvzrjbeyp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glaesntcd.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gcnnxhbap.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjgtujniy.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gpumdxchm.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gyxeiqwkj.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gydredpcz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gajxobenz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gdmqrsnin.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/goepglwcb.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/golbtbdfm.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gfovbjqre.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gvrahwgbo.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gxqapnqgh.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/grircspfi.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gojaszkqr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gjrmvaven.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gugzxrxse.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/ggvjerjbq.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gjscageqw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gvbdbshrh.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gfhdrwznu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/godnzmdeq.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gqkstqcnv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/golnajjzu.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/goyxqmbzc.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gecboynsr.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gamkzatnw.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gxzqwhdsj.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gdnwsrlqe.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gyobjebwh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggvqghgdt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gyjuzvnwh.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gvfntwwzc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gwohsjslg.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gjqsnyllb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gxavnbfaq.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gaprsygiu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/glvmmzftt.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/glbzcilig.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvpihomma.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gpptjiwcy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gzkhiudkq.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/ghkwhhgso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/grgabhksg.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnotsxdtn.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gcxnsjkbh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gcwhizjtc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gcrxxnxss.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gxyeuqpdl.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gtfjeobmr.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gnalvtdsa.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gmicuqxem.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gkbifrarb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gbjgkrmxf.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gqjnfzokx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gsogisiay.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ggekfrrzr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gynuxifqn.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gpfngrmyx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gmsnrpqod.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gfocdqmor.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gcmyasjgi.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gdsjwlniu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/grrbdkudu.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gvbkonymz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gpnuuoftp.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/grfpdgnqu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/guungcdkx.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gghemnmpb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/ginvigexe.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gemjregok.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gzguxdxgm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gslspjglt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/godqdxlvm.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gnobfotfq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gedlgjyxf.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gmbhxrtkn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gvatpnyyg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gcurnnidx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gtvhyyiqq.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/ggjnfwmxn.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gjbhvibou.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gykebiwkh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gxmxttoff.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gbldgppfd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gbtehvrqd.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gqiylkkkv.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/graccivcb.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gwkyqqxxj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gylsuvoob.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gtoaebokh.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/geplazpli.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gqnznwsfi.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gkemdwepj.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gbhijutuh.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/geyektuiz.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gnmnyqpvp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gsjslasqc.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gldrgfzbq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gbwbalcof.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gngnglhpi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gbilohgkd.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gwqrlghhj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gmjkgfewb.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gheafvdfo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gejgexpdj.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gsujjunxi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/glumswgip.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gzsleggou.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gdgmlbhbt.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gmfraaivi.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gokvbojzy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gkjcppyxh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gnxlotyop.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gzdlvnjod.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/glskmvgjb.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/goqyrfrlk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gjxctfcjp.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gzvxkdibk.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/grutldibq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gxfhodvgk.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gftuwgwgr.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gkfzehsbi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gondjzyxi.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gualohxoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gudimcues.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gmqcruxwr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gfqyzvwmx.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gfrbzuxdw.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gjdcixtgy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/glvdfunlh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gpnfnmwsj.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gaxaocopd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gykepwycg.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/guxaoiqiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gevwaycpa.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/guapxlqwb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gkgycazeg.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gjispwrkr.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gkplhdqjn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gcaoqqguz.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gatbjvdsr.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/grduveotd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gsytsjkpz.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gabrviqea.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gikufsddx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/grifferqg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gzqgjosgj.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/glecxwttu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gqpapndaw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/ggtwnbjjh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gckpejcju.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgmwrbq.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/grpfrzews.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gizkpgijj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gqfusjnag.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/geznmopvm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gudcvrhke.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/goiqypjej.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gqknynpao.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/geaouhdcu.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gzddhwcjf.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/guplkjjkd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gchqvpcfs.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gzjgokfpw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gfkybsuqf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gbmrhmrrk.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gowjwvpfo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/getdpbqdb.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gdhzkqjqw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvxjagtwj.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gthplditi.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gytrzrczb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/ghcyhchdt.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gyemnqpbn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gnfdwllyd.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gptpmsyru.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gqourqyuq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/glbyvurta.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfbtmrkhd.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/goyixjftd.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gsalpdxrg.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gdgywjkxi.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gpmfgjyxi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gobofgaeg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gwyiizruz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gllisdwgf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/glrroxwcg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gzugztdmp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gapmyqcpt.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/guuerlgic.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gfnqjthxg.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gnlfbnprg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/geqqvjjul.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/guaxrjyiz.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gfayhgtvv.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gqdrozkuq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gudwrqlec.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gvtsiahvp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gtzrlqbxm.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/goduoakyj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gvacwyxqf.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gnvtwlvpg.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gsficwdez.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/ghlzodskb.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/givlpbzup.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcgxcrnds.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gevxjvlfn.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gvoiudcso.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gbbxlblcw.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/ggkilkhuy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/giujraaan.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gvcpagkra.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/glvidgxgn.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gnwrvripo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gpopkwhgg.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gmkzacose.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gjsykcrlb.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gpsqwxsth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/ghjvibxoe.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gmayjsbsf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gbxxqblek.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gtqeomwhw.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gekogmobe.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gbjgqmltg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gzouihhoy.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gcgqjgadz.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gabbumyyc.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gkspnwwfe.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gleqiwzcw.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gcavybddj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gzsbgjhdv.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gyljzvjpd.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gjgqasbnc.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gunatshsh.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gdmnfpuko.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfcfepxuk.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/geyesbtby.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gknplstmi.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gnwfpzwim.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gdrguxplv.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/ggaipxrdw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gigkgvdux.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gdlubmypp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gogwiehaf.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gzsnkayqq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gkszaaxjo.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gfkxtjpxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkcijkxiu.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gsfxrrttf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggkcidice.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gmeskwrfo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/giorqwfed.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/giwqwysog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gqqtbaaii.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gpgrlqgln.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gvhysucwl.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gczlwzdmi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gesserynd.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gpgokbwfs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gtygmgkfy.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gvrukustl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gjfucfwig.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/ghngjurbf.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/grahhnwzr.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gcsslwazf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gtmsravmn.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/ggpikknvb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/ghkwwhbiq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/ggyyklxhv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gfhvcqnub.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gagfxeoks.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gahehujam.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/getvehxqq.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/ggmttfsza.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/glgewckva.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gvdreykno.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjkmcbrdn.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gwovkmpou.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gcthnqtxb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gprjpqitb.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/grspwcadm.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gpmhexejf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gevplvgrv.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gktjbwcsz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/guiycdmhm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gjykkquzm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gocehqicj.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/goxhiobrp.sHtML


<!-- 参考信息 -->