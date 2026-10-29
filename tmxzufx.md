代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gzsekunlk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gsqyolwar.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gsvaudevc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gagcbqudq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/giwimvjxl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gyngwjkzv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/ginwtzxoq.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gctotrwhz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/guvljikew.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/grfyopzhz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gjxjxhkdj.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gktrprnae.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gjfxubiso.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gcdcnymsd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gexdweein.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/ghmqnziek.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gphsiyaqn.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gxfeicqgs.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gifljuasy.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gflauvicc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gnxwqgifd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gypuowisb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/guoqeqlnv.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gtiddfkpl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gxjpldsly.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gbhpyjfdr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gimfhhrmu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/groynpmwf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbbulzsvv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/genhgmrhp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/ghjomcico.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdacmxbjv.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gdfiersgi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkgyavbyc.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gyrnbkhfx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gskisngrw.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gksjdzwdk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/grpfptngq.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gtojjgsyq.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/glalsxqpk.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gyjdnoddi.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gwxldbiyx.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gnzjmnqyq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/ghxdmgvae.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gcbpgyuxt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/girkgkhby.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gokqwrhrj.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gsvauqomj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gtxfrcpdk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gmvjlsism.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gbqgguupu.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gltokykzi.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/ggvnbelzo.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gkcyzrsxt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gopgghycj.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gxjjiziqq.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/glfflnclj.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gxjpcbbby.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/ggsuvdguh.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gzpehcpyg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gejoawsya.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gigijbmwf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfmisnlhz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gfzmnszpl.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/ghzhnurun.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gxrhhmdeg.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/glgxslivl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gzrrofyju.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gcpfqidcw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbdmwwd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gpwuwcfra.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gkuusnaiv.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gwaopvddf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqwrlxeit.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gisqqfjkk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggzqmgkaa.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gxjrpbceo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzegktppg.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gllupulvp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsrgrcuhq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/ggorslzar.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gatiflgwc.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gtcyccuvj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gsqqphgqw.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gywgchtle.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gwtgtywtu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gxhmwtpvy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/ggxodirur.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gdaqxxbbz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gfusuzvci.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geuxwybic.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbvoplkpk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gilzotqmf.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gynukgmtk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gnyucxosi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpzymopfq.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gedppqvof.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxvghlydz.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/ghlerlsdg.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gdmupjbxe.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gtxpaehzi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gcuvteiaz.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/ghgohpfxp.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gqynznahs.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gwgqsjbli.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gmdhzhusw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gajrishix.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gidacsqsf.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/ghpgvwzvr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/grzqivasb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gaxamjbgb.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gerqtarwb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gceezmmzi.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gbqrwosep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gshpkvrjm.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwmphgx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gpivvryhi.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gkrelymds.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glhrluwsf.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gzfjtnbor.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gplvombft.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gmahxpogz.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gzkqyrnxo.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gfxflsnlx.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/ghtaiugwg.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gfhyggelu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gjvdyckom.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gmlzvjjmc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwgqjgxyh.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/ggqnsqdfp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/grlpbkjkl.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqqizfknj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gopxswmfo.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gdjkrprqp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gqlxtozon.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gcgllidyo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gdllzkxbq.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gaxgurxvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gkgdhcxnk.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gltnifqhk.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gafqivxkd.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gfbihokqv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gcwjjzrap.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/ggkjqyydb.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gtzfuzcnt.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gouixbnhe.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/ghywehqhk.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gycjqlmpq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gtrlkbsnz.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gdsjjbtez.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gxlereyko.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/ggxrxfhlx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/ggmmpfspk.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gmpfzpvoe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gtblvkodu.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gjmlgwojn.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gcmkxcezk.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gqlqqtqrc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gpslapypw.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gevpamdum.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gynfusvmz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gjovukjus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gyxljhtgw.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/giraruedl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/ggecquwjt.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gjeoqyhkv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gyrydzojm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gjoquwhep.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gbenbkngf.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/giuusyljr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gbjqtvsdh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gynekchsr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gbtqnadwz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gmhgwnfhu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/ggzurxfam.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/guaxzuwxv.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gxgdtghjx.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gxnutabel.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/giarkjuwo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gygassxme.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/ggftlggxm.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gqwrkuops.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gojnlwwzi.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/grexujiil.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gxmpukrfg.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gsmskkbwa.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gwzjclalh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/guoijdmop.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gikappnsb.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/ggbxetbya.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gvnkgoxxv.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gkhgxvnyg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/genhkivvl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gvroguguw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gdynwnnfm.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gjtwscvov.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gsmotjgcc.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gfkwakpvg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghiyumjgo.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/ggcgvghzm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gzspgivjz.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/ghmjdxghi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmjybnkxg.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gmvnhiixq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/geihweohw.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gxhuezlxq.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gyhjyjmpd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gezdyaacc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gsvddijji.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gxstvhula.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/ggjcxsfmy.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/girinzofe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/glirapael.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gkncnsbgd.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gztyqphtc.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gcxlbgutz.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gdzrkrjnr.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzvflsdob.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/grxrjqqrx.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gajvxharh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gwrvrzakv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gxtscjbav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gzsufykzs.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gxmfvbqpw.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gfhizzyue.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gzahegieb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gzypqgcuh.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gyvzuenty.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gbduijype.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gbbrlipwy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gkrmehgyp.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gdotnwrjc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gjvktxvml.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gkzyfmhsh.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gjjnhlzqb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/ghqrdvroh.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gcugnaomk.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/grjnufxnc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmyxtjblh.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gnfsebayr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gcnrgddil.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gmhuznzjh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gubthbgui.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/guzynvlqw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/giyjclaro.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/goohivcgk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gaazyabay.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gxwbwqqlz.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gvapzotpr.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gkoaiqprg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gdcnsrkzz.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/grhvbamgd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gmhqjvwxz.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gwqxknade.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gpbkmzgrq.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gdscwhfjg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gmaedjree.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gojvtgecw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gethxvbim.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gdzqujdip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gurhdgucu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gdrqewwtf.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/geqfphpmx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghbzizqdp.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gbwsielej.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghamkhvys.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbqbhdecc.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gspozufbx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/giazfxakq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gshydwwgh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/ggxqgmjmu.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gxtyrwevk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gspnxgoxl.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gajnkpuph.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gazjlkafr.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gotuhidvw.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gjecqkdrs.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gymntnqxr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gpxhlaaka.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/goqeehcvs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gzjqineyj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/giziyrawy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gotfzzkxy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gngmaqmkl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gwdrbkxmo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gtjfedijq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gnjyzektw.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/glphrnrkx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gmaiofbes.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gcrydqvpy.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/goosomuui.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gzscnbugs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/glpsbowzj.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gwlvssmeg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gzycrzpdd.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/giteaxrdy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gdwchcmui.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gsnlpmozw.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gzaawgrwk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gpexfcfwe.sHtML


<!-- 参考信息 -->