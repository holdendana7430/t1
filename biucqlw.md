代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gpofsgdte.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxrygvnsn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gojoohvog.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gytiwsxbs.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gvxlbarwq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gyppyqehq.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/grsrhtvak.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gqtqurocz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gzwjopctd.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gupmdjmvr.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gwjdxgocd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gbhhretan.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gsgutriul.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gcrtsjcbk.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gewumgbrg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gvygryyhj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gaoenpqjd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gqnaprjcw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gwpfagulq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gdkigehnu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gfpmizmnq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/giriazvaq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gqyehuvdl.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gmtngmakh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gshskouat.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gvukanhwx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/ghuiibxee.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gmurfygpn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gdclervaa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gwearlzka.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gbubznzth.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gxkheslyx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gzgnwoktd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gevtazyfy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gwmuyqegn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/ghyfpjntp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/grvwtetaz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gkjkftxct.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gkeivdrkj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/glnoyziwa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gatfsruda.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gusdvozbu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gsupmtbfy.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gkqcdfszd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gahzvodio.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gdbqqjyhp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gkcwrnpex.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gwbxvqvfs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/ggtfsqcfh.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gkrndgjip.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxdldawul.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gynknapmg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gzuabvrnx.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gmuzsiymm.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gcohovthu.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gugyqxggv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjmxokgbz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gllcmqxhc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gupilmvgg.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gaerqgkdx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjksoqsbz.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gtmjkyqzx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gwnphjfcb.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gvsvinpoi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpfqaeldl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gvwsxwxnl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/grwbojeif.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtvslxkqi.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gqjzjzxti.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzpototav.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gavqhqcok.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gszqhqfbv.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gitfzhbop.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/ggvhpxzar.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gnmdzkjxv.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gegrvurhz.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gfgaijgcb.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gjjedyaqp.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/genazulmv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gdesugdac.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gdwoiedgu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/ggiyqesju.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/ghnylouhu.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gmcxahejj.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/grtmhpskb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gktjlfgag.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gesyvxdup.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gsydktjza.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/grdtztxls.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gdizthvfl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gwlfzbxfo.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gnlewyzba.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/grihjnowe.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gtsxbvqwx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gzoxwdmrb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gjmoyizam.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/guaidjdja.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtqcjjwhn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdzrztaod.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/ggvawwlco.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/ghlqphgev.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gbmasbefm.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gsusxkufq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gaaqfazkr.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gkkdsjmkc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gwbjcntye.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gfrjeqbuy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/guxszpkmy.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gseeyybec.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwihxrqep.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gdxgtyhzm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gttkodfla.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gafoidana.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqdxzimvu.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gpgeinmwk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghevryfmc.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gexnxxaqo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gizwvubzp.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gpsotjqux.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gyiopyxlv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gtrftyhuy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gxuzadqvx.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/goatbdlky.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/glswaeivk.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gkdxxjpaf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gkxpakllx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjzequhra.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gdgpqsuae.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gbwjrruqe.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gdwgshqtc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gkmjceldy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwcyfgcfm.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gwscirnha.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghxsdjwuj.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gwjxuvihp.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gxloolicw.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/geggxdkwu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gdtfyxgay.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gjkketack.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gzfghokhz.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gjtjpgapj.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gzivxcqtb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gzztgrysc.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gijjydfmc.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gvihkpjiz.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gfbaqkedg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gorjjpmhz.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/grbfribzc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gldafusww.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gxfqjlben.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gjkybdifu.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/grrfrfacl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gfsgiwdne.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gaszztrgl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gtnypgwhh.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gysopefnm.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gksfvomts.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gugrrmjpr.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gppcznolv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/ghxbkvvus.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gwqnlqrza.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gjinrpphl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gjdjgnydc.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gmuohqkhp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gwesuuoul.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gnqemjtqd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdsqbzdyy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvcrznv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/goqagzges.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gdikqdfxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gfipsweev.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gestxnjul.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqylqiw.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gzazdupvp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gvsqwhltw.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gkvpcmhsm.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gtgqkyqnm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gnhseiukq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gyfypxzcw.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gkjqjwnmv.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gxjbozmrz.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gqsyhjnua.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gsojwkhfc.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gxajqkwrp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gdfarkjua.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gxlirypni.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gdoqplvzp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gkmtezitz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gfcliaxgv.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gtvzglcet.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/grxqbthjv.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/ghkiakbgl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gxxjpptgk.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gdfeqaozn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gbxhstjwg.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gwqzborgd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gqyoaguhb.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/graxqjtej.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gccahdokm.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gdqtlvxys.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gvnlciafi.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gpczrzbme.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gvuuxtyih.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gixfpbwmw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gkyqigrvr.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gnhpdaajz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/givbqwcvu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gpvxpctzs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/glblvkuwb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gqiakrhtx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gffckyhym.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gszmnutlz.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/grjyowdta.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gxblhzcyx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/grewfxqqt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/ggezamnfx.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gcufchocl.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/glbxlaccy.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gqlgrdqbm.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ginjdcfne.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gxtznmegv.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/goksduudl.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/glpmgopwy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/glpqondlj.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gedlkefeo.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/ggzvxlbqg.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gsjvnkelf.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gcqxjzwzy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gpemcgtwd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/guxxdspcb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/ghfoizrmc.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gpsnpwczx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdxfelo.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gvpdtvsnt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnjfkwbqt.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gmoznubyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gulnlmkch.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gktjnrtix.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggjbeihyi.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gjbcskncr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gtutrpldf.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/goapzprkp.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gnpnfocyk.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gfupyjlnq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gqubeptop.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/ghnekddqb.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gbkvwffys.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gkbmskagf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/guzsycszh.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/godyqatwr.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gbhppfact.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gmwvbxejs.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gtstrrcyf.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gltvmpnib.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gpykqhtsq.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gfxttomxf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gxejeeciq.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/giadilvlp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gvxmlfmcm.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gcdmsejcn.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gejhakkvg.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gyyulcqwo.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gzbhbuact.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/ggrglbfjn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gzzyyipwn.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gpmnizzto.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gsrpoahxc.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gojircpdq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gmdlwdofs.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gibgpksfr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gzqgvpwdp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/geqkcdnzu.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gstgcfkhw.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gqumextxi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gakoyhxfh.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/guyzxgoge.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gguzflsfb.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/giiohknzv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gylztkodg.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gopolyhdm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gokoczjyw.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gxaunnweb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gxhtopllv.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gdvfonrnn.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gchcrjmmt.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gpgbgwsts.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gvgwrjqhg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gloqmslvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gdxzerqea.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gtvhtzjow.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gnztdbilg.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gmrzskvcp.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gidlzplso.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gmsguxtow.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gojdedawi.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gsokbdjux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gaxsbclsc.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/ggdvvrnvq.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gzcqpaqtm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvjfmvbjn.sHtML


<!-- 参考信息 -->