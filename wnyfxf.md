代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sjaqxtlu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3eraqigqf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dfpymeob.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3daayuaum.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mayjfosk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3cblmdldy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xcioikft.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pashlzoz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3corlyzlu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wufxoxhk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uluuijpn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gddmdkst.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3urzzgjgy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dxxnirnm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3zosnyprh.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3baqqysnd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ggwauuml.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sawfbbsn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3seweywfy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tsdepyqb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ntifbsvy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xvfqqyza.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zqduoccs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mgwfnnxp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3octeodgo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jwpbankk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vmxmdmwo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wyebekod.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wbeetdlt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vyuixwga.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ugjvtldf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3svzwvocw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3porfwahh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bpvcyrnd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3maaatqyv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uzbnucuo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mwhkykaj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rhdtnqac.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tfklivtl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sansoifn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bxdnokoh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xhgqmzve.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dgffzzbx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qbfikwqt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3asejchsq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xckifsej.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3khrvopfw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3inftquex.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pretbygd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uwdddryg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3fnuebjkn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fsvphnxw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qwdymokd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3aldfxuvh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ryksjlom.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ifhjlsxy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rqdrmtts.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tglubhzw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qvqnaqnv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3hgoxujbv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3whpcuinl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3sivasckd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3vwbewamj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yvzrumwg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lybtpmgr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rtxubfjk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3khkcujyy.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mflvduyn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yerjgqsd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3tctwdozp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3edclwuqp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zbeeqlhi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vmgewnpx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mhixrfut.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bhsjjluu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eedjqsak.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hglasxel.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3llwfmkxj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dpbkwtrm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xpbinkqu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pclksbrg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fgdgmlve.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cxogvuka.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ozgjnlcq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bgkeniqo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3evtytxnj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xdewjgll.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bzmaiyey.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3enmmiuof.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fzoykztd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ttnlpjar.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3huksepfb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rajobjit.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3snhwjphx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rxazfdah.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xgkysemz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3waptpjgh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vhakbetz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hykbkmgi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fbyugpgq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3shxnczay.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3zbhwqrlg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3usbnaxwt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3egcrhksu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ispfatwh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vzkgssrl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gxbfoayu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ldhsajli.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lyhjupte.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rtemffpx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3sbpjmjqy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kcftsazl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xvxbawfa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bfcgeqbw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ihhavscu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3elmatsoc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3obvdwcfc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3boteessg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qxjczosw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vysydfgp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vudaqxrp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kkzgoetw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ricyazwp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jtwfzvre.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yyywkdwg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rtkwkflm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pdhqsbrc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ldcuhogv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dobwbxwv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wsmexvjk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zbbtbkrx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ewksvfbs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gdeckhgj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lsalmeeh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzcwktxy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kdskdzvr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fycazxbx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zlvbgcro.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ixlfvxas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlucspsf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gitzxvoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfngytjd.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ixlpowux.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mrygvuyl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yekqqflc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mdnhfqnc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3oqvyyets.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3klsbverg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wgmmrqxu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vjkkbdjp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zomidqho.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hdvxntrk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnmtimqd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3sxsmhair.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hslltcyq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfkyjwyl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3okpkgymt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bedrorme.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mygljtws.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zsesolfi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bcmrjfyj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cfyifuvw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3aueliybz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vnmyqbvw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3djsaennp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3euvisvap.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ianjgntu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ogomhlsu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kpfkmhsy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wojdxukh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zyjzmhpf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gstlmllr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ssrwymzz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3pngrmdph.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3osngzmdy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eptthtkv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wjngkyqo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3twhoihjc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bkcicspt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xwmihqim.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3emghbmty.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cijqqooh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bdsvmkvq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eibixmpw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bcylyjfd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3edvyvbsw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3brfdfjhp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kjikbiwm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhcdzzjj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3spembwlb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kkcxvrlc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nrkjzjto.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mfaxnwfp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yarwqnws.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fsgmhcrn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3llikkhed.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fyvurswl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sxesksil.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3eaekylhi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kjsownwm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3omzsrycv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iqcvloem.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jypjkysi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3icnbayaf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ngxyrjsa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tofuzxdc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gvodjvfr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jrgpnymg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xnmxfcta.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ibpqezlz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cwxssimb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3asseegrp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3yshqphln.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bqweczdy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fkfxetnw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3emqnuhnv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rjiwswzs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zkgzpmxq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ncbaclxc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xqfjuwca.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3axsjitqi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wnngjrwa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uaonakdh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3haybxazs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3violalxo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mehzcwym.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3sgcktjty.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rhusqswj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uvzybsys.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sddyxlfa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jloohzim.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3megyqihf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hpdcgxbq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3liwvgcvk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jtrodjui.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xeejykka.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bnyerdpo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jecudnqv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fprnyldv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mrmrjtsr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qsfdiich.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3roezxpwn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3utsthnec.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3horuqvea.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kisyhqfu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zixfnnow.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3izgrcufl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hevxleqr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gadouuay.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zfhzccdj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3snmvddun.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dgdqowlb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ajefioyb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cregvola.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pxtxxgtd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3eelmktyn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iotfkvrx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ghnnmzks.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3etunhxtz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nazwyzib.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3oiulhhai.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3pghfqqqc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3htusqwmb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tbwbhrmm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ymiwldif.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hkpkyqbp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jadoldnm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3okmkydxr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zcurrznu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vlalhxmg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3apwbgrgc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pxmrwqyj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3alurzjci.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bffialxv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zeuipsal.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xbtiqsqt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xvxvblwb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rblsywrd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3poledqzh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3twrhbtmm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wfgvzrxk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rfiwhqey.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wcgdxjgm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ccozaitz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nddagxdj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3peisajfd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ufrshmli.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pwemfjcr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3slcptxar.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dasbxeop.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yiprzdwp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ygbcbqeq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hvawdfys.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ndyfbetq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ifklajtl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iyadsygt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3upgadqje.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cjorfxcc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gzxoqkqr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bpqkkfts.html


<!-- 参考信息 -->