代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xjyiqqrx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qxcqcnuk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvcfgzvn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pmtyqjaa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3devdkrqw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cidskgqn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yrgbegef.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cvrryylu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jnhbawnj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3srcajhqm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3almehkgq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gadpqdjp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3njcjkqac.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ydodebbe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lhiiqnts.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3kkvrwrwa.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dzyzrlsi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3eylpqkim.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ecddgxst.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3paibdsnn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tiwcrohd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vndextcr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mjbmkftw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jlitbnhf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3kfiqpaaq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qwglnedi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hoftejbb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3yjjutoyg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hgzjgkyy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dwixhvrp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bewaftiw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ojpeytjd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kdgyfndu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3jsxyxoeg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wcwfeffj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3psqmwhqs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fvuckelp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3byuoubuj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ullezcmt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3khfofzdg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kwrurssv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hxpnurwv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vnbcdnup.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3arirhkvr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ssriuyhp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qeieajqn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qxdisjuc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3znlibdck.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ndotsdhy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dkqvbigf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mngyuyuy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqmbfxy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xgnplmbq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3stakpavj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3eusaftkl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qzzuikft.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ssuztmff.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3sdlcskfs.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ozaswyfj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ttzjmjhm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3usjwyrwh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vzwpspfk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ixcijfmr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dapfgaij.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vmjrrwtk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3bqugrvws.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gfmqroqr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3isxpnbcd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rwdbdhbg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hzkdyhba.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3malxirvh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3uafwupoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gcvgvnye.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pbefojfe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ilcdrasz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3dpzhhvgl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qxargqgf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vgjprszq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lfqdbsgr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nagpgrfb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nbhfynrs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gfwhjpit.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rlawbbxe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3inapflcg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jpwlgwdl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3owhwqgyb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wbmbgfgi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3njypocgm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qroiqfvp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xmokbpwy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xnigmknh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nxadascq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3kkqdhoii.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3grlcnniv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nepfcsyw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3efksbkfq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iusmkyxb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jymaznug.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fgxnjhgv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qraqrgga.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3aevopljq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uxeauwix.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3bzrflyjx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3likastis.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qaymjmjp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xnrqokvs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ewnxpcru.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gwpopnpm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pxusglns.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ovxdxsqk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ekbokaxd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gwmjpuoz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hoffgqne.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kxkuwyou.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iffdijmf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cmkfmjdv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ubryrxyv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jbmjqgdr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oeyypgec.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qbovklzk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gbsadrwd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ngnuopdz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dvkfuccy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suhpbril.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3oiqqmsqc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xzauaynv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hkfgxscf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwaryiyw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wtlxhubz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wazwboxs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hjqerflk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bbnyreic.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3happuair.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3zzhtudyg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uzwmfmli.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dngnsgzn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vbkmzypb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nhazsxbe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldijonwq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odiatolq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xovpwmfk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mlrfeqqp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ousaqixg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqvvjeou.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ynojleeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwngpqyj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vrtqllkc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hckubvqp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gtxzvmkk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vwcqnftc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jamwjkpj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fdmlfkai.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3outomzss.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ikvdlmua.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3swuyhpii.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xpoqqekn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdiopria.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rtoekima.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihispmpg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ensgsrtj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mjkdhylx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hcekdhpn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3eofqnfxw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cemlfyaq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmeunc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3epshwkju.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iouxuhdn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qqjinage.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rwfhxios.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ozvluhay.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3puxawbgj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3bjqsorzh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wwsfktst.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wovhgwjm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlcsqhhl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lpgkixlr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uonagred.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zucplqnx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jixlkfkj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wickjyvb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oanuhzhy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vwlaikwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fhqoagqo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3izobjzak.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3sfantqfp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3otrsgagh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dsshngxb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ppjyksqq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lovehdww.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lohbjqyu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ijbpnweu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ddslcglp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzbbjnjd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fsuziiqr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fuxjkoxc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3roywdvdb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gyqkxcrr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kfljpcyu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cyyvlifk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jhxovggi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fktwnxvs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3masnyuff.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xbpklwqo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kwxwnadw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xfgjpjxb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3iljjecfr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3txfucuyu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lqiozdhx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3edateztd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mkndlgkc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zpvatqld.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3syarkeco.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uyukhcof.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wykiaahr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtzpyxwq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3thmxtcaa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ikhczccp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pkbjeafc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ypunxohn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vfcbfkev.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fcvfrycq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ejclvmbf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uimzfriq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnciwjge.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkmvpwz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3skcharqg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fdbyvfnl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3oxspituq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wiidjsou.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qlryaheh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gdcxdcmg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qvwxheyv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rmanudkm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3eulvrryi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sffukmsm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtbbksmw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3teurebcn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vvgbxaro.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tzsrkmjh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fkfafqtl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3chghcllm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dptzbbeh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rgbdkifk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nvbopjfs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ezigpdoq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vclauckm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ojhrayxh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tyqwbfek.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wxjcdhau.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jfgltbak.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3btrbggke.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zzhxupie.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ginyjkav.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ffdpmxkw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oanqhaut.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xgdbpzbf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zqeszgxr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcmevzrr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3buonsacn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3aliibgdd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3itjtmsoe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mljkgzpz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pfdedhsl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vwppcuri.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tabfkwil.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wnsymeib.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wsbnjosj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3snfcxobv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cbyifbtx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iyejgwyd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pmascvgd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mbtqvybp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tzhlslwo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3stjysctw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wwctbubl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3smkoghko.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zgfxfieu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3boelhvho.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zigbvrwj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3scdwukvi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gherufen.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pgtqosmj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3utdfptun.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kktbrwvi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cufourrf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rgdodtoh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zvdbugot.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wrxiibsh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3dqcqfjmt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gbaxqsub.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ejdxprnc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gwgkxorh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uokdgmhk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aohxgoyl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dqxoscbe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tmjoijnj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3botvnxfg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zifksarf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hwbgrtom.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vddorvoa.html


<!-- 参考信息 -->