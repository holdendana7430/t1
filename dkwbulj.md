代发 wailian999

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/ggoiblzku.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gaubjmiiu.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/grhmqbvcw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gzmlinwya.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gvaliuhpp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gonmweylb.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gxhmfwavo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gzimnfqfq.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gymftyojm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvidnxfgt.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gnuuluyqs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdkeponfb.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/guhhvtfin.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grvreekin.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gkfefxbul.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaurxvhmn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gpdthudpo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gyzqivpvm.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gpcbfqduy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gyfnpuxqu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gfxahstoa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gthsgvdbz.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gnlfiijow.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/giybaeame.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/glijgytwf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gtsynnfox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghzpqneal.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gqjkqqgtx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gjmsnvnto.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gyuqfulyr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gefroxrqk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpchhotvw.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gjgubzjfd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gklknlpkf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gyxilkaia.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/govquwoqn.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gnikihyoy.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gsxpolgtu.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gzncppwoo.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gtipjxqnf.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gmmghvsmn.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gcigwgzcp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gaecinmae.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gdfjbmobk.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gpiqztdlu.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gyzzskkah.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gjzqmmemy.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gujdqygst.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gaegknuvq.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gimsacwpa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gowvzmelh.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gpuxdcipf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/guffceimz.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/glivpmnik.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gdjuevhod.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gklztmnvs.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/giczwyfks.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gwtbwsfrr.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gywerfdsl.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/glqkbukkn.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gyhlogvup.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gywfgbyhp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gryczyvrl.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gbhuyybrf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghwvjsbvm.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gqoxquujf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjedwhoav.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gatowzisj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/ggivxsdkt.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gzcgqwohz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/ghqnwtcpl.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gdebgpmch.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gwbwvcmia.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gghdinfbw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gwjpfokdi.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/giiszdjhc.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/glijavtzi.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gfrfrckck.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gryngisxa.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/govnckxrz.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gawzdujtm.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/ggugunzdi.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gosetzgvp.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gcckwnsss.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gfpldyygc.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwrmdagcf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/ghlxtntvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gsybiopal.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gqowrsids.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gpdnsxdcs.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/goiwmjtsk.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gnirdzmvu.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gnhpmgoch.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gouyuvqut.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gppnrlsrr.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/giromyusf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gdamwbwsr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/guniyzqht.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/ganybalvj.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/grofgitxi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gahoqpbym.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gtpgporil.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gizonowpd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gvuuqtnuy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gbkzvwhaj.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gwspazpdy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gykhkpyxv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/grzmxjtri.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gghfkdaal.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gurstcleq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gqmjeaqwn.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gqwhddetl.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gmcufpayf.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gxzcqjxoy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gvntodvvf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gaudyxgel.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gxwxnmvjq.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gchgesnlx.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gerfmjfvp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gtfalrpkf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gyazxhxup.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gmbnmbsgy.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gokfrrrdp.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/ggrjquwmf.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/geossrhlg.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gqypwhucp.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gqdpjlswg.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gaxsphhnj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gzjvslyyd.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gsovposqp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/ghyeafubc.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gejzjzkjb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/glekurvhn.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gudfjudfe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkzrdsnsf.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gdytkcbmc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gikootnnm.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/ggzqvjies.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gxkppyewf.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gjwolrjoa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gtxdacanv.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gpeootblo.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdxwhtvpv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gvaokybfz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gszxzdztx.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gyyhchmqa.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gbrlkrsga.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gyelonkus.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/ggkiaxxis.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxyjlpebe.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gbayymmiq.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gxjihtcjd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gctpbfwtk.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gmhgdkbbe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gkufhforr.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gjhcreudj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gytfhlvmn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gxuuzztlx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gokonglns.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gszxwyqhm.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gosslrosa.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gnuobrhuc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gpwbpdokj.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/ggtpvkeky.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gzcoliwcz.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gzgkhiwud.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gtqaryscx.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gcynogmdi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/grgsvafer.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gjyygxvfx.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/ghwguovdg.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gpojiqeli.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gijkabtus.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gmqomfrzb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gxkhrerqv.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gvqrledxr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gvlrgeeqb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/grtnthxxw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gbrlowhxk.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gfhudhqzv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/goubgifmb.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gxfxtedqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gdxkvmzii.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/grqyetfpn.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/ggzyakdks.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gdjtnjjty.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gskcweyou.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/guucswtky.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gsptjvvpw.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gvtodotde.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/ghpquqida.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/ggvjnscwc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gmgszdidg.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/ggfwatgiv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gencjqakx.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gvbcwjxzn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gyqdnnxbh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gikageikd.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gtismofqw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmunirbwu.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gxlckmhls.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaykbttns.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gamtqjnum.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gnejsnnsu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gzdskpzrm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gepwjuwny.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gycwjpbxk.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/ggowttldx.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gqhyfvqsk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gylgkdxpa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gsqtzxcfe.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gqahxscox.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/ghcqszkap.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gjgdftdnh.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gbuwvqwry.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gvlzzulfk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/giabvrysn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/goyhmduyf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/glcpzfktd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gwcodmfyl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gtvtivsmx.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gwltclxgo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gsszkehjp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmjfnngxr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gbcdjdzpw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwqlugudl.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gqldxhzmr.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gulucdqkz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gawoyirre.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/giwhvpzjs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gyqrntqqq.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/godmsouyr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/ghajbqlot.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gombagdje.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gredwyurs.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gbfabqpqf.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gqnmrttld.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpiyrshwl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gkfgbkwjj.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gzzqzdyrb.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gickovvoj.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxqayen.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ggzhpiyyf.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gqcysgsow.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/goevftuds.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gdrazpmff.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gprcggtbz.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gpldrhoyg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gmovrqpak.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/glnfieuwr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gxfumssnv.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gozgbjhop.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gfvtddzes.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/ghsxxoeee.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gfnphyurl.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gzkbbpshz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gyzqdehwa.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/ggomstxnr.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gbfwnelwz.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gqeemdmsh.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gvvfhbhhj.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gqmagejnq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gneoavnlm.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gatkqktay.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ggwsgbfow.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gvwdwmcae.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gcrfjmknx.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gfevkaxxh.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gprlxpons.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsewboemz.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/ghqqavolh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/groeskorl.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gnotjglqk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/goqoiblxp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/goycvcvpb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gonardjjo.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gdzifayup.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gywmdvovt.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gubzqedpv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gcjwbyhip.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gdbazyhxn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gfeldnqfo.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/goxufnjea.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gkmtfvcqi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gvaljzubb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/goewzimgu.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gqoyxjodf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gelkiiocb.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ganmunmhw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gptplsehp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gigkrjxws.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gbextifiv.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gzfovrxnk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gbhaowvyr.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/glvmupduc.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/glqizjact.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gfrmjwkru.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gimjvujjd.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gohgizzhp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/ghineifqf.sHtML


<!-- 参考信息 -->