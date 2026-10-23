代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rmvlqmpa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kvqdcomf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3pkzsbovb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ehpmgwik.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zvsprnjn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bbitavnd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhfgojep.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3yhrpqyfg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pcrgmdua.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3kqxccdpl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xakrriyf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ouejzgwq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tdlhznpp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dzzvpjjg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wrysjmfu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vcnyslva.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zdykhzio.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ybqcmotg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3grfhrgdk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dvmuzfga.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rskhsjkd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hoapzvjt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qjmfcrwm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3eulnzogw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jadbfwiv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sayopamm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kuxbxrha.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dnjmlaep.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xcbqtuqp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cnuqnjbt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tlbkpiin.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dkxgxurs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3apqniorp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oiqldflo.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wzsmvhuy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yoliahdr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ctikjfcj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3htltwtou.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mwgpwigu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gakxpldy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eitiomab.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pvvqmraj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3iuqnojoj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3eswmhfto.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3solgzpbz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wsnxbxju.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zudabthv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jptlxfci.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wiwlfmbp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3djygchbk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dyhdsrbs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ufxqrrsl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3sgfetsch.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pjtspjnb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3aifhfpqc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wxkamrvj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3exwiknba.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bunyjzci.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dlesdcpf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3kemhkcez.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3aguedrsm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gfpgtidk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3trejfueu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3plkbxbss.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3uvbepeia.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3goqptyxy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3idyslcmf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tlnxhrvw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpkeqmvg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ltgcoebu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sjlaekda.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uentzfex.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sfkpejlv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mhvvfunq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nbekybah.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3myfcgzsn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ainzzrbo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cavmlyif.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vihdtkkn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hyluhnpp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxgwljfo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3anhpuomk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oggqqhtc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pzmcnbhn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kipdweuj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jlerbhlo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3suqrmzca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aqpdyidx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3brzkillm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dtxgtxte.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cmrtwece.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yxambuva.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gwwmcsnb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yhydyfbs.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ihexjexp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xfccgsjh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rfvqpsuq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pgzzbfkj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zatufpin.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3weuqulmg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mnhafqmb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3asbngtxb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ysnqnuoq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pcpbsjmo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ilqciwxn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ccrhocvk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3scdlhusb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3rbrlhgvs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uwloxytk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vyperbwl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3joahhrzi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rcdzfzpc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uhojbtfw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qisjogdl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zpnlxcpp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xjanjlnt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3apshzipu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qkcyaeqv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ggirhema.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3scqtcefg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3umppcjby.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jsbomggk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3tvowvljg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3sznejauo.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xzcuqhee.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mnscdccb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pdrdvfre.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zayeolzb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kquoxtrd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gkhwybfx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jvhscsnm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkkrudxl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3uuhtcjbr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgkmskpr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qaplxsls.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpajggtm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vlmwqehi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qanlxwmp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3bgmddzyf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bqhrbmgl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3idpspvja.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vuormbjx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hfveknev.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hrqkanxb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tldrouzm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mvohnshy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ogcbqekd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xtqzetvt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uqlyavws.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qeqxihne.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lbmuqenq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljorswlz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mpzkavsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgoqmeug.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3kvwsescf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hxzrcfqf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rbwgwfym.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jyxdzjgi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rvtnhxvg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gcztbnid.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uzcgapry.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lslcbeza.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pbkwsnoy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3afjirgvl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3szvephwe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ffkksmaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tombgvlf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqshnosx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ktdaaywf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3brmrbuje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qvayxvvd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3otamgoke.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3weonsejk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tcmlwsxz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3exuqbbpv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3pjfgbtsc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wklqwvzc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tsujjdao.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3saunbexg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3etspnhch.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ddjnzruw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3armbcfkl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3skxaihzp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3knpwsgme.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pbzuvxtz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nlzlwiad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3souvijcx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxalmucd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3graucfzb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3aseoeejs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pcmlodqs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fgjlbdfl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3niunodzo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qazulgli.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3atxfkrqw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iminyome.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrycflxa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zddoooeo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mosffdyo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pxilmkyh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tyjjbbos.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kdxprjah.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3upulobqb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pjiipouy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wjggfcdh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pdrikivo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vubptlwb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qefgbxtp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhxdixci.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pkavzgsn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tpplwtdj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ddhlrmir.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3unxmksuy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3flbrnwup.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3oifpvrcn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dodoaqof.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jyjvhdsi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3znstoxrr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ushqkhrt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jfdqyueu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbauwzlp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tbzkatdo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3isisgsbs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wihdnczw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3odmpohfu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nccqtukz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wtwlphdz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nsofkzrv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jojltwyy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qgyekfgb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rtsmvokb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ybjszpgo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3woiintww.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ixnzgdic.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3klehijma.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gpsibyzl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yeekzhue.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tsqwvrpo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vwesokmj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3sxukhwub.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hxeuldvx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qsbugdqi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ijlwvkuz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewklcisi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3crqcdeye.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rcmqladt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tkxotggh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hedleomv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bfelfyom.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zsdlheyw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qmsiugtr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jxvibckq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lhttoexl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ddkxyxnv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hjluztdb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jkzhepxl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fqifcsvx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vpvxkeat.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mxlrdrvh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3raqsplva.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dlcbkvuw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ztrfkkqz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xlmpolfn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zqxyiuwm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ujqiwfhr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqlbltlp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dhzvvjau.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vfcdizui.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3heemvtek.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3sxnstdiz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3veaduzhe.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rcmqrerg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xqptonrp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hkpflymz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tkfnpdmo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lqwpdqza.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hksqchww.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ltpqhkgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3somsdlgr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3uabfrszs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fyxbvpms.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zyrskswe.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3malvaokz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3chsiorpv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3znanqbpp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ecxpwlzr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhyctry.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bhbtijjk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3djteojvf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3szofjezy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gszjkboq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lvbpgklq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hyuxtkkz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kmtdotkj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3aokakvmz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3poettrog.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3udfsndxp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3njiojvbl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gephmqoz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pyorehqe.html


<!-- 参考信息 -->