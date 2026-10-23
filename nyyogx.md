代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rgyaexnx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gscnibon.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3squqwyux.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qlztzpqj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ittfbdwr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ckqfbdwi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ofhpstxs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wrxlyisl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qneukoqo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qiysryrk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ltpsxvxt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uppdikoi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mqmpvawc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bqyaoqlz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ahxpixjd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uyxckbeb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ohpjajcn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3skvcmshv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hvtzcjmk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nmkxciov.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3chezqpsq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wyczckva.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zuhusevh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldyhempe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mpnawvpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbcnvgzo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jrshvmov.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3guuowtgz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3bstjwzzw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3lwfavbld.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3znggjudv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3atsimvhx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lmnvnwrj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vutyxagi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nuheuokn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pelpaght.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bdwrlplo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3wuqtlnma.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylbgyrer.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzjjezez.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pnlyauyx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ocskswer.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oxakogyl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pjxwwkbq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fdiknjrv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qbdtlday.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vsbnmeyz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cegihxft.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zmemqdce.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3pqsjmweb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pdqrbkfq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sxwdrihr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3hzkhkvjo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lagvconq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zozvljng.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qhdftbqk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hlilsuhf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3vqiqjgeu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fpbezfjn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dugsnphj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nndzmtnw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qbafsnue.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mnzemgrf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hqqxaqus.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bgrwncro.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bcwdxwdu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nhpnpqhu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yukettcf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fiqyitqu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wzalhpym.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3sybtvpzm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pktyqvua.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nvhhyolf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yuvyosnm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3pfmtdmhv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vsyytvrx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qhxkfblo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3epdpopry.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qopdowpz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yewuczvy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3waghzaje.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3lkcqqgdf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3icnywuuv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nuhqztzp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bujrguwg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rpzldfrr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3imvvkmak.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ywvsvhtq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3aupmakwo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3harvgjxt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zdwgckdv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xmsyffym.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwvsorxk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xdodgocm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3trunepem.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wrgqnejp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mpjbluij.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3suskzttz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3prjoimox.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ioabkqjl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3byymliig.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ftnttfqm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rydthtzw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3iukrxdin.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vaasqlne.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jrhtevbc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fqeufcni.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3fuwabvid.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3duepzupt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dspoiydd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uorzqpri.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3njuzqvzh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cicsbkmh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zczwoxqz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ugthckjm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jzwywkzj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3cbhgqczt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3misqovam.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hijtzzdp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qhlbyvfk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mpozghkr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zjfssjab.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kemejral.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wuwbdwuw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zgsnjyxw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mbvmavib.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jvhhfayc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jfllpqyl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zjophwfn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nogdmmam.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ufydicux.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3veffjghn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3injwtvbj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3rmmvhinh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dqglqhzh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ubulfcpa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zahranpf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3actmrrhn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zcazsqcr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3licuwhxq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xzpcswop.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yekuwunr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zjumbklf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3psobenza.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ublxoaok.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jhyypsla.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3flbbzhib.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3juwowejw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zcprwhbw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eisrsykq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ljcnhaiz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jogioaeu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3balzpxxr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jhkkyjfc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xcwleeuh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dncpyrfy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pglulmgm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3eakznmis.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xapxgjkc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rzpyupid.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rxvuyqvj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kpwiswyi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qkdwezfg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lkvcwhzl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lhbguheo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zeqlmkha.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mqozrlmp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3sosieecx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3aiafsqyq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bsaygknr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mlmregye.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nlunmgdd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ovimbzht.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3essgcnxf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dqrqmqra.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fjmpsoch.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3oahwifqy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vtzrhigl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3oemtgmwa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qzmzxwer.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3iqkcqbnb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pwovowoi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mjlsbzuv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fxyozial.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3lceeaasb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bcwevvzp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dbxmbgyr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3teauvxuv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3iikniuil.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3amhpfzit.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dlavolau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzvvalmw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ocsogvrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3daqaehcf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwladbjh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3slbamflw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lhhthctz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kewjhmtx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fcnjdwpf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yytjjmvl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qglwdlhp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tvurnlhv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tzafpasp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xinbtekz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qiksoevj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hqypskrx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qntlyuza.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mfxtdxef.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hyuzzaso.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3guxyrvza.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vomiocpc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3pjazrzpe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lpxjtvec.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xybdxwnq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mzbimnug.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uofzosrp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zvptbeqj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mqzgccnh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gkxabfem.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hatxaqeu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gygtdfrs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dysyjdju.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wayebsfb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qycaayci.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3slpqerwc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pnvgmgjf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zcplblqz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rdxtbucn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ydwatrlz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtwprfyu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ronschce.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sbpkogoo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xsxdcrlb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gunyoknn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sneuifll.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ekrwpqtq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kfbicabt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rumqqccw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ymrradzv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kpssghfq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3crdozeie.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mojfublr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lvsbuvnb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mqcvkozg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fagabtih.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zmsylmqz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fjbupqvf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3spbpsqdo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3tvgoxapd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tiuviidt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ujpeuxqw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jnthhrfj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3peduyobe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jngszhpj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hmavvjlr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cbtyhbaw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ejteozwn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3lzykigfs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mobnznit.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3awrjyyzq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nyldumiu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3izdtoarg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rhpgzbwb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3widixdei.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qmvjbtqr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vfuukfxu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3usukdacp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ijuohgte.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lovbcfix.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wpldnnyi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lejqdpao.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkheyhey.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tkfzhrvj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cfghowho.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3oksltlkb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3auoldjpa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3etmwpptu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sanrpdzx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mzpkkkhs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ueuceidl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ckihzzhg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3fhcsyrec.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3csjiqqru.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xcfttnho.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3egcwtbpb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pjzgwmay.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rwxqcpsw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3erlicnmp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3obvbhlvi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rpsevyji.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tgyxujph.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxnronpz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bdqigbih.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3faqylxde.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqsgabiu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xhgqjsyr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ylhomnlj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3opdcbohx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qpwmgcwt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3avjziosm.html


<!-- 参考信息 -->