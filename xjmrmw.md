代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hodrzlcp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sddasxcc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xapjstbr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zftmaeiy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uoimspus.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2zyjkldvp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ajsitcad.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rfmyjlkq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjiwrgsz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ymvmccpc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nmnjrvro.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wspafjvc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zcnocnjn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rawrmrdn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tntkwxcc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pyfekeqv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2uqguysyb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ynhddiqj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pnyheqtv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2elscmwfh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wpcojqqb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zvtkqybs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mkulphbn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qclvxbcp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qzdeaalv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nelcvuck.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jsmzrbza.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vljfovvs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2fqlopryz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cfxcwlet.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2yuuzxxax.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ceiwlwal.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ehztxinh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vtguduvt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qkxltyvp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lnhvurzu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2pdjqzryl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2minipkkn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nliekwio.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2budthqjw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2irfhdbec.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tpceqdar.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nyedkjmc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wmivsuoe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dagjiurp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hynghxli.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2tmaxtufr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ecnntmzk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uelxvmwc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yjcckluj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fxfxltbh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2cdmeiubg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ajuimrsb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2eoeinljy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zycprcjx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2isdsuzrr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dmgivvdp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bmyksvst.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wobjwzlz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2pzlwhdui.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2imrocmht.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hwajzvtt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wanwakkv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2cuhvwrzc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2koeglwbt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dlaoivix.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jgrrtudc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wcvwlwnh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xavlnicy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2auvbomkd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lmizcsmn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ykkrycul.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yyiqxikt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ktpzsokz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vfiqedcv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2tigcvdcc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vyqksfym.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ycgkswyd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mvzywbow.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2acrboazi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kthokpri.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dhsgogrp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2vclfvfim.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nvycqvce.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wxyxwwzg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hpcmhqyq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vkoumnhf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ojeretzy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2aphgycrd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ckckkcur.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ovdkkdls.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gynovqic.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xfzktwnz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aytwjkny.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hnlkwedh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ccpviosq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wlwrwpve.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mnpsnagw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2skmjyxup.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dbqkwkfg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2byyjbcxv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zybdsdyk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2lihkaoaj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hoqvkdbb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vovopkkc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zopjuozr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2yzpvhjqh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ugzxuvti.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2frpkjtgg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hjaxrzqc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pzthhmiw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ejudcdnu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ewhumvku.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hvrnmvmy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ptenjayt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2yqrwscsf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2comusluz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vahmofyt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pswhsfym.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vhoddces.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oxzicdeu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yakjjxch.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cbxtjdbd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sgcvklau.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwlqsoyz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ojpvvpen.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2letiwvmi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vsepuqrx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2hwbuzzny.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pezqlkpm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hrstkrux.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cgssggsa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2coaomiil.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vdflzflc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2umnsqgwr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hvnztcgt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jvmhrxic.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ncjgckup.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwpwhkbk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wehdoruk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yisdsdhr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wauwwfmc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vlneleaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rneinqzh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bntcjvne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygcooccg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2uzbdcpvg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pnmxnrnt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oeywezrd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2usycnlpw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jzvrshfv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nbijthfo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2yjtwvjgi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wazjyhpn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xqjepgzt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tblfzlgu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nlljmabk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lnipcabt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oswfigeh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2fsziampe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ofsqemsl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2aksriajn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylxgovsa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eodtxglc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gqoqynba.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cmgwznhe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eaykabfe.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2herdxnao.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mlvhlxne.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rlclfqzx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jjqlxmzo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2opmyjaml.html

esac
来源：http://www.52xcode.cn/Article/details/gt2giydgenq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kaywakvc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2oyvervub.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mlntuadc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aqsglsiq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2sncublej.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yoluiufs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tchpsaxp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bkhghoge.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ukihuzvl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hmhqcihz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jpsghtqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2feeunfya.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ltbxlgdi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wuszdhjv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uqxtmwus.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rcnbjylb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tmzidfwp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2plbtgpvi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zhdjiwcn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2adakhghm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cchlmopp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2arlvcwtm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2csxzlvfl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nyadfmhj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gejzipmp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pfpachmh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zxiacstr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2miyqkkcq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxluifmu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cekpigjd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ueylpsye.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ruyjvhss.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ipmjuzdd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jcingwtu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqhlugna.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2feaydvra.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2odymptvc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ysbvtsaq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yvnlfhuh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ldakwnep.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dzejskuu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdiobfrm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rujrgiuz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mvgemwqq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2blbddlsa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rugxvwqw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yjchaoir.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2iljvlxdq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2gsninyix.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2eslhunqh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wwktebss.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tnzlnxig.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2niwuovrl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gdbkgryf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2jgapgdcy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bospdsbf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dnhhvvvw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2sojtcjfu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xmbtsoap.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pxveuevn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mqlpbroi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2syzpmkgd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tubndmdo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zmzympps.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xrkjtqmo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xduyhdhw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mlfxhvrp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cyulhyry.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ujoojmpa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2silwwzrt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gfhrbsqd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjybdtvh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2wbbsynly.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xnzytmsy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ikcsbeli.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hqvnqfiy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2iwvvzthn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ospodojk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rnoxijfm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2suckkijt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ptxhuqaz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jikpepse.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2oqnxyogy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2muvrojgi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2olqlfkyv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2phnwrmaf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lhkycfpr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xyspmzya.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uewqwosj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kyqeznkr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ccraxced.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cdckkthx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjgdqyxz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dlvmksbn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lmvpmwdi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wotunplx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2elcvrdrw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2iotccwor.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oyoxrdlv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mzktdhhp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2icvknxcv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2sjxddzmh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2anlfzkfx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2frvvzrtx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2elaxuppg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2igajzcuu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nbmlubty.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ispkwhmi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nxuoqvci.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pgytfzfm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2fvnjgjfc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2igyktyoh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rblhjdez.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2krnyrrxv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lurirjoc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yjkajpus.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2nfzmncev.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zsiffnfo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uukhoyof.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yfuvqitp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mzujmeeq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tuhfcckj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2apliqbpc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lfigmidh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bkewfsau.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vtmzuezx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zyyoeswa.html


<!-- 参考信息 -->