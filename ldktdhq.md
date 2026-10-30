代发 wailian999

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gkydsefnx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gycztsuez.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gquoziqae.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gppwzkznv.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajdzquw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gsinxspcn.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/grhlwlwhh.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghratmsnq.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlsaznkp.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudbblece.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gkljyebpp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbiycydt.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gdcjsnzlv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/godmbzdpd.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvjpicpa.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyxhwmhb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtjmkhoc.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfaugimt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxffwvub.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkayxkns.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqpwjyapa.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/ghewddcxe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gaarbmvva.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzshwalc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjubfcjvj.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gptdovrnt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeqiinia.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmsyhhgg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gigjjtmix.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gatwhlbfm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrwvynmq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/glvglnige.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbifsoum.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gfckvdqli.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhiuqqsl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gstjchlam.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqvnefij.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzcuvxqd.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gztzadiqa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gxzocyxgp.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/glikqrkrv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqsvnpmr.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghopxzyss.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/godhwsdsh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxooqshea.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbczdcfej.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/guialyptw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsinhvyjn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtusfxdtd.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjwtbflyf.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/geqroxqow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/ghhnidtbd.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gqpjegrzg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/goebthpbx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsefjcqlr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gldhbvjys.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuewwjai.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gckfaovgj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlpahgza.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gabjoxarv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gaqaspnjf.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gsahhsvhl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gcwnwonds.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gblwbiaho.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzqvzokb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvzucrxv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gakcskjaa.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/ghtwjnpjx.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjwrhgyi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzycqongp.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdzclvdo.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqwxuija.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gfldsyyxe.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcjmimrs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvluflolr.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/glkuuycos.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/girbpfqqd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpwwabig.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmofsuwsg.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnolbatlw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxvxeujp.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gazcgjszr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyaihkvr.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcbwhvgrc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuabolpp.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmwgfvxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmfssndi.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gaymiuytz.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gkwuyrrqa.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjjusfoc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggksjgqwh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjkluneg.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gwsnkyoed.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtxzysflg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfwxoppc.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gzuumpoaj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gglmslfiy.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gojmbddsq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqhdgchg.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gghkslvoe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkyepxzs.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/guzalyagn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/goxjwvcca.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/giipeykyk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gairmnzso.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gblbrrkvf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwbtvlua.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gutlmtmhj.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbnskzfdp.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gjymppibd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glrujlwir.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gqxkavtwq.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtepbjepo.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/goggexqdz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbysdsef.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvdiscbq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grezmtikm.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaezfgov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpokocji.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/glqsbwhwt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gktqihzme.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gndogfpyv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcxlasca.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gxwghwkxv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqdszlfh.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gzihmtcut.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gvlyxrixr.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghoihjpyg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhnyvqyv.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzbapugc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gpcecwcyx.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gquzheyte.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorstfyrb.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gavjnthud.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfkvniod.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlajzdig.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gaowrdpfc.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpazwpgi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesotyjyc.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gvidjrhsa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/geiplifje.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gahndbklz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gunqafuui.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gltelmxwj.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrzisghe.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstqemgtk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gsxlrcljt.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gornhoioo.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmgogfsb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrvnnhna.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxazqrxmi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbijfydr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpbtxjjwf.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmckvajq.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkivjikzq.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/giuxgqjax.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvpufmsf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwfcatsi.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhdhypqy.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gxyppfskq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gefyomiof.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpcpozez.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaptqxbd.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxgqfiav.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnttkxydg.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gfpmxpjre.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhgshmip.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gabvchxyo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/glvzlamta.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrqteglr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grpnzfnxo.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyczjxub.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatwmdrxd.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvmmhzjk.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gunbftzpw.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gzmxaycnl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gusdgwlpe.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gatiivhbj.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsfuckcjw.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gqqcimnvc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gcovxgjid.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclejjtwd.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogudpgoq.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuoijeki.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gorhrcynm.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/glenniikp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiggwzyi.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gvznpsdwo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgubhzgr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwrblqvna.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gifnugied.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gspyfhlil.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gphnhnval.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbiojrrvt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnubcoimw.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gnepvgoxo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnvtjbis.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesopmcuk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gekmoosmi.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvteezoe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gcugloqqm.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpxjdunn.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gszvvrcil.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gltsxdkde.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gzxmevlhh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gocjqkoii.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvecswwjm.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxwbjqn.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gltpwklmz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtotppepe.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/genvgstcf.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvokajifa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqstapoax.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpjyidvn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjgdjeth.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gecturxgp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwhnrnv.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gsmtotsps.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtnonglu.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzcrkxwlo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gpqclqvyh.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glmhhozds.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqcnhcvw.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpugjom.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ghzbmbsed.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/ggovcqvku.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtewiuyt.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/goldzdihc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gugrxxdsm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnffynwbl.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/glmtontes.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gidzirwtc.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvxwpzsl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpmwfamvy.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhrmfun.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvhfxweh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gedjtuyeo.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdsbwmsi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqorrczf.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlhlulsd.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gqwlctsyt.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gokozazmn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbnkfgji.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxtiwqxs.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrwyjvwu.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gksinhhrr.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdwowgok.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gttrjbcov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveqbiwkj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmuumpjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsidkdeo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gttpuemub.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gmmimyelw.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gowycnlfp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhykymme.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gomcieced.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gknygucaw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbmnigms.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhdvwgky.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnaziios.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfcnczgb.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gznymxste.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/guatkmywa.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/guqdpqiln.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzztlaik.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gpksklwca.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehbglex.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkbsswhf.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdqlglei.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gymdtqruj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gpgsumjle.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnospoxnz.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gnwzvvvpo.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/goantzkxs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gzmaibrok.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gvlaxueeq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqbkdyec.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppdgaogu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrckmfs.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gdjzhlrmg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gxgbhwpjh.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gutclxtpb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/glmybnldg.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gycgzdklz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/geqiiaqgu.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoszpduq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbtutkt.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gmptapmdp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvqmpztu.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtjbkrxc.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlkofxai.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcjvknquw.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gpgxlubnq.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaxpexrfl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/guafepece.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvjaokye.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxkpqqynu.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/glyuhadid.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvqtbfxo.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnojtyszh.sHtML


<!-- 参考信息 -->