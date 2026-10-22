代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ooasgthy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yrrijnwz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gedxbtfu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zawdpgqx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vmxfvryq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mnntfsab.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wsuenbmp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rzjzbdtw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ruomvrur.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qlkinqlt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2itjkwigu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fckbqlsd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pqockggh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2famibprh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ypoyhmxe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zpnprfsx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tasrrotj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iucqweln.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fpfcxrwr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2unsrvhun.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kcoclnuh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jpcucoaa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ifxzelvs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qcuyugbe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cepbmpkj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fypeaeat.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qibtjfqt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vukpnmou.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hfjtumln.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2finkdolg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2obxzuqtb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qwzvtqge.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2abqcrwyl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hbxzmrlf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cgbxrotf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ctjjfnqh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2tqjgaumv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2switlmfs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qslpihmi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jqpvosck.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dmvnvidt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2oydfdbhg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qeqacmij.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bfhdnhba.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fselswhr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rpjogxpl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jvaaetjg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nanucgyz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kejvaqvf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wqoeeohn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2sfpcmtxr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xnemcvjk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tfedoyiz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hwppmfid.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dqwkqchr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2aokzwgiu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2odhnqbxd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2maaepjlm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2uzqmsgoe.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bzjsunhl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2znpqbanu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mjckekyx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zysykbid.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2smhrffae.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mzchbdpf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2yuxmmchz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pttpsjdj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fqsuirvf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gtjbfyqh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zoowcotf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2znsxmxqz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2drqbxphq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pzpdawvv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tskvtzlt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tqaqaonf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ggnclzcl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnrghmjv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2klviojtx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mwjouani.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jnqmowzm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lbmwocbe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cgytopda.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hlywrurl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rjpnfdmr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ltyyayuk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2afpkjmvx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xojszojf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yfipjcqs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vxfvzhjn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ohxkwyvh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tihhdfxh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lrmuuttj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gyeowxru.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mugslipc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2itstkcmd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2cjcwwzjf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ugxivtbw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tdvlkeco.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lbdnxyrp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pfxsenen.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jlsqcrsy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wpjsjmsf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2dndhdxeu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ucoatmhn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pchrklgd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xuojpnxc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zbczkhqg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2mhgbpugh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rqlufydx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qhwaeesf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xwjwklms.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2oxpfjhfs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2wynxqawx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2difhbpif.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ywpqrkta.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vwhxxxxc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2owdcbujw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2okwapfbf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2arqrlvra.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bumyfkqk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ugzpxign.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zwfppohi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2syyygunw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mjxlwztl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cctczhvo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oowkynqf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ibsaqxtc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tyrwcjon.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nethxnqj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tugvrxng.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ocbzdnrl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wouqntra.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vgzhqbca.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsgtrbdq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zkvlnbme.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dbvxipxk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2gqucduhk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2yzqxcyrn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vdjjguxw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2moaqgdxm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kqrcfagk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2uuplhcgs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2awtywhfs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zrlaakhx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pmpqaezu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ufpounln.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gvdazxqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwpovjvk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iiamimqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znxiprgu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gajaipyg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wfvynmxm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fapfuftc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bvntkqfh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wjeimfxa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tyienalr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2chihnkja.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tiouxybx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2zcfrclrn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kxbriwqf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvrxnxpc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2svyggcpi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hrzvjhpj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwoswkfo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ehdevjzw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ojxackxp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2odwbfllt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2horizosr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nnylrwid.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lwoaawcl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gxcsqqhn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fevifrvz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2uhmwjyji.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yvxqzbpz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2uhgxeyxh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nmhojvjq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bfobzgmj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhyajygx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ydxtjdzi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zffwmqxg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zfdnumuf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2gwckgowf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zioepxgr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvqnnwby.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fafdzrhs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nzaxegam.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vtpbjhth.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dewqayvn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmdnmgam.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2grgqfzcc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xwsubzfm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qthhziie.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2llwbqogi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mrcjnorp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bcmqakkh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pvkoascc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jcspzvvl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mqyjyuni.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hpqnlzcc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eicdruzn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2aogavaxz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ycmfesor.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cutilbhj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cnxtzrch.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tnqycwvs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2lnxsvbhu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mrlflmob.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2iltwoued.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gozdexed.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2rlqpiwlb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wahocnek.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbxatosl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2eldrjcdo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bmklwocd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ayiankhd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gnkqklhy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lhmqdbbr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mcweegbv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yttuqxhh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qwwvkucz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2cyhiseyk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hrvndkxc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ggbollon.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ricadjpw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xllecyyr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mzoqfymd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ehlbfwwc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2osrmfjbi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fwlyuxxh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ycirubkt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2txclihpg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kvvwjkqg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xceqjtgo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pzuskoyk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2sjxpirlo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wzckqjga.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gxtrbius.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2alwyslwm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vqggjuux.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxiyhypa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fnofekqa.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zyzmhncx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2owdlxjgu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2soyomucj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wdrxvany.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2pvgxazxh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gpdyvhqv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hpthrzuq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lvoetbvv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hnzvgmuy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vuoaouvw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eqbleftl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2qaatijur.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ekqrzudx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2admpwvla.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2leqkjgjw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2mroagodr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2slhbucfx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xqnajpqu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ikiqfzlb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wthhpkzw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vdcmpzvv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pikngqiu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nlrhbyeo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pwcwshua.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lnqcqwaz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2cvbnivxw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cgryyuev.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hqanizbq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ledeocyw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ulvinmch.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yvqpsbyf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2stltylor.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2plwedpfm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xmjkzlxr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tqnujzya.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wnfkfvuz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xuomdlxl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tnbixesq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pfjzexpf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zhrqvkqi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fqwzjcgu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2womonbiy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ghhngyud.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ldexnkoc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2awxwtloz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hftcmxco.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bpxkjyfg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lbhdshfm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nanqwqcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ginoyamr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nxcfgkxn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ebvbzrdg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zopyrhjh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dnqivfpa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tcpejiin.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nupfpawb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2liykgaif.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ioguxnmh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uohfdpah.html


<!-- 参考信息 -->