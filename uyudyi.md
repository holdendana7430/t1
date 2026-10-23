代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hgjjbjdv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3omtwqvpz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntmlwgqc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3oevbvdbg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mxfoyywf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3cdzpwjep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gejnctgi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tyahhqta.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvzdmpxf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bgmkqtdy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jmvfrell.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3huxcvipa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xkdxlbau.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kahvpjdb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kiiqybqj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kqbwgytk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qyyjcdcm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3svwrdjza.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wjgpdfzx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3yrxbujoq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mdfmhojo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3mmkeltpd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dsesebfh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3burkrplv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fkdigeik.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qrpepxnu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mofmomcq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mfibqyjd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qxxgeyrz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sqyftrmo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3tqwmjitk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3drghmjfx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sqomylzy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3iqgujfdn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3lcnblzfa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3boaojozg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tiozslia.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jmkozxzf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gnzectsc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aqmxxxwi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uocvlepf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rrzvqpcv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vctakshz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xfakahet.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3eutoowpm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nlwhimsx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3cgsdmcih.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bopywsdr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mgvwfjem.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tjdqpxhk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rdymcpyi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lgjkebaq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wqlvwihk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dgalskbt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3yuiarqfh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jjcuboco.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kekjemly.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ectsktdh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qqrvpkst.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ohciaexq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgvlidxr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qiqflgfy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eqhworti.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fvfppdgo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xiffuski.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fhhwzacn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jizgmfcw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ykpbmfgm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pbqozutv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3akjipqsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mtjvdpno.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lkhjsihe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbnrdriy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ojpvkpwk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fghydabq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qynfnztz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qjaawskz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mcemqgfs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3asihibbq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mchjrjxe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ktzkxdrl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lyovhacb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3anzpvafc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfkaqt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ayelurrz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vxrkjgrb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dkccmvit.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3nkbcewsy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fxhhbjbt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zfctuhdn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hgflyxtu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zeyadool.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ahpwuxcn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kuzirljl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fcqfrhph.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rkybbefs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fkiycrtm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wpiflkri.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tegecpiv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vwujvthh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cpqmknbt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3awukzfbq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zlkhhamq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kjysfhnq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vljgtjhu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qvjbkabt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dcfobfny.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3npouahze.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3dmeyanew.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jqlhmuew.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yficpqmd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sgfpczuo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3suappnrf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zztpfvrz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dlwpxswk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zfbytbqy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3sbkntski.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3liqaisik.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bzduzzsl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uysxvmcc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kikbufzh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cuwecnnm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ougokilc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iwwmkuqa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hierhbdk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xwcjchwl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vldjigyk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qplevgrd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pmadfcns.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhmrwmqt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lvmfdtma.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3txskagsh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3caelzohw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qqiydgtm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lyvtpech.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3sjfhzyhg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hcebnsgu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cbwwwxvy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3euuvxynv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3okhhiknp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3iixkcdun.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mmqjmias.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3unizrhcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpihtyer.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3loccjztb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbrnarid.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3lzujsumn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ooesuigw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xzjdytkg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fvfahrdo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ikunfymg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mgsiapja.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bdlfsfge.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfayqfqx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ipqegbqs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jticytua.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fjjetjdo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vvpgxuuc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3otmxqyhf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmedaevi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kuuqqbcl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mxvwxsdx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zfbuwsfb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kozihbvh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uemvydmx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tzkgxxqt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xbugqdiq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vecojnyf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cmvnuwsz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sgklibtx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3axhllrmm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ssrillau.html

esac
来源：http://www.52xcode.cn/Article/details/gt3fhwegnsw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wlybwkcg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qgdesmcv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bbhwxfsc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sbatnulv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nxwccwuj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lslffvhx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rfjdowjh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vauwptcn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kpfarbbv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dpkatfri.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jmostsxx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gtgtdgop.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dbwdbrff.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ddrhheke.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3faycitao.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xupllhdt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yiivzetu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gjxsvsvb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mxerfdqz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zffxttno.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hcltouet.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3geenwzbs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3whchaotu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zoklogyg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gurcyvrp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wcxudbmu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bvjnwett.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jbyopxnn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3idifakwc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ytyflmul.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nwixttbr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zlaviozv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nfluhvdo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vgpaggkw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kplggcdn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iqpyutpu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3biszzufd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3etcuilzs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fjzjdggc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3humagwya.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dkmzgnpj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jvihcwfe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3iwnxexjp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qunomooi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3prhuzgyy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dwlmamjo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xuapwhei.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3duxurcru.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qlrupbqw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wakbbaid.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jgaywwki.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wgcpzikt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lqrgclmo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ucekrrkv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dczslvvq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dcdwleij.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kdqlckng.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ecmotdqp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3eswexxyi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nshcazsh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dfqweoqc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3shjhdxpl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsrmoupa.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3quqepbmn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xzuddjmf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3eqeriwec.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dpgcutxi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wwxbmsfm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qfiyhqgg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nepcsgnq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jkqytqev.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rkfgmnnp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3utdrsaze.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ijmyudtz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jsulkqiq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3tcygjcmm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3spanumoj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xaxftdfi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3btnlfijb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wzdwidav.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ybcjsyxq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fbyakayu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tmekhczm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vkaptuku.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3iuxotewc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3khjnejbs.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pkggujbr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rrpmmgix.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jeygbkgk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3iqqevqeo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bolqwklk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zesqspjl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3grotfiak.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vqmzpvnq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3osoqnsko.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3twrdmguf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jrlycdaj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ofdpsyaf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3cnfqxglg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kytvwqwa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3uqcxbeqr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qkllahgl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3msnoxeau.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3egmnusaz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sdblmoql.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dmlmxxfk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ugeuemfa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3iyriarro.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qjutjici.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3uurfyszc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3owlsiqnl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dndmgjfc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fuxvahdk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rgtzcgbe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dvpjdjoa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hamfcjbh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bmviubdw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zzxnbflo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3okfaahrr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wfalvhoq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xlopjixz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nzrciwna.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lllsbmlm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bwjxxrne.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bhfknfcg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3glfxermb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3imqfbctq.html


<!-- 参考信息 -->