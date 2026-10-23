代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rwzmvtpy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vyzseenm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3buqpiwax.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3mmqeykan.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ymwwcyhp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rgthexyh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kwzjfjjk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3yomcrbyc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3pjregvli.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tzxjrmho.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3adoilqtd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rxhqddip.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3przfqouj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3eyfoilvq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kfrvebqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpjnrnrs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ehaonyxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjqhgadl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kecoknvc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hupncqix.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dljopizp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3knuzhmmj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ykirhsrz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gjqaidzr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3nyqnvtez.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jwcrthwx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3eujcvsfi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hbzoapwr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3lmrybiab.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3squratzi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jzkhryrd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3idzpejhs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ffwquzgk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jftpfujk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uhqujuec.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pqjkmrzl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3axsgfzfs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cgbcteqb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3grkqlpvk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nbhsjixi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pfrozsnw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3iviocdcr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kgsfuczo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wncgvkfu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hbgqrted.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfefdeji.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rdfhtuqh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yvmucpyx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xbikcycc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ilrcrsyq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uqwsjrzn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xzkpmyyz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jdaztqhl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qvkdpwtm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gslbnsgw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3okugfhra.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nrggsfii.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vhxevpzs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3auhlfutx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jigrmjhw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ofjwgmey.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dfaobkhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xrobruao.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bgfgohti.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pqyslfrp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gwnjwgwl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ibemqkjv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3crggxngj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3buxhwjoj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nfpqjesg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kksrtsbv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3htuvicuk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3czkcslmk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ndnokzla.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3slksrqht.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3quhlvqjd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vkluxmkj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wjhkpawn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gtrdkogh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xniqqolo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hetsquyb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rkxbhzub.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qvsumrgf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zeqsuimj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajqkyeid.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hfpwmhch.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mocnsgqo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3lfdjhyfy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3szdivqqf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ahfzofen.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3debyrqsf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vninolnk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jqnwtofp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xuvhmvtb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zquxidvs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pgepsugz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ukbabqim.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cqqhvkej.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3amsrzfcp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jsjlxspw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rtgwyren.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3loumyhen.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jnjrtefu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3udcatvkr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tgbseios.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lgzenpqp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rbpquagm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyyjzugh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sjtsmocj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3csjxdjxp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3scoohdly.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ynatjmbb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dwxcdhnk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3vpwhijof.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wncbrntr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mbyuecip.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mujqjyxg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3obibfeue.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3igwnokly.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lrjxhoke.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jvbnxmqg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3knwtrqrx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gzxigqat.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xjkdltps.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pywjagnl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ddhahxjw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mfcsuwso.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dpxolkgu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lflzrwka.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fakwutpk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lhvbtpub.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hhozolix.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rrxkmiuw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pqtbzrrx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3oezsnqxt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wxyxqzus.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3utvmvecl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3lcquimid.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rbzdzlym.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3akzsnsud.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sxzpvewo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bmmfyahc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3igilrttm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3furrenpx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3erlklvyh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvmhcdyi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yycbkkgo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zewefxra.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zvzodkwo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3iwqblxgs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ywkjjtdd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cnnolafs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ytvlugkj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zmdlckhh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fdgpgduk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yxggxdch.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jqjacbic.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cekqgtkj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qanqnsrd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bnnwcncd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mteaovce.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ffdhseqy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hphvubuz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3evzdkygf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yfnlkmsk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ugegnifj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3knbitsqp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3baxgsnea.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ofhxnelu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vqaumapb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3emqfrdvy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tnlpfrje.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mndxoeuu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zidlfgie.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rxockoyd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fmaiuxik.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gpsqhyka.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ukuzrtnv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3knkliido.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3urvyikli.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zlugbsjy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ndgvypgy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cmwmfssd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kurawidc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yakvlcku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voxrfznc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3slndyqtc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rdndpuyv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3smrtipla.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pwwsgxkt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3uxfszsab.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tehvicou.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3npcjixev.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3aseeoqer.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ahrcslix.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pouphjqf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3peekfqms.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lxwgzufe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3omecxnby.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3shvffcad.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bsdemiij.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3lrqqhphi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sjsoelsp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3bdxmooph.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3flqhqzfh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cxgfzmip.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cfvmekwp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxunavng.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ewxlkdse.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ynptquwd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3toopmqsz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnjrionn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cjvbnibw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dfazsixu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mbdqidgs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wmcerfwu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gdcuacgs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nttzrgom.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ssvzaadv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lgnphrhr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kszsnvbe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zahviyse.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3uulovhgz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gziehpff.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vmuxgcgv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3prsrtqaq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ruyjjfua.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tewcbgri.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3evlcfilt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sqodzhdq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3khizvkcg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3srfurqoy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ybpxmmxu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3osdcdxdp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3blinmabb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bwwiktqq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vqmimvwm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ckxiltlm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ybkrbupy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kseaasfy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ldtykcnb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3idtbqnej.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ydlvznak.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yyljmeko.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wpcnudwf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddnximnt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lqaxzwrp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fdnkxtnk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dvxggqhy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tdjwgxro.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3yucqvmsk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hquzpkew.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bmyecati.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gjsnbpem.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ysxqhpad.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hxsqisiz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cprsjiqm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ectvrnkn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xrixafdq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmtbvcd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bdjslcrp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3noojghbt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nvjwyimj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dfjrivxi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zhiyhciz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pzdybcqz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3npygmbim.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lblytmzz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xpvzzofj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rfexnith.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bphvbzte.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ioticktr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xxctpmty.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3oeodvkaw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcfaoxsj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gkypnpln.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tqvktolx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ailbfuws.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kozrlmst.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsiahpsd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3anjscknc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zpzdtfon.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3risnrrsy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wztewgix.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3prjcuawm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rhppzjin.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztjuyeye.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xffmgavp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ixlzzhhw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pcynaoiv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hfcpdjxq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jzakbqqe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yfcodlal.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wimvdttz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tksalpii.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fhqsngyd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zrytvqce.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3tfrcvxkq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3inpsktvl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xqdysduo.html


<!-- 参考信息 -->