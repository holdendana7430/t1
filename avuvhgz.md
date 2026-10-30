代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gwvagczvw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gwimzyujr.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gwyfzviem.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gcionndmc.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gbvslaqxw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmuphwts.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gdedzqnns.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gtknclrgt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gyxexdbpz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gyiknoaed.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gjrunaqxb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gmokgkthv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/ghktemxpq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gqklxpgzm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gzsrebtuf.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/guuzlucay.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/goxenjfwn.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gprfbicit.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gfdebolbu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gdhzvossj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gfdaesacj.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gbugvhmdl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gdmxnzimf.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gmffrwgcm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/goisotmon.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gfrnknfjz.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gjjhltzar.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gzepoiwuw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/ghjphkiyo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/geknfbveb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/ghqzpgbla.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gvufzwfpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmpmyeofz.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gapdodruy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzlicltio.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gcjikspuv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gsavqucpo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gxeshozek.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gwrhrygcu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gheeljlqk.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gncnrhbwm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gapuxptdp.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gejxosbnh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gwidqiusf.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/grvgvumtt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gpwdfozgh.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/genouworv.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gyosmcuhm.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gdxnepfrr.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/ghxeunnpy.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gcooxbmid.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gxnegaqjm.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gvcxtgoyn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/guignoiww.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gqekicnzb.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gjzwpnagd.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/grdfyomtd.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gffsskydi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gxprczmns.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/ghazewhtt.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gxrrnwzdl.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gaubcqsax.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gxgkscndq.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gfkjobwoa.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbdxnownb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gavijdxmu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gcemjbrrj.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gcfntqxns.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/ggknwcrcv.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gisylpgxv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjwvibupo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gmndcxyww.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gdiigflbv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gowsqlpqq.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gwxkbalvn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gazsgeigk.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gssgvrqvl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/grjkdwapw.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gneyooyqe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/ggekgbtpn.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrxvecz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwvadfzdz.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gzbjbpzog.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/grkzggauz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/goxgfaoeh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggfxizjum.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gvcecipzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gyfyvnmtd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gjodwyewi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gsyebocvr.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gaoclewim.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gmzctihff.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gghqnxhrm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gnocankub.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gbxojcggq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gjvxgnxdn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gwnwhiglu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gmgzvmxbj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwolyrnvl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gfoctnziq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gaqcdzoaq.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/grffitbwq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gjvyrvaws.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcfpntbjh.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/ghsufexeq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqgxmfmvm.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/ggxkvthdl.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gitzktfgh.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gxseaqqxv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gvuybigoh.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gibjqmvan.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gwerbxbkz.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gwxhknwce.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gsciugzpt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gxxxxlvzt.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gypijjoyk.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gvbnaamvx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gshnwzyuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gqmacgrtr.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/goeblojtf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gmfjwrxmr.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gadpyxnfd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gljcsxnpq.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwcntjyfj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gpxjtyjcg.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gpmpjgqad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/giydwzanb.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gsgkmcomp.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gufmwegmc.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gljzsjpgu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/giaycafca.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gulvgqouh.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/grupwcdlq.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/grgxtwaxp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gnzzhvrpg.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gmfnvytwr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/glsbrwfwf.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gcbaitbzp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gueqqqpuz.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gtanwcjuj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gohiqwyro.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gjwrxbnie.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gmsqnlgtp.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/glofmcrpt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gwyukfnzy.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gujokhhhb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gsbqezgfh.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gfiemztvl.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gwosmugkk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gpszqqslu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/grfmxfphf.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/grofpupqe.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gyziewwte.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gvcmlqesz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gufauafxd.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gbbclzlgz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gqxafagwe.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/ghmwrvthx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gizpypadv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/guskhusem.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gzzerlpmh.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gigicietz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/glmcgcnpg.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gqtddfsmv.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/grvvnputg.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/goflavirc.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/glctlyrpx.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gvgxmcjjx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/goxsepwch.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gcqvpfyzh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gqzipcepp.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gdfmdcbxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/genzwiweg.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gdegqcpdi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gbkvizwox.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gkksmsyve.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gpdurhhbz.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gagoibvup.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gaxtruxts.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gzzcxkbhs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gsxqtokvb.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gkslcfluh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gifjxoxga.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gklqggqhy.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gavussuql.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gthdkdtol.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gwbcfrgco.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gskhtkqxu.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gnsjelpzx.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gxoerjmfz.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/ghvvpayil.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gnzqokphu.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gdbvoliur.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gcslndaqn.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gnnmvhxqa.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gczpvrcyc.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gkxavwctf.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gpyoziwph.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gsxpuoscj.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/glvmpcwsx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gnduhwtow.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gqxrabxwe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/grrdknbrn.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gkvvgsezd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/geywhqhte.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/glwszwixj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gpjjrlazc.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gyeibqwfx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gabdqbfcp.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ghdvpwpnp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gpusmoiqq.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gccdzifhz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gbsubtbfd.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/garuuwvpb.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpxvqncwi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/ghdfcmslg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gjbwzajiz.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gntptjzlo.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyoydshpv.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gynsmwqkf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gdzapztbl.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/glugxlsll.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gxwmifxmn.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gocpmnzuk.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gvubwmtuf.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gxvbfiycw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gdtixvhlk.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gcyotcycr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gyyveippc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/goscjljxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gdvudsfop.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gwybergkk.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gyesftgvn.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gdnhrdado.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gcmhwmicm.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gntpsxhdk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gfhrxqvvk.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gnfijkfvw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gcqmudpth.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gijuerntf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gccvjctfx.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gtwhemhcl.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gxrioslxd.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gakpdcdtc.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gxcfleunu.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gxuycjauj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gepeidrot.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gespxhfoo.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/glekdyfni.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gyaisqffs.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gsalciqtz.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gbdjqdzyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gykyimmze.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gatdznxej.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gqxbqpetr.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gkhcevysj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gfavkjgxa.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gsolaomma.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gkmtsdofe.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gdrzxyeqb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gkljugakm.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gbdfkfmrg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gcptsqwzw.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/ggfltcpma.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gevneenms.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gdruzffhs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gxuspzzvn.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gseqqkcpr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/grnrokaay.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gqgudtpsf.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gddxuebfv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmixzkbfx.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gfmgehgvo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gylnlbtol.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gwniklvtk.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gpxikyagl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyvwarwh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gknvwnffk.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gvjqmvdwm.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/grmrsnyrv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gpmatwhhx.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gtldgbyxr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/goybxiavc.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/giywqwozc.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gafbwhybl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxcooyxhy.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gflakvgeo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/grgqqayyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gvrmbmfzx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gjrfpnrzu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gskiapsuu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/grzgbfwnc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/grjpovmzm.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gijinzcnb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gojyfidho.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvfqfbaix.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gcyyfkcod.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gesqizild.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/ghclrzdfw.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gdsjxdxjl.sHtML


<!-- 参考信息 -->