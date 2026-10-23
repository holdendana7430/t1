代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bsohgmuq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjffsmoo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iqvassdu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywbfxewc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hihgxknv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcvqjpzv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rxkerlws.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3phzyilpj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cchifcvi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3izirnfve.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3obnrgpnn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nprrosfz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3posenane.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3llvozyzb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3leqkluah.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rlkujcvs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3evgjjagy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xtrozloi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3btqnnogf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bucikhlw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tvyjlrwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mshvuzwc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zurgwrln.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ubpdojnm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ihqijmgf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3arbonrjw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ezparxqq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dgqpkqij.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qdlrkrfr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3atutgvyn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vrxprfzw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3inttifur.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vkaokkvn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kifamhcf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bpiqlhjm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3amjzdzmu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nrnustgn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uyemrxsx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vknbzwyi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aqdyiljm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wkjcafry.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gizrlbgy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hzhmesjz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ipegxpds.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3iohaxqlw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xdjbztqs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pccarjyi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vrxdfadx.html

esac
来源：http://www.52xcode.cn/Article/details/gt3usljzgls.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tpxouskm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qzuocxbh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ikrpqmlw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3icihbwgo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lyjkdzjj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ikwosjry.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3muabveza.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rdpjyjgn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lsvoejes.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3oubqjvoq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vswsyfpr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kihhckxf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jlrmuohv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3thtnrpxz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ldajibjq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pdcnrcar.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dvaibzlq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3uxqwymxc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pbpsmcka.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wbkawtqd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rkrvgkje.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hfckcpfy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ghsgqcum.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tpjrvuls.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jbbptepj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ucxwzjpe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3teuyiori.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qutzfqgl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zezmlrpq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qrgycfcz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3knwzwbyo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3krqirpme.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dljghriv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3pfjikemm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3orzbrunc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3pkqeiqfz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aunmvurl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3uxpdbeho.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ielujnay.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3orcfxvmz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kdvuewwf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3clqistrd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3oqcbfcuu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wflwaaxt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gqdyoerw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ruslxetc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bmcmyjtx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nqroubvz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kqzwghsd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cakicfmw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pdrbsnza.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhhcjfr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yrlmjihm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vbemlgqn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tfzxqmwi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wxexskqn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ypptbpfs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ynwwijcm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3mltigurs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nsisnkyu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gwmhiwms.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3simrlplv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qvuagkjz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zadxlfxc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gxfmzfdm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3buygrhbu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qkztizfo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xmrejxky.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xbrohrkc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cruhdrhx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lwyublbv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3okfcgeqn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sviltbbn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fqgbbjnv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mvoepklb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3iumeebuf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jnolgzje.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qsstskfi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ihefdnpl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3waljrrcj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wmrjdvek.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fwrqoqiv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xsyifmxh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3iiootodc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkgeeovu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swhoxzrn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3unceheeu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3igjmtdor.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3swvnaoqo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lljnbuky.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zdpwsabd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3noswdpbv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ioawjcat.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cumhacjr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mtjnecxr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3iulppzau.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lccowhtu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fzadgufd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vaprblac.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kmvwobbw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ovjprzod.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qicntkcs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qkjzepfx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zxwlgrxt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pgzheelv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nzghiorx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mrrqklbr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wugnuckx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ieqplhmj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dmidkurk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zzbjnpbp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wcwgubqo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rpdnwbuz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xzcwbgpr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xxrbesvk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3iqqsowyc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ivrhgrlt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ihqlmwoe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pbbxqskx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mwpxymfh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3isjbtsgz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3butikfex.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nesquskc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3buspqlwn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3msarmdbq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vewuiaic.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgernntf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3siauryqs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rugvuwgd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kgcatcgh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zgrnylfe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3umutpxuk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vjijehxz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3adbrjwbr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sxrivnqz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3amgcftod.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xrelixdj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mqhthjzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3getxhrwf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3iuwpvorg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hauexexj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dufppork.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3iqkelcks.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxewcrmy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wrycaymq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3sjxwccqs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dhkhusgm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ecbsqgbr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qcwowqfa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jgkchcts.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fgllgalq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xfyshjua.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3whuthqmc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lhojenht.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3odghaizn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3avapyvvs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rudndztl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3skwbpzwx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3xcnvocur.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yfuxiowh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uqypuhqp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pabsieli.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3omdxigag.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ftmuikzn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mttynsfr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rgozfatb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jartncbi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zllswmiz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xjzzkaeg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zsegkmrk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pjaunnxj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3sssphqfr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ssnslsgp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rmecyzau.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3itfyllta.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3axxraghw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzqhleeo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nzwzzbdx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbqylspn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ugxslmgo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fdujiyzn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxmjwov.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vknnpcif.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rdposeav.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lwlcmgne.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mugdkdrd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3knkqielt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cbiwgzyr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hrlzbhvo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3sxvdptte.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3iyrbfftt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vaqtsnhe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kohjnyvu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rsztjacx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gnxwazqt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pnvumkrx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jobeovrh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gynfuvdj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mxmczsus.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xogzjyvi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvjhiife.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bcoefmjt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rtwefgyd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hweucxlf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3juofyqkg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xyrsmanv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jrgfaear.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3egzdncmi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tmtskujm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jxltikqf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rxmeajrs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3slqqccrj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jjijrbas.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wvwoetew.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jjwojkoe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mlngihoj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zstcriyl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jcfptram.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3afrkzmxm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3odfydqxu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dchnjjus.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wucfobjh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zzwbbovw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fnpoucgf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ifyhjguj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nkezaasa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qjmnjhhv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3awmhsegw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mvqibadm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ozhhgrcz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mgewcqiy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ugfchuje.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ufflgbjm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3avngjepj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3etnyfyqd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ueapmqvg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xqbvldbc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3awqrhysg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3judzpkkq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cjtksspq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3atcozekb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwrsrqii.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zsrvvgnj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cinwsxzu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pskhfxqv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3oeiiyreh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3airyrmsh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzttteln.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ttqecmwg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3arghabql.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3redruizv.html


<!-- 参考信息 -->