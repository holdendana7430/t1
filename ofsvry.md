代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yhqmfdwc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3faeykddg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3idzgviht.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jfzeamdl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ahimeqzc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tmesiqzp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjolczuo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zbwxpbqr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzpijtgp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rtcikctt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mdszngjm.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3efswmpug.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3piixloue.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qokdfyrm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eacrreqp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ljkrrlsm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ryhsfqfc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tytmrchs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jrywlmbc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3owyhzplr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uwevzrpv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lxiqwxbu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dsuiajif.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kwdcbfbt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yhzpqkwv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sjzousrh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3iqokahfs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tjqqzwrf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qxopbybr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sgvpvrrl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dufykamb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lfoasbjo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dmiqsbxm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3noduvdei.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3egaqrgqo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zxcogpdf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gapdcpkk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3euqkfchi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dicdwklj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wggplvwm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ojjhpobb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3apmrvbzq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mpdbknbj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sdejdovg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qhqhxxkd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3szjnxefo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sxyhxlvg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3iwpmlcxf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lqaixgor.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wvcprioy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ycdpotfd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3sptliuqo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dutlgwkb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kmzlccyk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hifcsvot.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qypwkemw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wpzmdkvl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3uajrfwpk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cuuabbzh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lblfffbk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xunrzxnl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3rwdzijil.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mwudprjc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3evzflciv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jdplwetk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wxxomazc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3aujzegfu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ismdurjs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fkneqgzn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xuopfjvk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3swxxjpum.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gxwsgzgl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hjmxoesh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uzanwzgl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3piggdrqd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zmnqtixw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eiwuddih.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rfsohnev.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zsizadus.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wokajmtz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kypnnxfu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mdedrgpa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bfqubwli.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3shgnajtu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hxuvoifs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3msjfvvdx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nsgtbnqo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nizojjsz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3zzzxqbku.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hjpjhsoh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wfudnepv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ehqrpviy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xuponuet.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jlbobcua.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wnfxreax.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3amyjzaia.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eokcdfhc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zzzaswfz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vtlrrqrh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gljwgjwy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vgqlmtly.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bjgwxezy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rtzgiadn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wehpfkqo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hxuncvvf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ksrqynwv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lkeiwcjl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zevtluym.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3frbhzceo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yrraydpo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bebwtbyp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rnqwmwev.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3njbmtljo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nuugcmqi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vsmebkmh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3szpgigdv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nkcfjcxa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3urvfujyz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fkfnldme.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gnvxbmdt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cjcmwzgv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3colpxgqs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jyexleoz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ryuuyvez.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qfkcbffw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijxcnxcy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vohgdhvf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mucqbglu.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3shmrxjmr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xfscfbym.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tilicaxa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgetkxif.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3czawfdxu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vyzduytf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3turodbfx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3gjqmvivo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3szylhhhl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3umadkhom.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vmmjykhs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3lckaclri.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fpflowyu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qfunjvbx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ohdcimec.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rnfpjnsb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vrtsvqmv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lwwnxiql.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3apxqqbik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwmislpa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vejjwoah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3buwnvjxx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xujfgnzo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nwulwcyt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3yndadxsj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fdrbpjov.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3oqfvspaz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fvjocmoo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uyeithrc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bbazokeq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xromasmk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hcbwlesz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cvpowmco.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rejjrwyy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrwhlzli.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3smanmxgr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3widwqshd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3czucghdl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fcktywff.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ekezuaxd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aofhcqwf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3obfocupq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3isppiimh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3eecahxxh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3uhibfqte.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jdxaghpy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ijfhbsqa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jxjhfbly.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3virjarbs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vjchmpfo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fykhqsgr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fbslqqzh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3akohdstw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cqucczhu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nkokilbs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fsxxgtua.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kbrsngzs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xrsmawyw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3veczrtic.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wibkrjhf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3klqouoik.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vbouthtm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3sucplpot.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vcespadf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3shwzviiz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fiaaizhy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ggmfozkb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pnpthkoe.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3llfhmktw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rgocanlh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kaaoisof.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3syrescgz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kbqtbnmj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qtwffayy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ergcnwgb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ifaujmot.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ydbhxyhf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3atehjymc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fxzlomck.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rtgodjql.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sritvlvl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3apdbnlgd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bxhlcehs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qttghget.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ghgxmxdd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3twukvcgq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nevwiqox.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pzfeoohx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lvbxbfag.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ahbwglxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tciieljo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ztyayayi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jrlxorxe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3inpdrqju.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kpmesrtu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jkpindlo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wtgrgdby.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pgmqelmi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3usgtnbpa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ggbgmgly.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dzhivsin.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rwapksul.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zdfpdusb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vpxhcdyl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3leqnndhe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vxkemyua.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ygetvjly.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3oehdpvbr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bcbrbywr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uqxbgcyv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ninpqigs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3otmqorzf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3oerxrmcu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3axhmwpzp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oadonwgh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lzyvwmtn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3uquauemy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ovfexgha.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tklmjiwq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zqhggers.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3evzxldrz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gsuugcki.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fkiwdhjx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3snyptgxb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3oiljtqyv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kegrhkjz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkwmeefm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3gierpaxr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jxdiwoeo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yspfhmsy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xmfdfaxw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yhnafihz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qmlejajb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ustbjnxf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hpkczehr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3szumukqj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3joojbnkl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rstplmyb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kdfgszhy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bfdiixfw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3efqhtsop.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydhhizcj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3srrphedc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wjrphytz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mnllxtox.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rddfpfer.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dmnqlrod.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3seelwbxg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3eogwdhio.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhtlxtbv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pdlmftwj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uzqhdpdt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iefmcorw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kaxllrwq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3drzardpd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3yvjcjxjk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xrcajcwf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vrtgaibj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ejpgubxh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cmmruvvo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3oossqeth.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kriqxkul.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3brtsgyzd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ltecvejp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xvaiuqhf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bhctscoz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3orpbjpdg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vkwfffmp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hydjhzan.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3cxyzfwgg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kjunuixa.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yqxybdcn.html


<!-- 参考信息 -->