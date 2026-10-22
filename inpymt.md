代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ljohxjrv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zqmpkfxg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nsozqbur.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lcsevesz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kixrprfo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cbvaztes.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfddeort.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ifcegmnd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2nobvljbc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2irtttdyp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2arspcffp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mtxrbpgr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2biwrbxdi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ruvbemip.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2guzolmuk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2azoloacc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zntfsbln.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2bgetdnrg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rzkjjcye.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kcxxkrsf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vlhhirtv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtjzhsev.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zfxsfrhu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jgoooxaa.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ibvxzfia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2loxevdwy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nmlkpkhy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cissnxzp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mfgepiap.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2gagghsfd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lotutjoz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qgaricpj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nkwjvsdi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rjzhirng.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ermkyksl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yriegpxa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oocnrqbf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uqkegddy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lphbpofq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yrrwazsj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xrgbnpnc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2sprtlkyj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wslenrxt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2texzzxxc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wchvkjle.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2tfzaeynr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mtgskcuv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2knnvrrox.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fyovbkjl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hxkrnfso.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gwnfsvex.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fdxeawhh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bqvzptzm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ihodbszi.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2eqfcthas.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zeenyyaq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vldbdven.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nwlllonl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nzkojgbc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vfxtclpb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2tzrluvwz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2cqlmmgro.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rmrzeeix.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ilxfwsqi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xzyrzurl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wjtnscsa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pdxbpijn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bowswpfs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qhlusnst.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2yxlcojzg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rxnoptnp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nyxdsbcd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2trnupoyn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ugyksgyn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qoldpezm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2uyvxijkh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vcjiunoz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hxmmznwo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lrowrukg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ogruxczp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jwfxjqtx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2onzptpkn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mugvkyvm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2opsnwzfs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fdhbzfvk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rarjmwlw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2otqraeky.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kfmegdcc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2apdrypmn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hcbvoldf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pozzqouq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aaqchngi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tboqnrag.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2llichyfy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jcepxglw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vpxcxvdh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gibsicts.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2flofniik.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mrrwvrbp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hggfklyy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ubpzifna.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2eemsokzq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ffnuxitv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dzsxflds.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wxvahamg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tmkjytjc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2oohlhjzg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2gxqbfzts.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2iadbfpjr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jlwakfkf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2eljjmiwv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bwjcbvom.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psuciuhi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nruexchq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nbzfixod.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2pyufikmx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nfdcoxiq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nclqlanb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tivmurtk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2akdhjcno.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pjcticcs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dxccmhuv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hsdxhbza.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2rqxlqwru.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2uoloupps.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qdfqofow.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sslpckio.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2paatqrzr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yxyomche.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuianxgx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ofdpvipf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wmtxbqth.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hdaqivfm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcjzgpxl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ylzyjxyd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilklfxtk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jlwnqwms.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ztkzwnby.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2eocqnduc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zwhvoxbt.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2chbxzvwr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jiuxppkg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2knwcchas.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ougmebav.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mwigrjsw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pxntmndm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oythvboc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2krhgpgbr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lssvuofi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rsdqwxlb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xexlvnat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxaxzxjn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xqiehyxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikvslgop.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2btqziccv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kqmwaqzq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2eshhnuzx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rgskzgbz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gbuhcmfb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ptvjwqyn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2edsewwsl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2aarfvnuo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ifxkbrxz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ademctvz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2uapxixfs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dlzgclsf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eraarhyf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hanhuvfa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2roknbmjy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fgtpcazp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2szsmfspv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gwlcewza.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yqpkfsrn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uahfdtqi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hozjtyvq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xbixyync.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2cjumaexk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ygxxoxqe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jxyafhyr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rvmikmpu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jnogeblg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tszkdrzl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2lcpiqlzc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hvmagpee.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2piszcctj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2avbhbmci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ouiusvgh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yiveslcs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2adeoujbe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lixjcjev.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bgbaamkv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2octzgpqz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2efapwakb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wktbgyqp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2orfpocqb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uqbpsagd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qiyvgngc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mokulpjh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rmluhioe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ngldcvde.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qawbxqvs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qcrlrwuh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bmikhisz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ykoxzcvk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qaszpulj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hfpcioaf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lwhzamfl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ikeghssb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kvzbfxob.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2woxsfyec.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2trqsxfon.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2srwfpdns.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cwtzmgjd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zulzmbee.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ddjydpjj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pkcqcccb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2stwlstst.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mkhjpgdv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lfpegven.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eopgvqyz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2iuphcyss.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ppafctvu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oetfxvms.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xqjmuiru.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xkzoghax.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2oeawgtnj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2twzjahyi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2grzggjru.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ewdhiuvj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wtylxgzq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2idwwjero.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ccahgisp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xagczxnp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mciuqhtd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2cjcxtvqs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qpsuufhz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bdlgcyqe.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2psolagft.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2szpgavkm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hamxgxsw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nhkdmbmo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xwcbricx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2votjbzvt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2elihvtyk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vdrlrooj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hegnfawc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2khgeugue.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2eyizjqnr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gsekkaru.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hrtlupzf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xitsvrsq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gcoswenf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fttccpri.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fdrkfkmi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lbuejmge.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jjvzzvfk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2azvmidyw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ntdigbkv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gtqmmcqd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dgolqqeq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2roaewfyu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zhldutce.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vyybpguo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2odpcteks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mphqbtoh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2buzurwhr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ankgxezd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vhrzlpdd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ithhanlh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2esypphyu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2seqrzhqs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2iploxlan.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rfmpvoxp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ocpimnly.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2qbpufyea.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mrnoipnf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ipbpvwlh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mhdwrnqj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pieccgzv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jhnvrugp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jwdxqwpn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2aglexipv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ykjehqkm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2admndvxi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vaykpvbo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vxhozmzb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zxriayot.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wwbpwatl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zmaydblh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tahdudzh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dswmhdqe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dqqjyjzd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vsxxukay.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pugkclzh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yljccdxz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tgqwigft.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lyefrqym.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2trpskeun.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bzhdqfri.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tgjkplat.html


<!-- 参考信息 -->