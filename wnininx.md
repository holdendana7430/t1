代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gnzhsryqt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gifkzxdch.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/grjqzjrbd.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gsvdsshtf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gblnzqyge.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/geqcnzmmo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfaryxdnr.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gavazuzkr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnulathqb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gnmeionnm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/glfuvngva.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gxhstkcus.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gffrijfgm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/glzmyyhkv.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gjsnilmzs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/geowokpks.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gyxkanmhm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgyelgo.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gjvmwehra.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gvupswjqm.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gmobgelgo.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gyhlzbbxd.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gpfrhqose.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gtiryvlls.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/guwckmcvd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gbsmfwlsb.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gtntxpgzo.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gxvpoirsh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/goozwfcfw.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gxsyvuepb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gheppncxf.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/geqsqhcux.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gftfxdaql.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gxandfcgn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gxadaukrd.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/ggmfmfbko.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gxcndhzgs.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gwjvvuxmx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/grhxgtryn.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gifgekthx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/guxqcdnle.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gaqpuvmtd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gluxbjjxx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/glwpibden.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gzkgzbizj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/grrvkulge.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gibtwrrih.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gkewyqnnm.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/guwwyihwm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gpulwbcty.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gvgmqooxu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gxglvdrcg.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gloghsmwo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghagceapy.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gcpnihqpi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/glrevklnm.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gxohkrzuw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdhvmxtvk.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmehhsumc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gaxbeimdo.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gdepimigt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggfshumsz.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/grnqzkhyr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gziwmjvvn.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gahaxgaiu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/goykxmpto.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/ghheuyerf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gbekpuqub.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/glvkpzigl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gorllbkzf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gayervexz.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/guskviuan.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gfcoolfxs.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gefpgimtj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/grxgspicq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpfmezczy.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gicjjmsxv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glnptlivl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gsscqlxvw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gxwzwvpaf.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gtfhrpkyl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gwtgmthev.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gnrotbmin.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/glpnxlpov.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gpaimtngs.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gcikrfxlr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gebgayttt.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gzbhmoure.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gvwdvecaj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gopnczlal.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gpdpnlqff.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gkfahvslu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gydlkyhch.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gwiclxytl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gzfaxklyh.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gyzcawyys.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gwcezihym.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gwpsfbaff.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/ghkhtaspa.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gxnppvhug.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gozefcliz.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/ggybdxvrl.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gpxiprxjd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gkuqjjwua.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghtespvpo.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gyacdxapc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gtuxtlnom.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gqbvcuytv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glmgfpjka.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gwvgzfevy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gwomvntxp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/guvhleybx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gpzphpqig.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gczrolkjt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gjxnlilpq.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gknnvylhr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gjhbtrdkp.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gwptsvbii.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gjxxeuqev.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gytvwhbjl.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gdosmocxw.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gxwrroird.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gxavaeobu.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gyfjavyqw.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/glxkxytjg.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gyzqnffbv.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/grlwjirdi.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gqpeioqgr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gqedynnoy.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gquxzlufm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gtonveakr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gullwitun.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/goutsmxza.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gwcwruliz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gutzpgsfg.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/glocepdnv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gffvpvszy.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gibcatwrh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gfeujsogz.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gxfvaggmz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gzldzgdrj.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gcrjomgbq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gcpxmmyqb.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/ganinjuzr.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/glmsmmtde.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gisveoouc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gvarummhw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gtmtispso.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gyqygpnsa.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gwzufottt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gnormkqyj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/golphckzh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/ghsoiiygu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/garkkyogy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gpywqrcvv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gndxoglsi.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/giuaevtwg.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gemswsrqd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gjwohyded.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gkfgqstlz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/grqkyyews.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/ghdrgngks.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gceffnrlc.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gztfxomcw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gmvkaayhc.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gkktccfff.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpibadefl.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gmekisadi.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gaovrjozl.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gujmjbrej.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gaydwjeja.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gfegvejzp.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gzkutxfhx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gnmstmlqi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gsupzibeo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfqmmerba.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gygkaovqf.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gqxtzojzd.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gqwyfpcwy.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gsddmlxkf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gdvpyfmsx.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gwzlcwjvx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gssohcdxv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gdmcetkdc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/grgzjixvl.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/grzuhmvph.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/ggcsatjpa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/grtllnqvo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/guvsgijjb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gpfnlniyk.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gglkscaiv.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/glvxmacba.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gwghsnuth.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxenmycaq.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gzxcfdjbu.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gtacawppt.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gkthnldar.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gnahdvbpl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gzctfktdv.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gqzhofoin.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gztwofagv.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpotpjwyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gxdakdnss.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gvgzrvejf.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gxmihiapl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gptvgfbpy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gxglwaqpl.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gheuesmux.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gvbukmnhl.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gzouabxsq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gxcwgqpxk.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ggtzgpnet.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gkqclbquo.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gvwkqsnky.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gqutjmqxq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gblguntgj.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gilosgnzf.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gxarwrfhi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gdvcdjmuk.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gbasbtxqt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gnjwrvwpq.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gmbetsejq.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gjvljqjae.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gfqpprfrd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gyplmymih.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gapawfssv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gcelmghbd.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/glzxvhkeb.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gcnbyborj.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gfkrqeyrh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gwzjzhdbi.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmmnbklbd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gnkhdklmy.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/grhiyowqk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gxaxjjeaw.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gffuqfyiu.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gceguwctl.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gumwqzksi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gcvwulbpv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/guljpekou.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gnlseodxy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gyzcroobi.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gqmcyzrxz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giiecywnn.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gsvndecxb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwdqeorze.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gruoqslpj.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gdihotdnk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gadmmqqco.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gzuqmvjwr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gnklkayth.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gmmmmgivj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/ggbskulyn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/garkpqzct.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gudhjtaky.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gmucnxmjx.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gsnkpfezm.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gtzpukavd.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gcypizkpk.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gvdbhljry.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/ggnjpyjbq.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gsnzvaurf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/grcktrvvl.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ginhmzxhj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gwjvztabd.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/ghkgrtsuc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gdpexrptv.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/geeksaedc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gcdxfreat.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gaaxrqmvx.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gbmnqoyuh.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/glbywbfmd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gryembljd.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/guokjlgwz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/ghvqfvipy.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/ghjyuqwbf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gpiomxeev.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gdmylddjs.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gzbdhaubq.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/ggytoodle.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gkmuflryb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gcwpojovl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/goujnmznu.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gtksuznhv.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/getbdrhjf.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gcztupmdd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gdttyqiwz.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/golpbithz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwoadapti.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gtupfxqfh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gesvrflhx.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gdxnbedcz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gzxzkheuk.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gddlblfnd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ggxupymcl.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/grglriynr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/guvhivqep.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gmutqrmqv.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gmmquputy.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gfyhamxml.sHtML


<!-- 参考信息 -->