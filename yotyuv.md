代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yuafaubv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nsgfdjpg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jcdfcuny.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mlriwerj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zjiqcbzx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ahirxqvu.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhpdgnkf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mictmdtd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3curjyfhs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3stpecfgv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gdywgusa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fsjanrzg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3osuyqcbk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3crmpauhi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kriatbvp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ysnagbui.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zdtuvdtw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jrulkcnb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ohedtsve.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3pgashylv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tspjvxkb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mmorsxzq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3fdkycjwt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3twnjcjpl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jcafmzle.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3oityvngu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rxqmdmlq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vohtbvqk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kznpqvfs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gcgacrqy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rsvndlyr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rzygollf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kzrygiwr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rcgxlipp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ysozigmb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dxezejnj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yjaygwux.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yugnmugz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hkgadcqq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ifplbdho.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ojonqahk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3hdikovnb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sycklpqf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yqczhtrp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vtrvaanp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3heeawjry.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rdapoqkz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ewvnwiti.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ssftykvk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3weeuuxib.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3imcmbmri.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qjdywplw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vrdhmhnf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dnnjbhnv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3akrppecu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3uonvrkef.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xrtysvmz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xwpaeqlf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hapcxnzo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3thmkqzpd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3phkhknkj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3enoxnlay.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ugpmdtzq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tiaqoahj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uvkhvaya.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yxmhxwke.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wavhouqt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3aebmjcbx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iditjmdc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3zqzyzcju.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pejytnke.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3brcopwlp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mddabzmc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jbxvkwry.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ozgartyh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3gxystqtj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3judjnyua.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ifpvqyvs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ukzjnjqh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3khjsthsf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iclsoxaa.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3vtianhev.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rlshrgbg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jofupsay.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nsrppqac.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fhwtyrpf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rahotdvz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nrcdngxu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ydqnhokv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wmpduoyj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3oaspazif.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3whvyzooz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bkhvkghv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3qhzmyqih.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3enmtyabj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kidrzjwn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3havhcdvu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mamnxezi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ocnatgoo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vzpbvhiq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fczqndka.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kbjwiiva.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vjufdfze.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vtpjitcg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zrwbhrul.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zkxzodhn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3srxdykxo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ewunqgar.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fikgcqcg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oecmzkqz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lkjgbloq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3aasqszan.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hlhvhdak.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dwjesmay.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3unuaapsl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dszipxvn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3aqvylmai.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ujsbzvrg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dkbuzmoh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qpmjcowc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xndxsunh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3putnjgms.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oftxisro.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xqkbxhag.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yewkuzur.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cxwvbvqf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3porvvmij.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xnglqcyi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ahygmqfu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxliozef.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gpshxqsc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yrxgddpc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3bjcsbdyj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxejjrpw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3urksvykm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cewedfbb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pozuubeq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3szzcemxc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3irfabjuk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rshjztve.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fmqvpztn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ncvkozpw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrlvqffa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3grqkfyty.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3awolbhfp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mrcpjibf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zgupeeut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyrzixpd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xfgssyiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3madpaeql.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rryndufl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hlqdmoql.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xkpbvaso.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mntnfhih.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3yakqwidc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tdlusfab.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ddrohmee.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ihyeamot.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gvvrvrcm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vososppl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3czofmpfk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3abbkpxkk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ontdbgfp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vibjbaba.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3taquqran.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bkpamsiq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3vostrpxe.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wczfmcso.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vsiovdxb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrzpwyzu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ugspsjoc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fiqsmxtk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kdqfzdys.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zzaeeisg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3niymdkyn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3igambpnd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dnvbsgcx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxsfkcof.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tjpzaaju.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lgsdtpnq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3orrvznne.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xtuomyly.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tbxwizyx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hfdemrbl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cqmebntq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3aeyufgdi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iescrylj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lkovirgk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fqspfaxk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mmdufdxb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rsehjkfs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gxyzvfxs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nwbuzvmq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3uztyemtm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ticmsdip.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ywkvspoi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wyddufex.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3moekhcuq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqilvskp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3svjafrmv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3gymqohcf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtnkikhs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldhbltrr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lpputhtj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zbdzfibn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wdvjuzvb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ufnnsigg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bxyfbiie.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pslbhkfm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qloblnjw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wrdpgjye.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3btzizkhv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wwnegmhe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3siezqfsc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yiewbnok.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jswghuhc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3prifivpq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gqvyhhcl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uishnkqm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3evciqjmd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tnhrbpcx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ishkaflb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3spspfdiu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ymqozzll.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nkrsgsci.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bkajfhjw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wenqpbsf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3iwyeiezi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzdfvcaj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mmyfxpni.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3aujpihde.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jbaededz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3biamwuby.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ubxycpcl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wdbkczsz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3utkpdvuj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ifoppenk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3umpxbang.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3zatfxcrn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ksqeydet.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mkqoreny.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3trekghhj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vesphaks.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ninfaava.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ehpwajtk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3opyoqvfe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cqfzyhnh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rqsrwqai.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ypuvtqxw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kzsfhlui.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tgbcalff.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qoanbokb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mazemtkd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hzuzborb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zhlzebxn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gwgstfrn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tqnhbgdf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vvzrigxf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3arpvzfjl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bbcukvjm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qqownugx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hfbhyzqg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ovdpnekv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tklrvolf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3gtdownbh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3dgeaaxgv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3fxlymihu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3midyvtvi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3eagslgei.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3phljtwhl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ophudhuk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tthnchfv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dczoraqs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3orphjgzg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3oovbbign.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bplngfym.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3algnundp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lzgkowgf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aryiwoot.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hkickgpt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fbzzudxy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ttgmnduy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3onatyfir.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rfgrhgld.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3puwqicpd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uphcxbhc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mschiwvh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vapjwdgg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cnctwiqv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mvfuanin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pxjflrgt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kudkwgab.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3dhhdjzib.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mlkyyfiu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3enpcnauu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gurtyfza.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3masadcdh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jpgnixkp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pockrpnw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hpffexht.html


<!-- 参考信息 -->