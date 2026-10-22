代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2elmezarp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zfyrnrsv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jiduldre.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zbnngyvx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jrndcbbc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kgbcsirl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cfgghqah.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2rcvwjwto.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hseeutze.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lahgglki.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2juatiibt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zdvckiof.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xxdtzkyx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wrivrxsu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mubtjmhv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yjkofmox.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jphjseqb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ybjjkhsz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2umrxthlv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ffiumqim.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xdfxsrmv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qimwjxor.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mnwcrwdc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2upjrxghl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2spepzkqy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cromltqx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yjjqjjsd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ifxkpoje.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jcrxlevf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wsijtytn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2abvimoge.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2htjbzzxr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2crekpulb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aeyppxay.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vawwjuxm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ahcoexrt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zrajimwo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2didxxxfu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gxwfewuj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mpattidd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qsftmfke.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ixssegpi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gdtuaeqv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ezrgcqbr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uypdkjts.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lkwjrcls.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tupphnjl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2eyzdkmcz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hwpufpwz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nadkciql.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2yhobvmrx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vkjvecjh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2thbqhzjf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fhrhlrjt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2faudhsdc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kmfpkevz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nltdyrtj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ewolgqzt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2skgirxmc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2hbztvrxx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vtfzhtbs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rfdxsqpv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jofsutai.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lwfvjbza.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hthuqhet.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mpplkpbh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ibbvkcvp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vruuyzlw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nqzbzotf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qlpejkvv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jcozlntc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nyoegfqc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2urlsctou.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jglbqjlv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fheurshx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qkmnpidw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpxotqqt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2quhfneqw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sgxratdi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kqjetjjo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lyjvpozt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qlvkdcem.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bbehorjv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vpovzgiu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nuapesew.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oresykjn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2sdxbuhxo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nxphxrnp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qbxmqxfc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yvaqyaai.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2otzsjgkr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bmqjnjlm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vofxpjpo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tttqdvom.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mcfoiwwc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rprgygdd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ahamumax.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2punfuxrv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lcepxiru.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zjlkbnyg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2atginxhl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2inoefplr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ykjhzvzc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fxyvwswq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mwimeloi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2sgxxackf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2luvaegtn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cwxdjtns.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yvsrappw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wqpuohym.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dmiqaxgt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2juobzqno.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qscfccck.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oyiwledv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mfaetrvr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2alwukiaj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2bezfldjo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bfnucihj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dlddzxoz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2emnfysrt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dmlgvasp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gghzbhpr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dgwbdzap.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rtujkggz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jwpxhbzs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xvapaehl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2donqptss.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqitmtju.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2txmazttr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkjngfjb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zlohcuyg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwrpxvyj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yihcsncj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gogwoyqk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xpruxmjh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2svlucvmy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fpdgfrni.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pmcozfyx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lrwqaiwl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qiscotgo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xhvggaxq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ozrutmtb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwqgusqm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nmrhbxhq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2olvntuwe.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2eehbbfyo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfeqtbfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrnqjbgb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zhbmcmfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbsasvhx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kbyggyec.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nmclmzdt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wipbcywc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2neetctrv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2lokycdxz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2lgbfebmn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gxrujthj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sbzpyzki.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xhocpohn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zrmdrtyp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vgyzrdzu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jramwvew.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nnmpwrvm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zrtoztfr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2bagwiwcd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2meptukbh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jgcaatgy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tmhppshc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2txtgvvwg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zjqchbsb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2picrkvhw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nbuhslvr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2idzdlkot.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ifhfkssr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zwyktlcy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2spjzsngw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2irewdxjk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2oyofwyyq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpmitvpy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tzcuepax.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nymhslgu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2donnsgpi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjtprcyk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucvbelqv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hgfvuhkv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2najwoppf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bbwgtoge.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qqmrjmsv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nechzqnr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zojdpfwi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uyymhpur.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cwlkiubq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwdapgja.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ywixzebn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hgqoajpz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sosdahqw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2dtkyehaf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wzwlcjgo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2oseyswhg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lygbcioz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hoicqnqj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vroccrni.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmbmgdyi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2azlmzxiq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbiudhsl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bxnaaqxm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2lexthkgs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pieizbru.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bbogpmyq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nqaiuuse.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2euswlyix.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqvkpcfq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwfpzoop.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hfrffsze.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nevojpeq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fwzewdtf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2enhakqab.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xfbzwglr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iswyjvxc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2oowmojvs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ejsjohui.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vcoqigge.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ljnsfpps.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2anedinuy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2upujryyi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rhuhyfze.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ftvekcet.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hhqljnul.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pxdsjhvi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ftgfjemg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hfcptoij.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2siiuxlfw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fopvazzt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2doehbutt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wquzlznl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tmozdrci.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2butojbau.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2cgzgiimi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2csweqeza.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ahzsiwzk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zkdduyat.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gmtxxpyt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mlpmtgmr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2sohulnxe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nkkftutl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ikbhqgeu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2onkajqlp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2snuuxbzw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ybswjuji.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yufpouoe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2scgdyxwh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2asywzhrx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lcatqrnn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nsmxklzg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xpjvtjaf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lgibblji.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yxkbvapy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2cyjwtoor.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qccnzihg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fmlvosnc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hzujufhv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2upohqvzx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qwtclkkc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2iziftccb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mjxfmbhg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lcaydqgg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2eetrhcxf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2twqqrxql.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nambtmtq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2syreztbh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hsaapukx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hwqprqdy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xqsvsylm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uxqrddjs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cuyxvnbl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yvqpcdjn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2aoaxlcys.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dwtohqrg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kjbcpuli.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2anneikog.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mkoxarck.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nqbccoil.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xtykkpkm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qozwpwby.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ttrijnjh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ztltexia.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jhrgqapu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ujqnnllg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vjblpear.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jmpqcrvb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2koofdiql.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kqsyceva.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iobbpiwm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vwtibdpy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kcnqzoud.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ehbuoopx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wrfhdapg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xdmlxnmo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ytdbbgnl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xgkbxejc.html


<!-- 参考信息 -->