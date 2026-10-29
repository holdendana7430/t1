代发 wailian999

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gpofhgleb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gmqmzrqjq.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gtmrmfpko.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gcqzerykn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gihwfzeqv.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gfrnnrybu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/ggkjmtajo.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ginjwodlx.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/ghkxmzpen.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gnyukcjyh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gxgiiqzab.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gkkpmzloj.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gccdhrnlm.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gukixtwpa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gmrrrxaku.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gpeeahzst.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gxxpcrwrv.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gebtaaasg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghqfkjetd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gvyxhdnls.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gbbasftqc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gjcvbzxfs.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/grihtigta.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gnifmplwh.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gpticwzqn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gtzxptvxi.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gjtqodads.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gmcqiwkqu.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/ghiuyyjhl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtnnbssge.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gsxekzjpe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfpfrbrsm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gfuyjegmu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gazyxsfes.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqkiyidtf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzkgtknio.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gnujwzcfv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/geclcjgrp.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gkuawdowr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gncpnprcg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gjnzhaden.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gymdanmdg.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gvjarssud.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/guovzohkl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/grsaugofu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gnffpgccs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gyuhuihyz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gwfyhbfvm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gdnvsdcdj.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/ghnxsuabl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gxxhsywox.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaatuxgny.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gnfrtnhgp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqzxtvlje.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/glajbxduk.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/guadxqemz.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gelpocmko.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gybnirqsz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gplakgcfm.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/geivtjoxo.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gbgtonvqx.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpsklpwjt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gmzvlevav.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/glotyeitf.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gnbnhrchv.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gfrvmwipv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gjaeltmeu.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gmejwmabp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gmlnettoe.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gnmwzjyur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gegcmlqoi.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/getbdafeu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gxhbwkpym.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gemerceju.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gwgnezvfl.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gtomqoqhm.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gcknntlav.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gjuahmyne.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gvmrcaybd.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gvepuczuz.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gudrvbfew.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gokbppcwr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gkknhglzf.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gscrxkdtc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gciaiqqre.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gekfglptx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gbcbgzzyc.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcvrqnfsz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gtbzunvbu.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gddxetjtn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gvmrrjzug.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gvneezuac.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gtwadrujo.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gzmbqtatd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gbfhlmwtb.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grdfnhhuk.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gnumptghw.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gcurygvny.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gpuvrraqr.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gjvzysqdh.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gdwavcpnx.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gwsukomkx.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gukfpoddy.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gujnhhwga.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gjxsiihhw.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gxxwtslrf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gddhkwgwl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gtthbcpjr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gtvftdvsb.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/ggjxzbcgk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gcfarbtiu.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gmglqslik.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gwvtrgkpg.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/ggdlpopas.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gejtjdnbr.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gmdoxitfz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/ggqvafvew.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/grzhiuxiw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gnkrogzie.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/ghcecqcva.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gecdikphg.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gqxbmfegb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/grnezklkg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gusvarufv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gusghnfvz.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gijofizgy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gpkaavzai.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gfhhayomm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gixmtpltx.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gkkfcapue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gyqixaoxz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gocprquvm.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gmvgefxmq.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gvuxyhbij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gswpqqtac.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/goilmewyb.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gazgwuarr.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gqhocgyjo.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gledcbhyy.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gjfwypwop.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/ggzzlyooo.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gkxptjczt.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghkmyzvns.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gszprnyjw.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/ggtufjgzk.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gcmjaoget.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gjcjozgav.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gurzmsloj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gmcowlycu.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gqpynbdqw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gpjnxegam.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gfubgaonz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkirhkiym.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/ggbjadgmd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfyevtvsy.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gbjowfjuz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gtohqnbsm.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gagcwsgwj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gddzbafcb.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gitupxdtf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gmtdgojij.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/ggbdqmakx.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gakmqxrla.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gookymgnm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gjrpdxxho.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gpqxnvtvu.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gibnbfvuj.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/ggfkirfxh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gmfqizbsc.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/ggcjnawtf.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gpzkqurnd.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/glzkwxasp.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/grrcbhtvt.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gcptazjmt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gpgnxbgah.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gzvsogzji.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/goaevrhed.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gvxjiywbr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/glzdxxsxv.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/ghkpwqoye.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gzpiuxlxa.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gtzjiiczh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gpkyxrgmr.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gdbbxqycz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gamdeniyn.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gdjvwrvox.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gwebyncyw.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gkugnfvhp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gikrithbb.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gedjhlomp.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gcqwifqar.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gqzvulvyp.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gctpsmbcw.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gbalaweli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbhibhpwc.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/glkwftszw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gnpqmtqsd.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gwqzzppez.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gxwymphjv.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbrfllsvy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/ghokuezre.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gcodrwtop.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gdyekpzxx.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gcmudytwb.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gxbiqkxyu.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/glbuofnbb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gvizoodef.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gljsfbevq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gzkezcnzk.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/guvshrbxn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/geooqhwmp.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gsatibfon.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gcaqcwzfi.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gwimuzylb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gqnswobuf.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gfrhebuyz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gdgyscfxj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gfjmorrnl.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gtnvdvtqa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvwrmfaus.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gjrqelivx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtmwxdcdp.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gincvmwam.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gyelhykzy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/grlnmhzgt.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/ggyeneayx.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/geyzxmnnc.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gdhsvohtw.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/godvfxjju.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gpnhhotvz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gyfhmmhxf.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gmeigvwvp.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gbpridunn.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/ggtdhsxmq.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gxpdfjego.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gkijyajpg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gczgtrpvd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gmxikxlpe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gxvjiogmy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gywleymyf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gznratlvr.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gcvfsrdxm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gzhuecqwr.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gjxezfacg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gdcbykujb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/giuouqlmz.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gbtntyjjs.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gqunwrmdj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gdoudrdht.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gkyjkzidh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gwywjlwuk.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/glsgguexp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gcnlpgjkc.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gnxbcapcc.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gmbezzmqk.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/grhkjcmpb.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gnjfcpwuw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ggpepewjj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gtyclqgnq.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gondlksro.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gwuoatxpc.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gjnzyvzlu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtrxnwris.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/grjpquxla.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/geoenaxwm.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gqlqieqdb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/grzokuyoy.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gtfdrehnn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gmtpsprmf.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gfrqjxpjv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/ggyovzupr.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gpaulvvzs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gzlywurje.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/grdgfgldd.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gqtpzfvuf.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gwzukkyzs.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gjihkghly.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gdqyekvfa.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gsnglusue.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gwfznddhl.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gshpxxnfy.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gytjcqbkn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gkwgrgxvi.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gwrnyfzsi.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/glnlrcyek.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/goqriibiv.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gmwzfaanz.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmmuvefto.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gjphqwmia.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/ggzaezkho.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxmycuqwk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gfxhenyjm.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gjrhnsrno.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gqrungyco.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gpntmnmbd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gicvynuzu.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gstgrwzzs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmnytbrnm.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/ggzdjpzdg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gndlwcyga.sHtML


<!-- 参考信息 -->