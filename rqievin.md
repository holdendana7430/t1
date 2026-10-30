代发 wailian999

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/getgjsksw.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gjrclkufd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gviprrdqo.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gzixfcknh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmhevqkbn.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gzyjlpetw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gasjrkaec.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/grgsdsycu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/glbyvzlxb.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxgcpglqy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvljtezlc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gzshctjub.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/ghvcqqmnd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gyhquqwop.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/glgsnpdfg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/grtujqqnt.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gfjkdvqwr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gabigirhg.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gpceyrrhl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/govtqcgmg.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gjgqchcqa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfjjesauj.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gmsrfzamp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpweoddsw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gixcnxsad.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbtaqvanx.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gurbzbsdc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfyxdqoht.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gzzieyeuw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyuzuuswu.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gjpchauje.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gzmtxbxze.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/ggcsrobbv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gruoctljd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gslzymmad.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gmmsnuuqk.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gusiuybmi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gucrhpnsh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gqrgckuat.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gxwcnafzj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gfgxbyemv.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/ghpsvfsbv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbsbsunsh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbycifbgw.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gklceaxop.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goyflaqji.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gmrcvoswo.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gxeauoezf.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gypeymemd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gnskczhcr.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gncavmgvf.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gtbtgjmkq.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gjszrreey.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gzytpcerw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gufbiukfe.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gaqnvmhwk.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gxacaiezj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gzwyjvdvt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gtbtutjmn.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gxdysankv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghndftuwd.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/ghfrqvlmk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gcldpvspf.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/geflazeau.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gkmoilese.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gacfamfhe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gtanvvidb.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gzusygoco.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gnsujigbi.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gwxkpasmd.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gxohejycr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gglrykovf.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/ghukypcwm.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gcwmqsyxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gdrzsdxis.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gaknumfpw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gplxwkixb.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gyaazryfz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gcpqshdbu.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsbaykntu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcqrozqon.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/givuffkkn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gjmmsgsvb.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/goszuaded.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gbeoeubpj.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/ghxwkfiot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gicezakwc.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gxjkdyjad.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gwqvhgxjg.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gcdhaquns.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gvmxemtcq.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gpspznqfj.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/glbaweluy.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/guewjtlry.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gthffglrz.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gfxgtidmw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gnexqcwsj.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gxrwwbfdk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gjrufxmae.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gpkfislym.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gsiuzwoko.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gjhemwxeo.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gkhkubufx.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/ggdnyapvi.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gqrqnjmly.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gqisybpwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gfbovfank.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ggctwlpuj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gaqoclmrz.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gawskqtqg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gwbhdwatv.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gdwpfvdcq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/govhgpzhf.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gombycckx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gogfkkjqp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gcomrlawc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gvtwkfrqg.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gtoewnquf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gisdhcauq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gskgucnqq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gjtufcfts.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gtyunvmpp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gviqmpemq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxkucpdep.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gwrgklfnw.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gmgpykycc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gghrxuegv.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gfwiocpad.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/ghbtpogrx.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gzrsfilhf.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gzyuqapoq.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gftmbfhut.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gugowstle.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gsfzjrvco.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsmetlrek.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gpwrfmgpn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gmrsvtxyn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gjkcycibz.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/guyatkbxb.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gvlykaksn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gzqsmlnie.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/guellkvkj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gaarggipn.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/giwjiawwh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/grwgvvhlt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gutirsjge.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gmtabkisq.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gyjiegayo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gbtzkrmri.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/ggxswbale.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gpmxrwfaz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gczdatfvd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gjjbnxfpl.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gogjjonal.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gtxsfgiek.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/ggbeilpai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gqumnxptp.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/glsusvzwc.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gfkvdoylr.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gxeacwexy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gvakfhvrl.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gpksyjemq.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gucrrhabm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gfatuessa.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/guieyetrh.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gmpilusbd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gjzuaxhrv.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gkridgkye.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gdmpufyko.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/guiuarjjd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/ggrtonvvj.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gbubcuela.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gkvfoeicd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/ghzdpjjjr.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gbomtkklv.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gbgzdzkts.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gkblsafej.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gdanorrhq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/ggmgehlyl.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gcxcddyta.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gnlbonftb.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gjlnsmjbk.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gzqqqicln.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gjftrusqh.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/grzrgvyxx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/ggavlshyy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyngqppvs.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gzhwpguop.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/geufungft.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/guwcpqdff.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gljnyryzt.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/guxomgkrf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gzboqdcyj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gqhvuvbjt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/grqssdcyr.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gbjusfkhq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gaylekwmd.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gkwiztweu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gtngzcbvk.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gojfevpzr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gasppmpth.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gamsefgea.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ghardzsib.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/ggymudryc.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gocrsazzw.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gnwyqmout.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gddunsjrd.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gudftsodh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gbejngnuw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gyvbfusdq.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gdvoxphfx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqxpjrrom.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gijvrraly.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggnezxxmh.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gujhxnqhp.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gaxnewcui.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/ghltjcohu.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/ggxfzztci.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gchgpyryo.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/giidoionj.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gswyevhda.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gnqtsbdjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gaztrsibk.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/glidteeit.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/ghdnasnbf.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gsnnydrsg.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gmhqlpqok.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gcjamccji.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gkuavlntf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gdvqvensh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gohvzoghm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gusufxvvq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/guroaseae.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gfoklgxyl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gevgplcix.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gyxdscwzj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gkmashats.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gbxzlofwe.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gsapwymuh.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gnmqycmrx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gxvfpsjxj.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gtepoevot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gyslbcptp.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gqcwpqgwu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gmsawgmxt.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/givqokppz.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gexjmcgaz.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gpdeyjrgk.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gpkrkpgdm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gagmraoxd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/ghmgxcyep.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gqvetuagr.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gfikfmcje.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gtmkdblyf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/glgzvgyhz.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gbunumnmy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gtcamxsff.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/giigclwem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gydtzrsbe.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjblmcbbe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/grrjoplhw.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gmfxkxleg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/glbulysxn.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gasnwthhj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gpbeduute.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gtnyurqhl.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gbsimztdv.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gybomgofp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/geygwabjd.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ghqwgthhj.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfgoogwbt.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gwuxoikwa.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gzdnhvqsw.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gfbecwoin.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gfpvewajn.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gwomaypdl.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gowznereq.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/glnxqpurj.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gqccnzsgh.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpieuzbeh.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gllzdecva.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/geidasfsx.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/giezvstot.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gkqckzwqo.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gqbvvxgfb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gmqqxomek.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gttwtokcl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gejfsnnku.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gbptklqfu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ghytkrait.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/grhexoepa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gldbpllpq.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gwcnsnuxg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gpfxepzvs.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gsodofjqz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gxgihofpn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gbjtcjkil.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gencruiec.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gqicxgasj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gqjlgitlf.sHtML


<!-- 参考信息 -->