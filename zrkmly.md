代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbmifuhg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wkkyywby.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tsbiglfc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3upezwylx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3valvuucd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqaoqxqs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mevjxuya.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3tnbgzoiw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3swufsebz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pjvzfjtk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ydopbeab.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zeayybik.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3lqbkgngj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wiejcsib.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3iqhjxdmk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vbkuiomu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sntdxyli.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ohhiobfl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xldxppzu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qezlbxbp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3euaqyhad.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zrlhzcmg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3yigxiqtg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dcldwkdp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3gfkervva.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qoqqfhdy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fqfemhfv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3jbyqmbnu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3buadkeeb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gpmjuezs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vlrwvnje.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pmwvyluq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ogynustw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3lnhpppni.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cjpozbej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3grmyqjrn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cnvzajgp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wjfwxjwi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ypdebppg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tfcxqeeg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ryglhiki.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tyxghfkw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3auwjktoz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3btplvhyq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bjkghrlb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vxacplmr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wexwhjau.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kaelalqv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nmcueotd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wfbeyhyq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rxvkrafu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hzafaeks.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pttqlhju.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rgivblsp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mszgwhae.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jwyrfzxn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wvaohoth.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3hzbmxudi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jdpxctad.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3mzedpuvo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3havldqmv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jupnhjjz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jgwylohq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lzsbrspe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3suwhpcjw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3uqhtgfea.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nehfnrum.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3bwlcuxvw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hrvotjoh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hfxumouo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gfevfgvt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fdztsczm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3eqwwrmpt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fyqjkmxp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cqcxnsmd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3izyjkocz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jzqyakmw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tcemhimt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3slebbczb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3evwbqcxi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fqelcjyl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lalqklae.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3gkvvmlqg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ftdjcpcg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rnyugxkj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zrryeqak.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3jthyeeik.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3shkhoebi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fdiodfbt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3oqtwkizv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zfsqduyq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mhpvwpjl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3egtysdwx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3urnpuuub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gmswmpok.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kzyywtjx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xeffsiba.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dufvidym.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jbmdgknq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nlxoknqw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rgsrzzyo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jmxmpbsy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vuouozyn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3dqltzaur.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3grzprens.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mgwbzwdi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ewdhvjal.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3fqanvvnt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3lwumswir.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ggvmrdal.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pmlppugz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ivlqvmwi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mpremhyy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bulxttos.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rdxpxlch.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qyczdkvg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wnispufs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suaoojmg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3twctueyg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oawgwhed.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3icpgnuxg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3touzudcl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3chyfjzfb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3cwwwegqn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3afiakeol.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dpncdnkb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uwuoxxkf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3svzuuwoz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uzozkrxg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zfjgtdfx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmabdlea.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lmhmabaf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ckhkhiiq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3apreoibz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3inrdiwik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyfbwdrp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jcisuxpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydoauizl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qxquqtxi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kxkrqiyi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3aogpkemw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nypwnrii.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kwwuwjkq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3svnbuueb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fltpolru.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3sqthpexq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ggegbzla.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aburcdpi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3havgbnom.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wmvkfred.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rclkjaxh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3trelhohw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tfyyuatu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdlaxeyh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zqvxenfq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oosqtnzj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3blblhoqp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gohfffcx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ockpxseq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3bnfaqsnr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wasdgjei.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zfzdwitv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3japxsizl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jmfgckvd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3yhxylgrt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3opfrafgo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kbseqwpd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3itqicfio.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3edgjjrag.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dvyjvljf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3oxtenhpw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdqkvucy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rxguzjqs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wxzcfdyf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xcgvmrbe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tulvbcli.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3kcrbfcwb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ufrfxsgd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pewhiswq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3yahkodcx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jmnfiquu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3uwegsssi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nrlrnmlm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yuqrfmni.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3liuizxdk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bpnwxjmi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rnepiwwz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dgvbvpty.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ivejjmmj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ktxbhqce.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dgvfxyzo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vdacooob.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3yfbzbmou.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qgffnqvp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3poylbfrt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3copcmhgt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wyrftsnv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3erqvdgjq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zxxvejzx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jhnqmboz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3enukxtrc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tiarsddw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hvxscuzs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pxzybgce.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqyonodh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tddovjpj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddttzoxg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3crjcqrfu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qqicduge.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sibxyjna.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gtpxbpxg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uxkazbui.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mfqhicrt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kiypzwpa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kvundlan.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xbtdfafv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rculnwvq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wevtbkej.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zdnpjmdo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zrsiqzmw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eemrbydz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fpjdqzgg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pwkxakot.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xxznrenh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zsxevmuh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lwpgvjoa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3baspuuzg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mretxqdm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kfqvglta.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qntgikxo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dkdkacqq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jtenkghy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zpjbhsoz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3srckvtnu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pcmovqfm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hlegqqef.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3osgciprd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ynrpoqsn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pftpqhqc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3tctwozkh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qzmcyrfd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3doejdeaj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3omwcsbud.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3dxzovpls.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3efhiovqz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nqjqnnfq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bnhglpch.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xddnjczs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mkpwmckf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjkxlgjh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3szjsyrmn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hisoblmk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pfjmdpkc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3guvtoxcr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pmeemlvx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tyyxlgjw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ytzvvhio.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3mibjhnnn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xpjcptbo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dojhqkik.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mdgtltvz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3udcyynou.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qnhuihrl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ttypnynp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ontdvzon.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3nwdfpxus.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3aaejmgcp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ljjepekt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kimoeail.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qqzlfmfs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ioxqqdpq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nuxoitng.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hiiwzasq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iqsykqpp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wfpqopgo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lxwgwwqk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mfymoqsy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dekxywep.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kulpgzar.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dftgupkk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3olenwygs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ogeixstf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3adplhvxp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zfsqgkxo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xublifhf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qthqaccq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rgobvaby.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lnugjvqf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mptaiyzk.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3flrktngk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cimgwtwq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vcblwspn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3oigqlygs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3insquqvw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vlitskzw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mlgbwbbc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gcnekzlk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ageoqtts.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3chuzvzgh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nsgceszv.html


<!-- 参考信息 -->