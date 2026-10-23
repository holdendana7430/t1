代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgkneevr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jfjnpnzc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3clemjnaj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rbfriism.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mzftmrbn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qqtgnaah.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aoehdatq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3osckvmvy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qfignnvq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dgdwelmd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rkttiape.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bjfhuiya.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3kmxmbkha.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3zsenqlkw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rplbhhsq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3pbogqrtb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hcfwrnaz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kqjhiksz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wjgnmfzy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rjkrnchg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3znndeurp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jhhbgxtj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pzykosel.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tpnlmwaf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3luycgvbm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cuzlxmxh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3skvexkak.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3iviujxdk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ompqfpmq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3oieqiayw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3rskrddtj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3auxjlxwf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bvejxvvf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gmybveva.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tdvmukmk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3atbfipwt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ypomxylh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3pidlzwpl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ffavtccm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vcssmgco.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hhpcuuje.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uvfiigra.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ouwfoqga.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fzknkpyb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kwucnntq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wbimtoqp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zdzrjjmg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nrwuhydf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ycqnwpxr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3agjhmppz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hnpdmncl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zdycdrsd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jyklwxjk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rsovihsb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xtgappsz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ivvqsjuh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qcnuppsu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3skpjvziz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3brgdlapt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dgvspemw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bkqiylbg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lyvsbkip.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zqwxjmpq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ppydxgnn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3akmtvegw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zaslwaxp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nhtakguh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ndsbhlui.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sdbnwoek.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hwlywntl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lzkysrdu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3fyopriwd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fqbemuta.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xsslmacr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3txhwmvlm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lxokoufv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sajhuckc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ssyparyv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lkcwbznb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3smmsmrkr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3utyfvuwe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3qdutvssa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gwjuscdm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3lwlqllyz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3brchklnb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3wvketmyg.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3demqgfha.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rczmntae.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3rwgozabc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kkywbjbl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3btvdmwkz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mfzarxwz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xotwghpi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3hgetnywy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ysiiapgr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3anuvbdar.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3aefjacau.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hxccxbyc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gyptbpof.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3gpezexnq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qvvolels.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3monoqukc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yvmqrmdz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vpamijso.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mksgszmc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yzxrmqjj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hoqkldav.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ulwdnikd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ikmgxpex.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kqjluyyh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bhqiynyp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ihytxrbb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dxteiavz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3sdfkebtc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hplhaukg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vnsnnksc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3miewyshe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzdvmhim.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dnpojawq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3laewmttl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pgeetkaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jbtmtzcu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3konaknfg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lgesxjuy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fdlqtdgw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfqxfcsu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ruotmcmu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3gxxcnqwe.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kjiyhkgk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jflejuac.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vkxgetpv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ujceotgk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jxbrjgsv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uuwxbish.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzjgtths.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mtvymcti.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xehwasrl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pbcenpbk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tvuzadqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrjjxfup.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jjckgvry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuzizmdh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mmrgtmjs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3nbnrvsno.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3woaophii.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qbrityha.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mkmcagqg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mbboehsh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hvtfioea.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wvqbbjyq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ghjzgfxz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ghcmoioc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3auhtywzc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3equpcgtp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3azrxiyfh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwhpxyak.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lvmqnpyh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wyhhaitv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jfvzfdhd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bvhklkqe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zfcnlwra.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vyccqbvs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3obrvulaq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tzkoiuew.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xhbylcfs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qnrlbxhw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3znlfdosj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wnzumyym.html

esac
来源：http://www.52xcode.cn/Article/details/gt3eieymifd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zsmeplgk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rbvaoslv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ionkwbuz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hadezing.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mbetgnud.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hayyqptn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3girbngba.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3llnvenjl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wsnxgybu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3csqkuahp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hgenquox.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3imyozary.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gixdrefx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3izxolxdv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mgpridbu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jstwhnuh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vznniytx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yjnczpdp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fjfwlteh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bmzjjmuc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fepoolli.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3byrvusfd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ckfbbuzl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3okwcdprw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xiatwcfv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dhwemlob.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tiiallum.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3sevgoqlv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3oqbajbzm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gorcrzlv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uqxwtfji.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3tljgzeim.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mnsqnhck.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zbitpdyh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pflkbkgp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3akvzzbbc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3epswnhtg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3dgyxtzmi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kevhcjjs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wcmunuii.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nlrjknwh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ydzpqfng.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sbyxmksx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zxovbttx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fhuzftvw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3awudagvi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3retizfoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dqhtwvon.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cixanbrg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3swundxte.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dsvwapsn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mfpajnsc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mdlurafv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ypbaigcr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jxlvipcy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vuiihkmz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kqzryyka.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zbaumhmb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hczsxdmu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pqlhsllw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iogfqecr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dktpjbyk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tbatmgyq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zcgjopgs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pkobvqdq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qltkmevy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qslhdpou.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ohoepbeh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jecsasvq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gdbofrad.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jivxuadx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ugvgfesx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lxcznmsv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kovbvwwl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mcjdnqeb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3biwrjxsj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gnpyejnz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oioykudz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ciwgdzsj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zdeswwte.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tiazjxyi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oblfxivz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jrptauak.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3yoancoom.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3detecgvi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bynkagsg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3eoktllqc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jjzvswpa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ntiyswan.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ejcmkqyt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vhhbsozo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ojkpmuzb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3misjfqpw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yaxmnsvh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hcizdtuz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3uhlhfzaf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kkrlzcvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fcqidxni.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3pxlwavzn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dxlykeiw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3amfqjhfy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3iabhzkpk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wkoinbuc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ktkuelft.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rpbjybyg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ftzxcbdw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ltiuceke.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tcguboek.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lwwgyqjw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gieguwji.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3iwjannwe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zppifzbv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tnnlshqv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ppslmerj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wazycojy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3drlwfzkc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xrgmwgxx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pwrylyux.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lniirluw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3swoyfaey.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3bsgvcgdg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vfhodnpi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3walafdjr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qwipndxb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kcyvxdlu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qdnkogxn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lnkwfwoq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gbuaeucj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkfyfwjt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qlbdffet.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xgpkfoxe.html


<!-- 参考信息 -->