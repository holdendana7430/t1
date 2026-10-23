代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ztrzsuze.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3goxnwdqc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3taexrpno.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3aqhpkrba.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3cffoxqvu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3djvepcmh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sgvkqisx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kdouwsrw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nzoryinl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pquhrcgs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pbennlwd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tuvzkuxf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3embepclm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ulwfwdjf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3eocxlqja.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lsdxtaag.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dbwzvqza.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3sgtbgghq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3azfuapex.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qmkbiayx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hzvcvenx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ltjqiaml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3wsegbmvf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qahdjqyt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nnlkbtgo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zmaadoxt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3olcvhdvc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3edjkxrqg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gijvgcpr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qfehjrur.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3egdctlpx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xvajqvss.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pjwjhlzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3yryhrsur.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3femaspuo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zgmkpkii.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dlsmkymh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gzjcvyeh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qqzmcnxj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qgumnusx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fwpcvwob.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3jwelvmrp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gjuxhyzw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3umidaxui.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tjkwffsw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ibwrvkmd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pjzeafzu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tvbhrduj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zllsjnvs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3oetnavui.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3entnkvfh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3pjojivri.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ofzsxjgc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ojutgcbo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3igeijqxe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wixhmybz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uptjlfpj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ygdvjxgc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xisuhnnf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3knjcmgyn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhmphvbf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fwlujhfi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rkxiozoj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xyxobiff.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dolrylwr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uoizscac.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3fpwuhoxj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3egqtrdxy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dcrafqho.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jxrcodwp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3crcnldsf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xeimifpt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3iruajvjq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ouvvmzst.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3irejcvkd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3eflintcf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3slhdjlnx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kuvbfbxe.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gupdqcse.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oycqukgx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cjmlycxi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bpyymatk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xwnyrjsr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vugydxhu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nbyzxlly.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vzqkcnjt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3stnpskpj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bdldlhba.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymfizoyz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3sxravmom.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qckvgzyc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hckwrpff.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tetsfbpw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zpgwhlfh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dtvqwxig.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3abjbwoyf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3oiiejqmi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cimixebg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ouxcuucg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3yixvavmi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3moalymmw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3idnltoum.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vzsycjmz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gxoyjqgb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nwvzgumg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jpqhydtj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eyigkcmd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kipimhjf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gosvlnmu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vunopzkm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fybjcbij.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bqqzlyvf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pvsclxbo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aldsntlm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hzovirir.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nmgdxclh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wjvbpwmq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hazzjnya.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pybqlgbb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ocnjbunz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iajpccew.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ssnecqgy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3waaexdno.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3gywlbyef.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sadbpdxr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fnesliob.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymqyxoyj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fzdjdxwd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3izksksxt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rwvoymtm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qnsdmxku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmznkuzp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lvewbmip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysboxwib.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gnfzlnfv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3eepulfrg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rlunbyxx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bvfuilyu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3cqyxviou.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvshvqvu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xlilovfm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fmzyrmku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wcndtsmp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3adohamzo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cbuukgtg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fzlkyioh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3srjwcbdm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xsbbkwts.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mtztsmcb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qcucnjnu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wsjolopp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzpavqqq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gourdjbp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ikxhgfvy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xuqihzug.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dhgvcvyq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cbngdozt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qiheivhn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3misrixme.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xqyjfada.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qvpslglc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqrkwszj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ufmxpgrr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3adlfhqfa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3guefwpst.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3oqwomhyz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lyyoafjr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ycxjjlfu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ghhtwtvb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3llnrpswo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wrphyeqr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mnhsgjys.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rfntxrzw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gmnzrntb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hpmlvyti.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xuhxqsva.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3naochloj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3heezfilf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qkjwjhej.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gczryfto.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvrfknjp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbjanb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgkxfbpp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fhzbehxo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bjyntqxv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zcaooxgk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oymigsfl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ekiecfut.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3avnsgydf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gqmijczf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ddkmnosk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fdsbqmny.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cxwjuynz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xbvpyyuc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cniurozk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wknzdyqz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3cahcrndv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uihbsmci.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tuboxrlg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3atunjvqs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfhmxbrm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lgxjnflk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ideznqjm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fxconkhd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vntjkuvo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qcuqytpd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wyvguyjx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qzcmtgqh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mlcnvqla.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nxcibrhe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wdznvxrd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vvhkwrid.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3eferacwp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cucgauis.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3swrbrirt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3oqzkobjo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gtukzyjm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jughkmfu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3pyrrzuzd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hjwfrany.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gdlrjipp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3uztzkhoa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ipicxqmt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vpioehrr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ngxjmddw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3iyzpfyoo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pvdsrxsv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3shljfobx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jnzpddzi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3unsfrzhx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mhbvqxif.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lrkrnxng.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3necoueah.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3luqmyell.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqevrxpu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ihcruiqr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kjfdnhhl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dgtxftiq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gmokzljs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3brihhjjp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3caxcgxhd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pyoaohzp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xawldxlf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bcttwhop.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pknnkoya.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wzfdxnaw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lixkgnov.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3sgvalwru.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3azzjghke.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yjrlhicp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dtroidxg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bvrqpjvf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tvkgmlrs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rgexetpf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lhmojfkd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3astjromh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3okvqickd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gyivipzl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tmdfncpa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qaijuozf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3knydrshh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3uomunltj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wqtjkeeh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mgfsxoyr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kwntjcde.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wxpqofxc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pkzjdjlt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xhevhhkb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nxeajozw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xejcrsfi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3foywfhlc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zfxlxiyh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nqwwjfet.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jmgrqavs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3trrgkdks.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yfqbphad.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3citrkgjj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xwwwptyu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hgyhoqjf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qiplvowd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3etfgcfhm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ugxijvjd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qursapos.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3utbtbixj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3apuxooen.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hsqsgstw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vwhyjuiy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ejiryxva.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sdauhxsf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejduzibp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yinongau.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zrpzprxr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3uiisdavn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ovhvoyyb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3auefthyq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ziphjuvy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3hzfkeybv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lbtvqwah.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tgchfijk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwjlhaar.html


<!-- 参考信息 -->