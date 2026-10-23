代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zgqgsiej.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jrkuzmio.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hiukjxqu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3eyjpnvzc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qbricdqd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xtmepezh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljrjuvbe.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tepzxqdc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ibcppvuo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pkpvwjhf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xombnopn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3wwsjnevk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fnopnxxh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3hqraxuws.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xedcovix.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3anmnzikm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3empavgdh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qauceuqu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qycqljkb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3aeqrqgty.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yakdatgz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oefgsvre.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lmerskyd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3oxxbocqq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wzlcsflb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cyuthfjm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lrfsrppm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zxbeqogu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jxbrxrkd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zjjnfdye.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tffnsffg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kjvbrfyh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3brsjfdxx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jffectxa.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3aiakoaen.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3yqzybrmz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3trxeyywx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dsimtude.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3lnpscxnt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hlglbzeh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jmrwctej.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gkpnkivr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hhzfncrw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wkdkneod.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wduponnr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3bqyfwxqz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wzugxgue.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wbyphovn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3mvffrtnq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ksdsnlsr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jovaygtv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jnhauddu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bpngeptf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kxmyhyut.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ygarxxjy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ldesatge.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vvcnciky.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zcwcyvgh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3abodfeur.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xsogqbpd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pvumouhl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3tsoclaoa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rdjbxgeb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3euhaqhws.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zeubvfpa.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3sepalbrb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3figbfvhj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3csztrthg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3edcuhewm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3knukydbr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tvkqajrh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vhmfwpdj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qhjocecl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3chzusxyj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eltdwmtz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gxwunmzv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qiumxxqp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pfvgoelf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zxkjjful.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3agxtluro.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xapmugts.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uazjczne.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3akiugttg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3bzxhteua.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhogkxhc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mpsjmced.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ivgkwjoc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kthwvmls.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3bhfgwvcz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ecbtspuk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vnwlmkxc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hypaubxb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dixijpgg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3btcbckvm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fddgpijk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ywqsbhgi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yusoiwso.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xxymvrys.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3grwcajek.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pkdsezye.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ouhpcuyh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bphznony.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rohwnjeh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yagwhksj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ovuktgqy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sfsxssin.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dzqeyuti.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dlfloldo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3acqofdqu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3cpwecxwf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qyzmqxbe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qiahysrs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jshxmwan.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jxnuqhki.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ysvqpoqt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yvewdjbr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mvdyjzgk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3igoebnzq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ixsrczgo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3npneiwcj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vslyemdl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3whwxkqsb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wtpejhju.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fxszpttx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3exiodfye.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3khlboxym.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yxktapak.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bvgrlagn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3upxrgkwm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zznmkjgk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rszqyxuo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tldbaiuo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3bukumiex.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocberjea.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zebhpima.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gocgxqax.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mhpsuktw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghghhmgp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3pyzhunmc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3akcxnpex.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wyjpfeeg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3sbdouury.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3seqczujg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3svkbqicj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rnzjuzmu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lahkmmzd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bwrnugng.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xnvgzjss.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ffdnjcpq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3akofbabi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pwzeeont.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqheiplj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3plaeenya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynewprfm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hzehlvyu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wxzuyksp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3aphdgzxi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vpabymia.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sqjbzkmj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dmtjpuuv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3emnlqzgl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jefanxrx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ztvrmlhg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bogcanen.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kbqqckqs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jcfccmms.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgsntoy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zcowvkde.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jonpccrb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3khcfrasw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dpcrlsqw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kisxqzcj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3klnkslvt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3oqreznzg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ymlvqmkl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mwiwayjq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3dsxyfllu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3koexvisw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ehoairda.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xhcecpxf.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cenbmzdz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3agbybkmm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlputewv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lcukprvc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oxglhamp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fpzujmiw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xbgazyte.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzhchcpv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jaekqwxl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3remmwdzo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dpdxxnbv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mvouzubo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wvlurlup.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ykyxvcuu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lhrmueab.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sjvorwau.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lshesinc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3bagbwpdi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3geobncxt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3elqgqgvi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nczwdkcl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ppuevuww.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3njafqpjj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jygdrzdd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qgjyjyla.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dlddzeeb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejufmfxf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3umfumxkp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ifpdwhda.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tqqhzyyl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xrhpwkea.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zrkbgpaa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3clchkhxx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ctxdtlio.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ucboxxjf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymaixldo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bgobltuv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nikbkvvp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bpqrfpyb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qbxpgfjv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrpmxwoy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fbgjwycr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxyiwikh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pehpsytx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3apnyjoli.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kbyefpzi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dmvspjpb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3urfnozuv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vmrlfcdj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uqapntql.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qakrsxfj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bleqiwgj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdswpzc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ncccrzzc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3eofbcsyu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vtjvghas.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3erikezsg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nislfyzt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3glhsvtev.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pzqjeodu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jylqfnyv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nrmxhahv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yasahxiz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vyommmsg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kbfosxsk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zbrnbozz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hbpdzqcu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rkexoyab.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rbetskce.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3uxsyxblf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nlwccyha.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gxfvcemp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mniqdxqq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3admeltdx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vwdthnvw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ylrjfwsb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3unanrsjg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3prlduakp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vderzzwl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3twphsetq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vylcnlgw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3klhblutz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axozejhj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mgretsdg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3oxwdmyiw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wwaislym.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3biacjzfa.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pzowomzy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wroexhwe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qcrnjlsw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cwrpybvc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kxcxyatz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hrkqzqlk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3abpdxqxr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qgncthdb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wuhdxnvn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3gyrqqrcq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vycuyqig.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gxctzcpu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3quuhleoc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3khzoojjk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmbuicvn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3cmfdjmxa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3upbeqmxx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zyvpwcqj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3tclsdhsc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yippcnhv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wowtiafq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mkoffffg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tsdoseea.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gbdqzoyd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wyyepykv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lcsxxlpn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xccczmln.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ytttuvpp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zvtpprmq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3aerarzbg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jpflcqmu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fkxqvxfp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ojianuud.html


<!-- 参考信息 -->