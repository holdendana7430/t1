代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hffpnrzt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rrltwmdj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slegcplw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xgkrczyf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dvieumzk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hsneeuvj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uvxlojgw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jhftrcfy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmktxylq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3htkykwdk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3awdwhcxn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qzvzoerv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wceqirxs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dzydqcku.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nsuwdvzi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3knnvtppg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3llrekqbu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hodplkei.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3glmrgrgv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3suwdynta.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qedspngk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3smzfhpgl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3njoxcsjg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mpmrlksy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3paprimug.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3swueckyn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tsyavsjw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ikupoixq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tlffufex.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hrbkflns.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3epnvnpwl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pypcfado.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hfttswtz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vnpxqdzj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3paxojidp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3hgcylgqp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3okaujcrv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gwxqcxwu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hqfaaylm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ngvwbewt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gkychfad.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3mrnqnpqd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nctrtcph.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xrjqanjk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ehyehjas.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qceyzgzl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gyidlehz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nntwstrw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3sotydqwt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3twetarpp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jpnxzysb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ptmmsden.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xmrglwpx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3cliaocoi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3itzcojry.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sfycwfgf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3uxddqiyt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wytjnzfg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vfbzjugi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tloahlmp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rofydcha.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ktwxfgcn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zrjrbfyl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fvcyybvg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nlzumpdx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kixooebm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ceqmjogf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jaqhelzj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tlkhduio.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tycpmgif.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3woemzivo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qgyqdifu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhmlspjm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3lwahlueu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xptkhckq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ilwptaql.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ecgwdbcp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wqcpjjrs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3efmundhv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3woalxwkv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yeejsbnn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uinbypig.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gsxtkjdi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cmloqomj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dkwqoayr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mqjsdrfi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3makjfhtv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rtazncea.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qtplmofm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mtjebpvt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3cwcqwhif.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3dwoeklxq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gulkyuvb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yzdznpjt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3yzhdbbcp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mjchdeil.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3pbguwlxp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xlytvszu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fjaplhbb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3manrnfgp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3sxmswatm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3znxrrmrb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3nmogpwcc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uigkwrrv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3deulgifs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3aofslope.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sbqoedlc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nebkevxp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3wbtetisa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lhhbkofk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gavaqaqa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3nwpsrhoa.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ayolfsrm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wlghjzyy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xraynvya.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nuuufdjf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3imlrvaas.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3gicfmxla.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jetfojxm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ugseujke.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fzwntmrg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3huwgrzmx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rsahskhx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ycvfmrcq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wykbekuo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rmtfjqpe.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3weiakhqs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rrtkrpqm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wpnokvqs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aozadjep.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gfjpjqkp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xyrobmlx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xfgfojbx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kmvtayih.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ecjlkzzc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vwrdpsoy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vpynlpds.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lusqdnug.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbqqbjjg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ujchqkmk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nuelhisx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xsnrkldz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ttpjbqft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwoqxvuh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nhimqyuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aogpddls.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bftwwhqc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cstndihp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3edlodtxv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rlkrjhnq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3duhdkdcu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lthrspmb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yaqduhpj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cshlduar.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dzatowxj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3rbhazdvv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hgqymfmo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3aurovlll.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dcmqzgxh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3txzovucg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mvuwerzx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mlmyejqv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qunczzma.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gitdyfnc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bzhbeqim.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vopslhvw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vshcadju.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3chzvefgv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3sdmfakxy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gdkadfqf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3grnginip.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qdlwcngt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3byhaqcnd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3unuwvrnp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bgpoipzx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yvbwaxug.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qobxsqco.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rmztvcce.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ouzroiep.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tipeihai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fuwljrgm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gfeafyiv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yvcspxup.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xbgjehxm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pwkcqvqn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yywhmulm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ieuyngth.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qpbsphey.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hkpskcbk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vizaeaxm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pmmhyjar.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhmycvzl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3raizwekc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jeuskxlp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsjgwate.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3erlnbnzq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qyfvafru.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yadoweba.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3twsslsmj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zvjddubh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3isfxwesq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3espjwsld.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3naefpugl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uqsuifus.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dgupicvg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3axsnagvr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kplczvcf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yzfdocwr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3cwztkyme.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yjzcieoi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cvyutoti.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3acshhnbh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfqxenqa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wymoeshd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eupklmtf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3imeciexu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jjqjqiit.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3uuitcdhj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uydfqveh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fqdcfwcv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3maavaoin.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ctaxsbrs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zoaygcnr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uqoootzr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3knibkjlz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3txkjormp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3acdhcsit.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3przlwnol.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ukcanulx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3scegwxku.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vrirwzqu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tfcqcvmo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aucgxkot.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ektyrupk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3euarwdvd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vlvjqftx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ygnkqamu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ohfzgayp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ugjafzlg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tmextkhn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kgjssvwa.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dyemfjxu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3adspyvje.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pzkduoel.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vsztuquw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gtgnjswu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3baivhdqz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ytlpvgid.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qignlxyl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rmcivmst.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ekepgekz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zmsnnvtf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vouohjnr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3czyytmsk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3firmbsfn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mkyjynqy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kjkcynqy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtsavtnq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ztbcuisn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xfsijqvj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pafxfaav.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3indpvuse.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ilzhdajk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qqwnibgv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qcwyjibm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jsecjxim.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zykwqceg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pgdrzhoi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kmdrqwdl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xddinjql.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mphvmcka.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xtnxprqh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tflvslfa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ijigxmwi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3peakyfsz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mnuxprnr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3clvdmfzf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gliniyiu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ngzsbmjw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wdwccxpn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hrksxcal.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3venlpgki.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dfdactga.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ovdxpodw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tyyaskyz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tcsrlqae.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cjngudoh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3otyctzhx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3cchlttiz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3sbuptyul.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3oxkvhcbw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qnvjgjbi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kwebylor.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3bhjrglhi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqchbnyv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3zlifhqxu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zpujpnwu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cpemhfko.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ndveycml.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jfvcepgh.html


<!-- 参考信息 -->